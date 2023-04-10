# Comparing `tmp/openai_chat-0.0.1.tar.gz` & `tmp/openai_chat-0.0.2.tar.gz`

## Comparing `openai_chat-0.0.1.tar` & `openai_chat-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 openai_chat-0.0.1/.python-version
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_chat-0.0.1/gpt4/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_chat-0.0.1/gpt4/main.py
--rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openai_chat-0.0.1/.gitignore
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_chat-0.0.1/README.md
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 openai_chat-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      484 2020-02-02 00:00:00.000000 openai_chat-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openai_chat-0.0.2/.python-version
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_chat-0.0.2/openai_chat/__init__.py
+-rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 openai_chat-0.0.2/openai_chat/chat.py
+-rw-r--r--   0        0        0     4238 2020-02-02 00:00:00.000000 openai_chat-0.0.2/openai_chat/main.py
+-rw-r--r--   0        0        0       10 2020-02-02 00:00:00.000000 openai_chat-0.0.2/.gitignore
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_chat-0.0.2/README.md
+-rw-r--r--   0        0        0      859 2020-02-02 00:00:00.000000 openai_chat-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      505 2020-02-02 00:00:00.000000 openai_chat-0.0.2/PKG-INFO
```

### Comparing `openai_chat-0.0.1/pyproject.toml` & `openai_chat-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "openai-chat"
-version = "0.0.1"
-python_requires = ">=3.10"
+version = "0.0.2"
+python_requires = ">=3.9"
 description = "A CLI for chatting with OpenAI's API."
 authors = [
     {name = "Ryan Young", email = "dev@ryayoung.com"}
 ]
 readme = "README.md"
 license = "MIT"
-homepage = "https://github.com/ryayoung/gpt4"
-repository = "https://github.com/ryayoung/gpt4"
-documentation = "https://gpt4.readthedocs.io"
+homepage = "https://github.com/ryayoung/openai-chat"
+repository = "https://github.com/ryayoung/openai-chat"
+documentation = "https://openai-chat.readthedocs.io"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.11",
     "Topic :: Software Development :: Libraries"
 ]
 dependencies = [
     'requests',
-    'openai'
+    'openai',
+    'click',
 ]
+
+[project.scripts]
+ai = "openai_chat.main:main"
```

