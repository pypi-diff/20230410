# Comparing `tmp/joeypan-0.0.7.tar.gz` & `tmp/joeypan-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joeypan-0.0.7.tar", last modified: Wed Mar 29 18:27:20 2023, max compression
+gzip compressed data, was "joeypan-0.0.8.tar", last modified: Mon Apr 10 18:01:09 2023, max compression
```

## Comparing `joeypan-0.0.7.tar` & `joeypan-0.0.8.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-03-29 18:27:20.945687 joeypan-0.0.7/
--rw-rw-rw-   0        0        0     1091 2023-03-18 12:37:40.000000 joeypan-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      457 2023-03-29 18:27:20.945687 joeypan-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-03-29 16:16:24.000000 joeypan-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-03-29 18:27:20.925686 joeypan-0.0.7/joeypan/
--rw-rw-rw-   0        0        0      148 2023-03-26 13:45:32.000000 joeypan-0.0.7/joeypan/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-29 18:27:20.935686 joeypan-0.0.7/joeypan/config/
--rw-rw-rw-   0        0        0      870 2023-03-20 15:07:59.000000 joeypan-0.0.7/joeypan/config/__init__.py
--rw-rw-rw-   0        0        0     8001 2023-03-29 17:36:00.000000 joeypan-0.0.7/joeypan/config/settings.py
-drwxrwxrwx   0        0        0        0 2023-03-29 18:27:20.937688 joeypan-0.0.7/joeypan/core/
--rw-rw-rw-   0        0        0        0 2023-03-18 12:25:17.000000 joeypan-0.0.7/joeypan/core/__init__.py
--rw-rw-rw-   0        0        0      148 2023-03-28 16:16:23.000000 joeypan-0.0.7/joeypan/core/log.py
-drwxrwxrwx   0        0        0        0 2023-03-29 18:27:20.938688 joeypan-0.0.7/joeypan/resource/
--rw-rw-rw-   0        0        0     2845 2023-03-29 17:55:54.000000 joeypan-0.0.7/joeypan/resource/template.json
-drwxrwxrwx   0        0        0        0 2023-03-29 18:27:20.939686 joeypan-0.0.7/joeypan/test/
--rw-rw-rw-   0        0        0        0 2023-03-18 12:25:13.000000 joeypan-0.0.7/joeypan/test/__init__.py
--rw-rw-rw-   0        0        0      257 2023-03-28 17:21:19.000000 joeypan-0.0.7/joeypan/test/test_settings.py
-drwxrwxrwx   0        0        0        0 2023-03-29 18:27:20.943688 joeypan-0.0.7/joeypan/utils/
--rw-rw-rw-   0        0        0       93 2023-03-26 14:38:05.000000 joeypan-0.0.7/joeypan/utils/ErrorCode.py
--rw-rw-rw-   0        0        0      142 2023-03-26 13:58:18.000000 joeypan-0.0.7/joeypan/utils/__init__.py
--rw-rw-rw-   0        0        0      493 2023-03-26 14:36:27.000000 joeypan-0.0.7/joeypan/utils/exceptions.py
-drwxrwxrwx   0        0        0        0 2023-03-29 18:27:20.933688 joeypan-0.0.7/joeypan.egg-info/
--rw-rw-rw-   0        0        0      457 2023-03-29 18:27:20.000000 joeypan-0.0.7/joeypan.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      466 2023-03-29 18:27:20.000000 joeypan-0.0.7/joeypan.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-29 18:27:20.000000 joeypan-0.0.7/joeypan.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-03-29 18:27:20.000000 joeypan-0.0.7/joeypan.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-03-29 18:27:20.000000 joeypan-0.0.7/joeypan.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-03-29 18:27:20.946689 joeypan-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     3008 2023-03-29 18:23:57.000000 joeypan-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:01:09.170873 joeypan-0.0.8/
+-rw-rw-rw-   0        0        0     1091 2023-03-18 12:37:40.000000 joeypan-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0      450 2023-04-10 18:01:09.169874 joeypan-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-03-29 16:16:24.000000 joeypan-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 18:01:09.123871 joeypan-0.0.8/joeypan/
+-rw-rw-rw-   0        0        0      148 2023-03-26 13:45:32.000000 joeypan-0.0.8/joeypan/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:01:09.145874 joeypan-0.0.8/joeypan/config/
+-rw-rw-rw-   0        0        0      853 2023-04-10 16:40:37.000000 joeypan-0.0.8/joeypan/config/__init__.py
+-rw-rw-rw-   0        0        0    10733 2023-04-10 17:40:37.000000 joeypan-0.0.8/joeypan/config/settings.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:01:09.146874 joeypan-0.0.8/joeypan/resource/
+-rw-rw-rw-   0        0        0     3429 2023-04-10 17:57:32.000000 joeypan-0.0.8/joeypan/resource/template.json
+drwxrwxrwx   0        0        0        0 2023-04-10 18:01:09.150874 joeypan-0.0.8/joeypan/test/
+-rw-rw-rw-   0        0        0        0 2023-03-18 12:25:13.000000 joeypan-0.0.8/joeypan/test/__init__.py
+-rw-rw-rw-   0        0        0     1606 2023-04-10 17:43:58.000000 joeypan-0.0.8/joeypan/test/models.py
+-rw-rw-rw-   0        0        0      464 2023-04-10 17:15:31.000000 joeypan-0.0.8/joeypan/test/test_export_model.py
+-rw-rw-rw-   0        0        0      263 2023-04-10 17:06:28.000000 joeypan-0.0.8/joeypan/test/test_settings.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:01:09.168872 joeypan-0.0.8/joeypan/utils/
+-rw-rw-rw-   0        0        0       93 2023-03-26 14:38:05.000000 joeypan-0.0.8/joeypan/utils/ErrorCode.py
+-rw-rw-rw-   0        0        0      142 2023-03-26 13:58:18.000000 joeypan-0.0.8/joeypan/utils/__init__.py
+-rw-rw-rw-   0        0        0      559 2023-04-10 15:56:41.000000 joeypan-0.0.8/joeypan/utils/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-04-10 18:01:09.143872 joeypan-0.0.8/joeypan.egg-info/
+-rw-rw-rw-   0        0        0      450 2023-04-10 18:01:09.000000 joeypan-0.0.8/joeypan.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      478 2023-04-10 18:01:09.000000 joeypan-0.0.8/joeypan.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 18:01:09.000000 joeypan-0.0.8/joeypan.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-04-10 18:01:09.000000 joeypan-0.0.8/joeypan.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-04-10 18:01:09.000000 joeypan-0.0.8/joeypan.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 18:01:09.170873 joeypan-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     3148 2023-04-10 17:58:32.000000 joeypan-0.0.8/setup.py
```

### Comparing `joeypan-0.0.7/LICENSE` & `joeypan-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `joeypan-0.0.7/joeypan/config/__init__.py` & `joeypan-0.0.8/joeypan/config/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -32,9 +32,7 @@
         GLOBAL.settings[unique_id] = defaultdict
 
         def inner(*args, **kwargs):
             pass
 
 
 GLOBAL = Global()
-
-print(GLOBAL)
```

### Comparing `joeypan-0.0.7/joeypan/config/settings.py` & `joeypan-0.0.8/joeypan/config/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 import decimal
 import json
+import logging
 import logging.config
 import logging.handlers
 import os
 import warnings
 from abc import abstractmethod
-from typing import Optional, List
-
-from pydantic import BaseSettings, Field, BaseConfig, Extra, validator
+from contextlib import contextmanager
+from copy import deepcopy
+from typing import Optional, List, Union
+
+import redis
+from elasticsearch import Elasticsearch
+from pydantic import BaseSettings, Field, BaseConfig, Extra
 from pydantic.typing import StrPath
+from sqlalchemy import create_engine
+from sqlalchemy.orm import sessionmaker, scoped_session, Session
 
 from joeypan import RESOURCE_JOEYPAN_DIR
 
 # disable warning: pydantic set alias_namefor klass -> class
 warnings.filterwarnings("ignore", category=FutureWarning)
+LOG = logging.getLogger(__name__)
 
 
 class InjectSettings:
-    __DEFAULT_LOG_DIR = os.path.join(os.getcwd(), "logs")
+    __DEFAULT_LOG_DIR = os.environ.get("LOG_DIR") or os.path.join(os.getcwd(), "logs")
 
     @property
     def default_log_dir(self) -> str:
         return self.__DEFAULT_LOG_DIR
 
     def set_default_log_dir(self, log_dir: StrPath):
         if not os.path.exists(log_dir):
@@ -66,36 +74,82 @@
 
 class Server(AbstractSettings):
     port: int = Field(8080, description="服务端口")
     servlet: Servlet = Field(default_factory=Servlet)
 
 
 class Datasource(AbstractSettings):
+    SCOPED_SESSION: scoped_session = None
     url: str = Field(
         default="mysql+pymysql://user:password@localhost:3306/foo?charset=utf8mb4")
+    echo: bool = True
+    echo_pool: bool = False
+    pool_size: int = 10
+    pool_timeout: int = 3
+    pool_recycle: int = 10
+    pool_use_lifo: bool = True
+    query_cache_size: int = 500
 
+    @property
+    def __session(self) -> scoped_session:
+        if self.SCOPED_SESSION:
+            return self.SCOPED_SESSION
+        cfg = self.dict()
+        cfg.pop("SCOPED_SESSION", None)
+        url = cfg.pop("url", None)
+        engine = create_engine(url, **cfg)
+        session_factory = sessionmaker(engine)
+        self.SCOPED_SESSION = scoped_session(session_factory)
+        return self.SCOPED_SESSION
 
-class JedisPool(AbstractSettings):
-    max_active: int = Field(default=8)
-    max_wait: int = Field(default=-1)
-    max_idle: int = Field(default=8)
-    min_idle: int = Field(default=0)
+    @property
+    @contextmanager
+    def session(self) -> Session:
+        session = self.__session()
+        try:
+            yield session
+            session.commit()
+        except Exception as e:
+            LOG.error(f"commit failed: {e}")
+            session.rollback()
+            raise e
+        finally:
+            session.close()
 
 
-class Jedis(AbstractSettings):
-    pool: JedisPool = Field(default_factory=JedisPool)
-    timeout: int = Field(default=0)
+class JedisPool(AbstractSettings):
+    pass
 
 
 class Redis(AbstractSettings):
-    database: int = Field(default=0)
+    POOL: Union[redis.Redis, redis.RedisCluster] = None
+    db: int = Field(default=0)
     host: str = Field(default="localhost")
     port: int = Field(default=6379)
-    password: str = None
-    jedis: Jedis = Field(default_factory=Jedis)
+    password: str = None,
+    startup_nodes: list = None
+    jedis: JedisPool = Field(default_factory=JedisPool)
+
+    @property
+    def session(self):
+        if not self.POOL:
+            if self.startup_nodes:
+                kwargs = self.jedis.dict()
+                klass = redis.RedisCluster
+            else:
+                kwargs = {
+                    "db": self.db,
+                    "host": self.host,
+                    "port": self.port,
+                    "password": self.password
+                }
+                kwargs.update(self.jedis.dict())
+                klass = redis.Redis
+            self.POOL = klass(**kwargs)
+        return self.POOL
 
 
 class LogFormat(AbstractSettings):
     pass
 
 
 class SimpleFormat(LogFormat):
@@ -123,39 +177,29 @@
     stream: str = Field(default="ext://sys.stdout")
 
 
 class LogFileHandler(LogHandler):
     klass: str = Field(default="logging.handlers.RotatingFileHandler")
     level: int = Field(default=logging.DEBUG)
     formatter: str = Field(default="upgrade")
-    filename: StrPath = Field(default=os.path.join(
-        inject_settings.default_log_dir, "all.log"))
+    filename: StrPath = Field(default="all.log")
     maxBytes: int = Field(default=4194304)  # 4MB
     backupCount: int = Field(default=50)  # 保留多少个log文件
     encoding: str = Field(default="utf8")
 
-    @validator("filename")
-    def reset_filename(cls, filename):
-        return os.path.join(inject_settings.default_log_dir, "all.log")
-
 
 class LogServerHandler(LogFileHandler):
     klass: str = Field(default="logging.handlers.RotatingFileHandler")
     level: int = Field(default=logging.DEBUG)
     formatter: str = Field(default="simple")
-    filename: StrPath = Field(default=os.path.join(
-        inject_settings.default_log_dir, "server.log"))
+    filename: StrPath = Field(default="server.log")
     maxBytes: int = Field(default=4194304)  # 4MB
     backupCount: int = Field(default=20)  # 保留多少个log文件
     encoding: str = Field(default="utf8")
 
-    @validator("filename")
-    def reset_filename(cls, filename):
-        return os.path.join(inject_settings.default_log_dir, "server.log")
-
 
 class LogHandlers(AbstractSettings):
     console_handler: LogHandler = Field(default_factory=LogConsoleHandler)
     file_handler: LogHandler = Field(default_factory=LogFileHandler)
     server_handler: LogHandler = Field(default_factory=LogServerHandler)
 
 
@@ -181,19 +225,32 @@
     version: int = Field(default=1)
     disable_existing_loggers: bool = Field(default=True)
     formatters: LogFormats = Field(default_factory=LogFormats)
     handlers: LogHandlers = Field(default_factory=LogHandlers)
     loggers: LoggerInstances = Field(default_factory=LoggerInstances)
 
 
+class ES(AbstractSettings):
+    INSTANCE: Elasticsearch = None
+    hosts: List[dict] = Field(default=[{"host": "localhost", "port": 9200}])
+    kwargs: dict = Field(default_factory=dict)
+
+    @property
+    def session(self) -> Elasticsearch:
+        if not self.INSTANCE:
+            self.INSTANCE = Elasticsearch(hosts=self.hosts, **self.kwargs)
+        return self.INSTANCE
+
+
 class DefaultSettings(AbstractSettings):
     server: Server = Field(default_factory=Server)
     datasource: Datasource = Field(default_factory=Datasource)
     redis: Redis = Field(default_factory=Redis)
     log: Logger = Field(default_factory=Logger)
+    es: ES = Field(default_factory=ES)
 
 
 class UserSettings(DefaultSettings):
     pass
 
 
 class SettingsLoader(object):
@@ -246,14 +303,35 @@
         _instance = UserSettings(**data_json)
         cls.INSTANCE[name] = _instance
         cls.setup_log(_instance.log)
         return cls.INSTANCE.get(name)
 
     @classmethod
     def setup_log(cls, cfg: Logger):
-        logging.config.dictConfig(cfg.dict())
+        def update_log_path(file_name):
+            if file_name and os.path.basename(file_name) == file_name:
+                return os.path.join(inject_settings.default_log_dir, file_name)
+            return file_name
+
+        def update_dict(data: dict):
+            if data.get("filename"):
+                data["filename"] = update_log_path(data.get("filename"))
+            return data
+
+        temp_cfg = deepcopy(cfg)
+        temp_handlers = {}
+        for name, handler in cfg.handlers:
+            if isinstance(name, (str, bytes)):
+                if isinstance(handler, LogHandler):
+                    if hasattr(handler, "filename"):
+                        handler.filename = os.path.join(inject_settings.default_log_dir, handler.filename)
+                    temp_handlers[name] = handler
+                elif isinstance(handler, dict):
+                    temp_handlers[name] = update_dict(handler)
+        temp_cfg.handlers = temp_handlers
+        logging.config.dictConfig(temp_cfg.dict())
 
     @classmethod
     def default(cls):
         config_json_path = os.path.join(RESOURCE_JOEYPAN_DIR, "template.json")
         with open(config_json_path, "r", encoding="utf-8") as f:
             return cls.create(json.load(f))
```

### Comparing `joeypan-0.0.7/joeypan/resource/template.json` & `joeypan-0.0.8/joeypan/resource/template.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7388392857142857%*

 * *Differences: {"'datasource'": "{'url': 'mysql+pymysql://root:123456@localhost:3306/fastapi_db?charset=utf8mb4'}",*

 * * "'es'": "OrderedDict([('hosts', [OrderedDict([('host', '127.0.0.1'), ('port', 9200)])]), "*

 * *         "('kwargs', OrderedDict([('sniff_on_start', False), ('retry_on_timeout', True), "*

 * *         "('max_retries', 1), ('use_ssl', False), ('maxsize', 10), ('timeout', 5)]))])",*

 * * "'log'": "{'handlers': {'db_handler': OrderedDict([('class', "*

 * *          "'logging.handlers.RotatingFileHandler'), ('level', 20), ('format […]*

```diff
@@ -1,10 +1,26 @@
 {
     "datasource": {
-        "url": "mysql+pymysql://user:password@localhost:3306/foo?charset=utf8mb4"
+        "url": "mysql+pymysql://root:123456@localhost:3306/fastapi_db?charset=utf8mb4"
+    },
+    "es": {
+        "hosts": [
+            {
+                "host": "127.0.0.1",
+                "port": 9200
+            }
+        ],
+        "kwargs": {
+            "max_retries": 1,
+            "maxsize": 10,
+            "retry_on_timeout": true,
+            "sniff_on_start": false,
+            "timeout": 5,
+            "use_ssl": false
+        }
     },
     "joeypan_settings_name": "default_joeypan_settings",
     "log": {
         "disable_existing_loggers": true,
         "formatters": {
             "simple": {
                 "format": "%(asctime)s %(levelname)s %(message)s"
@@ -34,14 +50,23 @@
             },
             "console_handler": {
                 "class": "logging.StreamHandler",
                 "formatter": "upgrade",
                 "level": 10,
                 "stream": "ext://sys.stdout"
             },
+            "db_handler": {
+                "backupCount": 20,
+                "class": "logging.handlers.RotatingFileHandler",
+                "encoding": "utf8",
+                "filename": "db.log",
+                "formatter": "simple",
+                "level": 20,
+                "maxBytes": 4194304
+            },
             "file_handler": {
                 "backupCount": 50,
                 "class": "logging.handlers.RotatingFileHandler",
                 "encoding": "utf8",
                 "filename": "all.log",
                 "formatter": "upgrade",
                 "level": 10,
@@ -78,32 +103,33 @@
         "loggers": {
             "server": {
                 "handlers": [
                     "server_handler",
                     "console_handler"
                 ],
                 "level": 10
+            },
+            "sqlalchemy.engine": {
+                "handlers": [
+                    "db_handler"
+                ],
+                "level": 10
             }
         },
         "version": 1
     },
     "redis": {
-        "database": 0,
+        "db": 0,
         "host": "localhost",
         "jedis": {
-            "pool": {
-                "max_active": 8,
-                "max_idle": 8,
-                "max_wait": -1,
-                "min_idle": 0
-            },
-            "timeout": 0
+            "decode_responses": true
         },
-        "password": null,
-        "port": 6379
+        "password": "",
+        "port": 6379,
+        "startup_nodes": []
     },
     "server": {
         "port": 3306,
         "servlet": {
             "context_path": "."
         }
     }
```

### Comparing `joeypan-0.0.7/setup.py` & `joeypan-0.0.8/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import os
 import shutil
 import sys
 
 import setuptools
 
-VERSION = (0, 0, 7)
+VERSION = (0, 0, 8)
 
 
 def clear(clear_dist_dir=False):
     if clear_dist_dir and os.path.exists("dist"):
         shutil.rmtree("dist", ignore_errors=True)
     if os.path.exists("build"):
         shutil.rmtree("build", ignore_errors=True)
@@ -19,14 +19,19 @@
             if d == "__pycache__":
                 shutil.rmtree(os.path.join(root, d))
         for f in fs:
             if f and f[-4:] == ".pyc":
                 os.remove(os.path.join(root, f))
 
 
+def get_requires():
+    with open("requirements.txt", "r", encoding="utf-8") as f:
+        return [line.strip() for line in f.readlines()]
+
+
 def build():
     clear(True)
     print("DELETE BUILD CACHE DONE")
     current_version = ".".join(str(item) for item in VERSION)
     md_name = current_version + ".md"
     doc_path = os.path.join(os.getcwd(), "release_note", md_name)
     if not os.path.exists(doc_path):
@@ -35,15 +40,15 @@
         long_description = fh.read()
 
     setuptools.setup(
         name="joeypan",
         version=current_version,
         author="elijahxb",
         package_dir={"joeypan": "joeypan"},
-        install_requires=["pydantic==1.10.6"],
+        install_requires=get_requires(),
         author_email="elijahxb@outlook.com",
         description="A small package for web framework",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="http://www.joeypan.cn:9830/Elijahxb/joeypan",
         packages=setuptools.find_packages(exclude=["*.pyc", "__pycache__"]),
         include_package_data=True,
```

