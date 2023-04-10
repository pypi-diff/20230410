# Comparing `tmp/ecs_composex_msk_cluster-0.3.0.post0.tar.gz` & `tmp/ecs_composex_msk_cluster-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecs_composex_msk_cluster-0.3.0.post0.tar", max compression
+gzip compressed data, was "ecs_composex_msk_cluster-0.3.1.tar", max compression
```

## Comparing `ecs_composex_msk_cluster-0.3.0.post0.tar` & `ecs_composex_msk_cluster-0.3.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    16725 2022-04-24 10:25:44.149879 ecs_composex_msk_cluster-0.3.0.post0/LICENSE
--rw-r--r--   0        0        0      392 2022-04-24 10:25:44.055880 ecs_composex_msk_cluster-0.3.0.post0/MANIFEST.in
--rw-r--r--   0        0        0     1165 2023-03-16 20:50:05.293054 ecs_composex_msk_cluster-0.3.0.post0/README.rst
--rw-r--r--   0        0        0      176 2023-03-16 20:51:37.617062 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/__init__.py
--rw-r--r--   0        0        0     6556 2023-01-12 10:42:26.973223 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster.py
--rw-r--r--   0        0        0     1064 2022-11-21 21:44:03.087655 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_conditions.py
--rw-r--r--   0        0        0     1114 2022-11-21 21:44:03.103654 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_ecs.py
--rw-r--r--   0        0        0     7943 2022-11-21 21:44:03.104655 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_ecs_iam.py
--rw-r--r--   0        0        0     2816 2023-03-11 22:46:19.588524 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_logging.py
--rw-r--r--   0        0        0      501 2022-11-21 21:44:03.144654 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_module.py
--rw-r--r--   0        0        0     2391 2022-11-21 21:44:03.145654 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_params.py
--rw-r--r--   0        0        0      212 2023-03-16 20:51:38.061067 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_perms.json
--rw-r--r--   0        0        0     1731 2022-11-21 21:44:03.163654 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_stack.py
--rw-r--r--   0        0        0     8363 2022-11-21 21:44:03.164654 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_template.py
--rw-r--r--   0        0        0     1401 2022-11-21 21:44:03.186653 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_configuration.py
--rw-r--r--   0        0        0     8504 2023-03-11 22:44:53.532492 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_sg_ingress.py
--rw-r--r--   0        0        0     3144 2022-11-21 21:44:03.188653 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_storage_scaling.py
--rw-r--r--   0        0        0     8392 2023-03-16 20:51:38.061067 ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/x-msk_cluster.spec.json
--rw-r--r--   0        0        0     2341 2023-03-16 20:51:37.617062 ecs_composex_msk_cluster-0.3.0.post0/pyproject.toml
--rw-r--r--   0        0        0     1930 1970-01-01 00:00:00.000000 ecs_composex_msk_cluster-0.3.0.post0/setup.py
--rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 ecs_composex_msk_cluster-0.3.0.post0/PKG-INFO
+-rw-r--r--   0        0        0    16725 2022-04-24 10:25:44.149879 ecs_composex_msk_cluster-0.3.1/LICENSE
+-rw-r--r--   0        0        0      392 2022-04-24 10:25:44.055880 ecs_composex_msk_cluster-0.3.1/MANIFEST.in
+-rw-r--r--   0        0        0     1165 2023-03-16 20:50:05.293054 ecs_composex_msk_cluster-0.3.1/README.rst
+-rw-r--r--   0        0        0      170 2023-04-10 21:43:06.725304 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/__init__.py
+-rw-r--r--   0        0        0     6556 2023-01-12 10:42:26.973223 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster.py
+-rw-r--r--   0        0        0     1064 2022-11-21 21:44:03.087655 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_conditions.py
+-rw-r--r--   0        0        0     1114 2022-11-21 21:44:03.103654 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_ecs.py
+-rw-r--r--   0        0        0     7943 2022-11-21 21:44:03.104655 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_ecs_iam.py
+-rw-r--r--   0        0        0     2816 2023-03-11 22:46:19.588524 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_logging.py
+-rw-r--r--   0        0        0      501 2022-11-21 21:44:03.144654 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_module.py
+-rw-r--r--   0        0        0     2843 2023-04-10 21:42:45.826048 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_params.py
+-rw-r--r--   0        0        0      212 2023-04-10 21:43:07.170309 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_perms.json
+-rw-r--r--   0        0        0     1731 2022-11-21 21:44:03.163654 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_stack.py
+-rw-r--r--   0        0        0     9535 2023-04-10 21:42:45.826048 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_template.py
+-rw-r--r--   0        0        0     1401 2022-11-21 21:44:03.186653 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_configuration.py
+-rw-r--r--   0        0        0     8504 2023-03-11 22:44:53.532492 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_sg_ingress.py
+-rw-r--r--   0        0        0     3144 2022-11-21 21:44:03.188653 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_storage_scaling.py
+-rw-r--r--   0        0        0     8392 2023-04-10 21:43:07.170309 ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/x-msk_cluster.spec.json
+-rw-r--r--   0        0        0     2329 2023-04-10 21:43:06.725304 ecs_composex_msk_cluster-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     1924 1970-01-01 00:00:00.000000 ecs_composex_msk_cluster-0.3.1/setup.py
+-rw-r--r--   0        0        0     2506 1970-01-01 00:00:00.000000 ecs_composex_msk_cluster-0.3.1/PKG-INFO
```

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/LICENSE` & `ecs_composex_msk_cluster-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/README.rst` & `ecs_composex_msk_cluster-0.3.1/README.rst`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster.py` & `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_conditions.py` & `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_conditions.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_ecs.py` & `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_ecs.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_ecs_iam.py` & `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_ecs_iam.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_logging.py` & `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_logging.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_stack.py` & `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_stack.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_cluster_template.py` & `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_cluster_template.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from compose_x_common.aws.msk import list_all_kafka_versions
 from compose_x_common.compose_x_common import keyisset, set_else_none
 from ecs_composex.common.cfn_conditions import define_stack_name
 from ecs_composex.common.cfn_params import ROOT_STACK_NAME
 from ecs_composex.common.logging import LOG
 from ecs_composex.common.stacks import ComposeXStack
 from ecs_composex.common.troposphere_tools import (
+    Parameter,
     add_outputs,
     add_resource,
     build_template,
 )
 from ecs_composex.resources_import import import_record_properties
 from ecs_composex.vpc.vpc_params import (
     APP_SUBNETS,
@@ -42,14 +43,15 @@
     CLUSTER_PRIVATE_ONLY_CON,
     CLUSTER_PRIVATE_ONLY_CON_T,
     CLUSTER_PUBLICLY_ADDRESSED_CON,
     CLUSTER_PUBLICLY_ADDRESSED_CON_T,
 )
 from .msk_cluster_params import (
     MSK_CLUSTER_ADDRESSING_TYPE,
+    MSK_CLUSTER_INSTANCE_TYPES,
     MSK_CLUSTER_SG_PARAM,
     MSK_CLUSTER_USE_SASL_IAM,
     MSK_CLUSTER_USE_SASL_SCRAM,
     MSK_PORTS_MAPPING,
 )
 from .msk_sg_ingress import handle_msk_auth_settings
 from .msk_storage_scaling import add_storage_scaling
@@ -63,59 +65,89 @@
     def __init__(self, name, stack_template, cluster, top_stack, **kwargs):
         self.cluster = cluster
         super().__init__(name, stack_template, **kwargs)
         self.parent_stack = top_stack
         self.cluster.stack = self
 
 
-def validate_cluster_version(cluster: MskCluster, input_version) -> None:
+def validate_cluster_version(cluster: MskCluster, input_version) -> Parameter:
     """
     Validates the kafka version
     """
-    versions = list_all_kafka_versions(session=cluster.lookup_session)
-    for version in versions:
-        if version["Version"] == input_version:
-            break
-    else:
-        raise ValueError(
-            f"{cluster.module.res_key}.{cluster.name} - ",
-            f"Version {input_version} is not valid. Versions supported",
-            [_v["Version"] for _v in versions if _v["Status"] == "ACTIVE"],
+    valid_versions: list[str] = [
+        _version["Version"]
+        for _version in list_all_kafka_versions(session=cluster.lookup_session)
+        if _version["Status"] == "ACTIVE"
+    ]
+    if input_version in valid_versions:
+        return Parameter(
+            "KafkaVersion",
+            Type="String",
+            AllowedValues=valid_versions,
+            Default=input_version,
         )
-    if keyisset("Status", version) and version["Status"] != "ACTIVE":
+    else:
         raise ValueError(
-            f"{cluster.module.res_key}.{cluster.name} - "
-            f"Version {version['Version']} is not active: {version['Status']}"
+            "Version {} is not valid. Active versions supported: {}".format(
+                input_version, valid_versions
+            )
         )
 
 
 def set_msk_cluster_template(module: XResourceModule, cluster: MskCluster) -> Template:
     template = build_template(
         f"{module.res_key}.{cluster.name} Stack Template",
         [
             MSK_CLUSTER_USE_SASL_IAM,
             MSK_CLUSTER_USE_SASL_SCRAM,
             MSK_CLUSTER_ADDRESSING_TYPE,
             VPC_ID,
             STORAGE_SUBNETS,
             APP_SUBNETS,
             PUBLIC_SUBNETS,
+            MSK_CLUSTER_INSTANCE_TYPES,
         ],
     )
     template.add_condition(
         CLUSTER_PUBLICLY_ADDRESSED_CON_T, CLUSTER_PUBLICLY_ADDRESSED_CON
     )
     template.add_condition(CLUSTER_PRIVATE_ONLY_CON_T, CLUSTER_PRIVATE_ONLY_CON)
     template.add_condition(CLIENTS_USE_SASL_SCRAM_CON_T, CLIENTS_USE_SASL_SCRAM_CON)
     template.add_condition(CLIENTS_USE_SASL_IAM_CON_T, CLIENTS_USE_SASL_IAM_CON)
     template.add_condition(CLIENTS_USE_TLS_AUTH_CON_T, CLIENTS_USE_TLS_AUTH_CON)
     template.add_mapping("MSKPorts", MSK_PORTS_MAPPING)
     return template
 
 
+def set_instance_type(cluster: MskCluster, cluster_stack: ComposeXStack) -> None:
+    """
+    Checks the instance type value. Replaces it with parameter.
+    Updates parameter value if valid, uses Default if not
+    """
+    instance_type = getattr(cluster.cfn_resource.BrokerNodeGroupInfo, "InstanceType")
+    if instance_type not in MSK_CLUSTER_INSTANCE_TYPES.AllowedValues:
+        LOG.error(
+            "{}.{} - {} InstanceType is not valid. Using default {}".format(
+                cluster.module.res_key,
+                cluster.name,
+                instance_type,
+                MSK_CLUSTER_INSTANCE_TYPES.Default,
+            )
+        )
+    else:
+        cluster_stack.Parameters.update(
+            {MSK_CLUSTER_INSTANCE_TYPES.title: instance_type}
+        )
+    setattr(
+        cluster.cfn_resource.BrokerNodeGroupInfo,
+        "InstanceType",
+        Ref(MSK_CLUSTER_INSTANCE_TYPES),
+    )
+
+
 def build_msk_clusters(module: XResourceModule, msk_top_stack: ComposeXStack):
     """
     Creates a new MSK cluster from properties
     Each MSK cluster gets its own template & own stack to allow for better re-usability.
     """
     for cluster in module.new_resources:
         cluster_template = set_msk_cluster_template(module, cluster)
@@ -183,28 +215,33 @@
             cluster_props.update(
                 {
                     "BrokerNodeGroupInfo": {"SecurityGroups": security_groups},
                     "ClientSubnets": Ref(cluster.subnets_override),
                 }
             )
         cluster.cfn_resource = AwsMskCluster(cluster.logical_name, **cluster_props)
-        validate_cluster_version(cluster, cluster.cfn_resource.KafkaVersion)
+        version_param = cluster_template.add_parameter(
+            validate_cluster_version(cluster, cluster.cfn_resource.KafkaVersion)
+        )
+        setattr(cluster.cfn_resource, "KafkaVersion", Ref(version_param))
         cluster_stack = MskClusterStack(
             cluster.logical_name,
             cluster=cluster,
             stack_template=cluster_template,
             top_stack=msk_top_stack,
             stack_parameters={
                 ROOT_STACK_NAME.title: Ref(ROOT_STACK_NAME),
                 VPC_ID.title: Ref(VPC_ID),
                 STORAGE_SUBNETS.title: Ref(STORAGE_SUBNETS),
                 PUBLIC_SUBNETS.title: Ref(PUBLIC_SUBNETS),
                 APP_SUBNETS.title: Ref(APP_SUBNETS),
+                version_param.title: version_param.Default,
             },
         )
+        set_instance_type(cluster, cluster_stack)
 
         handle_msk_auth_settings(cluster)
         add_resource(cluster_template, cluster.cfn_resource)
         add_storage_scaling(cluster, cluster_template)
         add_resource(msk_top_stack.stack_template, cluster_stack)
         cluster.init_outputs()
         cluster.generate_outputs()
```

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_configuration.py` & `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_configuration.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_sg_ingress.py` & `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_sg_ingress.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/msk_storage_scaling.py` & `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/msk_storage_scaling.py`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/ecs_composex_msk_cluster/x-msk_cluster.spec.json` & `ecs_composex_msk_cluster-0.3.1/ecs_composex_msk_cluster/x-msk_cluster.spec.json`

 * *Files identical despite different names*

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/pyproject.toml` & `ecs_composex_msk_cluster-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ecs_composex_msk_cluster"
-version = "0.3.0.post0"
+version = "0.3.1"
 description = "msk_cluster - AWS MSK Cluster module for ECS Compose-X"
 authors = ["johnpreston <john@compose-x.io>"]
 license = "MPL-2.0"
 
 classifiers = [
   "Development Status :: 4 - Beta",
   "Intended Audience :: Developers",
@@ -76,15 +76,15 @@
   "*/cli.py"
 ]
 
 [tool.tbump]
 github_url = "https://github.com/compose-x/ecs_composex_msk_cluster"
 
 [tool.tbump.version]
-current = "0.3.0.post0"
+current = "0.3.1"
 
 regex = '''
   (?P<major>\d+)
   \.
   (?P<minor>\d+)
   \.
   (?P<patch>\d+)
```

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/setup.py` & `ecs_composex_msk_cluster-0.3.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 install_requires = \
 ['compose-x-common>=1.2,<2.0', 'ecs_composex>=0.23.7,<0.24.0']
 
 setup_kwargs = {
     'name': 'ecs-composex-msk-cluster',
-    'version': '0.3.0.post0',
+    'version': '0.3.1',
     'description': 'msk_cluster - AWS MSK Cluster module for ECS Compose-X',
     'long_description': '\n.. meta::\n    :description: ECS Compose-X MSK Cluster\n    :keywords: AWS, ECS, docker, compose, MSK, kafka\n\n================\nmsk_cluster\n================\n\n.. image:: https://img.shields.io/pypi/v/ecs_composex_msk_cluster.svg\n    :target: https://pypi.python.org/pypi/ecs_composex_msk_cluster\n\n\nThis package is an extension to `ECS Compose-X`_ that manages Creation of new MSK clusters and automatically links\nto services to grant access and permissions.\n\nInstall\n==========\n\n.. code-block:: bash\n\n    python3 -m venv venv\n    source venv/bin/activate\n    # With poetry\n\n    pip install pip poetry -U\n    poetry install\n\n    # Via pip\n    pip install pip -U\n    pip install ecs-composex-msk-cluster\n\nSyntax Reference\n==================\n\n.. code-block:: yaml\n\n    x-msk_cluster:\n          Properties: {}\n          Lookup: {}\n          Settings: {}\n          Services: {}\n\n`Full documentation <https://msk-cluster.docs.compose-x.io/>`_\n\nExamples can be found in ``use-cases`` in this repository.\n\n.. _ECS Compose-X: https://docs.compose-x.io\n.. _Properties for MSK Cluster: https://docs.aws.amazon.com/AWSCloudFormation/latest/UserGuide/aws-resource-msk-cluster.html\n',
     'author': 'johnpreston',
     'author_email': 'john@compose-x.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `ecs_composex_msk_cluster-0.3.0.post0/PKG-INFO` & `ecs_composex_msk_cluster-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ecs-composex-msk-cluster
-Version: 0.3.0.post0
+Version: 0.3.1
 Summary: msk_cluster - AWS MSK Cluster module for ECS Compose-X
 License: MPL-2.0
 Author: johnpreston
 Author-email: john@compose-x.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

