# Comparing `tmp/helyos_agent_sdk-0.1.6.tar.gz` & `tmp/helyos_agent_sdk-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "helyos_agent_sdk-0.1.6.tar", max compression
+gzip compressed data, was "helyos_agent_sdk-0.3.0.tar", max compression
```

## Comparing `helyos_agent_sdk-0.1.6.tar` & `helyos_agent_sdk-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       88 2023-01-26 14:16:59.066461 helyos_agent_sdk-0.1.6/helyos_agent_sdk/__init__.py
--rw-r--r--   0        0        0    10221 2023-01-26 14:16:30.860394 helyos_agent_sdk-0.1.6/helyos_agent_sdk/client.py
--rw-r--r--   0        0        0    14965 2023-01-26 14:16:49.073494 helyos_agent_sdk-0.1.6/helyos_agent_sdk/connector.py
--rw-r--r--   0        0        0      327 2023-01-26 14:13:46.294377 helyos_agent_sdk-0.1.6/helyos_agent_sdk/exceptions.py
--rw-r--r--   0        0        0     3404 2023-01-26 14:13:46.295378 helyos_agent_sdk-0.1.6/helyos_agent_sdk/models.py
--rw-r--r--   0        0        0     1071 2023-01-26 14:13:46.186379 helyos_agent_sdk-0.1.6/LICENSE
--rw-r--r--   0        0        0     1107 2023-02-01 14:24:37.651731 helyos_agent_sdk-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2589 2023-02-01 14:18:16.120422 helyos_agent_sdk-0.1.6/README.md
--rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 helyos_agent_sdk-0.1.6/setup.py
--rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 helyos_agent_sdk-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       88 2023-01-26 14:16:59.066461 helyos_agent_sdk-0.3.0/helyos_agent_sdk/__init__.py
+-rw-r--r--   0        0        0    12352 2023-04-10 14:11:35.649809 helyos_agent_sdk-0.3.0/helyos_agent_sdk/client.py
+-rw-r--r--   0        0        0    14965 2023-01-26 14:16:49.073494 helyos_agent_sdk-0.3.0/helyos_agent_sdk/connector.py
+-rw-r--r--   0        0        0      463 2023-04-10 14:06:03.061672 helyos_agent_sdk-0.3.0/helyos_agent_sdk/exceptions.py
+-rw-r--r--   0        0        0     3404 2023-01-26 14:13:46.295378 helyos_agent_sdk-0.3.0/helyos_agent_sdk/models.py
+-rw-r--r--   0        0        0     1071 2023-01-26 14:13:46.186379 helyos_agent_sdk-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1107 2023-04-10 14:12:16.868334 helyos_agent_sdk-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2589 2023-02-01 14:18:16.120422 helyos_agent_sdk-0.3.0/README.md
+-rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 helyos_agent_sdk-0.3.0/setup.py
+-rw-r--r--   0        0        0     3580 1970-01-01 00:00:00.000000 helyos_agent_sdk-0.3.0/PKG-INFO
```

### Comparing `helyos_agent_sdk-0.1.6/helyos_agent_sdk/client.py` & `helyos_agent_sdk-0.3.0/helyos_agent_sdk/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -142,37 +142,76 @@
     
         
         # step 2 - creates a temporary queue to receive checkin response
         temp_queue = self.guest_channel.queue_declare(queue='', exclusive=True)            
         self.checkin_response_queue = temp_queue.method.queue 
         self.guest_channel.basic_consume(queue=self.checkin_response_queue, auto_ack=True, on_message_callback=self.__checkin_callback)
 
+
+    def __prepare_checkin_for_already_connected(self):
+         # step 1 - use existent connection
+        self.guest_channel = self.channel
+        # step 2 - creates a temporary queue to receive checkin response
+        temp_queue = self.guest_channel.queue_declare(queue='', exclusive=True)            
+        self.checkin_response_queue = temp_queue.method.queue 
+        self.guest_channel.basic_consume(queue=self.checkin_response_queue, auto_ack=True, on_message_callback=self.__checkin_callback)
+
+
+    def connect_rabbitmq(self, username, password):
+        """ Connect to RabbitMQ 
+
+        :param username:  username previously registered in RabbitMQ server
+        :type username: str
+        :param password: password previously registered in RabbitMQ server'
+        :type password: str
+        """
+
+        try:
+            self.connection = connect_rabbitmq(self.rabbitmq_host, self.rabbitmq_port, username, password) 
+            self.channel = self.connection.channel()
+            self.rbmq_username = username
+
+        except Exception as inst:
+            print(inst)
+            raise HelyOSAccountConnectionError(
+                    f"Not able to connect as {username} to rabbitMQ to perform check in.")
+
+
+
     def perform_checkin(self, yard_uid, status='free', agent_data={}):
-        """ Check in the agent
+        """ Check in the agent: The checkin procedure registers an agent to a specific yard, and retrives the data about this yard. 
+            If the agent does not have a rabbitMQ account, helyOS will create an rabbitmq account using the agent's uuid as username.
+            Username and password are transmitted to the agent inside the check-in data.
 
         :param yard_uid: Yard UID
         :type yard_uid: str
         :param status: Agent status, defaults to 'free'
         :type status: str
         """
-        self.__connect_as_anonymous()
+        if self.connection:
+            self.__prepare_checkin_for_already_connected()
+            username = self.rbmq_username
+        else:
+            self.__connect_as_anonymous()
+            username = 'anonymous'
+
         self.yard_uid = yard_uid
         checkin_msg = {  'type': 'checkin',
                          'uuid': self.uuid,
                          'status': status,
                          'body': {'yard_uid': yard_uid, 
                                   'public_key':self.public_key.decode("utf-8"),  
                                   'public_key_format': 'PEM', 
                                   'registration_token': REGISTRATION_TOKEN,
                                   **agent_data},
                        }
 
         self.guest_channel.basic_publish(exchange = AGENT_ANONYMOUS_EXCHANGE,
                                   routing_key =  self.checking_routing_key,
-                                  properties=pika.BasicProperties(reply_to = self.checkin_response_queue),
+                                  properties=pika.BasicProperties(reply_to = self.checkin_response_queue, user_id = username),
                                   body=json.dumps(checkin_msg))
         
 
     def __checkin_callback(self, ch, method, properties, received_str):
         received_message_str = json.loads(received_str)['message']    
         received_message = json.loads(received_message_str)
         
@@ -181,27 +220,31 @@
             print("waiting response...")
             return
         
         body = received_message['body']
         response_code = body.get('response_code', 500)
         if response_code!='200':
             print(body)
-            raise HelyOSCheckinError(f"Check in refused: code {response_code}")
+            message  = body.get('message', "Check in refused")
+            raise HelyOSCheckinError(f"{message}: code {response_code}")
             
-        password = body['rbmq_password']
+        password = body.get('rbmq_password', None)
         try:
-            self.connection = connect_rabbitmq(self.rabbitmq_host, self.rabbitmq_port, body['rbmq_username'], password)
-            self.channel = self.connection.channel()
+            if password:
+                self.connection = connect_rabbitmq(self.rabbitmq_host, self.rabbitmq_port, body['rbmq_username'], password)
+                self.channel = self.connection.channel()
+                self.rbmq_username = body['rbmq_username']
+                print('username', body['rbmq_username'])
+                print('password', body['rbmq_password'])
             self.uuid = received_message['uuid']
             self.checkin_data = body
             ch.stop_consuming()
             
             print('uuid', self.uuid)
-            print('username', body['rbmq_username'])
-            print('password', body['rbmq_password'])
+
         except  Exception as inst: 
             self.tries += 1
             print(f"try {self.tries}")
             if self.tries > 3:
                 ch.stop_consuming()
 
 
@@ -213,18 +256,20 @@
             :param encrypted: If this message should be encrypted, defaults to False
             :type encrypted: str
             :param exchange: RabbitMQ exchange, defaults to env.AGENTS_UL_EXCHANGE
             :type exchange: str
         """
 
         try:
-            self.channel.basic_publish(exchange, routing_key, body=message)
+            self.channel.basic_publish(exchange, routing_key, properties=pika.BasicProperties(user_id = self.rbmq_username), body=message)
         except ConnectionResetError:
             self.channel = self.connection.channel()
-            self.channel.basic_publish(exchange, routing_key, body=message)
+            self.channel.basic_publish(exchange, routing_key,
+                                       properties=pika.BasicProperties(user_id = self.rbmq_username),
+                                       body=message)
 
     @auth_required            
     def set_assignment_queue(self, exchange=AGENTS_DL_EXCHANGE):
         self.assignment_queue = self.channel.queue_declare(queue='')        
         self.channel.queue_bind(queue=self.assignment_queue.method.queue,
                                 exchange=exchange, routing_key=self.assignment_routing_key) 
         return self.assignment_queue
```

### Comparing `helyos_agent_sdk-0.1.6/helyos_agent_sdk/connector.py` & `helyos_agent_sdk-0.3.0/helyos_agent_sdk/connector.py`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.1.6/helyos_agent_sdk/models.py` & `helyos_agent_sdk-0.3.0/helyos_agent_sdk/models.py`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.1.6/LICENSE` & `helyos_agent_sdk-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.1.6/pyproject.toml` & `helyos_agent_sdk-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "helyos_agent_sdk"
-version = "0.1.6"
+version = "0.3.0"
 description = ""
 authors = ["Carlos Viol Barbosa <you@example.com>"]
 readme = "README.md"
 packages = [{include = "helyos_agent_sdk"}]
 keywords = ["autonomous driving", "helyos", "sdk"]
 
 homepage = "https://helyos.ivi.fraunhofer.de"
```

### Comparing `helyos_agent_sdk-0.1.6/README.md` & `helyos_agent_sdk-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `helyos_agent_sdk-0.1.6/setup.py` & `helyos_agent_sdk-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 install_requires = \
 ['dataclasses-json>=0.5.7,<0.6.0',
  'pika>=1.3.1,<2.0.0',
  'pycryptodome>=3.15.0,<4.0.0']
 
 setup_kwargs = {
     'name': 'helyos-agent-sdk',
-    'version': '0.1.6',
+    'version': '0.3.0',
     'description': '',
     'long_description': '<div id="top"></div>\n\n<!-- PROJECT LOGO -->\n<br />\n<div align="center">\n  <a href="https://github.com/">\n    <img src="helyos_logo.png" alt="Logo"  height="80">\n    <img src="truck.png" alt="Logo"  height="80">\n  </a>\n\n  <h3 align="center">helyOS Agent SDK</h3>\n\n  <p align="center">\n    Methods and data strrctures to connect autonomous vehicles to helyOS.\n    <br />\n    <a href="https://fraunhoferivi.github.io/helyOS-agent-sdk/"><strong>Explore the docs »</strong></a>\n    <br />\n    <br />\n    <a href="https://github.com/">View Demo</a>\n    ·\n    <a href="https://github.com/FraunhoferIVI/helyOS-agent-sdk/issues">Report Bug</a>\n    ·\n    <a href="https://github.com/FraunhoferIVI/helyOS-agent-sdk/issues">Request Feature</a>\n  </p>\n</div>\n\n## About The Project\n\nThe helyos-agent-sdk python package encloses methods and data structures definitions that facilitate the connection to helyOS core through rabbitMQ.\n\n### List of features\n\n*   RabbitMQ client to communicate with helyOS. \n*   Check-in method.\n*   Agent and assignment status definitions. \n*   Easy access to helyOS assignments via callbacks. \n*   Application-level encryption.\n\n### Install\n\n```\npip install helyos_agent_sdk\n\n```\n### Usage\n\n```python\nos.environ[\'AGENTS_UL_EXCHANGE\'] = "xchange_helyos.agents.ul"\nos.environ[\'AGENTS_DL_EXCHANGE\'] = "xchange_helyos.agents.dl"\nos.environ[\'AGENT_ANONYMOUS_EXCHANGE\'] = "xchange_helyos.agents.anonymous"\nfrom helyos_agent_sdk import HelyOSClient, AgentConnector\n\n# Check in\ninitial_agent_data = {\'name\': "vehicle name", \'pose\': {\'x\':-30167, \'y\':-5415, \'orientations\':[0, 0]}, \'geometry\':{"my_custom_format": {}}}\nhelyOS_client = HelyOSClient(rabbitmq_host, rabbitmq_port, uuid=AGENT_UID)\nhelyOS_client.perform_checkin(yard_uid=\'1\', agent_data=initial_agent_data, status="free")\nhelyOS_client.get_checkin_result()\n\n\n# Communication\nagent_connector = AgentConnector(helyOS_client)\nagent_connector.publish_sensors(x=-30167, y=3000, z=0, orientations=[1500, 0], sensor= {"my_custom_format": {}})\n\n# ... #\n\nagentConnector.publish_state(status, resources, assignment_status)\n\n# ... #\n\nagentConnector.consume_instant_action_messages(my_reserve_callback, my_release_callback, my_cancel_assignm_callback, any_other_callback)\nagentConnector.consume_assignment_messages(my_assignment_callback)\nagentConnector.start_consuming()\n\n\n```\n\n\n### Contributing\n\nKeep it simple. Keep it minimal.\n\n### Authors \n\n*   Carlos E. Viol Barbosa\n*   ...\n\n### License\n\nThis project is licensed under the MIT License',
     'author': 'Carlos Viol Barbosa',
     'author_email': 'you@example.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://helyos.ivi.fraunhofer.de',
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \
 ['helyos_agent_sdk'] package_data = \ {'': ['*']} install_requires = \
 ['dataclasses-json>=0.5.7,<0.6.0', 'pika>=1.3.1,<2.0.0',
 'pycryptodome>=3.15.0,<4.0.0'] setup_kwargs = { 'name': 'helyos-agent-sdk',
-'version': '0.1.6', 'description': '', 'long_description': '
+'version': '0.3.0', 'description': '', 'long_description': '
 \n\n\n
 \n
                           \n \n_[Logo]\n_[Logo]\n\n\n
                           **** helyOS Agent SDK ****
                                      \n\n
   \n Methods and data strrctures to connect autonomous vehicles to helyOS.\n
                            \n Explore_the_docs_Â»\n
```

### Comparing `helyos_agent_sdk-0.1.6/PKG-INFO` & `helyos_agent_sdk-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: helyos-agent-sdk
-Version: 0.1.6
+Version: 0.3.0
 Summary: 
 Home-page: https://helyos.ivi.fraunhofer.de
 Keywords: autonomous driving,helyos,sdk
 Author: Carlos Viol Barbosa
 Author-email: you@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: Environment :: Console
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: helyos-agent-sdk Version: 0.1.6 Summary: Home-page:
+Metadata-Version: 2.1 Name: helyos-agent-sdk Version: 0.3.0 Summary: Home-page:
 https://helyos.ivi.fraunhofer.de Keywords: autonomous driving,helyos,sdk
 Author: Carlos Viol Barbosa Author-email: you@example.com Requires-Python:
 >=3.7,<4.0 Classifier: Environment :: Console Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.7 Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
```

