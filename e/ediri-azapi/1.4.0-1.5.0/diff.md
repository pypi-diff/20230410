# Comparing `tmp/ediri_azapi-1.4.0.tar.gz` & `tmp/ediri_azapi-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ediri_azapi-1.4.0.tar", last modified: Thu Mar  2 13:19:23 2023, max compression
+gzip compressed data, was "ediri_azapi-1.5.0.tar", last modified: Mon Apr 10 19:25:09 2023, max compression
```

## Comparing `ediri_azapi-1.4.0.tar` & `ediri_azapi-1.5.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:19:23.846847 ediri_azapi-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-03-02 13:19:23.846847 ediri_azapi-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:19:23.842846 ediri_azapi-1.4.0/ediri_azapi/
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:19:23.846847 ediri_azapi-1.4.0/ediri_azapi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi/get_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     9854 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi/get_resource_action.py
--rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    30697 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    39377 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    26754 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi/resource_action.py
--rw-r--r--   0 runner    (1001) docker     (123)    32928 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi/update_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-02 13:19:23.846847 ediri_azapi-1.4.0/ediri_azapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      605 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/ediri_azapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-02 13:19:23.846847 ediri_azapi-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-03-02 13:19:23.000000 ediri_azapi-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:09.242724 ediri_azapi-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-04-10 19:25:09.242724 ediri_azapi-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:09.242724 ediri_azapi-1.5.0/ediri_azapi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/ediri_azapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/ediri_azapi/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8122 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/ediri_azapi/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:09.242724 ediri_azapi-1.5.0/ediri_azapi/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/ediri_azapi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4935 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/ediri_azapi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9319 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/ediri_azapi/get_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/ediri_azapi/get_resource_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5815 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/ediri_azapi/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30697 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/ediri_azapi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/ediri_azapi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/ediri_azapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    39377 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/ediri_azapi/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24128 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/ediri_azapi/resource_action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29364 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/ediri_azapi/update_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 19:25:09.242724 ediri_azapi-1.5.0/ediri_azapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5645 2023-04-10 19:25:09.000000 ediri_azapi-1.5.0/ediri_azapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      605 2023-04-10 19:25:09.000000 ediri_azapi-1.5.0/ediri_azapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:25:09.000000 ediri_azapi-1.5.0/ediri_azapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 19:25:09.000000 ediri_azapi-1.5.0/ediri_azapi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-10 19:25:09.000000 ediri_azapi-1.5.0/ediri_azapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-10 19:25:09.000000 ediri_azapi-1.5.0/ediri_azapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 19:25:09.242724 ediri_azapi-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-04-10 19:25:08.000000 ediri_azapi-1.5.0/setup.py
```

### Comparing `ediri_azapi-1.4.0/PKG-INFO` & `ediri_azapi-1.5.0/ediri_azapi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ediri_azapi
-Version: 1.4.0
+Name: ediri-azapi
+Version: 1.5.0
 Summary: A Pulumi package for creating and managing Azapi resources
 Home-page: https://github.com/dirien/pulumi-azapi
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-azapi
 Keywords: pulumi azapi category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ediri_azapi-1.4.0/README.md` & `ediri_azapi-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.4.0/ediri_azapi/__init__.py` & `ediri_azapi-1.5.0/ediri_azapi/__init__.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.4.0/ediri_azapi/_inputs.py` & `ediri_azapi-1.5.0/ediri_azapi/_inputs.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.4.0/ediri_azapi/_utilities.py` & `ediri_azapi-1.5.0/ediri_azapi/_utilities.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.4.0/ediri_azapi/config/vars.py` & `ediri_azapi-1.5.0/ediri_azapi/config/vars.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.4.0/ediri_azapi/get_resource.py` & `ediri_azapi-1.5.0/ediri_azapi/get_resource.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.4.0/ediri_azapi/get_resource_action.py` & `ediri_azapi-1.5.0/ediri_azapi/get_resource_action.py`

 * *Files 10% similar despite different names*

```diff
@@ -118,32 +118,14 @@
                         type: Optional[str] = None,
                         opts: Optional[pulumi.InvokeOptions] = None) -> AwaitableGetResourceActionResult:
     """
     This resource can perform resource action which gets information from an existing resource.
     It's recommended to use `ResourceAction` data source to perform readonly action, please use `ResourceAction` resource,
     if user wants to perform actions which change a resource's state.
 
-    ## Example Usage
-
-    ```python
-    import pulumi
-    import pulumi_azapi as azapi
-    import pulumi_azure as azure
-
-    example_resource_group = azure.core.ResourceGroup("exampleResourceGroup", location="west europe")
-    example_account = azure.automation.Account("exampleAccount",
-        resource_group_name=example_resource_group.name,
-        location=example_resource_group.location,
-        sku_name="Basic")
-    example_resource_action = azapi.get_resource_action_output(type="Microsoft.Automation/automationAccounts@2021-06-22",
-        resource_id=example_account.id,
-        action="listKeys",
-        response_export_values=["*"])
-    ```
-
 
     :param str action: The name of the resource action. It's also possible to make Http requests towards the resource ID if leave this field empty.
     :param str body: A JSON object that contains the request body.
     :param str method: Specifies the Http method of the azure resource action. Allowed values are `POST` and `GET`. Defaults to `POST`.
     :param str resource_id: The ID of an existing azure source.
     :param Sequence[str] response_export_values: A list of path that needs to be exported from response body.
            Setting it to `["*"]` will export the full response body.
@@ -184,32 +166,14 @@
                                type: Optional[pulumi.Input[str]] = None,
                                opts: Optional[pulumi.InvokeOptions] = None) -> pulumi.Output[GetResourceActionResult]:
     """
     This resource can perform resource action which gets information from an existing resource.
     It's recommended to use `ResourceAction` data source to perform readonly action, please use `ResourceAction` resource,
     if user wants to perform actions which change a resource's state.
 
-    ## Example Usage
-
-    ```python
-    import pulumi
-    import pulumi_azapi as azapi
-    import pulumi_azure as azure
-
-    example_resource_group = azure.core.ResourceGroup("exampleResourceGroup", location="west europe")
-    example_account = azure.automation.Account("exampleAccount",
-        resource_group_name=example_resource_group.name,
-        location=example_resource_group.location,
-        sku_name="Basic")
-    example_resource_action = azapi.get_resource_action_output(type="Microsoft.Automation/automationAccounts@2021-06-22",
-        resource_id=example_account.id,
-        action="listKeys",
-        response_export_values=["*"])
-    ```
-
 
     :param str action: The name of the resource action. It's also possible to make Http requests towards the resource ID if leave this field empty.
     :param str body: A JSON object that contains the request body.
     :param str method: Specifies the Http method of the azure resource action. Allowed values are `POST` and `GET`. Defaults to `POST`.
     :param str resource_id: The ID of an existing azure source.
     :param Sequence[str] response_export_values: A list of path that needs to be exported from response body.
            Setting it to `["*"]` will export the full response body.
```

### Comparing `ediri_azapi-1.4.0/ediri_azapi/outputs.py` & `ediri_azapi-1.5.0/ediri_azapi/outputs.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.4.0/ediri_azapi/provider.py` & `ediri_azapi-1.5.0/ediri_azapi/provider.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.4.0/ediri_azapi/resource.py` & `ediri_azapi-1.5.0/ediri_azapi/resource.py`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.4.0/ediri_azapi/resource_action.py` & `ediri_azapi-1.5.0/ediri_azapi/resource_action.py`

 * *Files 4% similar despite different names*

```diff
@@ -305,46 +305,14 @@
         """
         This resource can perform any Azure resource manager resource action.
         It's recommended to use `ResourceAction` resource to perform actions which change a resource's state, please use `ResourceAction` data source,
         if user wants to perform readonly action.
 
         > **Note** When delete `ResourceAction`, no operation will be performed.
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import ediri_azapi as azapi
-        import pulumi_azure as azure
-
-        config = pulumi.Config()
-        enabled = config.get_bool("enabled")
-        if enabled is None:
-            enabled = False
-        example = azure.core.ResourceGroup("example", location="west europe")
-        test = azure.appplatform.SpringCloudService("test",
-            resource_group_name=azurerm_resource_group["test"]["name"],
-            location=azurerm_resource_group["test"]["location"],
-            sku_name="S0")
-        start = []
-        for range in [{"value": i} for i in range(0, 1 if enabled else 0 == True)]:
-            start.append(azapi.ResourceAction(f"start-{range['value']}",
-                type="Microsoft.AppPlatform/Spring@2022-05-01-preview",
-                resource_id=test.id,
-                action="start",
-                response_export_values=["*"]))
-        stop = []
-        for range in [{"value": i} for i in range(0, 0 if enabled else 1 == True)]:
-            stop.append(azapi.ResourceAction(f"stop-{range['value']}",
-                type="Microsoft.AppPlatform/Spring@2022-05-01-preview",
-                resource_id=test.id,
-                action="stop",
-                response_export_values=["*"]))
-        ```
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] action: The name of the resource action. It's also possible to make Http requests towards the resource ID if leave this field empty.
         :param pulumi.Input[str] body: A JSON object that contains the request body.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid modify azapi resources at the same time.
         :param pulumi.Input[str] method: Specifies the Http method of the azure resource action. Allowed values are `POST`, `PATCH`, `PUT` and `DELETE`. Defaults to `POST`.
         :param pulumi.Input[str] resource_id: The ID of an existing azure source.
@@ -366,46 +334,14 @@
         """
         This resource can perform any Azure resource manager resource action.
         It's recommended to use `ResourceAction` resource to perform actions which change a resource's state, please use `ResourceAction` data source,
         if user wants to perform readonly action.
 
         > **Note** When delete `ResourceAction`, no operation will be performed.
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import ediri_azapi as azapi
-        import pulumi_azure as azure
-
-        config = pulumi.Config()
-        enabled = config.get_bool("enabled")
-        if enabled is None:
-            enabled = False
-        example = azure.core.ResourceGroup("example", location="west europe")
-        test = azure.appplatform.SpringCloudService("test",
-            resource_group_name=azurerm_resource_group["test"]["name"],
-            location=azurerm_resource_group["test"]["location"],
-            sku_name="S0")
-        start = []
-        for range in [{"value": i} for i in range(0, 1 if enabled else 0 == True)]:
-            start.append(azapi.ResourceAction(f"start-{range['value']}",
-                type="Microsoft.AppPlatform/Spring@2022-05-01-preview",
-                resource_id=test.id,
-                action="start",
-                response_export_values=["*"]))
-        stop = []
-        for range in [{"value": i} for i in range(0, 0 if enabled else 1 == True)]:
-            stop.append(azapi.ResourceAction(f"stop-{range['value']}",
-                type="Microsoft.AppPlatform/Spring@2022-05-01-preview",
-                resource_id=test.id,
-                action="stop",
-                response_export_values=["*"]))
-        ```
-
         :param str resource_name: The name of the resource.
         :param ResourceActionArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(ResourceActionArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `ediri_azapi-1.4.0/ediri_azapi/update_resource.py` & `ediri_azapi-1.5.0/ediri_azapi/update_resource.py`

 * *Files 4% similar despite different names*

```diff
@@ -364,56 +364,14 @@
         """
         This resource can manage a subset of any existing Azure resource manager resource's properties.
 
         > **Note** This resource is used to add or modify properties on an existing resource.
         When delete `UpdateResource`, no operation will be performed, and these properties will stay unchanged.
         If you want to restore the modified properties to some values, you must apply the restored properties before deleting.
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import ediri_azapi as azapi
-        import json
-        import pulumi_azure as azure
-
-        example_resource_group = azure.core.ResourceGroup("exampleResourceGroup", location="west europe")
-        example_public_ip = azure.network.PublicIp("examplePublicIp",
-            location=example_resource_group.location,
-            resource_group_name=example_resource_group.name,
-            allocation_method="Static")
-        example_load_balancer = azure.lb.LoadBalancer("exampleLoadBalancer",
-            location=example_resource_group.location,
-            resource_group_name=example_resource_group.name,
-            frontend_ip_configurations=[azure.lb.LoadBalancerFrontendIpConfigurationArgs(
-                name="PublicIPAddress",
-                public_ip_address_id=example_public_ip.id,
-            )])
-        example_nat_rule = azure.lb.NatRule("exampleNatRule",
-            resource_group_name=example_resource_group.name,
-            loadbalancer_id=example_load_balancer.id,
-            protocol="Tcp",
-            frontend_port=3389,
-            backend_port=3389,
-            frontend_ip_configuration_name="PublicIPAddress")
-        example_update_resource = azapi.UpdateResource("exampleUpdateResource",
-            type="Microsoft.Network/loadBalancers@2021-03-01",
-            resource_id=example_load_balancer.id,
-            body=json.dumps({
-                "properties": {
-                    "inboundNatRules": [{
-                        "properties": {
-                            "idleTimeoutInMinutes": 15,
-                        },
-                    }],
-                },
-            }),
-            opts=pulumi.ResourceOptions(depends_on=[example_nat_rule]))
-        ```
-
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
         :param pulumi.Input[str] body: A JSON object that contains the request body used to add on an existing azure resource.
         :param pulumi.Input[bool] ignore_casing: Whether ignore incorrect casing returned in `body` to suppress plan-diff. Defaults to `false`.
         :param pulumi.Input[bool] ignore_missing_property: Whether ignore not returned properties like credentials in `body` to suppress plan-diff. Defaults to `true`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] locks: A list of ARM resource IDs which are used to avoid create/modify/delete azapi resources at the same time.
         :param pulumi.Input[str] name: Specifies the name of the azure resource. Changing this forces a new resource to be created.
@@ -436,56 +394,14 @@
         """
         This resource can manage a subset of any existing Azure resource manager resource's properties.
 
         > **Note** This resource is used to add or modify properties on an existing resource.
         When delete `UpdateResource`, no operation will be performed, and these properties will stay unchanged.
         If you want to restore the modified properties to some values, you must apply the restored properties before deleting.
 
-        ## Example Usage
-
-        ```python
-        import pulumi
-        import ediri_azapi as azapi
-        import json
-        import pulumi_azure as azure
-
-        example_resource_group = azure.core.ResourceGroup("exampleResourceGroup", location="west europe")
-        example_public_ip = azure.network.PublicIp("examplePublicIp",
-            location=example_resource_group.location,
-            resource_group_name=example_resource_group.name,
-            allocation_method="Static")
-        example_load_balancer = azure.lb.LoadBalancer("exampleLoadBalancer",
-            location=example_resource_group.location,
-            resource_group_name=example_resource_group.name,
-            frontend_ip_configurations=[azure.lb.LoadBalancerFrontendIpConfigurationArgs(
-                name="PublicIPAddress",
-                public_ip_address_id=example_public_ip.id,
-            )])
-        example_nat_rule = azure.lb.NatRule("exampleNatRule",
-            resource_group_name=example_resource_group.name,
-            loadbalancer_id=example_load_balancer.id,
-            protocol="Tcp",
-            frontend_port=3389,
-            backend_port=3389,
-            frontend_ip_configuration_name="PublicIPAddress")
-        example_update_resource = azapi.UpdateResource("exampleUpdateResource",
-            type="Microsoft.Network/loadBalancers@2021-03-01",
-            resource_id=example_load_balancer.id,
-            body=json.dumps({
-                "properties": {
-                    "inboundNatRules": [{
-                        "properties": {
-                            "idleTimeoutInMinutes": 15,
-                        },
-                    }],
-                },
-            }),
-            opts=pulumi.ResourceOptions(depends_on=[example_nat_rule]))
-        ```
-
         :param str resource_name: The name of the resource.
         :param UpdateResourceArgs args: The arguments to use to populate this resource's properties.
         :param pulumi.ResourceOptions opts: Options for the resource.
         """
         ...
     def __init__(__self__, resource_name: str, *args, **kwargs):
         resource_args, opts = _utilities.get_resource_args_opts(UpdateResourceArgs, pulumi.ResourceOptions, *args, **kwargs)
```

### Comparing `ediri_azapi-1.4.0/ediri_azapi.egg-info/PKG-INFO` & `ediri_azapi-1.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: ediri-azapi
-Version: 1.4.0
+Name: ediri_azapi
+Version: 1.5.0
 Summary: A Pulumi package for creating and managing Azapi resources
 Home-page: https://github.com/dirien/pulumi-azapi
 License: Apache-2.0
 Project-URL: Repository, https://github.com/dirien/pulumi-azapi
 Keywords: pulumi azapi category/cloud
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `ediri_azapi-1.4.0/ediri_azapi.egg-info/SOURCES.txt` & `ediri_azapi-1.5.0/ediri_azapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ediri_azapi-1.4.0/setup.py` & `ediri_azapi-1.5.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.4.0"
-PLUGIN_VERSION = "1.4.0"
+VERSION = "1.5.0"
+PLUGIN_VERSION = "1.5.0"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'azapi', PLUGIN_VERSION, '--server', 'github://api.github.com/dirien/pulumi-azapi'])
         except OSError as error:
```

