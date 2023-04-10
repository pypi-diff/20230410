# Comparing `tmp/gptdeploy-0.18.4.tar.gz` & `tmp/gptdeploy-0.18.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gptdeploy-0.18.4.tar", last modified: Mon Apr 10 00:25:45 2023, max compression
+gzip compressed data, was "dist/gptdeploy-0.18.5.tar", last modified: Mon Apr 10 18:52:43 2023, max compression
```

## Comparing `gptdeploy-0.18.4.tar` & `gptdeploy-0.18.5.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14228 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/gptdeploy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18231 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/gptdeploy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/gptdeploy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/gptdeploy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/gptdeploy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/gptdeploy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/gptdeploy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/src/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/jina_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/key_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)    14312 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/prompt_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/prompt_tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:45.000000 gptdeploy-0.18.4/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-10 00:25:28.000000 gptdeploy-0.18.4/src/utils/string_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:52:43.000000 gptdeploy-0.18.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-04-10 18:52:43.000000 gptdeploy-0.18.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15000 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:52:43.000000 gptdeploy-0.18.5/gptdeploy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19283 2023-04-10 18:52:43.000000 gptdeploy-0.18.5/gptdeploy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-10 18:52:43.000000 gptdeploy-0.18.5/gptdeploy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:52:43.000000 gptdeploy-0.18.5/gptdeploy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 18:52:43.000000 gptdeploy-0.18.5/gptdeploy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-10 18:52:43.000000 gptdeploy-0.18.5/gptdeploy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-10 18:52:43.000000 gptdeploy-0.18.5/gptdeploy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 18:52:43.000000 gptdeploy-0.18.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:52:43.000000 gptdeploy-0.18.5/src/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/src/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14780 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/src/executor_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4649 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/src/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/src/jina_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/src/key_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/src/prompt_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5974 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/src/prompt_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1520 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/src/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:52:43.000000 gptdeploy-0.18.5/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/src/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/src/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1600 2023-04-10 18:52:30.000000 gptdeploy-0.18.5/src/utils/string_tools.py
```

### Comparing `gptdeploy-0.18.4/PKG-INFO` & `gptdeploy-0.18.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdeploy
-Version: 0.18.4
+Version: 0.18.5
 Summary: Use natural language interface to create, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/gptdeploy
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Description: <h1 align="center">
         GPT Deploy: One line to create them all 🧙🚀
@@ -46,49 +46,79 @@
         ## Quickstart
         ### Installation
         ```bash
         pip install gptdeploy
         gptdeploy configure --key <your openai api key>
         ```
         If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
+        Your api key must have access to gpt-4 to use this tool. 
+        We are working on a way to use gpt-3.5-turbo as well.
         
-        ### run
+        ### Create Microservice
         ```bash
         gptdeploy create --description "Given a PDF, return it's text" --test "https://www.africau.edu/images/default/sample.pdf"
         ```
         To create your personal microservice two things are required:
         - A `description` of the task you want to accomplish.
         - A `test` scenario that ensures the microservice works as expected.
         
         The creation process should take between 5 and 15 minutes.
-        During this time, GPT iteratively builds your microservice until it finds a strategy that make you test scenario pass.
+        During this time, GPT iteratively builds your microservice until it finds a strategy that make your test scenario pass.
         Once the microservice is created and deployed, you can test it using the generated Streamlit playground.
+        The deployment is made on the Jina`s infrastructure. 
+        When creating a Jina account, you get some free credits, which you can use to deploy your microservice ($0.025/hour).
+        If you run out of credits, you can purchase more.
+        
+        ### Delete Microservice
+        To save credits you can delete your microservice via the following commands:
+        ```bash
+        jc list # get the microservice id
+        jc delete <microservice id>
+        ```
         
         ## Overview
-        The graphic below illustrates the process of creating a microservice and deploying it to the cloud.
+        The graphic below illustrates the process of creating a microservice and deploying it to the cloud elaboration two different implementation strategies.
+        
         ```mermaid
+        
         graph TB
-            AA[Task: Generate QR code from URL] --> B{think a}
-            AB[Test: https://www.example.com] --> B{think a}
-            B -->|Identify Strategie 1| C[Strategy 1]
-            B -->|Identify Strategie 2| D[Strategy 2]
-            B -->|Identify Strategie N| E[Strategy N]
-            C --> F[executor.py, test_executor.py, requirements.txt, Dockerfile]
-            D --> G[executor.py, test_executor.py, requirements.txt, Dockerfile]
-            E --> H[executor.py, test_executor.py, requirements.txt, Dockerfile]
-            F --> I{Build Image}
-            G --> I
-            H --> I
-            I -->|Fail| J[Apply Fix and Retry]
-            J --> I
-            I -->|Success| K[Push Docker Image to Registry]
-            K --> L[Deploy Microservice]
-            L --> M[Create Streamlit Playground]
-            M --> N[User Tests Microservice]
+        
+            description[description: generate QR code from URL] --> make_strat{think a}
+        
+            test[test: https://www.example.com] --> make_strat[generate strategies]
+        
+            make_strat --> implement1[implement strategy 1]
+        
+            implement1 --> build1{build image}
+        
+            build1 -->|error message| implement1
+        
+            build1 -->|failed 10 times| implement2[implement strategy 2]
+        
+            build1 -->|success| registry[push docker image to registry]
+        
+            implement2 --> build2{build image}
+        
+            build2 -->|error message| implement2
+        
+            build2 -->|failed 10 times| all_failed[all strategies failed]
+        
+            build2 -->|success| registry[push docker image to registry]
+        
+            registry --> deploy[deploy microservice]
+        
+            deploy --> streamlit[create streamlit playground]
+        
+            streamlit --> user_run[user tests microservice]
+        
         ```
+        
+        
+        
+        
         1. GPT Deploy identifies several strategies to implement your task.
         2. It tests each strategy until it finds one that works.
         3. For each strategy, it creates the following files:
         - executor.py: This is the main implementation of the microservice.
         - test_executor.py: These are test cases to ensure the microservice works as expected.
         - requirements.txt: This file lists the packages needed by the microservice and its tests.
         - Dockerfile: This file is used to run the microservice in a container and also runs the tests when building the image.
@@ -372,16 +402,18 @@
         Use natural language interface to create, deploy and update your microservice infrastructure.
         
         ## ✨ Contributers 
         If you want to contribute to this project, feel free to open a PR or an issue.
         In the following, you can find a list of things that need to be done.
         
         Critical:
-        - [ ] fix problem with package installation
-        - [ ] add instruction about cleanup of deployments
+        - [ ] check if windows and linux support works
+        - [ ] support gpt3.5-turbo
+        
+        
         
         Nice to have:
         - [ ] hide prompts in normal mode and show them in verbose mode
         - [ ] tests
         - [ ] clean up duplicate code
         - [ ] support popular cloud providers - lambda, cloud run, cloud functions, ...
         - [ ] support local docker builds
@@ -395,14 +427,17 @@
         - [ ] The playground is currently printed twice even if it did not change. 
         Make sure it is only printed twice in case it changed.
         - [ ] allow to update your microservice by providing feedback
         - [ ] bug: it can happen that the code generation is hanging forever - in this case aboard and redo the generation
         - [ ] feat: make playground more stylish by adding attributes like: clean design, beautiful, like it was made by a professional designer, ...
         - [ ] support for other large language models like ChatGLM
         - [ ] for cost savings, it should be possible to insert less context during the code generation of the main functionality - no jina knowledge is required
+        - [ ] use gptdeploy list to show all deployments
+        - [ ] gptdeploy delete to delete a deployment
+        - [ ] gptdeploy update to update a deployment
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.4 Summary: Use natural
+Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.5 Summary: Use natural
 language interface to create, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/gptdeploy Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Description:
         ****** GPT Deploy: One line to create them all ð§ð ******
                                 [Jina NOW logo]
     Turn your natural language descriptions into fully functional, deployed
       microservices with a single command! Your imagination is the limit!
@@ -12,36 +12,44 @@
                          4a03-9af2-3a977fbb014b.mov))
 This project streamlines the creation and deployment of microservices. Simply
 describe your task using natural language, and the system will automatically
 build and deploy your microservice. To ensure the microservice accurately
 aligns with your intended task a test scenario is required. ## Quickstart ###
 Installation ```bash pip install gptdeploy gptdeploy configure --key  ``` If
 you set the environment variable `OPENAI_API_KEY`, the configuration step can
-be skipped. ### run ```bash gptdeploy create --description "Given a PDF, return
-it's text" --test "https://www.africau.edu/images/default/sample.pdf" ``` To
-create your personal microservice two things are required: - A `description` of
-the task you want to accomplish. - A `test` scenario that ensures the
-microservice works as expected. The creation process should take between 5 and
-15 minutes. During this time, GPT iteratively builds your microservice until it
-finds a strategy that make you test scenario pass. Once the microservice is
-created and deployed, you can test it using the generated Streamlit playground.
-## Overview The graphic below illustrates the process of creating a
-microservice and deploying it to the cloud. ```mermaid graph TB AA[Task:
-Generate QR code from URL] --> B{think a} AB[Test: https://www.example.com] --
-> B{think a} B -->|Identify Strategie 1| C[Strategy 1] B -->|Identify Strategie
-2| D[Strategy 2] B -->|Identify Strategie N| E[Strategy N] C --> F[executor.py,
-test_executor.py, requirements.txt, Dockerfile] D --> G[executor.py,
-test_executor.py, requirements.txt, Dockerfile] E --> H[executor.py,
-test_executor.py, requirements.txt, Dockerfile] F --> I{Build Image} G --> I H
---> I I -->|Fail| J[Apply Fix and Retry] J --> I I -->|Success| K[Push Docker
-Image to Registry] K --> L[Deploy Microservice] L --> M[Create Streamlit
-Playground] M --> N[User Tests Microservice] ``` 1. GPT Deploy identifies
-several strategies to implement your task. 2. It tests each strategy until it
-finds one that works. 3. For each strategy, it creates the following files: -
-executor.py: This is the main implementation of the microservice. -
+be skipped. Your api key must have access to gpt-4 to use this tool. We are
+working on a way to use gpt-3.5-turbo as well. ### Create Microservice ```bash
+gptdeploy create --description "Given a PDF, return it's text" --test "https://
+www.africau.edu/images/default/sample.pdf" ``` To create your personal
+microservice two things are required: - A `description` of the task you want to
+accomplish. - A `test` scenario that ensures the microservice works as
+expected. The creation process should take between 5 and 15 minutes. During
+this time, GPT iteratively builds your microservice until it finds a strategy
+that make your test scenario pass. Once the microservice is created and
+deployed, you can test it using the generated Streamlit playground. The
+deployment is made on the Jina`s infrastructure. When creating a Jina account,
+you get some free credits, which you can use to deploy your microservice
+($0.025/hour). If you run out of credits, you can purchase more. ### Delete
+Microservice To save credits you can delete your microservice via the following
+commands: ```bash jc list # get the microservice id jc delete  ``` ## Overview
+The graphic below illustrates the process of creating a microservice and
+deploying it to the cloud elaboration two different implementation strategies.
+```mermaid graph TB description[description: generate QR code from URL] --
+> make_strat{think a} test[test: https://www.example.com] --> make_strat
+[generate strategies] make_strat --> implement1[implement strategy 1]
+implement1 --> build1{build image} build1 -->|error message| implement1 build1
+-->|failed 10 times| implement2[implement strategy 2] build1 -->|success|
+registry[push docker image to registry] implement2 --> build2{build image}
+build2 -->|error message| implement2 build2 -->|failed 10 times| all_failed[all
+strategies failed] build2 -->|success| registry[push docker image to registry]
+registry --> deploy[deploy microservice] deploy --> streamlit[create streamlit
+playground] streamlit --> user_run[user tests microservice] ``` 1. GPT Deploy
+identifies several strategies to implement your task. 2. It tests each strategy
+until it finds one that works. 3. For each strategy, it creates the following
+files: - executor.py: This is the main implementation of the microservice. -
 test_executor.py: These are test cases to ensure the microservice works as
 expected. - requirements.txt: This file lists the packages needed by the
 microservice and its tests. - Dockerfile: This file is used to run the
 microservice in a container and also runs the tests when building the image. 4.
 GPT Deploy attempts to build the image. If the build fails, it uses the error
 message to apply a fix and tries again to build the image. 5. Once it finds a
 successful strategy, it: - Pushes the Docker image to the registry. - Deploys
@@ -142,34 +150,35 @@
 3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-
 assets/master/models/wolf.obj") [//]: # (```) [//]: # () [//]: # (### Bounding
 Box) [//]: # (```bash) [//]: # (gptdeploy create --description "Given an image,
 return the bounding boxes of all animals" --test "...") [//]: # (```) ## ð®
 vision Use natural language interface to create, deploy and update your
 microservice infrastructure. ## â¨ Contributers If you want to contribute to
 this project, feel free to open a PR or an issue. In the following, you can
-find a list of things that need to be done. Critical: - [ ] fix problem with
-package installation - [ ] add instruction about cleanup of deployments Nice to
-have: - [ ] hide prompts in normal mode and show them in verbose mode - [ ]
-tests - [ ] clean up duplicate code - [ ] support popular cloud providers -
-lambda, cloud run, cloud functions, ... - [ ] support local docker builds - [ ]
-autoscaling enabled for cost saving - [ ] don't show this message: ð You are
-logged in to Jina AI as florian.hoenicke (username:auth0-unified-
-448f11965ce142b6). To log out, use jina auth logout. - [ ] add more examples to
-README.md - [ ] support multiple endpoints - example: todolist microservice
-with endpoints for adding, deleting, and listing todos - [ ] support stateful
-microservices - [ ] The playground is currently printed twice even if it did
-not change. Make sure it is only printed twice in case it changed. - [ ] allow
-to update your microservice by providing feedback - [ ] bug: it can happen that
-the code generation is hanging forever - in this case aboard and redo the
-generation - [ ] feat: make playground more stylish by adding attributes like:
-clean design, beautiful, like it was made by a professional designer, ... - [ ]
-support for other large language models like ChatGLM - [ ] for cost savings, it
-should be possible to insert less context during the code generation of the
-main functionality - no jina knowledge is required Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Description-Content-Type:
-text/markdown
+find a list of things that need to be done. Critical: - [ ] check if windows
+and linux support works - [ ] support gpt3.5-turbo Nice to have: - [ ] hide
+prompts in normal mode and show them in verbose mode - [ ] tests - [ ] clean up
+duplicate code - [ ] support popular cloud providers - lambda, cloud run, cloud
+functions, ... - [ ] support local docker builds - [ ] autoscaling enabled for
+cost saving - [ ] don't show this message: ð You are logged in to Jina AI as
+florian.hoenicke (username:auth0-unified-448f11965ce142b6). To log out, use
+jina auth logout. - [ ] add more examples to README.md - [ ] support multiple
+endpoints - example: todolist microservice with endpoints for adding, deleting,
+and listing todos - [ ] support stateful microservices - [ ] The playground is
+currently printed twice even if it did not change. Make sure it is only printed
+twice in case it changed. - [ ] allow to update your microservice by providing
+feedback - [ ] bug: it can happen that the code generation is hanging forever -
+in this case aboard and redo the generation - [ ] feat: make playground more
+stylish by adding attributes like: clean design, beautiful, like it was made by
+a professional designer, ... - [ ] support for other large language models like
+ChatGLM - [ ] for cost savings, it should be possible to insert less context
+during the code generation of the main functionality - no jina knowledge is
+required - [ ] use gptdeploy list to show all deployments - [ ] gptdeploy
+delete to delete a deployment - [ ] gptdeploy update to update a deployment
+Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-
+Content-Type: text/markdown
```

### Comparing `gptdeploy-0.18.4/README.md` & `gptdeploy-0.18.5/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -38,49 +38,79 @@
 ## Quickstart
 ### Installation
 ```bash
 pip install gptdeploy
 gptdeploy configure --key <your openai api key>
 ```
 If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
+Your api key must have access to gpt-4 to use this tool. 
+We are working on a way to use gpt-3.5-turbo as well.
 
-### run
+### Create Microservice
 ```bash
 gptdeploy create --description "Given a PDF, return it's text" --test "https://www.africau.edu/images/default/sample.pdf"
 ```
 To create your personal microservice two things are required:
 - A `description` of the task you want to accomplish.
 - A `test` scenario that ensures the microservice works as expected.
 
 The creation process should take between 5 and 15 minutes.
-During this time, GPT iteratively builds your microservice until it finds a strategy that make you test scenario pass.
+During this time, GPT iteratively builds your microservice until it finds a strategy that make your test scenario pass.
 Once the microservice is created and deployed, you can test it using the generated Streamlit playground.
+The deployment is made on the Jina`s infrastructure. 
+When creating a Jina account, you get some free credits, which you can use to deploy your microservice ($0.025/hour).
+If you run out of credits, you can purchase more.
+
+### Delete Microservice
+To save credits you can delete your microservice via the following commands:
+```bash
+jc list # get the microservice id
+jc delete <microservice id>
+```
 
 ## Overview
-The graphic below illustrates the process of creating a microservice and deploying it to the cloud.
+The graphic below illustrates the process of creating a microservice and deploying it to the cloud elaboration two different implementation strategies.
+
 ```mermaid
+
 graph TB
-    AA[Task: Generate QR code from URL] --> B{think a}
-    AB[Test: https://www.example.com] --> B{think a}
-    B -->|Identify Strategie 1| C[Strategy 1]
-    B -->|Identify Strategie 2| D[Strategy 2]
-    B -->|Identify Strategie N| E[Strategy N]
-    C --> F[executor.py, test_executor.py, requirements.txt, Dockerfile]
-    D --> G[executor.py, test_executor.py, requirements.txt, Dockerfile]
-    E --> H[executor.py, test_executor.py, requirements.txt, Dockerfile]
-    F --> I{Build Image}
-    G --> I
-    H --> I
-    I -->|Fail| J[Apply Fix and Retry]
-    J --> I
-    I -->|Success| K[Push Docker Image to Registry]
-    K --> L[Deploy Microservice]
-    L --> M[Create Streamlit Playground]
-    M --> N[User Tests Microservice]
+
+    description[description: generate QR code from URL] --> make_strat{think a}
+
+    test[test: https://www.example.com] --> make_strat[generate strategies]
+
+    make_strat --> implement1[implement strategy 1]
+
+    implement1 --> build1{build image}
+
+    build1 -->|error message| implement1
+
+    build1 -->|failed 10 times| implement2[implement strategy 2]
+
+    build1 -->|success| registry[push docker image to registry]
+
+    implement2 --> build2{build image}
+
+    build2 -->|error message| implement2
+
+    build2 -->|failed 10 times| all_failed[all strategies failed]
+
+    build2 -->|success| registry[push docker image to registry]
+
+    registry --> deploy[deploy microservice]
+
+    deploy --> streamlit[create streamlit playground]
+
+    streamlit --> user_run[user tests microservice]
+
 ```
+
+
+
+
 1. GPT Deploy identifies several strategies to implement your task.
 2. It tests each strategy until it finds one that works.
 3. For each strategy, it creates the following files:
 - executor.py: This is the main implementation of the microservice.
 - test_executor.py: These are test cases to ensure the microservice works as expected.
 - requirements.txt: This file lists the packages needed by the microservice and its tests.
 - Dockerfile: This file is used to run the microservice in a container and also runs the tests when building the image.
@@ -364,16 +394,18 @@
 Use natural language interface to create, deploy and update your microservice infrastructure.
 
 ## ✨ Contributers 
 If you want to contribute to this project, feel free to open a PR or an issue.
 In the following, you can find a list of things that need to be done.
 
 Critical:
-- [ ] fix problem with package installation
-- [ ] add instruction about cleanup of deployments
+- [ ] check if windows and linux support works
+- [ ] support gpt3.5-turbo
+
+
 
 Nice to have:
 - [ ] hide prompts in normal mode and show them in verbose mode
 - [ ] tests
 - [ ] clean up duplicate code
 - [ ] support popular cloud providers - lambda, cloud run, cloud functions, ...
 - [ ] support local docker builds
@@ -387,7 +419,10 @@
 - [ ] The playground is currently printed twice even if it did not change. 
 Make sure it is only printed twice in case it changed.
 - [ ] allow to update your microservice by providing feedback
 - [ ] bug: it can happen that the code generation is hanging forever - in this case aboard and redo the generation
 - [ ] feat: make playground more stylish by adding attributes like: clean design, beautiful, like it was made by a professional designer, ...
 - [ ] support for other large language models like ChatGLM
 - [ ] for cost savings, it should be possible to insert less context during the code generation of the main functionality - no jina knowledge is required
+- [ ] use gptdeploy list to show all deployments
+- [ ] gptdeploy delete to delete a deployment
+- [ ] gptdeploy update to update a deployment
```

#### html2text {}

```diff
@@ -8,36 +8,44 @@
                          4a03-9af2-3a977fbb014b.mov))
 This project streamlines the creation and deployment of microservices. Simply
 describe your task using natural language, and the system will automatically
 build and deploy your microservice. To ensure the microservice accurately
 aligns with your intended task a test scenario is required. ## Quickstart ###
 Installation ```bash pip install gptdeploy gptdeploy configure --key  ``` If
 you set the environment variable `OPENAI_API_KEY`, the configuration step can
-be skipped. ### run ```bash gptdeploy create --description "Given a PDF, return
-it's text" --test "https://www.africau.edu/images/default/sample.pdf" ``` To
-create your personal microservice two things are required: - A `description` of
-the task you want to accomplish. - A `test` scenario that ensures the
-microservice works as expected. The creation process should take between 5 and
-15 minutes. During this time, GPT iteratively builds your microservice until it
-finds a strategy that make you test scenario pass. Once the microservice is
-created and deployed, you can test it using the generated Streamlit playground.
-## Overview The graphic below illustrates the process of creating a
-microservice and deploying it to the cloud. ```mermaid graph TB AA[Task:
-Generate QR code from URL] --> B{think a} AB[Test: https://www.example.com] --
-> B{think a} B -->|Identify Strategie 1| C[Strategy 1] B -->|Identify Strategie
-2| D[Strategy 2] B -->|Identify Strategie N| E[Strategy N] C --> F[executor.py,
-test_executor.py, requirements.txt, Dockerfile] D --> G[executor.py,
-test_executor.py, requirements.txt, Dockerfile] E --> H[executor.py,
-test_executor.py, requirements.txt, Dockerfile] F --> I{Build Image} G --> I H
---> I I -->|Fail| J[Apply Fix and Retry] J --> I I -->|Success| K[Push Docker
-Image to Registry] K --> L[Deploy Microservice] L --> M[Create Streamlit
-Playground] M --> N[User Tests Microservice] ``` 1. GPT Deploy identifies
-several strategies to implement your task. 2. It tests each strategy until it
-finds one that works. 3. For each strategy, it creates the following files: -
-executor.py: This is the main implementation of the microservice. -
+be skipped. Your api key must have access to gpt-4 to use this tool. We are
+working on a way to use gpt-3.5-turbo as well. ### Create Microservice ```bash
+gptdeploy create --description "Given a PDF, return it's text" --test "https://
+www.africau.edu/images/default/sample.pdf" ``` To create your personal
+microservice two things are required: - A `description` of the task you want to
+accomplish. - A `test` scenario that ensures the microservice works as
+expected. The creation process should take between 5 and 15 minutes. During
+this time, GPT iteratively builds your microservice until it finds a strategy
+that make your test scenario pass. Once the microservice is created and
+deployed, you can test it using the generated Streamlit playground. The
+deployment is made on the Jina`s infrastructure. When creating a Jina account,
+you get some free credits, which you can use to deploy your microservice
+($0.025/hour). If you run out of credits, you can purchase more. ### Delete
+Microservice To save credits you can delete your microservice via the following
+commands: ```bash jc list # get the microservice id jc delete  ``` ## Overview
+The graphic below illustrates the process of creating a microservice and
+deploying it to the cloud elaboration two different implementation strategies.
+```mermaid graph TB description[description: generate QR code from URL] --
+> make_strat{think a} test[test: https://www.example.com] --> make_strat
+[generate strategies] make_strat --> implement1[implement strategy 1]
+implement1 --> build1{build image} build1 -->|error message| implement1 build1
+-->|failed 10 times| implement2[implement strategy 2] build1 -->|success|
+registry[push docker image to registry] implement2 --> build2{build image}
+build2 -->|error message| implement2 build2 -->|failed 10 times| all_failed[all
+strategies failed] build2 -->|success| registry[push docker image to registry]
+registry --> deploy[deploy microservice] deploy --> streamlit[create streamlit
+playground] streamlit --> user_run[user tests microservice] ``` 1. GPT Deploy
+identifies several strategies to implement your task. 2. It tests each strategy
+until it finds one that works. 3. For each strategy, it creates the following
+files: - executor.py: This is the main implementation of the microservice. -
 test_executor.py: These are test cases to ensure the microservice works as
 expected. - requirements.txt: This file lists the packages needed by the
 microservice and its tests. - Dockerfile: This file is used to run the
 microservice in a container and also runs the tests when building the image. 4.
 GPT Deploy attempts to build the image. If the build fails, it uses the error
 message to apply a fix and tries again to build the image. 5. Once it finds a
 successful strategy, it: - Pushes the Docker image to the registry. - Deploys
@@ -138,26 +146,27 @@
 3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-
 assets/master/models/wolf.obj") [//]: # (```) [//]: # () [//]: # (### Bounding
 Box) [//]: # (```bash) [//]: # (gptdeploy create --description "Given an image,
 return the bounding boxes of all animals" --test "...") [//]: # (```) ## ð®
 vision Use natural language interface to create, deploy and update your
 microservice infrastructure. ## â¨ Contributers If you want to contribute to
 this project, feel free to open a PR or an issue. In the following, you can
-find a list of things that need to be done. Critical: - [ ] fix problem with
-package installation - [ ] add instruction about cleanup of deployments Nice to
-have: - [ ] hide prompts in normal mode and show them in verbose mode - [ ]
-tests - [ ] clean up duplicate code - [ ] support popular cloud providers -
-lambda, cloud run, cloud functions, ... - [ ] support local docker builds - [ ]
-autoscaling enabled for cost saving - [ ] don't show this message: ð You are
-logged in to Jina AI as florian.hoenicke (username:auth0-unified-
-448f11965ce142b6). To log out, use jina auth logout. - [ ] add more examples to
-README.md - [ ] support multiple endpoints - example: todolist microservice
-with endpoints for adding, deleting, and listing todos - [ ] support stateful
-microservices - [ ] The playground is currently printed twice even if it did
-not change. Make sure it is only printed twice in case it changed. - [ ] allow
-to update your microservice by providing feedback - [ ] bug: it can happen that
-the code generation is hanging forever - in this case aboard and redo the
-generation - [ ] feat: make playground more stylish by adding attributes like:
-clean design, beautiful, like it was made by a professional designer, ... - [ ]
-support for other large language models like ChatGLM - [ ] for cost savings, it
-should be possible to insert less context during the code generation of the
-main functionality - no jina knowledge is required
+find a list of things that need to be done. Critical: - [ ] check if windows
+and linux support works - [ ] support gpt3.5-turbo Nice to have: - [ ] hide
+prompts in normal mode and show them in verbose mode - [ ] tests - [ ] clean up
+duplicate code - [ ] support popular cloud providers - lambda, cloud run, cloud
+functions, ... - [ ] support local docker builds - [ ] autoscaling enabled for
+cost saving - [ ] don't show this message: ð You are logged in to Jina AI as
+florian.hoenicke (username:auth0-unified-448f11965ce142b6). To log out, use
+jina auth logout. - [ ] add more examples to README.md - [ ] support multiple
+endpoints - example: todolist microservice with endpoints for adding, deleting,
+and listing todos - [ ] support stateful microservices - [ ] The playground is
+currently printed twice even if it did not change. Make sure it is only printed
+twice in case it changed. - [ ] allow to update your microservice by providing
+feedback - [ ] bug: it can happen that the code generation is hanging forever -
+in this case aboard and redo the generation - [ ] feat: make playground more
+stylish by adding attributes like: clean design, beautiful, like it was made by
+a professional designer, ... - [ ] support for other large language models like
+ChatGLM - [ ] for cost savings, it should be possible to insert less context
+during the code generation of the main functionality - no jina knowledge is
+required - [ ] use gptdeploy list to show all deployments - [ ] gptdeploy
+delete to delete a deployment - [ ] gptdeploy update to update a deployment
```

### Comparing `gptdeploy-0.18.4/gptdeploy.egg-info/PKG-INFO` & `gptdeploy-0.18.5/gptdeploy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gptdeploy
-Version: 0.18.4
+Version: 0.18.5
 Summary: Use natural language interface to create, deploy and update your microservice infrastructure.
 Home-page: https://github.com/jina-ai/gptdeploy
 Author: Florian Hönicke
 Author-email: florian.hoenicke@jina.ai
 License: UNKNOWN
 Description: <h1 align="center">
         GPT Deploy: One line to create them all 🧙🚀
@@ -46,49 +46,79 @@
         ## Quickstart
         ### Installation
         ```bash
         pip install gptdeploy
         gptdeploy configure --key <your openai api key>
         ```
         If you set the environment variable `OPENAI_API_KEY`, the configuration step can be skipped.
+        Your api key must have access to gpt-4 to use this tool. 
+        We are working on a way to use gpt-3.5-turbo as well.
         
-        ### run
+        ### Create Microservice
         ```bash
         gptdeploy create --description "Given a PDF, return it's text" --test "https://www.africau.edu/images/default/sample.pdf"
         ```
         To create your personal microservice two things are required:
         - A `description` of the task you want to accomplish.
         - A `test` scenario that ensures the microservice works as expected.
         
         The creation process should take between 5 and 15 minutes.
-        During this time, GPT iteratively builds your microservice until it finds a strategy that make you test scenario pass.
+        During this time, GPT iteratively builds your microservice until it finds a strategy that make your test scenario pass.
         Once the microservice is created and deployed, you can test it using the generated Streamlit playground.
+        The deployment is made on the Jina`s infrastructure. 
+        When creating a Jina account, you get some free credits, which you can use to deploy your microservice ($0.025/hour).
+        If you run out of credits, you can purchase more.
+        
+        ### Delete Microservice
+        To save credits you can delete your microservice via the following commands:
+        ```bash
+        jc list # get the microservice id
+        jc delete <microservice id>
+        ```
         
         ## Overview
-        The graphic below illustrates the process of creating a microservice and deploying it to the cloud.
+        The graphic below illustrates the process of creating a microservice and deploying it to the cloud elaboration two different implementation strategies.
+        
         ```mermaid
+        
         graph TB
-            AA[Task: Generate QR code from URL] --> B{think a}
-            AB[Test: https://www.example.com] --> B{think a}
-            B -->|Identify Strategie 1| C[Strategy 1]
-            B -->|Identify Strategie 2| D[Strategy 2]
-            B -->|Identify Strategie N| E[Strategy N]
-            C --> F[executor.py, test_executor.py, requirements.txt, Dockerfile]
-            D --> G[executor.py, test_executor.py, requirements.txt, Dockerfile]
-            E --> H[executor.py, test_executor.py, requirements.txt, Dockerfile]
-            F --> I{Build Image}
-            G --> I
-            H --> I
-            I -->|Fail| J[Apply Fix and Retry]
-            J --> I
-            I -->|Success| K[Push Docker Image to Registry]
-            K --> L[Deploy Microservice]
-            L --> M[Create Streamlit Playground]
-            M --> N[User Tests Microservice]
+        
+            description[description: generate QR code from URL] --> make_strat{think a}
+        
+            test[test: https://www.example.com] --> make_strat[generate strategies]
+        
+            make_strat --> implement1[implement strategy 1]
+        
+            implement1 --> build1{build image}
+        
+            build1 -->|error message| implement1
+        
+            build1 -->|failed 10 times| implement2[implement strategy 2]
+        
+            build1 -->|success| registry[push docker image to registry]
+        
+            implement2 --> build2{build image}
+        
+            build2 -->|error message| implement2
+        
+            build2 -->|failed 10 times| all_failed[all strategies failed]
+        
+            build2 -->|success| registry[push docker image to registry]
+        
+            registry --> deploy[deploy microservice]
+        
+            deploy --> streamlit[create streamlit playground]
+        
+            streamlit --> user_run[user tests microservice]
+        
         ```
+        
+        
+        
+        
         1. GPT Deploy identifies several strategies to implement your task.
         2. It tests each strategy until it finds one that works.
         3. For each strategy, it creates the following files:
         - executor.py: This is the main implementation of the microservice.
         - test_executor.py: These are test cases to ensure the microservice works as expected.
         - requirements.txt: This file lists the packages needed by the microservice and its tests.
         - Dockerfile: This file is used to run the microservice in a container and also runs the tests when building the image.
@@ -372,16 +402,18 @@
         Use natural language interface to create, deploy and update your microservice infrastructure.
         
         ## ✨ Contributers 
         If you want to contribute to this project, feel free to open a PR or an issue.
         In the following, you can find a list of things that need to be done.
         
         Critical:
-        - [ ] fix problem with package installation
-        - [ ] add instruction about cleanup of deployments
+        - [ ] check if windows and linux support works
+        - [ ] support gpt3.5-turbo
+        
+        
         
         Nice to have:
         - [ ] hide prompts in normal mode and show them in verbose mode
         - [ ] tests
         - [ ] clean up duplicate code
         - [ ] support popular cloud providers - lambda, cloud run, cloud functions, ...
         - [ ] support local docker builds
@@ -395,14 +427,17 @@
         - [ ] The playground is currently printed twice even if it did not change. 
         Make sure it is only printed twice in case it changed.
         - [ ] allow to update your microservice by providing feedback
         - [ ] bug: it can happen that the code generation is hanging forever - in this case aboard and redo the generation
         - [ ] feat: make playground more stylish by adding attributes like: clean design, beautiful, like it was made by a professional designer, ...
         - [ ] support for other large language models like ChatGLM
         - [ ] for cost savings, it should be possible to insert less context during the code generation of the main functionality - no jina knowledge is required
+        - [ ] use gptdeploy list to show all deployments
+        - [ ] gptdeploy delete to delete a deployment
+        - [ ] gptdeploy update to update a deployment
         
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.4 Summary: Use natural
+Metadata-Version: 2.1 Name: gptdeploy Version: 0.18.5 Summary: Use natural
 language interface to create, deploy and update your microservice
 infrastructure. Home-page: https://github.com/jina-ai/gptdeploy Author: Florian
 HÃ¶nicke Author-email: florian.hoenicke@jina.ai License: UNKNOWN Description:
         ****** GPT Deploy: One line to create them all ð§ð ******
                                 [Jina NOW logo]
     Turn your natural language descriptions into fully functional, deployed
       microservices with a single command! Your imagination is the limit!
@@ -12,36 +12,44 @@
                          4a03-9af2-3a977fbb014b.mov))
 This project streamlines the creation and deployment of microservices. Simply
 describe your task using natural language, and the system will automatically
 build and deploy your microservice. To ensure the microservice accurately
 aligns with your intended task a test scenario is required. ## Quickstart ###
 Installation ```bash pip install gptdeploy gptdeploy configure --key  ``` If
 you set the environment variable `OPENAI_API_KEY`, the configuration step can
-be skipped. ### run ```bash gptdeploy create --description "Given a PDF, return
-it's text" --test "https://www.africau.edu/images/default/sample.pdf" ``` To
-create your personal microservice two things are required: - A `description` of
-the task you want to accomplish. - A `test` scenario that ensures the
-microservice works as expected. The creation process should take between 5 and
-15 minutes. During this time, GPT iteratively builds your microservice until it
-finds a strategy that make you test scenario pass. Once the microservice is
-created and deployed, you can test it using the generated Streamlit playground.
-## Overview The graphic below illustrates the process of creating a
-microservice and deploying it to the cloud. ```mermaid graph TB AA[Task:
-Generate QR code from URL] --> B{think a} AB[Test: https://www.example.com] --
-> B{think a} B -->|Identify Strategie 1| C[Strategy 1] B -->|Identify Strategie
-2| D[Strategy 2] B -->|Identify Strategie N| E[Strategy N] C --> F[executor.py,
-test_executor.py, requirements.txt, Dockerfile] D --> G[executor.py,
-test_executor.py, requirements.txt, Dockerfile] E --> H[executor.py,
-test_executor.py, requirements.txt, Dockerfile] F --> I{Build Image} G --> I H
---> I I -->|Fail| J[Apply Fix and Retry] J --> I I -->|Success| K[Push Docker
-Image to Registry] K --> L[Deploy Microservice] L --> M[Create Streamlit
-Playground] M --> N[User Tests Microservice] ``` 1. GPT Deploy identifies
-several strategies to implement your task. 2. It tests each strategy until it
-finds one that works. 3. For each strategy, it creates the following files: -
-executor.py: This is the main implementation of the microservice. -
+be skipped. Your api key must have access to gpt-4 to use this tool. We are
+working on a way to use gpt-3.5-turbo as well. ### Create Microservice ```bash
+gptdeploy create --description "Given a PDF, return it's text" --test "https://
+www.africau.edu/images/default/sample.pdf" ``` To create your personal
+microservice two things are required: - A `description` of the task you want to
+accomplish. - A `test` scenario that ensures the microservice works as
+expected. The creation process should take between 5 and 15 minutes. During
+this time, GPT iteratively builds your microservice until it finds a strategy
+that make your test scenario pass. Once the microservice is created and
+deployed, you can test it using the generated Streamlit playground. The
+deployment is made on the Jina`s infrastructure. When creating a Jina account,
+you get some free credits, which you can use to deploy your microservice
+($0.025/hour). If you run out of credits, you can purchase more. ### Delete
+Microservice To save credits you can delete your microservice via the following
+commands: ```bash jc list # get the microservice id jc delete  ``` ## Overview
+The graphic below illustrates the process of creating a microservice and
+deploying it to the cloud elaboration two different implementation strategies.
+```mermaid graph TB description[description: generate QR code from URL] --
+> make_strat{think a} test[test: https://www.example.com] --> make_strat
+[generate strategies] make_strat --> implement1[implement strategy 1]
+implement1 --> build1{build image} build1 -->|error message| implement1 build1
+-->|failed 10 times| implement2[implement strategy 2] build1 -->|success|
+registry[push docker image to registry] implement2 --> build2{build image}
+build2 -->|error message| implement2 build2 -->|failed 10 times| all_failed[all
+strategies failed] build2 -->|success| registry[push docker image to registry]
+registry --> deploy[deploy microservice] deploy --> streamlit[create streamlit
+playground] streamlit --> user_run[user tests microservice] ``` 1. GPT Deploy
+identifies several strategies to implement your task. 2. It tests each strategy
+until it finds one that works. 3. For each strategy, it creates the following
+files: - executor.py: This is the main implementation of the microservice. -
 test_executor.py: These are test cases to ensure the microservice works as
 expected. - requirements.txt: This file lists the packages needed by the
 microservice and its tests. - Dockerfile: This file is used to run the
 microservice in a container and also runs the tests when building the image. 4.
 GPT Deploy attempts to build the image. If the build fails, it uses the error
 message to apply a fix and tries again to build the image. 5. Once it finds a
 successful strategy, it: - Pushes the Docker image to the registry. - Deploys
@@ -142,34 +150,35 @@
 3d Object" --test "https://raw.githubusercontent.com/polygonjs/polygonjs-
 assets/master/models/wolf.obj") [//]: # (```) [//]: # () [//]: # (### Bounding
 Box) [//]: # (```bash) [//]: # (gptdeploy create --description "Given an image,
 return the bounding boxes of all animals" --test "...") [//]: # (```) ## ð®
 vision Use natural language interface to create, deploy and update your
 microservice infrastructure. ## â¨ Contributers If you want to contribute to
 this project, feel free to open a PR or an issue. In the following, you can
-find a list of things that need to be done. Critical: - [ ] fix problem with
-package installation - [ ] add instruction about cleanup of deployments Nice to
-have: - [ ] hide prompts in normal mode and show them in verbose mode - [ ]
-tests - [ ] clean up duplicate code - [ ] support popular cloud providers -
-lambda, cloud run, cloud functions, ... - [ ] support local docker builds - [ ]
-autoscaling enabled for cost saving - [ ] don't show this message: ð You are
-logged in to Jina AI as florian.hoenicke (username:auth0-unified-
-448f11965ce142b6). To log out, use jina auth logout. - [ ] add more examples to
-README.md - [ ] support multiple endpoints - example: todolist microservice
-with endpoints for adding, deleting, and listing todos - [ ] support stateful
-microservices - [ ] The playground is currently printed twice even if it did
-not change. Make sure it is only printed twice in case it changed. - [ ] allow
-to update your microservice by providing feedback - [ ] bug: it can happen that
-the code generation is hanging forever - in this case aboard and redo the
-generation - [ ] feat: make playground more stylish by adding attributes like:
-clean design, beautiful, like it was made by a professional designer, ... - [ ]
-support for other large language models like ChatGLM - [ ] for cost savings, it
-should be possible to insert less context during the code generation of the
-main functionality - no jina knowledge is required Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha Classifier: Intended Audience ::
-Developers Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3 Classifier: Programming
-Language :: Python :: 3.6 Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Description-Content-Type:
-text/markdown
+find a list of things that need to be done. Critical: - [ ] check if windows
+and linux support works - [ ] support gpt3.5-turbo Nice to have: - [ ] hide
+prompts in normal mode and show them in verbose mode - [ ] tests - [ ] clean up
+duplicate code - [ ] support popular cloud providers - lambda, cloud run, cloud
+functions, ... - [ ] support local docker builds - [ ] autoscaling enabled for
+cost saving - [ ] don't show this message: ð You are logged in to Jina AI as
+florian.hoenicke (username:auth0-unified-448f11965ce142b6). To log out, use
+jina auth logout. - [ ] add more examples to README.md - [ ] support multiple
+endpoints - example: todolist microservice with endpoints for adding, deleting,
+and listing todos - [ ] support stateful microservices - [ ] The playground is
+currently printed twice even if it did not change. Make sure it is only printed
+twice in case it changed. - [ ] allow to update your microservice by providing
+feedback - [ ] bug: it can happen that the code generation is hanging forever -
+in this case aboard and redo the generation - [ ] feat: make playground more
+stylish by adding attributes like: clean design, beautiful, like it was made by
+a professional designer, ... - [ ] support for other large language models like
+ChatGLM - [ ] for cost savings, it should be possible to insert less context
+during the code generation of the main functionality - no jina knowledge is
+required - [ ] use gptdeploy list to show all deployments - [ ] gptdeploy
+delete to delete a deployment - [ ] gptdeploy update to update a deployment
+Platform: UNKNOWN Classifier: Development Status :: 3 - Alpha Classifier:
+Intended Audience :: Developers Classifier: License :: OSI Approved :: Apache
+Software License Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.6 Classifier: Programming Language ::
+Python :: 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Description-
+Content-Type: text/markdown
```

### Comparing `gptdeploy-0.18.4/setup.py` & `gptdeploy-0.18.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 def read_requirements():
     with open('requirements.txt', 'r', encoding='utf-8') as f:
         return [line.strip() for line in f.readlines() if not line.startswith('#')]
 
 
 setup(
     name='gptdeploy',
-    version='0.18.4',
+    version='0.18.5',
     description='Use natural language interface to create, deploy and update your microservice infrastructure.',
     long_description=open('README.md', 'r', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Florian Hönicke',
     author_email='florian.hoenicke@jina.ai',
     url='https://github.com/jina-ai/gptdeploy',
     packages=find_packages(),
```

### Comparing `gptdeploy-0.18.4/src/constants.py` & `gptdeploy-0.18.5/src/constants.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.4/src/gpt.py` & `gptdeploy-0.18.5/src/gpt.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.4/src/jina_cloud.py` & `gptdeploy-0.18.5/src/jina_cloud.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.4/src/main.py` & `gptdeploy-0.18.5/src/executor_factory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,262 +1,259 @@
 import random
 
-import click
-
 from src import gpt, jina_cloud
-from src.jina_cloud import push_executor, process_error_message, jina_auth_login
-from src.key_handling import set_api_key
+from src.jina_cloud import push_executor, process_error_message
 from src.prompt_tasks import general_guidelines, executor_file_task, chain_of_thought_creation, test_executor_file_task, \
     chain_of_thought_optimization, requirements_file_task, docker_file_task, not_allowed
 from src.utils.io import recreate_folder, persist_file
 from src.utils.string_tools import print_colored
 
-
 import os
 import re
 
 from src.constants import FILE_AND_TAG_PAIRS
 
-gpt_session = gpt.GPTSession()
 
-def extract_content_from_result(plain_text, file_name):
-    pattern = fr"^\*\*{file_name}\*\*\n```(?:\w+\n)?([\s\S]*?)```"
-    match = re.search(pattern, plain_text, re.MULTILINE)
-    if match:
-        return match.group(1).strip()
-    else:
-        return ''
-
-def write_config_yml(executor_name, dest_folder):
-    config_content = f'''
-jtype: {executor_name}
-py_modules:
-  - executor.py
-metas:
-  name: {executor_name}
-    '''
-    with open(os.path.join(dest_folder, 'config.yml'), 'w') as f:
-        f.write(config_content)
-
-def get_all_executor_files_with_content(folder_path):
-    file_name_to_content = {}
-    for filename in os.listdir(folder_path):
-        file_path = os.path.join(folder_path, filename)
-
-        if os.path.isfile(file_path):
-            with open(file_path, 'r', encoding='utf-8') as file:
-                content = file.read()
-                file_name_to_content[filename] = content
-
-    return file_name_to_content
-
-def files_to_string(file_name_to_content):
-    all_executor_files_string = ''
-    for file_name, tag in FILE_AND_TAG_PAIRS:
-        if file_name in file_name_to_content:
-            all_executor_files_string += f'**{file_name}**\n'
-            all_executor_files_string += f'```{tag}\n'
-            all_executor_files_string += file_name_to_content[file_name]
-            all_executor_files_string += '\n```\n\n'
-    return all_executor_files_string
-
-
-def wrap_content_in_code_block(executor_content, file_name, tag):
-    return f'**{file_name}**\n```{tag}\n{executor_content}\n```\n\n'
-
-
-def create_executor(
-        description,
-        test,
-        output_path,
-        executor_name,
-        package,
-        is_chain_of_thought=False,
-):
-    EXECUTOR_FOLDER_v1 = get_executor_path(output_path, package, 1)
-    recreate_folder(EXECUTOR_FOLDER_v1)
-    recreate_folder('../flow')
-
-    print_colored('', '############# Executor #############', 'red')
-    user_query = (
-            general_guidelines()
-            + executor_file_task(executor_name, description, test, package)
-            + chain_of_thought_creation()
-    )
-    conversation = gpt_session.get_conversation()
-    executor_content_raw = conversation.query(user_query)
-    if is_chain_of_thought:
-        executor_content_raw = conversation.query(
-            f"General rules: " + not_allowed() + chain_of_thought_optimization('python', 'executor.py'))
-    executor_content = extract_content_from_result(executor_content_raw, 'executor.py')
-
-    persist_file(executor_content, os.path.join(EXECUTOR_FOLDER_v1, 'executor.py'))
-
-    print_colored('', '############# Test Executor #############', 'red')
-    user_query = (
-            general_guidelines()
-            + wrap_content_in_code_block(executor_content, 'executor.py', 'python')
-            + test_executor_file_task(executor_name, test)
-    )
-    conversation = gpt_session.get_conversation()
-    test_executor_content_raw = conversation.query(user_query)
-    if is_chain_of_thought:
-        test_executor_content_raw = conversation.query(
-            f"General rules: " + not_allowed() +
-            chain_of_thought_optimization('python', 'test_executor.py')
-            + "Don't add any additional tests. "
+class ExecutorFactory:
+    def __init__(self):
+        self.gpt_session = gpt.GPTSession()
+
+    def extract_content_from_result(self, plain_text, file_name):
+        pattern = fr"^\*\*{file_name}\*\*\n```(?:\w+\n)?([\s\S]*?)```"
+        match = re.search(pattern, plain_text, re.MULTILINE)
+        if match:
+            return match.group(1).strip()
+        else:
+            return ''
+
+    def write_config_yml(self, executor_name, dest_folder):
+        config_content = f'''
+    jtype: {executor_name}
+    py_modules:
+      - executor.py
+    metas:
+      name: {executor_name}
+        '''
+        with open(os.path.join(dest_folder, 'config.yml'), 'w') as f:
+            f.write(config_content)
+
+    def get_all_executor_files_with_content(self, folder_path):
+        file_name_to_content = {}
+        for filename in os.listdir(folder_path):
+            file_path = os.path.join(folder_path, filename)
+
+            if os.path.isfile(file_path):
+                with open(file_path, 'r', encoding='utf-8') as file:
+                    content = file.read()
+                    file_name_to_content[filename] = content
+
+        return file_name_to_content
+
+    def files_to_string(self, file_name_to_content):
+        all_executor_files_string = ''
+        for file_name, tag in FILE_AND_TAG_PAIRS:
+            if file_name in file_name_to_content:
+                all_executor_files_string += f'**{file_name}**\n'
+                all_executor_files_string += f'```{tag}\n'
+                all_executor_files_string += file_name_to_content[file_name]
+                all_executor_files_string += '\n```\n\n'
+        return all_executor_files_string
+
+    def wrap_content_in_code_block(self, executor_content, file_name, tag):
+        return f'**{file_name}**\n```{tag}\n{executor_content}\n```\n\n'
+
+    def create_executor(
+            self,
+            description,
+            test,
+            output_path,
+            executor_name,
+            package,
+            is_chain_of_thought=False,
+    ):
+        EXECUTOR_FOLDER_v1 = self.get_executor_path(output_path, package, 1)
+        recreate_folder(EXECUTOR_FOLDER_v1)
+        recreate_folder('../flow')
+
+        print_colored('', '############# Executor #############', 'red')
+        user_query = (
+                general_guidelines()
+                + executor_file_task(executor_name, description, test, package)
+                + chain_of_thought_creation()
+        )
+        conversation = self.gpt_session.get_conversation()
+        executor_content_raw = conversation.query(user_query)
+        if is_chain_of_thought:
+            executor_content_raw = conversation.query(
+                f"General rules: " + not_allowed() + chain_of_thought_optimization('python', 'executor.py'))
+        executor_content = self.extract_content_from_result(executor_content_raw, 'executor.py')
+
+        persist_file(executor_content, os.path.join(EXECUTOR_FOLDER_v1, 'executor.py'))
+
+        print_colored('', '############# Test Executor #############', 'red')
+        user_query = (
+                general_guidelines()
+                + self.wrap_content_in_code_block(executor_content, 'executor.py', 'python')
+                + test_executor_file_task(executor_name, test)
         )
-    test_executor_content = extract_content_from_result(test_executor_content_raw, 'test_executor.py')
-    persist_file(test_executor_content, os.path.join(EXECUTOR_FOLDER_v1, 'test_executor.py'))
+        conversation = self.gpt_session.get_conversation()
+        test_executor_content_raw = conversation.query(user_query)
+        if is_chain_of_thought:
+            test_executor_content_raw = conversation.query(
+                f"General rules: " + not_allowed() +
+                chain_of_thought_optimization('python', 'test_executor.py')
+                + "Don't add any additional tests. "
+            )
+        test_executor_content = self.extract_content_from_result(test_executor_content_raw, 'test_executor.py')
+        persist_file(test_executor_content, os.path.join(EXECUTOR_FOLDER_v1, 'test_executor.py'))
 
-    print_colored('', '############# Requirements #############', 'red')
-    user_query = (
-            general_guidelines()
-            + wrap_content_in_code_block(executor_content, 'executor.py', 'python')
-            + wrap_content_in_code_block(test_executor_content, 'test_executor.py', 'python')
-            + requirements_file_task()
-    )
-    conversation = gpt_session.get_conversation()
-    requirements_content_raw = conversation.query(user_query)
-    if is_chain_of_thought:
-        requirements_content_raw = conversation.query(
-            chain_of_thought_optimization('', '../requirements.txt') + "Keep the same version of jina ")
-
-    requirements_content = extract_content_from_result(requirements_content_raw, '../requirements.txt')
-    persist_file(requirements_content, os.path.join(EXECUTOR_FOLDER_v1, '../requirements.txt'))
-
-    print_colored('', '############# Dockerfile #############', 'red')
-    user_query = (
-            general_guidelines()
-            + wrap_content_in_code_block(executor_content, 'executor.py', 'python')
-            + wrap_content_in_code_block(test_executor_content, 'test_executor.py', 'python')
-            + wrap_content_in_code_block(requirements_content, '../requirements.txt', '')
-            + docker_file_task()
-    )
-    conversation = gpt_session.get_conversation()
-    dockerfile_content_raw = conversation.query(user_query)
-    if is_chain_of_thought:
-        dockerfile_content_raw = conversation.query(
-            f"General rules: " + not_allowed() + chain_of_thought_optimization('dockerfile', 'Dockerfile'))
-    dockerfile_content = extract_content_from_result(dockerfile_content_raw, 'Dockerfile')
-    persist_file(dockerfile_content, os.path.join(EXECUTOR_FOLDER_v1, 'Dockerfile'))
-
-    write_config_yml(executor_name, EXECUTOR_FOLDER_v1)
-
-
-def create_playground(executor_name, executor_path, host):
-    print_colored('', '############# Playground #############', 'red')
-
-    file_name_to_content = get_all_executor_files_with_content(executor_path)
-    user_query = (
-            general_guidelines()
-            + wrap_content_in_code_block(file_name_to_content['executor.py'], 'executor.py', 'python')
-            + wrap_content_in_code_block(file_name_to_content['test_executor.py'], 'test_executor.py', 'python')
-            + f'''
+        print_colored('', '############# Requirements #############', 'red')
+        user_query = (
+                general_guidelines()
+                + self.wrap_content_in_code_block(executor_content, 'executor.py', 'python')
+                + self.wrap_content_in_code_block(test_executor_content, 'test_executor.py', 'python')
+                + requirements_file_task()
+        )
+        conversation = self.gpt_session.get_conversation()
+        requirements_content_raw = conversation.query(user_query)
+        if is_chain_of_thought:
+            requirements_content_raw = conversation.query(
+                chain_of_thought_optimization('', '../requirements.txt') + "Keep the same version of jina ")
+
+        requirements_content = self.extract_content_from_result(requirements_content_raw, '../requirements.txt')
+        persist_file(requirements_content, os.path.join(EXECUTOR_FOLDER_v1, '../requirements.txt'))
+
+        print_colored('', '############# Dockerfile #############', 'red')
+        user_query = (
+                general_guidelines()
+                + self.wrap_content_in_code_block(executor_content, 'executor.py', 'python')
+                + self.wrap_content_in_code_block(test_executor_content, 'test_executor.py', 'python')
+                + self.wrap_content_in_code_block(requirements_content, '../requirements.txt', '')
+                + docker_file_task()
+        )
+        conversation = self.gpt_session.get_conversation()
+        dockerfile_content_raw = conversation.query(user_query)
+        if is_chain_of_thought:
+            dockerfile_content_raw = conversation.query(
+                f"General rules: " + not_allowed() + chain_of_thought_optimization('dockerfile', 'Dockerfile'))
+        dockerfile_content = self.extract_content_from_result(dockerfile_content_raw, 'Dockerfile')
+        persist_file(dockerfile_content, os.path.join(EXECUTOR_FOLDER_v1, 'Dockerfile'))
+
+        self.write_config_yml(executor_name, EXECUTOR_FOLDER_v1)
+
+    def create_playground(self, executor_name, executor_path, host):
+        print_colored('', '############# Playground #############', 'red')
+
+        file_name_to_content = self.get_all_executor_files_with_content(executor_path)
+        user_query = (
+                general_guidelines()
+                + self.wrap_content_in_code_block(file_name_to_content['executor.py'], 'executor.py', 'python')
+                + self.wrap_content_in_code_block(file_name_to_content['test_executor.py'], 'test_executor.py',
+                                                  'python')
+                + f'''
 Create a playground for the executor {executor_name} using streamlit.
 The playground must look like it was made by a professional designer.
 All the ui elements are well thought out to make them visually appealing and easy to use.
 The executor is hosted on {host}. 
 This is an example how you can connect to the executor assuming the document (d) is already defined:
 from jina import Client, Document, DocumentArray
 client = Client(host='{host}')
 response = client.post('/', inputs=DocumentArray([d])) # always use '/'
 print(response[0].text) # can also be blob in case of image/audio..., this should be visualized in the streamlit app
 '''
-    )
-    conversation = gpt_session.get_conversation()
-    conversation.query(user_query)
-    playground_content_raw = conversation.query(
-        f"General rules: " + not_allowed() + chain_of_thought_optimization('python', 'app.py'))
-    playground_content = extract_content_from_result(playground_content_raw, 'app.py')
-    persist_file(playground_content, os.path.join(executor_path, 'app.py'))
-
-def get_executor_path(output_path, package, version):
-    package_path = '_'.join(package)
-    return os.path.join(output_path, package_path, f'v{version}')
-
-def debug_executor(output_path, package, description, test):
-    MAX_DEBUGGING_ITERATIONS = 10
-    error_before = ''
-    for i in range(1, MAX_DEBUGGING_ITERATIONS):
-        previous_executor_path = get_executor_path(output_path, package, i)
-        next_executor_path = get_executor_path(output_path, package, i + 1)
-        log_hubble = push_executor(previous_executor_path)
-        error = process_error_message(log_hubble)
-        if error:
-            recreate_folder(next_executor_path)
-            file_name_to_content = get_all_executor_files_with_content(previous_executor_path)
-            all_files_string = files_to_string(file_name_to_content)
-            user_query = (
-                    f"General rules: " + not_allowed()
-                    + 'Here is the description of the task the executor must solve:\n'
-                    + description
-                    + '\n\nHere is the test scenario the executor must pass:\n'
-                    + test
-                    + 'Here are all the files I use:\n'
-                    + all_files_string
-                    + (('This is an error that is already fixed before:\n'
-                        + error_before) if error_before else '')
-                    + '\n\nNow, I get the following error:\n'
-                    + error + '\n'
-                    + 'Think quickly about possible reasons. '
-                      'Then output the files that need change. '
-                      "Don't output files that don't need change. "
-                      "If you output a file, then write the complete file. "
-                      "Use the exact same syntax to wrap the code:\n"
-                      f"**...**\n"
-                      f"```...\n"
-                      f"...code...\n"
-                      f"```\n\n"
-            )
-            conversation = gpt_session.get_conversation()
-            returned_files_raw = conversation.query(user_query)
-            for file_name, tag in FILE_AND_TAG_PAIRS:
-                updated_file = extract_content_from_result(returned_files_raw, file_name)
-                if updated_file:
-                    file_name_to_content[file_name] = updated_file
-
-            for file_name, content in file_name_to_content.items():
-                persist_file(content, os.path.join(next_executor_path, file_name))
-            error_before = error
-
-        else:
-            break
-        if i == MAX_DEBUGGING_ITERATIONS - 1:
-            raise MaxDebugTimeReachedException('Could not debug the executor.')
-    return get_executor_path(output_path, package, i)
-
-class MaxDebugTimeReachedException(BaseException):
-    pass
-
-
-def generate_executor_name(description):
-    conversation = gpt_session.get_conversation()
-    user_query = f'''
+        )
+        conversation = self.gpt_session.get_conversation()
+        conversation.query(user_query)
+        playground_content_raw = conversation.query(
+            f"General rules: " + not_allowed() + chain_of_thought_optimization('python', 'app.py'))
+        playground_content = self.extract_content_from_result(playground_content_raw, 'app.py')
+        persist_file(playground_content, os.path.join(executor_path, 'app.py'))
+
+    def get_executor_path(self, output_path, package, version):
+        package_path = '_'.join(package)
+        return os.path.join(output_path, package_path, f'v{version}')
+
+    def debug_executor(self, output_path, package, description, test):
+        MAX_DEBUGGING_ITERATIONS = 10
+        error_before = ''
+        for i in range(1, MAX_DEBUGGING_ITERATIONS):
+            previous_executor_path = self.get_executor_path(output_path, package, i)
+            next_executor_path = self.get_executor_path(output_path, package, i + 1)
+            log_hubble = push_executor(previous_executor_path)
+            error = process_error_message(log_hubble)
+            if error:
+                recreate_folder(next_executor_path)
+                file_name_to_content = self.get_all_executor_files_with_content(previous_executor_path)
+                all_files_string = self.files_to_string(file_name_to_content)
+                user_query = (
+                        f"General rules: " + not_allowed()
+                        + 'Here is the description of the task the executor must solve:\n'
+                        + description
+                        + '\n\nHere is the test scenario the executor must pass:\n'
+                        + test
+                        + 'Here are all the files I use:\n'
+                        + all_files_string
+                        + (('This is an error that is already fixed before:\n'
+                            + error_before) if error_before else '')
+                        + '\n\nNow, I get the following error:\n'
+                        + error + '\n'
+                        + 'Think quickly about possible reasons. '
+                          'Then output the files that need change. '
+                          "Don't output files that don't need change. "
+                          "If you output a file, then write the complete file. "
+                          "Use the exact same syntax to wrap the code:\n"
+                          f"**...**\n"
+                          f"```...\n"
+                          f"...code...\n"
+                          f"```\n\n"
+                )
+                conversation = self.gpt_session.get_conversation()
+                returned_files_raw = conversation.query(user_query)
+                for file_name, tag in FILE_AND_TAG_PAIRS:
+                    updated_file = self.extract_content_from_result(returned_files_raw, file_name)
+                    if updated_file:
+                        file_name_to_content[file_name] = updated_file
+
+                for file_name, content in file_name_to_content.items():
+                    persist_file(content, os.path.join(next_executor_path, file_name))
+                error_before = error
+
+            else:
+                break
+            if i == MAX_DEBUGGING_ITERATIONS - 1:
+                raise self.MaxDebugTimeReachedException('Could not debug the executor.')
+        return self.get_executor_path(output_path, package, i)
+
+    class MaxDebugTimeReachedException(BaseException):
+        pass
+
+    def generate_executor_name(self, description):
+        conversation = self.gpt_session.get_conversation()
+        user_query = f'''
 Generate a name for the executor matching the description:
 "{description}"
 The executor name must fulfill the following criteria:
 - camel case
 - start with a capital letter
 - only consists of lower and upper case characters
 - end with Executor.
 
 The output is a the raw string wrapped into ``` and starting with **name.txt** like this:
 **name.txt**
 ```
 PDFParserExecutor
 ```
 '''
-    name_raw = conversation.query(user_query)
-    name = extract_content_from_result(name_raw, 'name.txt')
-    return name
-
-def get_possible_packages(description, threads):
-    print_colored('', '############# What package to use? #############', 'red')
-    user_query = f'''
+        name_raw = conversation.query(user_query)
+        name = self.extract_content_from_result(name_raw, 'name.txt')
+        return name
+
+    def get_possible_packages(self, description, threads):
+        print_colored('', '############# What package to use? #############', 'red')
+        user_query = f'''
 Here is the task description of the problme you need to solve:
 "{description}"
 First, write down all the subtasks you need to solve which require python packages.
 For each subtask:
     Provide a list of 1 to 3 python packages you could use to solve the subtask. Prefer modern packages.
     For each package:
         Write down some non-obvious thoughts about the challenges you might face for the task and give multiple approaches on how you handle them.
@@ -270,68 +267,43 @@
 The output must be a list of lists wrapped into ``` and starting with **packages.csv** like this:
 **packages.csv**
 ```
 package1,package2
 package2,package3,...
 ...
 ```
-    '''
-    conversation = gpt_session.get_conversation()
-    packages_raw = conversation.query(user_query)
-    packages_csv_string = extract_content_from_result(packages_raw, 'packages.csv')
-    packages = [package.split(',') for package in packages_csv_string.split('\n')]
-    packages = packages[:threads]
-    return packages
-
-@click.group(invoke_without_command=True)
-def main():
-    pass
-
-@main.command()
-@click.option('--description', required=True, help='Description of the executor.')
-@click.option('--test', required=True, help='Test scenario for the executor.')
-@click.option('--num_approaches', default=3, type=int, help='Number of num_approaches to use to fulfill the task (default: 3).')
-@click.option('--output_path', default='executor', help='Path to the output folder (must be empty). ')
-def create(
-        description,
-        test,
-        num_approaches=3,
-        output_path='executor',
-):
-    jina_auth_login()
-
-    generated_name = generate_executor_name(description)
-    executor_name = f'{generated_name}{random.randint(0, 1000_000)}'
-
-    packages_list = get_possible_packages(description, num_approaches)
-    recreate_folder(output_path)
-    # packages_list = [['a']]
-    # executor_name = 'ColorPaletteGeneratorExecutor5946'
-    # executor_path = '/Users/florianhonicke/jina/gptdeploy/executor/colorsys_colorharmony/v5'
-    # host = 'grpcs://gptdeploy-5f6ea44fc8.wolf.jina.ai'
-    for packages in packages_list:
-        try:
-            create_executor(description, test, output_path, executor_name, packages)
-            executor_path = debug_executor(output_path, packages, description, test)
-            print('Deploy a jina flow')
-            host = jina_cloud.deploy_flow(executor_name, executor_path)
-            print(f'Flow is deployed create the playground for {host}')
-            create_playground(executor_name, executor_path, host)
-        except MaxDebugTimeReachedException:
-            print('Could not debug the executor.')
-            continue
-        print(
-            'Executor name:', executor_name, '\n',
-            'Executor path:', executor_path, '\n',
-            'Host:', host, '\n',
-            'Playground:', f'streamlit run {os.path.join(executor_path, "app.py")}', '\n',
-        )
-        break
-
-@main.command()
-@click.option('--key', required=True, help='Your OpenAI API key.')
-def configure(key):
-    set_api_key(key)
-
-
-if __name__ == '__main__':
-    main()
+'''
+        conversation = self.gpt_session.get_conversation()
+        packages_raw = conversation.query(user_query)
+        packages_csv_string = self.extract_content_from_result(packages_raw, 'packages.csv')
+        packages = [package.split(',') for package in packages_csv_string.split('\n')]
+        packages = packages[:threads]
+        return packages
+
+
+    def create(self, description, num_approaches, output_path, test):
+        generated_name = self.generate_executor_name(description)
+        executor_name = f'{generated_name}{random.randint(0, 1000_000)}'
+        packages_list = self.get_possible_packages(description, num_approaches)
+        recreate_folder(output_path)
+        # packages_list = [['a']]
+        # executor_name = 'ColorPaletteGeneratorExecutor5946'
+        # executor_path = '/Users/florianhonicke/jina/gptdeploy/executor/colorsys_colorharmony/v5'
+        # host = 'grpcs://gptdeploy-5f6ea44fc8.wolf.jina.ai'
+        for packages in packages_list:
+            try:
+                self.create_executor(description, test, output_path, executor_name, packages)
+                executor_path = self.debug_executor(output_path, packages, description, test)
+                print('Deploy a jina flow')
+                host = jina_cloud.deploy_flow(executor_name, executor_path)
+                print(f'Flow is deployed create the playground for {host}')
+                self.create_playground(executor_name, executor_path, host)
+            except self.MaxDebugTimeReachedException:
+                print('Could not debug the executor.')
+                continue
+            print(
+                'Executor name:', executor_name, '\n',
+                'Executor path:', executor_path, '\n',
+                'Host:', host, '\n',
+                'Playground:', f'streamlit run {os.path.join(executor_path, "app.py")}', '\n',
+            )
+            break
```

### Comparing `gptdeploy-0.18.4/src/prompt_system.py` & `gptdeploy-0.18.5/src/prompt_system.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.4/src/prompt_tasks.py` & `gptdeploy-0.18.5/src/prompt_tasks.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.4/src/server.py` & `gptdeploy-0.18.5/src/server.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.4/src/utils/io.py` & `gptdeploy-0.18.5/src/utils/io.py`

 * *Files identical despite different names*

### Comparing `gptdeploy-0.18.4/src/utils/string_tools.py` & `gptdeploy-0.18.5/src/utils/string_tools.py`

 * *Files identical despite different names*

