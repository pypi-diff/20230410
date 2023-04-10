# Comparing `tmp/openai_chat-0.0.2.tar.gz` & `tmp/openai_chat-0.0.3.tar.gz`

## Comparing `openai_chat-0.0.2.tar` & `openai_chat-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openai_chat-0.0.2/.python-version
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_chat-0.0.2/openai_chat/__init__.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 openai_chat-0.0.2/openai_chat/chat.py
--rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 openai_chat-0.0.2/openai_chat/main.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openai_chat-0.0.2/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_chat-0.0.2/README.md
--rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 openai_chat-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 openai_chat-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openai_chat-0.0.3/.python-version
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_chat-0.0.3/openai_chat/__init__.py
+-rw-r--r--   0        0        0     2307 2020-02-02 00:00:00.000000 openai_chat-0.0.3/openai_chat/chat.py
+-rw-r--r--   0        0        0     7461 2020-02-02 00:00:00.000000 openai_chat-0.0.3/openai_chat/main.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openai_chat-0.0.3/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_chat-0.0.3/README.md
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 openai_chat-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      560 2020-02-02 00:00:00.000000 openai_chat-0.0.3/PKG-INFO
```

### Comparing `openai_chat-0.0.2/pyproject.toml` & `openai_chat-0.0.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openai-chat"
-version = "0.0.2"
+version = "0.0.3"
 python_requires = ">=3.9"
-description = "A CLI for chatting with OpenAI's API."
+description = "CLI for chatting through OpenAI's API."
 authors = [
     {name = "Ryan Young", email = "dev@ryayoung.com"}
 ]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/ryayoung/openai-chat"
 repository = "https://github.com/ryayoung/openai-chat"
@@ -22,12 +22,14 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries"
 ]
 dependencies = [
     'requests',
     'openai',
+    'colorama',
     'click',
+    'prompt-toolkit',
 ]
 
 [project.scripts]
-ai = "openai_chat.main:main"
+ai = "gpt_ai.main:main"
```

