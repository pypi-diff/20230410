# Comparing `tmp/wf-gqlpycgen-0.7.3.tar.gz` & `tmp/wf_gqlpycgen-0.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wf-gqlpycgen-0.7.3.tar", last modified: Tue Jul 26 20:20:54 2022, max compression
+gzip compressed data, was "wf_gqlpycgen-0.7.4.tar", max compression
```

## Comparing `wf-gqlpycgen-0.7.3.tar` & `wf_gqlpycgen-0.7.4.tar`

### file list

```diff
@@ -1,25 +1,11 @@
-drwxr-xr-x   0 pauldecoursey   (501) staff       (20)        0 2022-07-26 20:20:54.590113 wf-gqlpycgen-0.7.3/
--rwxr-xr-x   0 pauldecoursey   (501) staff       (20)     1087 2022-07-26 16:57:55.000000 wf-gqlpycgen-0.7.3/LICENSE
--rwxr-xr-x   0 pauldecoursey   (501) staff       (20)       50 2022-07-26 16:57:55.000000 wf-gqlpycgen-0.7.3/MANIFEST.in
--rw-r--r--   0 pauldecoursey   (501) staff       (20)      383 2022-07-26 20:20:54.590005 wf-gqlpycgen-0.7.3/PKG-INFO
--rwxr-xr-x   0 pauldecoursey   (501) staff       (20)       81 2022-07-26 16:57:55.000000 wf-gqlpycgen-0.7.3/README.md
--rwxr-xr-x   0 pauldecoursey   (501) staff       (20)        6 2022-07-26 20:20:40.000000 wf-gqlpycgen-0.7.3/VERSION
-drwxr-xr-x   0 pauldecoursey   (501) staff       (20)        0 2022-07-26 20:20:54.588953 wf-gqlpycgen-0.7.3/gqlpycgen/
--rwxr-xr-x   0 pauldecoursey   (501) staff       (20)     3174 2022-07-26 16:57:55.000000 wf-gqlpycgen-0.7.3/gqlpycgen/__init__.py
--rwxr-xr-x   0 pauldecoursey   (501) staff       (20)     5846 2022-07-26 16:57:55.000000 wf-gqlpycgen-0.7.3/gqlpycgen/api.py
--rwxr-xr-x   0 pauldecoursey   (501) staff       (20)     4461 2022-07-26 20:20:04.000000 wf-gqlpycgen-0.7.3/gqlpycgen/client.py
--rwxr-xr-x   0 pauldecoursey   (501) staff       (20)     3129 2022-07-26 16:57:55.000000 wf-gqlpycgen-0.7.3/gqlpycgen/loader.py
--rwxr-xr-x   0 pauldecoursey   (501) staff       (20)     7668 2022-07-26 16:57:55.000000 wf-gqlpycgen-0.7.3/gqlpycgen/models.py
--rwxr-xr-x   0 pauldecoursey   (501) staff       (20)     1064 2022-07-26 16:57:55.000000 wf-gqlpycgen-0.7.3/gqlpycgen/utils.py
--rw-r--r--   0 pauldecoursey   (501) staff       (20)       38 2022-07-26 20:20:54.590150 wf-gqlpycgen-0.7.3/setup.cfg
--rwxr-xr-x   0 pauldecoursey   (501) staff       (20)     1098 2022-07-26 16:57:55.000000 wf-gqlpycgen-0.7.3/setup.py
-drwxr-xr-x   0 pauldecoursey   (501) staff       (20)        0 2022-07-26 20:20:54.589173 wf-gqlpycgen-0.7.3/tests/
--rwxr-xr-x   0 pauldecoursey   (501) staff       (20)        0 2022-07-26 16:57:55.000000 wf-gqlpycgen-0.7.3/tests/__init__.py
--rwxr-xr-x   0 pauldecoursey   (501) staff       (20)     1799 2022-07-26 16:57:55.000000 wf-gqlpycgen-0.7.3/tests/test_client.py
-drwxr-xr-x   0 pauldecoursey   (501) staff       (20)        0 2022-07-26 20:20:54.589859 wf-gqlpycgen-0.7.3/wf_gqlpycgen.egg-info/
--rw-r--r--   0 pauldecoursey   (501) staff       (20)      383 2022-07-26 20:20:54.000000 wf-gqlpycgen-0.7.3/wf_gqlpycgen.egg-info/PKG-INFO
--rw-r--r--   0 pauldecoursey   (501) staff       (20)      421 2022-07-26 20:20:54.000000 wf-gqlpycgen-0.7.3/wf_gqlpycgen.egg-info/SOURCES.txt
--rw-r--r--   0 pauldecoursey   (501) staff       (20)        1 2022-07-26 20:20:54.000000 wf-gqlpycgen-0.7.3/wf_gqlpycgen.egg-info/dependency_links.txt
--rw-r--r--   0 pauldecoursey   (501) staff       (20)       48 2022-07-26 20:20:54.000000 wf-gqlpycgen-0.7.3/wf_gqlpycgen.egg-info/entry_points.txt
--rw-r--r--   0 pauldecoursey   (501) staff       (20)       92 2022-07-26 20:20:54.000000 wf-gqlpycgen-0.7.3/wf_gqlpycgen.egg-info/requires.txt
--rw-r--r--   0 pauldecoursey   (501) staff       (20)       16 2022-07-26 20:20:54.000000 wf-gqlpycgen-0.7.3/wf_gqlpycgen.egg-info/top_level.txt
+-rwxr-xr-x   0        0        0     1087 2023-04-10 15:30:00.080773 wf_gqlpycgen-0.7.4/LICENSE
+-rwxr-xr-x   0        0        0       81 2023-04-10 15:30:00.080932 wf_gqlpycgen-0.7.4/README.md
+-rwxr-xr-x   0        0        0     3219 2023-04-10 18:08:54.349085 wf_gqlpycgen-0.7.4/gqlpycgen/__init__.py
+-rwxr-xr-x   0        0        0     5871 2023-04-10 18:08:54.412538 wf_gqlpycgen-0.7.4/gqlpycgen/api.py
+-rwxr-xr-x   0        0        0     5081 2023-04-10 18:08:54.390875 wf_gqlpycgen-0.7.4/gqlpycgen/client.py
+-rwxr-xr-x   0        0        0     3129 2023-04-10 15:30:00.081516 wf_gqlpycgen-0.7.4/gqlpycgen/loader.py
+-rwxr-xr-x   0        0        0     7833 2023-04-10 18:08:54.436541 wf_gqlpycgen-0.7.4/gqlpycgen/models.py
+-rwxr-xr-x   0        0        0     1063 2023-04-10 18:11:10.592961 wf_gqlpycgen-0.7.4/gqlpycgen/utils.py
+-rw-r--r--   0        0        0     1250 2023-04-10 18:16:30.141454 wf_gqlpycgen-0.7.4/pyproject.toml
+-rw-r--r--   0        0        0     1048 1970-01-01 00:00:00.000000 wf_gqlpycgen-0.7.4/setup.py
+-rw-r--r--   0        0        0     1243 1970-01-01 00:00:00.000000 wf_gqlpycgen-0.7.4/PKG-INFO
```

### Comparing `wf-gqlpycgen-0.7.3/LICENSE` & `wf_gqlpycgen-0.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wf-gqlpycgen-0.7.3/gqlpycgen/__init__.py` & `wf_gqlpycgen-0.7.4/gqlpycgen/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,33 @@
-from gqlpycgen.models import GraphEnum, filter_enums, Object, filter_objects, \
-    filter_interfaces, filter_unions, filter_scalars, Union, Scalar, \
-    filter_input_objects, InputObject, Query, Mutation
+from gqlpycgen.models import (
+    GraphEnum,
+    filter_enums,
+    Object,
+    filter_objects,
+    filter_interfaces,
+    filter_unions,
+    filter_scalars,
+    Union,
+    Scalar,
+    filter_input_objects,
+    InputObject,
+    Query,
+    Mutation,
+)
 from gqlpycgen.loader import load_remote_schema
 
 
 def write_header(out):
     out.write("# this file is generated, do not modify\n")
     out.write("from enum import Enum\n")
     out.write("from typing import List, NewType, TypeVar, Union\n")
-    out.write('\n')
-    out.write('from gqlpycgen.api import QueryBase, ObjectBase, MutationBase\n')
-    out.write('\n')
-    out.write('\n')
+    out.write("\n")
+    out.write("from gqlpycgen.api import QueryBase, ObjectBase, MutationBase\n")
+    out.write("\n")
+    out.write("\n")
     out.write("ID = NewType('ID', str)\n")
     out.write("ID__Required = NewType('ID!', str)\n")
     out.write("Int = NewType('Int', int)\n")
     out.write("Int__Required = NewType('Int!', int)\n")
     out.write("String = NewType('String', str)\n")
     out.write("String__Required = NewType('String!', str)\n")
     out.write("Float = NewType('Float', float)\n")
@@ -24,26 +36,26 @@
     out.write("Boolean__Required = NewType('Boolean!', bool)\n")
 
 
 def do_remote(uri, filename, py36plus=True):
     schema = load_remote_schema(uri)
     schema_types = schema.get("types")
 
-    with open(filename, 'w') as out:
+    with open(filename, "w") as out:
         # includes the imports required and the core scalars
         write_header(out)
 
         # Pull all the scalars, filter_scalars skips the core primitives since we cover that in the headers
         for scalar in filter_scalars(schema_types):
             obj = Scalar(scalar)
             out.write(obj.toPython(py36plus=py36plus))
 
         # for PEP8
-        out.write('\n')
-        out.write('\n')
+        out.write("\n")
+        out.write("\n")
 
         # Pull all the ENUMs, turns them into python ENUM objects
         for enumType in filter_enums(schema_types):
             enum = GraphEnum(enumType)
             out.write(enum.toPython(py36plus=py36plus))
 
         # Pull interfaces, treat them as objects since in python they are just objects
@@ -62,22 +74,22 @@
             out.write(obj.toPython(py36plus=py36plus))
 
         # lastly pull the unions and define TypeVars for them
         for union in filter_unions(schema_types):
             obj = Union(union)
             out.write(obj.toPython(py36plus=py36plus))
 
-        out.write('\n')
-        out.write('\n')
+        out.write("\n")
+        out.write("\n")
 
         # Pull the Query object and generate the API object
         query = Query(schema.get("queryType"))
         out.write(query.toPython(py36plus=py36plus))
 
-        out.write('\n')
-        out.write('\n')
+        out.write("\n")
+        out.write("\n")
 
         mutation = Mutation(schema.get("mutationType"))
         out.write(mutation.toPython(py36plus=py36plus))
 
         # don't forget to flush
         out.flush()
```

### Comparing `wf-gqlpycgen-0.7.3/gqlpycgen/api.py` & `wf_gqlpycgen-0.7.4/gqlpycgen/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,30 +12,32 @@
 ISO_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
 
 
 def timestamp():
     return datetime.utcnow().strftime(ISO_FORMAT)
 
 
-union_template = Template("""{{ pre_prefix }}{{ name }} {
+union_template = Template(
+    """{{ pre_prefix }}{{ name }} {
 {{ prefix }}{% for type_obj in types %}... on {{ type_obj.__name__ }} {{ '{' }}
 {% for k, v in get_type_hints(type_obj.__init__).items() %}
 {{ property_to_gql(type_obj, k, v, indent + 1, True) }}
 {% endfor %}
 {{ prefix }}{{ '}' }}
 {% endfor %}
 }
-""")
+"""
+)
 
 
 def union_gql(union, name, indent):
     if indent > MAX_DEPTH:
         return ""
-    prefix = ("    " * indent)
-    pre_prefix = ("    " * (indent - 1))
+    prefix = "    " * indent
+    pre_prefix = "    " * (indent - 1)
     types = union.__args__[:-1]
     # TODO - known issue, for the case where two of the types have a property with the same name and the don't have the exact same type it blows up
     #   keep in mind String != String!
     # type_properties = dict()
     # for ty in types:
     #     props = dict()
     #     for k, v in get_type_hints(type_obj.__init__).items()
@@ -60,22 +62,21 @@
         value = value.__args__[0]
     if cls.TYPES[name].startswith("List["):
         value = value.__args__[0]
         if hasattr(value, "__args__"):
             value = value.__args__[0]
             if hasattr(value, "__args__"):
                 value = value.__args__[0]
-    if hasattr(value, 'gql'):
+    if hasattr(value, "gql"):
         return value.gql(name, indent + 1, None)
     else:
         return ("    " * indent) + name
 
 
 class QueryBase(object):
-
     def __init__(self, client: Client):
         self.client = client
 
     def query(self, query: str, variables: Dict) -> Dict:
         gql_query = query
         try:
             results = self.client.execute(gql_query, variables)
@@ -99,29 +100,27 @@
             else:
                 return "query { %s }" % (gql)
         else:
             return "query { %s }" % (name)
 
 
 class MutationBase(QueryBase):
-
     def prepare(self, cls, name, variables, var_types):
         if hasattr(cls, "gql"):
             gql = cls.gql(name, 1, variables)
             args = ", ".join(["${}: {}".format(arg, var_types[arg].__name__) for arg in variables.keys()])
             if len(variables):
                 return "mutation %s (%s) { %s }" % (name, args, gql)
             else:
                 return "mutation { %s }" % (gql)
         else:
             return "mutation { %s }" % (name)
 
 
 class ObjectBase(object):
-
     def to_json(self) -> Dict:
         result = {}
         for k in self.FIELDS:
             value = getattr(self, k)
             if isinstance(value, list):
                 result[k] = value
                 if len(value) and hasattr(value[0], "to_json"):
@@ -133,18 +132,20 @@
         return result
 
     @classmethod
     def gql(cls, name: str, indent: int, variables: Dict) -> str:
         if indent > MAX_DEPTH:
             return ""
         bits = []
-        prefix = ("    " * indent)
-        pre_prefix = ("    " * (indent - 1))
+        prefix = "    " * indent
+        pre_prefix = "    " * (indent - 1)
         if variables and len(variables):
-            bits.append(pre_prefix + name + "(" + ", ".join(["{}: ${}".format(arg, arg) for arg in variables.keys()]) + ") {")
+            bits.append(
+                pre_prefix + name + "(" + ", ".join(["{}: ${}".format(arg, arg) for arg in variables.keys()]) + ") {"
+            )
         else:
             bits.append(pre_prefix + name + " {")
         hints = get_type_hints(cls.__init__)
         for k, v in hints.items():
             bits.append(property_to_gql(cls, k, v, indent))
         bits.append(pre_prefix + "}")
         return "\n".join(bits)
@@ -156,20 +157,20 @@
         args = {}
         hints = get_type_hints(cls.__init__)
         for k, v in hints.items():
             if k in obj:
                 if cls.TYPES[k].startswith("List["):
                     values = obj[k]
                     v = v.__args__[0]
-                    if hasattr(v, 'from_json'):
+                    if hasattr(v, "from_json"):
                         args[k] = []
                         for value in values:
                             args[k].append(v.from_json(value))
                     else:
                         args[k] = values
-                elif hasattr(v, 'from_json'):
+                elif hasattr(v, "from_json"):
                     args[k] = v.from_json(obj[k])
                 else:
                     args[k] = obj[k]
             else:
                 args[k] = None
         return cls(**args)
```

### Comparing `wf-gqlpycgen-0.7.3/gqlpycgen/client.py` & `wf_gqlpycgen-0.7.4/gqlpycgen/client.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,109 +1,139 @@
 from collections import OrderedDict
 from uuid import uuid4
 
+from cachetools import TTLCache
+import logging
 import requests
-
 import tenacity
-import logging
 import time
 
 from gqlpycgen.utils import json_dumps
 
 logger = logging.getLogger(__name__)
 
 exponential_retry = tenacity.retry(
-    stop = tenacity.stop_after_attempt(4),
-    wait = tenacity.wait_exponential(multiplier=0.2/2),
-    before = tenacity.before_log(logger, logging.DEBUG),
-    after = tenacity.after_log(logger, logging.DEBUG),
-    before_sleep = tenacity.before_sleep_log(logger, logging.WARNING)
+    stop=tenacity.stop_after_attempt(4),
+    wait=tenacity.wait_exponential(multiplier=0.2 / 2),
+    before=tenacity.before_log(logger, logging.DEBUG),
+    after=tenacity.after_log(logger, logging.DEBUG),
+    before_sleep=tenacity.before_sleep_log(logger, logging.WARNING),
 )
 
-DEFAULT_HTTP_REQUEST_TIMEOUT = 30 # HTTP request timeout in seconds
+DEFAULT_HTTP_REQUEST_TIMEOUT = 30  # HTTP request timeout in seconds
 
-class FileUpload(object):
 
+class FileUpload(object):
     def __init__(self):
         self.map = dict()
         self.list = []
         self.containsFiles = False
 
     def add_file(self, var_path, filename, file, mimetype="application/octet-stream"):
         self.containsFiles = True
         file_id = uuid4().hex
         self.map[file_id] = [var_path]
-        self.list.append((file_id, (filename, file, mimetype, ), ))
+        self.list.append(
+            (
+                file_id,
+                (
+                    filename,
+                    file,
+                    mimetype,
+                ),
+            )
+        )
 
 
 class Client(object):
-
     def __init__(self, uri, accessToken=None, client_credentials=None, timeout=DEFAULT_HTTP_REQUEST_TIMEOUT):
         self.uri = uri
-        self.accessToken = accessToken
         self.client_credentials = client_credentials
-        self.headers = {'Content-Type': 'application/json'}
-        self.headers_files = {}
-        if self.accessToken:
-            self.headers["Authorization"] = self.headers_files["Authorization"] = f'bearer {self.accessToken}'
-        elif self.accessToken is None and self.client_credentials:
-            try:
-                auth_response = requests.post(
-                    client_credentials["token_uri"],
-                    {
-                        "audience": client_credentials["audience"],
-                        "grant_type": "client_credentials",
-                        "client_id": client_credentials["client_id"],
-                        "client_secret": client_credentials["client_secret"]
-                    },
-                    timeout=timeout
-                )
-                self.accessToken = auth_response.json().get('access_token')
-                if self.accessToken:
-                    self.headers["Authorization"] = self.headers_files["Authorization"] = f'bearer {self.accessToken}'
-                else:
-                    raise Exception("invalid client_credentials")
-            except Exception as err:
-                import traceback
-                logger.error("An exception occured during Authorization")
-                traceback.print_exc()
-                raise Exception("invalid client_credentials") from err
+        self.timeout = timeout
+        self.headers = {"Content-Type": "application/json"}
+
+        self.tokens = {}
+        if accessToken is not None:
+            self.tokens["access_token"] = accessToken
+
+        if accessToken is None and self.client_credentials is None:
+            raise ValueError("Cannot instantiate Honeycomb Client without an accessToken or client_credentials")
+
+    def refresh_token(self):
+        try:
+            auth_response = requests.post(
+                self.client_credentials["token_uri"],
+                {
+                    "audience": self.client_credentials["audience"],
+                    "grant_type": "client_credentials",
+                    "client_id": self.client_credentials["client_id"],
+                    "client_secret": self.client_credentials["client_secret"],
+                },
+                timeout=self.timeout,
+            ).json()
+
+            access_token = auth_response.get("access_token", None)
+            if access_token is None:
+                raise Exception("invalid client_credentials")
+
+            # Refresh token once TTL is less than 5 minutes
+            self.tokens = TTLCache(maxsize=1, ttl=auth_response.get("expires_in") - 300)
+            self.tokens["access_token"] = access_token
+
+        except Exception as err:
+            import traceback
+
+            logger.error("An exception occured during Authorization")
+            traceback.print_exception(err)
+            raise Exception("invalid client_credentials") from err
+
+    @property
+    def headers(self):
+        if "access_token" not in self.tokens:
+            self.refresh_token()
+
+        return {"Authorization": f"Bearer {self.tokens['access_token']}", **self._headers}
+
+    @headers.setter
+    def headers(self, header_dict: dict):
+        self._headers = header_dict
 
     @exponential_retry
     def execute(self, query, variables=None, files=None, timeout=DEFAULT_HTTP_REQUEST_TIMEOUT):
         overall_start = time.time()
-        logger.debug('Client execute request body JSON:\n{}'.format(query))
-        logger.debug('Client execute request variables JSON:\n{}'.format(json_dumps(variables)))
-        payload = OrderedDict({
-            'query': query,
-            'variables': variables or {},
-        })
+        logger.debug("Client execute request body JSON:\n{}".format(query))
+        logger.debug("Client execute request variables JSON:\n{}".format(json_dumps(variables)))
+        payload = OrderedDict(
+            {
+                "query": query,
+                "variables": variables or {},
+            }
+        )
         if files and files.containsFiles:
             file_processing_start = time.time()
             data = {
-                'operations': json_dumps(payload),
-                'map': json_dumps(files.map),
+                "operations": json_dumps(payload),
+                "map": json_dumps(files.map),
             }
             file_processing_time = time.time() - file_processing_start
             post_start = time.time()
-            request = requests.post(self.uri, data=data, files=files.list, headers=self.headers_files, timeout=timeout)
+            request = requests.post(self.uri, data=data, files=files.list, headers=self.headers, timeout=timeout)
             post_time = time.time() - post_start
         else:
             file_processing_time = 0.0
             data = json_dumps(payload)
             post_start = time.time()
             request = requests.post(self.uri, data=data, headers=self.headers, timeout=timeout)
             post_time = time.time() - post_start
         request.raise_for_status()
         json_extraction_start = time.time()
         result = request.json()
         json_extraction_time = time.time() - json_extraction_start
         if "errors" in result:
             return result.get("errors")
         overall_time = time.time() - overall_start
-        logger.info('GraphQL client execute operation completed in {:.1f} ms (file processing: {:.1f} ms, POST operation: {:.1f} ms, JSON extraction: {:.1f} ms)'.format(
-            overall_time*1000,
-            file_processing_time*1000,
-            post_time*1000,
-            json_extraction_time*1000
-        ))
+        logger.info(
+            "GraphQL client execute operation completed in {:.1f} ms (file processing: {:.1f} ms, POST operation: {:.1f} ms, JSON extraction: {:.1f} ms)".format(
+                overall_time * 1000, file_processing_time * 1000, post_time * 1000, json_extraction_time * 1000
+            )
+        )
         return result.get("data")
```

### Comparing `wf-gqlpycgen-0.7.3/gqlpycgen/loader.py` & `wf_gqlpycgen-0.7.4/gqlpycgen/loader.py`

 * *Files identical despite different names*

### Comparing `wf-gqlpycgen-0.7.3/gqlpycgen/models.py` & `wf_gqlpycgen-0.7.4/gqlpycgen/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,67 +1,67 @@
 import json
 
 from jinja2 import Template
 
 
-LF = '\n'
-LFLF = '\n\n'
-LFTABTAB = '\n        '
+LF = "\n"
+LFLF = "\n\n"
+LFTABTAB = "\n        "
 
 
 def resolve_type(typeObj):
     if typeObj.get("kind") == "LIST":
-        return 'List[{}]'.format(resolve_type(typeObj.get("ofType")))
+        return "List[{}]".format(resolve_type(typeObj.get("ofType")))
     if typeObj.get("kind") == "NON_NULL":
         ofType = typeObj.get("ofType")
         if ofType.get("kind") == "LIST":
             # TODO - Not sure how to handle this one - I think the type system for this
             # library needs a rework/refactor so it can handle theses cases more gracefully
-            return 'List[{}]'.format(resolve_type(ofType.get("ofType")))
+            return "List[{}]".format(resolve_type(ofType.get("ofType")))
         else:
             return required(typeObj.get("ofType").get("name"))
     elif typeObj.get("kind"):
         return typeObj.get("name")
     else:
-        raise Warning('type {} is not understood'.format(typeObj))
+        raise Warning("type {} is not understood".format(typeObj))
         return None
 
 
 def required(typeStr):
     return "{}__Required".format(typeStr)
 
 
 class Field(object):
-
     def __init__(self, name, gtype):
         self.name = name
         self.gtype = gtype
 
     def __str__(self):
         return "{}: '{}'=None".format(self.name, self.gtype)
 
 
-objectTemplate = Template("""class {{name}}(ObjectBase):
+objectTemplate = Template(
+    """class {{name}}(ObjectBase):
     FIELDS = [{% for name in field_names %}"{{ name }}", {% endfor %}]
     TYPES = {{ '{' }}{% for field in fields %}"{{ field.name }}": "{{ field.gtype }}"{% if not loop.last %}, {% endif %}{% endfor %}{{ '}' }}
 
     def __init__(self, {% for field in fields %}{{ field }}{% if not loop.last %}, {% endif %}{% endfor %}):{% for field in fields %}
         self.{{ field.name }}{% if py36plus: %}: '{{ field.gtype }}'{% endif %} = {{ field.name }}{% endfor %}
 
 
 class {{name}}__Required({{name}}):
     pass
 
 
 
-""")
+"""
+)
 
 
 class Object(object):
-
     def __init__(self, typeObj):
         self.name = typeObj.get("name")
         self.field_names = [field.get("name") for field in typeObj.get("fields")]
         self.fields = []
         self.generate_argument_list(typeObj.get("fields"))
 
     def list_dependencies(self):
@@ -80,28 +80,26 @@
     def generate_argument_list(self, fields):
         for field in fields:
             name = field.get("name")
             ftype = resolve_type(field.get("type"))
             if ftype:
                 self.fields.append(Field(name, ftype))
             else:
-                raise Warning('field {} on {}, type not understood'.format(name, self.name))
+                raise Warning("field {} on {}, type not understood".format(name, self.name))
 
 
 class InputObject(Object):
-
     def __init__(self, typeObj):
         self.name = typeObj.get("name")
         self.field_names = [field.get("name") for field in typeObj.get("inputFields")]
         self.fields = []
         self.generate_argument_list(typeObj.get("inputFields"))
 
 
 class GraphEnum(object):
-
     def __init__(self, typeObj):
         self.name = typeObj.get("name")
         self.values = [value.get("name") for value in typeObj.get("enumValues")]
 
     def toPython(self, py36plus=True):
         props = ['    {value} = "{value}"'.format(value=value) for value in self.values]
         return """class {0}(Enum):
@@ -110,37 +108,38 @@
     def __str__(self):
         return str(self.value)
 
 
 {0}__Required = {0}
 
 
-""".format(self.name, LF.join(props))
+""".format(
+            self.name, LF.join(props)
+        )
 
 
 class Union(object):
-
     def __init__(self, typeObj):
         self.name = typeObj.get("name")
         self.possible_types = [pt.get("name") for pt in typeObj.get("possibleTypes")]
 
     def toPython(self, py36plus=True):
         return """{0} = Union[{1}]\n{0}__Required = Union[{1}]\n""".format(self.name, ", ".join(self.possible_types))
 
 
 class Scalar(object):
-
     def __init__(self, typeObj):
         self.name = typeObj.get("name")
 
     def toPython(self, py36plus=True):
         return "{0} = NewType('{0}', str)\n{0}__Required = NewType('{0}', str)\n".format(self.name)
 
 
-queryMethodTemplate = Template("""
+queryMethodTemplate = Template(
+    """
     def {{name}}(self, {% for arg in args %}{{ arg }}{% if not loop.last %}, {% endif %}{% endfor %}) -> {{ returns }}:
         args = [{% for arg in args %}"{{ arg }}"{% if not loop.last %}, {% endif %}{% endfor %}]
         variables = dict()
         var_types = dict()
 {% for arg in args %}
         if {{ arg.name }} is not None:
             var_types["{{ arg.name }}"] = {{ arg.gtype }}
@@ -148,66 +147,68 @@
                 variables["{{ arg.name }}"] = {{ arg.name }}.to_json()
             else:
                 variables["{{ arg.name }}"] = {{ arg.name }}
 {% endfor %}
         query = self.prepare({{ returns }}, "{{ name }}", variables, var_types)
         results = self.query(query, variables)
         return {{ returns }}.from_json(results.get("{{ name }}"))
-""")
+"""
+)
 
 
 class QueryMethod(object):
-
     def __init__(self, typeObj):
         self.name = typeObj.get("name")
         self.returns = resolve_type(typeObj.get("type"))
         self.args = []
         self.generate_argument_list(typeObj.get("args"))
 
     def generate_argument_list(self, fields):
         for field in fields:
             name = field.get("name")
             ftype = resolve_type(field.get("type"))
             if ftype:
                 self.args.append(Field(name, ftype))
             else:
-                raise Warning('arg {} on {}, type not understood'.format(name, self.name))
+                raise Warning("arg {} on {}, type not understood".format(name, self.name))
 
     def toPython(self, py36plus=True):
         return queryMethodTemplate.render(**self.__dict__)
 
 
 class Query(object):
-
     def __init__(self, typeObj):
         self.methods = []
         for field in typeObj.get("fields"):
             if not field.get("name").startswith("_"):
                 method = QueryMethod(field)
                 self.methods.append(method)
 
     def toPython(self, py36plus=True):
         return """class Query(QueryBase):
 {}
-""".format(LF.join([method.toPython(py36plus=py36plus) for method in self.methods]))
+""".format(
+            LF.join([method.toPython(py36plus=py36plus) for method in self.methods])
+        )
 
 
 class Mutation(object):
-
     def __init__(self, typeObj):
         self.methods = []
         for field in typeObj.get("fields"):
             if not field.get("name").startswith("_"):
                 method = QueryMethod(field)
                 self.methods.append(method)
 
     def toPython(self, py36plus=True):
         return """class Mutation(MutationBase):
 {}
-""".format(LF.join([method.toPython(py36plus=py36plus) for method in self.methods]))
+""".format(
+            LF.join([method.toPython(py36plus=py36plus) for method in self.methods])
+        )
 
 
 def filter_enums(typeObjs):
     for typeObj in typeObjs:
         if not typeObj.get("name").startswith("_") and typeObj.get("kind") == "ENUM":
             yield typeObj
 
@@ -216,15 +217,19 @@
     for typeObj in typeObjs:
         if not typeObj.get("name").startswith("_") and typeObj.get("kind") == "INPUT_OBJECT":
             yield typeObj
 
 
 def filter_objects(typeObjs):
     for typeObj in typeObjs:
-        if not typeObj.get("name").startswith("_") and typeObj.get("kind") == "OBJECT" and typeObj.get("name") not in ["Query", "Mutation"]:
+        if (
+            not typeObj.get("name").startswith("_")
+            and typeObj.get("kind") == "OBJECT"
+            and typeObj.get("name") not in ["Query", "Mutation"]
+        ):
             yield typeObj
 
 
 def filter_interfaces(typeObjs):
     for typeObj in typeObjs:
         if not typeObj.get("name").startswith("_") and typeObj.get("kind") == "INTERFACE":
             yield typeObj
@@ -234,9 +239,13 @@
     for typeObj in typeObjs:
         if not typeObj.get("name").startswith("_") and typeObj.get("kind") == "UNION":
             yield typeObj
 
 
 def filter_scalars(typeObjs):
     for typeObj in typeObjs:
-        if not typeObj.get("name").startswith("_") and typeObj.get("kind") == "SCALAR" and typeObj.get("name") not in ["String", "Int", "Boolean", "Float", "ID"]:
+        if (
+            not typeObj.get("name").startswith("_")
+            and typeObj.get("kind") == "SCALAR"
+            and typeObj.get("name") not in ["String", "Int", "Boolean", "Float", "ID"]
+        ):
             yield typeObj
```

### Comparing `wf-gqlpycgen-0.7.3/gqlpycgen/utils.py` & `wf_gqlpycgen-0.7.4/gqlpycgen/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 def decode(val):
     if val and hasattr(val, "decode"):
         return val.decode("utf8")
     return val
 
 
 class CustomJsonEncoder(json.JSONEncoder):
-
     def default(self, obj):
         if isinstance(obj, bytes):
             return obj.decode("utf8")
         if isinstance(obj, datetime):
             return obj.strftime(ISO_FORMAT)
         if isinstance(obj, date):
             return obj.strftime(DATE_FORMAT)
```

