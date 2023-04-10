# Comparing `tmp/pyscora_wrangler-1.1.3.tar.gz` & `tmp/pyscora_wrangler-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyscora_wrangler-1.1.3.tar", max compression
+gzip compressed data, was "pyscora_wrangler-1.1.4.tar", max compression
```

## Comparing `pyscora_wrangler-1.1.3.tar` & `pyscora_wrangler-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1049 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/LICENSE
--rw-r--r--   0        0        0      659 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/README.md
--rw-r--r--   0        0        0     1116 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyproject.toml
--rw-r--r--   0        0        0       51 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyscora_wrangler/__init__.py
--rw-r--r--   0        0        0    14201 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyscora_wrangler/aws/README.md
--rw-r--r--   0        0        0       85 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyscora_wrangler/aws/__init__.py
--rw-r--r--   0        0        0     7114 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyscora_wrangler/aws/athena/__init__.py
--rw-r--r--   0        0        0    15796 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyscora_wrangler/aws/cognito/__init__.py
--rw-r--r--   0        0        0       88 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyscora_wrangler/aws/constants.py
--rw-r--r--   0        0        0     6697 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyscora_wrangler/aws/dynamodb/__init__.py
--rw-r--r--   0        0        0      671 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyscora_wrangler/aws/utils.py
--rw-r--r--   0        0        0      165 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyscora_wrangler/constants.py
--rw-r--r--   0        0        0      504 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyscora_wrangler/ldap/README.md
--rw-r--r--   0        0        0       60 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyscora_wrangler/ldap/__init__.py
--rw-r--r--   0        0        0     7512 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyscora_wrangler/ldap/service/__init__.py
--rw-r--r--   0        0        0       22 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyscora_wrangler/ldap/utils.py
--rw-r--r--   0        0        0     2692 2023-04-06 20:40:05.934980 pyscora_wrangler-1.1.3/pyscora_wrangler/utils.py
--rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 pyscora_wrangler-1.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1049 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/LICENSE
+-rw-r--r--   0        0        0      659 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/README.md
+-rw-r--r--   0        0        0     1116 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyproject.toml
+-rw-r--r--   0        0        0       51 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/__init__.py
+-rw-r--r--   0        0        0    14258 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/aws/README.md
+-rw-r--r--   0        0        0       85 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/aws/__init__.py
+-rw-r--r--   0        0        0     7114 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/aws/athena/__init__.py
+-rw-r--r--   0        0        0    15796 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/aws/cognito/__init__.py
+-rw-r--r--   0        0        0       88 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/aws/constants.py
+-rw-r--r--   0        0        0     6697 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/aws/dynamodb/__init__.py
+-rw-r--r--   0        0        0      671 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/aws/utils.py
+-rw-r--r--   0        0        0      165 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/constants.py
+-rw-r--r--   0        0        0      513 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/ldap/README.md
+-rw-r--r--   0        0        0       60 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/ldap/__init__.py
+-rw-r--r--   0        0        0     7761 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/ldap/service/__init__.py
+-rw-r--r--   0        0        0       22 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/ldap/utils.py
+-rw-r--r--   0        0        0     2692 2023-04-10 18:51:21.191627 pyscora_wrangler-1.1.4/pyscora_wrangler/utils.py
+-rw-r--r--   0        0        0     1998 1970-01-01 00:00:00.000000 pyscora_wrangler-1.1.4/PKG-INFO
```

### Comparing `pyscora_wrangler-1.1.3/LICENSE` & `pyscora_wrangler-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.3/README.md` & `pyscora_wrangler-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.3/pyproject.toml` & `pyscora_wrangler-1.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyscora-wrangler"
-version = "1.1.3"
+version = "1.1.4"
 description = "Python lib for DE"
 authors = ["Oncase <suporte@oncase.com.br>"]
 maintainers = ["Guilherme Morone <guilherme.morone@oncase.com.br>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/oncase/pyscora-wrangler"
 repository = "https://github.com/oncase/pyscora-wrangler"
```

### Comparing `pyscora_wrangler-1.1.3/pyscora_wrangler/aws/README.md` & `pyscora_wrangler-1.1.4/pyscora_wrangler/aws/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,221 +1,223 @@
+# AWS
+
 This module contains a set of functions to interact with AWS services.
 
-# Athena
+## Athena
 
 See `./athena/__init__.py` for more details.
 
-# Cognito
+## Cognito
 
-## `add_user_to_group`
+### `add_user_to_group`
 
-### Adds the specified user to the specified group
+#### Adds the specified user to the specified group
 
 Calling this action requires developer credentials.
 
-### Parameters
+#### Parameters
 
 |      Name       |          Type           |            Description             | Required | Default |
 | :-------------: | :---------------------: | :--------------------------------: | :------: | :-----: |
 |  `userpool_id`  |          `str`          | The user pool ID for the user pool |  `True`  |   `-`   |
 |   `username`    |          `str`          |     The username for the user      |  `True`  |   `-`   |
 |  `group_name`   |          `str`          |           The group name           |  `True`  |   `-`   |
 | `boto3_session` | `boto3.session.Session` |        Custom boto3 session        | `False`  | `None`  |
 
-### Returns
+#### Returns
 
 `None`
 
-## `authenticate_user`
+### `authenticate_user`
 
-### Initiates the authentication flow, as an administrator
+#### Initiates the authentication flow, as an administrator
 
 Calling this action requires developer credentials.
 
-### Parameters
+#### Parameters
 
 |        Name         |          Type           |                                      Description                                       | Required |       Default       |
 | :-----------------: | :---------------------: | :------------------------------------------------------------------------------------: | :------: | :-----------------: |
 |    `userpool_id`    |          `str`          |                         The ID of the Amazon Cognito user pool                         |  `True`  |         `-`         |
 |     `client_id`     |          `str`          |                                   The app client ID                                    |  `True`  |         `-`         |
 |     `username`      |          `str`          |                   The user name of the user you want to authenticate                   |  `True`  |         `-`         |
 |     `password`      |          `str`          |                               The password for the user                                |  `True`  |         `-`         |
 |     `auth_flow`     |          `str`          | The authentication flow for this call to run. The API action will depend on this value | `False`  | `ADMIN_NO_SRP_AUTH` |
 | `app_client_secret` |          `str`          |                          The app client secret, if configured                          | `False`  |       `None`        |
 |   `boto3_session`   | `boto3.session.Session` |                                  Custom boto3 session                                  | `False`  |       `None`        |
 
-### Returns
+#### Returns
 
 `Dict[str, Any]`: Initiates the authentication response, as an administrator.
 
-## `create_group`
+### `create_group`
 
-### Creates a new group in the specified user pool
+#### Creates a new group in the specified user pool
 
 Calling this action requires developer credentials.
 
-### Parameters
+#### Parameters
 
 |      Name       |          Type           |                   Description                    | Required | Default |
 | :-------------: | :---------------------: | :----------------------------------------------: | :------: | :-----: |
 |  `userpool_id`  |          `str`          |        The user pool ID for the user pool        |  `True`  |   `-`   |
 |   `username`    |          `str`          |      The name of the group. Must be unique       |  `True`  |   `-`   |
 |  `description`  |          `str`          | A string containing the description of the group | `False`  |  `''`   |
 | `boto3_session` | `boto3.session.Session` |               Custom boto3 session               | `False`  | `None`  |
 
-## `create_user`
+### `create_user`
 
-### Creates a new user in the specified user pool
+#### Creates a new user in the specified user pool
 
 Calling this action requires developer credentials.
 
-### Parameters
+#### Parameters
 
 |          Name          |          Type           |                                                                                            Description                                                                                             | Required | Default |
 | :--------------------: | :---------------------: | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------: | :-----: |
 |     `userpool_id`      |          `str`          |                                                                 The user pool ID for the user pool where the user will be created                                                                  |  `True`  |   `-`   |
 |       `username`       |          `str`          |           The username for the user. Must be unique within the user pool. Must be a UTF-8 string between 1 and 128 characters. After the user is created, the username can't be changed            |  `True`  |   `-`   |
 |   `user_attributes`    | `List[Dict[str, Any]]`  | An array of name-value pairs that contain user attributes and attribute values to be set for the user to be created. You can create a user without specifying any attributes other than `Username` | `False`  |  `[]`   |
 | `force_alias_creation` |         `bool`          |                                   TThis parameter is used only if the phone_number_verified or email_verified attribute is set to True. Otherwise, it is ignored                                   | `False`  | `False` |
 |    `boto3_session`     | `boto3.session.Session` |                                                                                        Custom boto3 session                                                                                        | `False`  | `None`  |
 
-#### Addition args can be found at [boto3 `admin_create_user` docs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp/client/admin_create_user.html)
+##### Addition args can be found at [boto3 `admin_create_user` docs](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/cognito-idp/client/admin_create_user.html)
 
-### Returns
+#### Returns
 
 `Dict[str, Any]`: The newly created user.
 
-## `get_all_users`
+### `get_all_users`
 
-### Lists the users in the Amazon Cognito user pool
+#### Lists the users in the Amazon Cognito user pool
 
-### Parameters
+#### Parameters
 
 |        Name         |          Type           |                                                                                 Description                                                                                  | Required | Default |
 | :-----------------: | :---------------------: | :--------------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :------: | :-----: |
 |    `userpool_id`    |          `str`          |                                                  The user pool ID for the user pool on which the search should be performed                                                  |  `True`  |   `-`   |
 | `attributes_to_get` |       `List[str]`       | An array of strings, where each string is the name of a user attribute to be returned for each user in the search results. If the array is null, all attributes are returned | `False`  |  `[]`   |
 |      `filter`       |          `str`          |     A filter string of the form “AttributeName Filter-Type “AttributeValue””. Quotation marks within the filter string must be escaped using the backslash () character      | `False`  |  `''`   |
 |   `boto3_session`   | `boto3.session.Session` |                                                                             Custom boto3 session                                                                             | `False`  | `None`  |
 
-### Returns
+#### Returns
 
 `List[Dict[str, Any]]`: The users returned in the request to list users.
 
-## `get_user`
+### `get_user`
 
-### Gets the specified user by user name in a user pool as an administrator. Works on any user
+#### Gets the specified user by user name in a user pool as an administrator. Works on any user
 
 Calling this action requires developer credentials.
 
-### Parameters
+#### Parameters
 
 |      Name       |          Type           |                                     Description                                     | Required | Default |
 | :-------------: | :---------------------: | :---------------------------------------------------------------------------------: | :------: | :-----: |
 |  `userpool_id`  |          `str`          | The user pool ID for the user pool where you want to get information about the user |  `True`  |   `-`   |
 |   `username`    |          `str`          |                   The user name of the user you want to retrieve                    |  `True`  |   `-`   |
 | `boto3_session` | `boto3.session.Session` |                                Custom boto3 session                                 | `False`  | `None`  |
 
-### Returns
+#### Returns
 
 `Dict[str, Any]`: Represents the response from the server from the request to get the specified user as an administrator.
 
-## `get_users_from_group`
+### `get_users_from_group`
 
-### Lists the users in the specified group
+#### Lists the users in the specified group
 
-### Parameters
+#### Parameters
 
 |      Name       |          Type           |                                 Description                                 | Required | Default |
 | :-------------: | :---------------------: | :-------------------------------------------------------------------------: | :------: | :-----: |
 |  `userpool_id`  |          `str`          | The user pool ID for the user pool on which the search should be performed. |  `True`  |   `-`   |
 |  `group_name`   |          `str`          |                            The name of the group                            |  `True`  |   `-`   |
 | `boto3_session` | `boto3.session.Session` |                            Custom boto3 session                             | `False`  | `None`  |
 
-### Returns
+#### Returns
 
 `List[Dict[str, Any]]`: The users returned in the request to list users.
 
-## `remove_user_from_group`
+### `remove_user_from_group`
 
-### Removes the specified user from the specified group
+#### Removes the specified user from the specified group
 
 Calling this action requires developer credentials.
 
-### Parameters
+#### Parameters
 
 |      Name       |          Type           |            Description             | Required | Default |
 | :-------------: | :---------------------: | :--------------------------------: | :------: | :-----: |
 |  `userpool_id`  |          `str`          | The user pool ID for the user pool |  `True`  |   `-`   |
 |   `username`    |          `str`          |     The username for the user      |  `True`  |   `-`   |
 |  `group_name`   |          `str`          |           The group name           |  `True`  |   `-`   |
 | `boto3_session` | `boto3.session.Session` |        Custom boto3 session        | `False`  | `None`  |
 
-### Returns
+#### Returns
 
 `None`
 
-## `remove_user_from_userpool`
+### `remove_user_from_userpool`
 
-### Deletes a user as an administrator. Works on any user
+#### Deletes a user as an administrator. Works on any user
 
 Calling this action requires developer credentials.
 
-### Parameters
+#### Parameters
 
 |      Name       |          Type           |                             Description                              | Required | Default |
 | :-------------: | :---------------------: | :------------------------------------------------------------------: | :------: | :-----: |
 |  `userpool_id`  |          `str`          | The user pool ID for the user pool where you want to delete the user |  `True`  |   `-`   |
 |   `username`    |          `str`          |             The user name of the user you want to delete             |  `True`  |   `-`   |
 | `boto3_session` | `boto3.session.Session` |                         Custom boto3 session                         | `False`  | `None`  |
 
-### Returns
+#### Returns
 
 `None`
 
-## `resend_confirmation_code`
+### `resend_confirmation_code`
 
-### Resends the confirmation (for confirmation of registration) to a specific user in the user pool
+#### Resends the confirmation (for confirmation of registration) to a specific user in the user pool
 
-### Parameters
+#### Parameters
 
 |      Name       |          Type           |                                    Description                                    | Required | Default |
 | :-------------: | :---------------------: | :-------------------------------------------------------------------------------: | :------: | :-----: |
 |   `client_id`   |          `str`          |                The ID of the client associated with the user pool                 |  `True`  |   `-`   |
 |   `username`    |          `str`          | The username attribute of the user to whom you want to resend a confirmation code |  `True`  |   `-`   |
 | `boto3_session` | `boto3.session.Session` |                               Custom boto3 session                                | `False`  | `None`  |
 
-### Returns
+#### Returns
 
 `Dict[str, Any]`: The code delivery details returned by the server in response to the request to resend the confirmation code.
 
-## `set_user_password`
+### `set_user_password`
 
-### Sets the specified user's password in a user pool as an administrator. Works on any user
+#### Sets the specified user's password in a user pool as an administrator. Works on any user
 
-#### The password can be temporary or permanent. If it is temporary, the user status enters the `FORCE_CHANGE_PASSWORD` state. When the user next tries to sign in, the InitiateAuth/AdminInitiateAuth response will contain the `NEW_PASSWORD_REQUIRED` challenge. If the user doesn't sign in before it expires, the user won't be able to sign in, and an administrator must reset their password.
+##### The password can be temporary or permanent. If it is temporary, the user status enters the `FORCE_CHANGE_PASSWORD` state. When the user next tries to sign in, the InitiateAuth/AdminInitiateAuth response will contain the `NEW_PASSWORD_REQUIRED` challenge. If the user doesn't sign in before it expires, the user won't be able to sign in, and an administrator must reset their password.
 
-#### Once the user has set a new password, or the password is permanent, the user status is set to `Confirmed`.
+##### Once the user has set a new password, or the password is permanent, the user status is set to `Confirmed`.
 
 Calling this action requires developer credentials.
 
-### Parameters
+#### Parameters
 
 |      Name       |          Type           |                                 Description                                  | Required | Default |
 | :-------------: | :---------------------: | :--------------------------------------------------------------------------: | :------: | :-----: |
 |  `userpool_id`  |          `str`          | The user pool ID for the user pool where you want to set the user's password |  `True`  |   `-`   |
 |   `username`    |          `str`          |           The user name of the user whose password you want to set           |  `True`  |   `-`   |
 |   `password`    |          `str`          |                          The password for the user                           |  `True`  |   `-`   |
 |   `permanent`   |         `bool`          |       `True` if the password is permanent, `False` if it is temporary        |  `True`  | `True`  |
 | `boto3_session` | `boto3.session.Session` |                             Custom boto3 session                             | `False`  | `None`  |
 
-### Returns
+#### Returns
 
 `None`
 
-# DynamoDB
+## DynamoDB
 
 See `./dynamodb/__init__.py` for more details.
 
-# Other Services
+## Other Services
 
 Check out [boto3 docs](https://boto3.amazonaws.com/v1/documentation/api/latest/index.html) and [awswrangler docs](https://pypi.org/project/awswrangler/) for more information.
```

### Comparing `pyscora_wrangler-1.1.3/pyscora_wrangler/aws/athena/__init__.py` & `pyscora_wrangler-1.1.4/pyscora_wrangler/aws/athena/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.3/pyscora_wrangler/aws/cognito/__init__.py` & `pyscora_wrangler-1.1.4/pyscora_wrangler/aws/cognito/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.3/pyscora_wrangler/aws/dynamodb/__init__.py` & `pyscora_wrangler-1.1.4/pyscora_wrangler/aws/dynamodb/__init__.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.3/pyscora_wrangler/aws/utils.py` & `pyscora_wrangler-1.1.4/pyscora_wrangler/aws/utils.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.3/pyscora_wrangler/ldap/service/__init__.py` & `pyscora_wrangler-1.1.4/pyscora_wrangler/ldap/service/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         Returns:
             bool: True if user is authenticated to ldap server, False otherwise.
         """
 
         return self.__user_is_authenticated
 
     def auth(self, username: str, password: str) -> bool:
-        """Authenticate user to ldap server
+        """Authenticate user to ldap server in SIMPLE mode
 
         Args:
             username (str): The user `username`.
             password (str): The user `password`.
 
         Raises:
             ValueError: If `username` or `password` is null or is empty string.
@@ -118,43 +118,53 @@
             if not self.__ldap_username or not self.__ldap_password:
                 logger_msg = 'Username argument cannot be null or empty.' if not self.__ldap_username else ''
                 logger_msg += 'Password argument cannot be null or empty.' if not self.__ldap_password else ''
                 logger.error(f'[auth] {logger_msg}')
 
                 raise ValueError('Invalid credentials.')
 
-            root_dn = self.ldap_config.get('root_dn', '')
             port = int(self.ldap_config.get('port', 389))
             server_alias = self.ldap_config.get('server_alias', [])
 
             server = Server(
                 self.ldap_config.get('server', ''),
                 get_info=ALL,
                 port=port,
                 allowed_referral_hosts=[(sa, True) for sa in server_alias]
                 if server_alias and len(server_alias)
                 else None,
             )
 
-            self.__ldap_user = f'CN={self.__ldap_username},{root_dn}'
-
             self.__ldap_connection = Connection(
-                server, user=self.__ldap_user, password=self.__ldap_password, raise_exceptions=False
+                server,
+                user=self.__ldap_username,
+                password=self.__ldap_password,
+                authentication='SIMPLE',
+                raise_exceptions=False,
             )
 
             if self.__ldap_connection.bind():
                 self.__user_is_authenticated = True
                 logger.info("[auth] Successful bind to ldap server.")
             else:
                 logger.error(f"[auth] Cannot bind to ldap server: {self.__ldap_connection.last_error}.")
         except Exception as err:
             logger.error(f'[auth] {err}')
 
         return self.is_user_authenticated()
 
+    def logout(self) -> None:
+        """Unbind the connect to the ldap server"""
+
+        if self.__ldap_connection:
+            try:
+                self.__ldap_connection.unbind()
+            except Exception as err:
+                logger.error(f'[logout] {err}')
+
     def get_ldap_groups(self) -> List[str]:
         """Returns A list containing the ldap groups."""
 
         return self.__ldap_groups
 
     def get_ldap_users(self) -> List[str]:
         """Returns A list containing the ldap users."""
```

### Comparing `pyscora_wrangler-1.1.3/pyscora_wrangler/utils.py` & `pyscora_wrangler-1.1.4/pyscora_wrangler/utils.py`

 * *Files identical despite different names*

### Comparing `pyscora_wrangler-1.1.3/PKG-INFO` & `pyscora_wrangler-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyscora-wrangler
-Version: 1.1.3
+Version: 1.1.4
 Summary: Python lib for DE
 Home-page: https://github.com/oncase/pyscora-wrangler
 License: MIT
 Keywords: wrapper,scora,python,data_engineering
 Author: Oncase
 Author-email: suporte@oncase.com.br
 Maintainer: Guilherme Morone
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyscora-wrangler Version: 1.1.3 Summary: Python lib
+Metadata-Version: 2.1 Name: pyscora-wrangler Version: 1.1.4 Summary: Python lib
 for DE Home-page: https://github.com/oncase/pyscora-wrangler License: MIT
 Keywords: wrapper,scora,python,data_engineering Author: Oncase Author-email:
 suporte@oncase.com.br Maintainer: Guilherme Morone Maintainer-email:
 guilherme.morone@oncase.com.br Requires-Python: >=3.8,<4.0 Classifier: Intended
 Audience :: Developers Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.8 Classifier:
```

