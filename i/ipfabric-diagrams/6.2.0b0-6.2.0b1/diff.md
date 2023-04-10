# Comparing `tmp/ipfabric_diagrams-6.2.0b0.tar.gz` & `tmp/ipfabric_diagrams-6.2.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipfabric_diagrams-6.2.0b0.tar", max compression
+gzip compressed data, was "ipfabric_diagrams-6.2.0b1.tar", max compression
```

## Comparing `ipfabric_diagrams-6.2.0b0.tar` & `ipfabric_diagrams-6.2.0b1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1829 2023-03-16 17:27:29.558755 ipfabric_diagrams-6.2.0b0/ipfabric/__init__.py
--rw-r--r--   0        0        0     1666 2023-03-16 17:12:51.405968 ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/__init__.py
--rw-r--r--   0        0        0     7488 2023-03-16 15:31:26.870204 ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/graphs.py
--rw-r--r--   0        0        0     3612 2023-03-16 15:41:35.747531 ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/icmp.py
--rw-r--r--   0        0        0      580 2023-03-16 15:28:22.610735 ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/input_models/__init__.py
--rw-r--r--   0        0        0     3755 2023-03-16 13:36:25.692670 ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/input_models/constants.py
--rw-r--r--   0        0        0        0 2022-08-08 12:49:07.558933 ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/input_models/factory_defaults/__init__.py
--rw-r--r--   0        0        0     7009 2022-08-08 12:49:18.134109 ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
--rw-r--r--   0        0        0     2277 2022-08-08 12:49:18.135111 ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
--rw-r--r--   0        0        0    10497 2023-03-16 15:25:53.031095 ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/input_models/graph_parameters.py
--rw-r--r--   0        0        0    10534 2023-03-16 15:25:53.055402 ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/input_models/graph_settings.py
--rw-r--r--   0        0        0        0 2022-08-08 12:49:07.564024 ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/output_models/__init__.py
--rw-r--r--   0        0        0     2608 2023-03-16 15:25:53.062465 ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/output_models/graph_result.py
--rw-r--r--   0        0        0     1388 2023-03-16 12:53:31.446672 ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/output_models/protocols.py
--rw-r--r--   0        0        0     2641 2023-03-16 15:25:53.039709 ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/output_models/trace.py
--rw-r--r--   0        0        0      898 2023-03-16 17:12:51.413969 ipfabric_diagrams-6.2.0b0/ipfabric_diagrams/__init__.py
--rw-r--r--   0        0        0      167 2023-03-16 16:54:12.019841 ipfabric_diagrams-6.2.0b0/ipfabric_diagrams/graphs.py
--rw-r--r--   0        0        0     1562 2023-03-16 16:27:26.311693 ipfabric_diagrams-6.2.0b0/ipfabric_diagrams/icmp.py
--rw-r--r--   0        0        0     1087 2023-03-16 12:53:31.420028 ipfabric_diagrams-6.2.0b0/LICENSE
--rw-r--r--   0        0        0     1682 2023-03-16 16:55:58.331108 ipfabric_diagrams-6.2.0b0/pyproject.toml
--rw-r--r--   0        0        0     2572 2023-03-16 16:54:08.805400 ipfabric_diagrams-6.2.0b0/README.md
--rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.2.0b0/setup.py
--rw-r--r--   0        0        0     3629 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.2.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1829 2023-03-16 17:27:29.558755 ipfabric_diagrams-6.2.0b1/ipfabric/__init__.py
+-rw-r--r--   0        0        0     1666 2023-03-16 17:12:51.405968 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/__init__.py
+-rw-r--r--   0        0        0     7488 2023-03-16 15:31:26.870204 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/graphs.py
+-rw-r--r--   0        0        0     3612 2023-03-16 15:41:35.747531 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/icmp.py
+-rw-r--r--   0        0        0      580 2023-03-16 15:28:22.610735 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/__init__.py
+-rw-r--r--   0        0        0     3755 2023-03-16 13:36:25.692670 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/constants.py
+-rw-r--r--   0        0        0        0 2022-08-08 12:49:07.558933 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/factory_defaults/__init__.py
+-rw-r--r--   0        0        0     7009 2022-08-08 12:49:18.134109 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json
+-rw-r--r--   0        0        0     2277 2022-08-08 12:49:18.135111 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json
+-rw-r--r--   0        0        0    10497 2023-03-16 15:25:53.031095 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/graph_parameters.py
+-rw-r--r--   0        0        0    10534 2023-03-16 15:25:53.055402 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/graph_settings.py
+-rw-r--r--   0        0        0       68 2023-03-28 16:36:30.062929 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/output_models/__init__.py
+-rw-r--r--   0        0        0     2608 2023-03-16 15:25:53.062465 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/output_models/graph_result.py
+-rw-r--r--   0        0        0     1412 2023-03-28 16:01:35.397194 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/output_models/protocols.py
+-rw-r--r--   0        0        0     3187 2023-03-28 16:54:47.000317 ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/output_models/trace.py
+-rw-r--r--   0        0        0      898 2023-03-16 17:12:51.413969 ipfabric_diagrams-6.2.0b1/ipfabric_diagrams/__init__.py
+-rw-r--r--   0        0        0      167 2023-03-16 16:54:12.019841 ipfabric_diagrams-6.2.0b1/ipfabric_diagrams/graphs.py
+-rw-r--r--   0        0        0     1562 2023-03-16 16:27:26.311693 ipfabric_diagrams-6.2.0b1/ipfabric_diagrams/icmp.py
+-rw-r--r--   0        0        0     1087 2023-03-16 12:53:31.420028 ipfabric_diagrams-6.2.0b1/LICENSE
+-rw-r--r--   0        0        0     1682 2023-03-28 17:56:52.632001 ipfabric_diagrams-6.2.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2572 2023-03-16 16:54:08.805400 ipfabric_diagrams-6.2.0b1/README.md
+-rw-r--r--   0        0        0     3600 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.2.0b1/setup.py
+-rw-r--r--   0        0        0     3629 1970-01-01 00:00:00.000000 ipfabric_diagrams-6.2.0b1/PKG-INFO
```

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric/__init__.py` & `ipfabric_diagrams-6.2.0b1/ipfabric/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/__init__.py` & `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/graphs.py` & `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/graphs.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/icmp.py` & `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/icmp.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/input_models/__init__.py` & `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/input_models/constants.py` & `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/constants.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json` & `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/factory_defaults/networkSettings.json`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json` & `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/factory_defaults/pathLookupSettings.json`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/input_models/graph_parameters.py` & `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/graph_parameters.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/input_models/graph_settings.py` & `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/input_models/graph_settings.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/output_models/graph_result.py` & `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/output_models/graph_result.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/output_models/protocols.py` & `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/output_models/protocols.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,16 +6,16 @@
     # TODO py37 & py38 required
     from typing import Annotated, Literal
 except ImportError:
     from typing_extensions import Annotated, Literal
 
 
 class Transport(BaseModel):
-    src: List[str]
-    dst: List[str]
+    src: Union[List[str], str]
+    dst: Union[List[str], str]
 
 
 class TCP(Transport, BaseModel):
     flags: List[str]
     type: Literal["tcp"]
```

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric/diagrams/output_models/trace.py` & `ipfabric_diagrams-6.2.0b1/ipfabric/diagrams/output_models/trace.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,65 +56,92 @@
     header: PROTOCOLS
     headerType: str
     index: int
     type: Literal["insert header"]
 
 
 class Patch(BaseModel):
-    stack: Optional[List[int]] = None
-    ttl: Optional[int] = None
+    stack: Optional[List[int]]
+    ttl: Optional[int]
 
 
 class PatchHeader(BaseModel):
     patch: Patch
     index: int
     type: Literal["patch header"]
 
 
 class DropPacket(BaseModel):
     type: Literal["drop packet"]
     reason: str
-    severityInfo: Optional[SeverityInfo] = None
+    severityInfo: Optional[SeverityInfo]
 
 
-class SecurityCheck(BaseModel):
-    type: Literal["security check"]
-    decidingPolicyName: Optional[str] = None
-    decidingRule: Optional[List[int]] = None
+class SeverityEvent(BaseModel):
+    type: Literal["severity event"]
+    severityInfo: Optional[SeverityInfo]
+
+
+class BaseEvent(BaseModel):
+    decidingPolicyName: Optional[str]
+    decidingRule: Optional[List[int]]
     protocolId: str
     securityType: str
-    severityInfo: SeverityInfo
+    severityInfo: Optional[SeverityInfo]
+
+
+class SecurityCheck(BaseEvent, BaseModel):
+    type: Literal["security check"]
 
 
-class SecurityCheckIgnored(SecurityCheck, BaseModel):
+class SecurityCheckIgnored(BaseEvent, BaseModel):
     type: Literal["security check ignored"]
 
 
 class VirtualRouting(BaseModel):
     type: Literal["virtual routing"]
     ifaceName: str
 
 
 class AcceptPacket(BaseModel):
     type: Literal["accept packet"]
 
 
+class DestinationNAT(BaseEvent, BaseModel):
+    type: Literal["destination NAT"]
+    field: str
+
+
+class SourceNAT(BaseEvent, BaseModel):
+    type: Literal["source NAT"]
+    field: str
+
+
+class PolicyBasedRouting(BaseEvent, BaseModel):
+    type: Literal["policy based routing"]
+    field: Optional[str]
+
+
 EVENT = Annotated[
     Union[
         PacketDataMatch,
         RemoveHeader,
         TableEntryMatch,
         TableEntryNotFound,
         VirtualRouting,
         AcceptPacket,
         InsertHeader,
         PatchHeader,
         DropPacket,
+        SeverityEvent,
         SecurityCheckIgnored,
         SecurityCheck,
+        DestinationNAT,
+        PolicyBasedRouting,
+        SourceNAT
     ],
     Field(discriminator="type"),
 ]
 
 
 class Trace(BaseModel):
     chain: str
```

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric_diagrams/__init__.py` & `ipfabric_diagrams-6.2.0b1/ipfabric_diagrams/__init__.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/ipfabric_diagrams/icmp.py` & `ipfabric_diagrams-6.2.0b1/ipfabric_diagrams/icmp.py`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/LICENSE` & `ipfabric_diagrams-6.2.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/pyproject.toml` & `ipfabric_diagrams-6.2.0b1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ipfabric-diagrams"
-version = "v6.2.0b0"
+version = "v6.2.0b1"
 description = "Python package for interacting with IP Fabric Diagrams"
 authors = [
     "Justin Jeffery <justin.jeffery@ipfabric.io>",
     "Community Fabric <communityfabric@ipfabric.io>"
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `ipfabric_diagrams-6.2.0b0/README.md` & `ipfabric_diagrams-6.2.0b1/README.md`

 * *Files identical despite different names*

### Comparing `ipfabric_diagrams-6.2.0b0/setup.py` & `ipfabric_diagrams-6.2.0b1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 ['ipfabric>=6.2.0b0,<6.3.0', 'typing-extensions>=4.5,<5.0']
 
 extras_require = \
 {'examples': ['rich>=13.3.0,<14.0.0']}
 
 setup_kwargs = {
     'name': 'ipfabric-diagrams',
-    'version': '6.2.0b0',
+    'version': '6.2.0b1',
     'description': 'Python package for interacting with IP Fabric Diagrams',
     'long_description': "# IP Fabric\n\nipfabric_diagrams is a Python module for connecting to and graphing topologies against an IP Fabric instance.\n\n## About\n\nFounded in 2015, [IP Fabric](https://ipfabric.io/) develops network infrastructure visibility and analytics solution to\nhelp enterprise network and security teams with network assurance and automation across multi-domain heterogeneous\nenvironments. From in-depth discovery, through graph visualization, to packet walks and complete network history, IP\nFabric enables to confidently replace manual tasks necessary to handle growing network complexity driven by relentless\ndigital transformation.\n\n## v7.0.0 Deprecation Notices\n\nIn `ipfabric>=v7.0.0` the following will be deprecated:\n\n- `ipfabric_diagrams` package will move to `ipfabric.diagrams`\n- Python 3.7 support will be removed.\n- The use of `token='<TOKEN>'` or `username='<USER>', password='<PASS>'` in `IPFClient()` will be removed:\n  - Token: `IPFClient(auth='TOKEN')`\n  - User/Pass: `IPFClient(auth=('USER', 'PASS'))`\n  - `.env` file will only accept `IPF_TOKEN` or (`IPF_USERNAME` and `IPF_PASSWORD`) and not `auth`\n\n## Versioning\n\nStarting with IP Fabric version 5.0.x the python-ipfabric and python-ipfabric-diagrams will need to\nmatch your IP Fabric version.  The API's are changing and instead of `api/v1` they will now be `api/v5.0`.\n\nVersion 5.1 will have backwards compatability with version 5.0 however 6.0 will not support any 5.x versions.\nBy ensuring that your ipfabric SDK's match your IP Fabric Major Version will ensure compatibility and will continue to work.\n\n## Installation\n\n```\npip install ipfabric-diagrams\n```\n\n## Introduction\n\nThis package is used for diagramming via the API for IP Fabric v4.3.0.  \nExamples can be located under [examples](examples/) directory.\n\n## Authentication\nPlease take a look at [python-ipfabric](https://gitlab.com/ip-fabric/integrations/python-ipfabric#authentication) \nfor all authentication options.\n\n```python\nfrom ipfabric.diagrams import IPFDiagram\nipf = IPFDiagram(base_url='https://demo3.ipfabric.io/', auth='token', verify=False, timeout=15)\n```\n\n## Development\n\nIPFabric uses poetry for the python packaging module. Install poetry globally:\n\n```\npip install poetry\n```\n\nTo install a virtual environment run the following command in the root of this directory.\n\n```\npoetry install\n```\n\nTo test and build:\n\n```\npoetry run pytest\npoetry build\n```\n\nPrior to pushing changes run:\n```\npoetry run black ipfabric_diagrams ipfabric\npoetry update\n```\n",
     'author': 'Justin Jeffery',
     'author_email': 'justin.jeffery@ipfabric.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams',
```

### Comparing `ipfabric_diagrams-6.2.0b0/PKG-INFO` & `ipfabric_diagrams-6.2.0b1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipfabric-diagrams
-Version: 6.2.0b0
+Version: 6.2.0b1
 Summary: Python package for interacting with IP Fabric Diagrams
 Home-page: https://gitlab.com/ip-fabric/integrations/python-ipfabric-diagrams
 License: MIT
 Keywords: ipfabric,ip-fabric,community-fabric
 Author: Justin Jeffery
 Author-email: justin.jeffery@ipfabric.io
 Requires-Python: >=3.7.1,<4.0.0
```

