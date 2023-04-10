# Comparing `tmp/aliyun-python-sdk-iotcc-2.0.4.tar.gz` & `tmp/aliyun-python-sdk-iotcc-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-iotcc-2.0.4.tar", last modified: Thu Aug 18 12:25:17 2022, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-iotcc-2.0.5.tar", last modified: Mon Apr 10 15:15:37 2023, max compression
```

## Comparing `aliyun-python-sdk-iotcc-2.0.4.tar` & `aliyun-python-sdk-iotcc-2.0.5.tar`

### file list

```diff
@@ -1,85 +1,95 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/
--rw-r--r--   0 root         (0) root         (0)      575 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)       40 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1547 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      531 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyun_python_sdk_iotcc.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1547 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyun_python_sdk_iotcc.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5025 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyun_python_sdk_iotcc.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyun_python_sdk_iotcc.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyun_python_sdk_iotcc.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       15 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyun_python_sdk_iotcc.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/
--rw-r--r--   0 root         (0) root         (0)       21 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/
--rw-r--r--   0 root         (0) root         (0)     2099 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/AddCidrToConnectionPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     2008 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/AddIoTCloudConnectorToGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2294 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/AssociateIpWithConnectionPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     2103 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/AssociateVSwitchWithIoTCloudConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     3455 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     3423 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2543 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateConnectionPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     2712 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateDNSServiceRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     3650 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateGroupAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     2752 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateGroupDNSServiceRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1663 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorBackhaulRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1909 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2853 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2666 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateServiceEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     2053 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1882 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1858 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteConnectionPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     1858 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteDNSServiceRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1922 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteGroupAuthorizationRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1898 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteGroupDNSServiceRuleRequest.py
--rw-r--r--   0 root         (0) root         (0)     1677 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     1637 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     1661 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnetorBackhaulRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     2027 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteServiceEntryRequest.py
--rw-r--r--   0 root         (0) root         (0)     1802 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1657 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DisableIoTCloudConnectorAccessLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2296 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DissociateIpFromConnectionPoolRequest.py
--rw-r--r--   0 root         (0) root         (0)     1667 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DissociateVSwitchFromIoTCloudConnectorRequest.py
--rw-r--r--   0 root         (0) root         (0)     2151 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/EnableIoTCloudConnectorAccessLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     1735 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/GetConnectionPoolIpOperationResultRequest.py
--rw-r--r--   0 root         (0) root         (0)     1255 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/GetDiagnoseResultForSingleCardRequest.py
--rw-r--r--   0 root         (0) root         (0)     1649 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/GetIoTCloudConnectorAccessLogRequest.py
--rw-r--r--   0 root         (0) root         (0)     2037 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/GetStsInfoAndOssPathRequest.py
--rw-r--r--   0 root         (0) root         (0)     1285 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/GrantVirtualBorderRouterRequest.py
--rw-r--r--   0 root         (0) root         (0)     1827 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListAPNsRequest.py
--rw-r--r--   0 root         (0) root         (0)     4337 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListAuthorizationRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2176 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListConnectionPoolAllIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2015 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListConnectionPoolIpsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2626 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListConnectionPoolsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3342 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListDNSServiceRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2019 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListDiagnoseInfoForSingleCardRequest.py
--rw-r--r--   0 root         (0) root         (0)     4275 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListGroupAuthorizationRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     3382 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListGroupDNSServiceRulesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2576 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorAccessSessionLogsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1295 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorAvailableZonesRequest.py
--rw-r--r--   0 root         (0) root         (0)     1653 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorEIPsRequest.py
--rw-r--r--   0 root         (0) root         (0)     2720 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorGroupsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3589 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorsRequest.py
--rw-r--r--   0 root         (0) root         (0)     1669 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListIoTCoudConnectorBackhaulRouteRequest.py
--rw-r--r--   0 root         (0) root         (0)     1217 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListRegionsRequest.py
--rw-r--r--   0 root         (0) root         (0)     3279 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListServiceEntriesRequest.py
--rw-r--r--   0 root         (0) root         (0)     2491 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1902 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/MoveAuthorizationRuleToDNSServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1942 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/MoveGroupAuthorizationRuleToDNSServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1036 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/OpenIoTCloudConnectorServiceRequest.py
--rw-r--r--   0 root         (0) root         (0)     1992 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/RemoveIoTCloudConnectorFromGroupRequest.py
--rw-r--r--   0 root         (0) root         (0)     2606 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/SubmitDiagnoseTaskForSingleCardRequest.py
--rw-r--r--   0 root         (0) root         (0)     3718 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateAuthorizationRuleAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2788 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateConnectionPoolAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2957 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateDNSServiceRuleAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     3758 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateGroupAuthorizationRuleAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2997 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateGroupDNSServiceRuleAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2625 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2047 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorGroupAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2256 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateServiceAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)     2541 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateServiceEntryAttributeRequest.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/__init__.py
--rw-r--r--   0 root         (0) root         (0)      102 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2462 2022-08-18 12:25:17.000000 aliyun-python-sdk-iotcc-2.0.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:15:37.000000 aliyun-python-sdk-iotcc-2.0.5/
+-rw-r--r--   0 root         (0) root         (0)      575 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       40 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-04-10 15:15:37.000000 aliyun-python-sdk-iotcc-2.0.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      531 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:15:37.000000 aliyun-python-sdk-iotcc-2.0.5/aliyun_python_sdk_iotcc.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-04-10 15:15:37.000000 aliyun-python-sdk-iotcc-2.0.5/aliyun_python_sdk_iotcc.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5668 2023-04-10 15:15:37.000000 aliyun-python-sdk-iotcc-2.0.5/aliyun_python_sdk_iotcc.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-10 15:15:37.000000 aliyun-python-sdk-iotcc-2.0.5/aliyun_python_sdk_iotcc.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-04-10 15:15:37.000000 aliyun-python-sdk-iotcc-2.0.5/aliyun_python_sdk_iotcc.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       15 2023-04-10 15:15:37.000000 aliyun-python-sdk-iotcc-2.0.5/aliyun_python_sdk_iotcc.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:15:37.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/
+-rw-r--r--   0 root         (0) root         (0)       21 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:15:37.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-10 15:15:37.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/
+-rw-r--r--   0 root         (0) root         (0)     2099 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/AddCidrToConnectionPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/AddIoTCloudConnectorToGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2294 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/AssociateIpWithConnectionPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/AssociateVSwitchWithIoTCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1848 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ConfirmIoTCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3455 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3423 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2543 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateConnectionPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2712 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateDNSServiceRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3650 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateGroupAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateGroupDNSServiceRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2571 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateGroupIpMappingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorBackhaulRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1909 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2853 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2531 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateIpMappingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2666 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateServiceEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1882 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1979 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteConnectionPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteDNSServiceRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1922 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteGroupAuthorizationRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteGroupDNSServiceRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1920 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteGroupIpMappingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1661 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnetorBackhaulRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1850 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteIpMappingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2027 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteServiceEntryRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1657 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DisableIoTCloudConnectorAccessLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DissociateIpFromConnectionPoolRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1667 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DissociateVSwitchFromIoTCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2151 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/EnableIoTCloudConnectorAccessLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1735 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/GetConnectionPoolIpOperationResultRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/GetDiagnoseResultForSingleCardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/GetIoTCloudConnectorAccessLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2037 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/GetStsInfoAndOssPathRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1285 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/GrantVirtualBorderRouterRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1827 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListAPNsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4851 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListAuthorizationRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2176 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListConnectionPoolAllIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2015 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListConnectionPoolIpsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2626 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListConnectionPoolsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3342 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListDNSServiceRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListDiagnoseInfoForSingleCardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     4275 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListGroupAuthorizationRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3382 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListGroupDNSServiceRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3232 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListGroupIpMappingRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorAvailableZonesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1653 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorEIPsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2720 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3589 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListIoTCoudConnectorBackhaulRouteRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3192 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListIpMappingRulesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1217 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3279 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListServiceEntriesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2491 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1902 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/MoveAuthorizationRuleToDNSServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1942 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/MoveGroupAuthorizationRuleToDNSServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/OpenIoTCloudConnectorServiceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/RemoveIoTCloudConnectorFromGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1637 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/RevertIoTCloudConnectorRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2606 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/SubmitDiagnoseTaskForSingleCardRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3718 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateAuthorizationRuleAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2788 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateConnectionPoolAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2957 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateDNSServiceRuleAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     3758 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateGroupAuthorizationRuleAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2997 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateGroupDNSServiceRuleAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2822 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateGroupIpMappingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2625 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2047 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorGroupAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2752 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateIpMappingRuleRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2256 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateServiceAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2541 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateServiceEntryAttributeRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      102 2023-04-10 15:15:37.000000 aliyun-python-sdk-iotcc-2.0.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-04-10 15:15:36.000000 aliyun-python-sdk-iotcc-2.0.5/setup.py
```

### Comparing `aliyun-python-sdk-iotcc-2.0.4/LICENSE` & `aliyun-python-sdk-iotcc-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/PKG-INFO` & `aliyun-python-sdk-iotcc-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-iotcc
-Version: 2.0.4
+Version: 2.0.5
 Summary: The iotcc module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-iotcc
```

### Comparing `aliyun-python-sdk-iotcc-2.0.4/README.rst` & `aliyun-python-sdk-iotcc-2.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyun_python_sdk_iotcc.egg-info/PKG-INFO` & `aliyun-python-sdk-iotcc-2.0.5/aliyun_python_sdk_iotcc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-iotcc
-Version: 2.0.4
+Version: 2.0.5
 Summary: The iotcc module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-iotcc
```

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyun_python_sdk_iotcc.egg-info/SOURCES.txt` & `aliyun-python-sdk-iotcc-2.0.5/aliyun_python_sdk_iotcc.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -10,33 +10,39 @@
 aliyun_python_sdk_iotcc.egg-info/top_level.txt
 aliyunsdkiotcc/__init__.py
 aliyunsdkiotcc/request/__init__.py
 aliyunsdkiotcc/request/v20210513/AddCidrToConnectionPoolRequest.py
 aliyunsdkiotcc/request/v20210513/AddIoTCloudConnectorToGroupRequest.py
 aliyunsdkiotcc/request/v20210513/AssociateIpWithConnectionPoolRequest.py
 aliyunsdkiotcc/request/v20210513/AssociateVSwitchWithIoTCloudConnectorRequest.py
+aliyunsdkiotcc/request/v20210513/ConfirmIoTCloudConnectorRequest.py
 aliyunsdkiotcc/request/v20210513/CreateAuthorizationRuleRequest.py
 aliyunsdkiotcc/request/v20210513/CreateAuthorizationRulesRequest.py
 aliyunsdkiotcc/request/v20210513/CreateConnectionPoolRequest.py
 aliyunsdkiotcc/request/v20210513/CreateDNSServiceRuleRequest.py
 aliyunsdkiotcc/request/v20210513/CreateGroupAuthorizationRuleRequest.py
 aliyunsdkiotcc/request/v20210513/CreateGroupDNSServiceRuleRequest.py
+aliyunsdkiotcc/request/v20210513/CreateGroupIpMappingRuleRequest.py
 aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorBackhaulRouteRequest.py
 aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorGroupRequest.py
 aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorRequest.py
+aliyunsdkiotcc/request/v20210513/CreateIpMappingRuleRequest.py
 aliyunsdkiotcc/request/v20210513/CreateServiceEntryRequest.py
 aliyunsdkiotcc/request/v20210513/CreateServiceRequest.py
 aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRuleRequest.py
+aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRulesRequest.py
 aliyunsdkiotcc/request/v20210513/DeleteConnectionPoolRequest.py
 aliyunsdkiotcc/request/v20210513/DeleteDNSServiceRuleRequest.py
 aliyunsdkiotcc/request/v20210513/DeleteGroupAuthorizationRuleRequest.py
 aliyunsdkiotcc/request/v20210513/DeleteGroupDNSServiceRuleRequest.py
+aliyunsdkiotcc/request/v20210513/DeleteGroupIpMappingRuleRequest.py
 aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorGroupRequest.py
 aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorRequest.py
 aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnetorBackhaulRouteRequest.py
+aliyunsdkiotcc/request/v20210513/DeleteIpMappingRuleRequest.py
 aliyunsdkiotcc/request/v20210513/DeleteServiceEntryRequest.py
 aliyunsdkiotcc/request/v20210513/DeleteServiceRequest.py
 aliyunsdkiotcc/request/v20210513/DisableIoTCloudConnectorAccessLogRequest.py
 aliyunsdkiotcc/request/v20210513/DissociateIpFromConnectionPoolRequest.py
 aliyunsdkiotcc/request/v20210513/DissociateVSwitchFromIoTCloudConnectorRequest.py
 aliyunsdkiotcc/request/v20210513/EnableIoTCloudConnectorAccessLogRequest.py
 aliyunsdkiotcc/request/v20210513/GetConnectionPoolIpOperationResultRequest.py
@@ -49,31 +55,35 @@
 aliyunsdkiotcc/request/v20210513/ListConnectionPoolAllIpsRequest.py
 aliyunsdkiotcc/request/v20210513/ListConnectionPoolIpsRequest.py
 aliyunsdkiotcc/request/v20210513/ListConnectionPoolsRequest.py
 aliyunsdkiotcc/request/v20210513/ListDNSServiceRulesRequest.py
 aliyunsdkiotcc/request/v20210513/ListDiagnoseInfoForSingleCardRequest.py
 aliyunsdkiotcc/request/v20210513/ListGroupAuthorizationRulesRequest.py
 aliyunsdkiotcc/request/v20210513/ListGroupDNSServiceRulesRequest.py
-aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorAccessSessionLogsRequest.py
+aliyunsdkiotcc/request/v20210513/ListGroupIpMappingRulesRequest.py
 aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorAvailableZonesRequest.py
 aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorEIPsRequest.py
 aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorGroupsRequest.py
 aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorsRequest.py
 aliyunsdkiotcc/request/v20210513/ListIoTCoudConnectorBackhaulRouteRequest.py
+aliyunsdkiotcc/request/v20210513/ListIpMappingRulesRequest.py
 aliyunsdkiotcc/request/v20210513/ListRegionsRequest.py
 aliyunsdkiotcc/request/v20210513/ListServiceEntriesRequest.py
 aliyunsdkiotcc/request/v20210513/ListServiceRequest.py
 aliyunsdkiotcc/request/v20210513/MoveAuthorizationRuleToDNSServiceRequest.py
 aliyunsdkiotcc/request/v20210513/MoveGroupAuthorizationRuleToDNSServiceRequest.py
 aliyunsdkiotcc/request/v20210513/OpenIoTCloudConnectorServiceRequest.py
 aliyunsdkiotcc/request/v20210513/RemoveIoTCloudConnectorFromGroupRequest.py
+aliyunsdkiotcc/request/v20210513/RevertIoTCloudConnectorRequest.py
 aliyunsdkiotcc/request/v20210513/SubmitDiagnoseTaskForSingleCardRequest.py
 aliyunsdkiotcc/request/v20210513/UpdateAuthorizationRuleAttributeRequest.py
 aliyunsdkiotcc/request/v20210513/UpdateConnectionPoolAttributeRequest.py
 aliyunsdkiotcc/request/v20210513/UpdateDNSServiceRuleAttributeRequest.py
 aliyunsdkiotcc/request/v20210513/UpdateGroupAuthorizationRuleAttributeRequest.py
 aliyunsdkiotcc/request/v20210513/UpdateGroupDNSServiceRuleAttributeRequest.py
+aliyunsdkiotcc/request/v20210513/UpdateGroupIpMappingRuleRequest.py
 aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorAttributeRequest.py
 aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorGroupAttributeRequest.py
+aliyunsdkiotcc/request/v20210513/UpdateIpMappingRuleRequest.py
 aliyunsdkiotcc/request/v20210513/UpdateServiceAttributeRequest.py
 aliyunsdkiotcc/request/v20210513/UpdateServiceEntryAttributeRequest.py
 aliyunsdkiotcc/request/v20210513/__init__.py
```

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/AddCidrToConnectionPoolRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/AddCidrToConnectionPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/AddIoTCloudConnectorToGroupRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/AddIoTCloudConnectorToGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/AssociateIpWithConnectionPoolRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/AssociateIpWithConnectionPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/AssociateVSwitchWithIoTCloudConnectorRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/AssociateVSwitchWithIoTCloudConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRulesRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateAuthorizationRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateConnectionPoolRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateConnectionPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateDNSServiceRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateDNSServiceRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateGroupAuthorizationRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateGroupAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateGroupDNSServiceRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateGroupDNSServiceRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorBackhaulRouteRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorBackhaulRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorGroupRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateIoTCloudConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateServiceEntryRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateServiceEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/CreateServiceRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteConnectionPoolRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteConnectionPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteDNSServiceRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteDNSServiceRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteGroupAuthorizationRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteGroupAuthorizationRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteGroupDNSServiceRuleRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteGroupDNSServiceRuleRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorGroupRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnetorBackhaulRouteRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteIoTCloudConnetorBackhaulRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteServiceEntryRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteServiceEntryRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DeleteServiceRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DeleteServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DisableIoTCloudConnectorAccessLogRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DisableIoTCloudConnectorAccessLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DissociateIpFromConnectionPoolRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DissociateIpFromConnectionPoolRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/DissociateVSwitchFromIoTCloudConnectorRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/DissociateVSwitchFromIoTCloudConnectorRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/EnableIoTCloudConnectorAccessLogRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/EnableIoTCloudConnectorAccessLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/GetConnectionPoolIpOperationResultRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/GetConnectionPoolIpOperationResultRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/GetDiagnoseResultForSingleCardRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/GetDiagnoseResultForSingleCardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/GetIoTCloudConnectorAccessLogRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/GetIoTCloudConnectorAccessLogRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/GetStsInfoAndOssPathRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/GetStsInfoAndOssPathRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/GrantVirtualBorderRouterRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/GrantVirtualBorderRouterRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListAPNsRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListAPNsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListAuthorizationRulesRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListAuthorizationRulesRequest.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,24 @@
 
 class ListAuthorizationRulesRequest(RpcRequest):
 
 	def __init__(self):
 		RpcRequest.__init__(self, 'IoTCC', '2021-05-13', 'ListAuthorizationRules','IoTCC')
 		self.set_method('POST')
 
+	def get_FuzzyDestination(self): # String
+		return self.get_query_params().get('FuzzyDestination')
+
+	def set_FuzzyDestination(self, FuzzyDestination):  # String
+		self.add_query_param('FuzzyDestination', FuzzyDestination)
+	def get_FuzzyAuthorizationRuleName(self): # String
+		return self.get_query_params().get('FuzzyAuthorizationRuleName')
+
+	def set_FuzzyAuthorizationRuleName(self, FuzzyAuthorizationRuleName):  # String
+		self.add_query_param('FuzzyAuthorizationRuleName', FuzzyAuthorizationRuleName)
 	def get_DestinationTypes(self): # RepeatList
 		return self.get_query_params().get('DestinationType')
 
 	def set_DestinationTypes(self, DestinationType):  # RepeatList
 		for depth1 in range(len(DestinationType)):
 			self.add_query_param('DestinationType.' + str(depth1 + 1), DestinationType[depth1])
 	def get_Destinations(self): # RepeatList
```

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListConnectionPoolAllIpsRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListConnectionPoolAllIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListConnectionPoolIpsRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListConnectionPoolIpsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListConnectionPoolsRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListConnectionPoolsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListDNSServiceRulesRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListDNSServiceRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListDiagnoseInfoForSingleCardRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListDiagnoseInfoForSingleCardRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListGroupAuthorizationRulesRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListGroupAuthorizationRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListGroupDNSServiceRulesRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListGroupDNSServiceRulesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorAccessSessionLogsRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/SubmitDiagnoseTaskForSingleCardRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,50 +15,53 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class ListIoTCloudConnectorAccessSessionLogsRequest(RpcRequest):
+class SubmitDiagnoseTaskForSingleCardRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'IoTCC', '2021-05-13', 'ListIoTCloudConnectorAccessSessionLogs','IoTCC')
+		RpcRequest.__init__(self, 'IoTCC', '2021-05-13', 'SubmitDiagnoseTaskForSingleCard','IoTCC')
 		self.set_method('POST')
 
-	def get_StartTime(self): # Long
-		return self.get_query_params().get('StartTime')
+	def get_DestinationType(self): # String
+		return self.get_query_params().get('DestinationType')
 
-	def set_StartTime(self, StartTime):  # Long
-		self.add_query_param('StartTime', StartTime)
-	def get_NextToken(self): # String
-		return self.get_query_params().get('NextToken')
-
-	def set_NextToken(self, NextToken):  # String
-		self.add_query_param('NextToken', NextToken)
-	def get_Destinationss(self): # RepeatList
-		return self.get_query_params().get('Destinations')
-
-	def set_Destinationss(self, Destinations):  # RepeatList
-		for depth1 in range(len(Destinations)):
-			self.add_query_param('Destinations.' + str(depth1 + 1), Destinations[depth1])
+	def set_DestinationType(self, DestinationType):  # String
+		self.add_query_param('DestinationType', DestinationType)
+	def get_Destination(self): # String
+		return self.get_query_params().get('Destination')
+
+	def set_Destination(self, Destination):  # String
+		self.add_query_param('Destination', Destination)
+	def get_Source(self): # String
+		return self.get_query_params().get('Source')
+
+	def set_Source(self, Source):  # String
+		self.add_query_param('Source', Source)
+	def get_ResourceUid(self): # Long
+		return self.get_query_params().get('ResourceUid')
+
+	def set_ResourceUid(self, ResourceUid):  # Long
+		self.add_query_param('ResourceUid', ResourceUid)
+	def get_SourceType(self): # String
+		return self.get_query_params().get('SourceType')
+
+	def set_SourceType(self, SourceType):  # String
+		self.add_query_param('SourceType', SourceType)
 	def get_EndTime(self): # Long
 		return self.get_query_params().get('EndTime')
 
 	def set_EndTime(self, EndTime):  # Long
 		self.add_query_param('EndTime', EndTime)
+	def get_BeginTime(self): # Long
+		return self.get_query_params().get('BeginTime')
+
+	def set_BeginTime(self, BeginTime):  # Long
+		self.add_query_param('BeginTime', BeginTime)
 	def get_IoTCloudConnectorId(self): # String
 		return self.get_query_params().get('IoTCloudConnectorId')
 
 	def set_IoTCloudConnectorId(self, IoTCloudConnectorId):  # String
 		self.add_query_param('IoTCloudConnectorId', IoTCloudConnectorId)
-	def get_SourceIpss(self): # RepeatList
-		return self.get_query_params().get('SourceIps')
-
-	def set_SourceIpss(self, SourceIps):  # RepeatList
-		for depth1 in range(len(SourceIps)):
-			self.add_query_param('SourceIps.' + str(depth1 + 1), SourceIps[depth1])
-	def get_MaxResults(self): # Integer
-		return self.get_query_params().get('MaxResults')
-
-	def set_MaxResults(self, MaxResults):  # Integer
-		self.add_query_param('MaxResults', MaxResults)
```

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorAvailableZonesRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorAvailableZonesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorEIPsRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorEIPsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorGroupsRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorGroupsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorsRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListIoTCloudConnectorsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListIoTCoudConnectorBackhaulRouteRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListIoTCoudConnectorBackhaulRouteRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListRegionsRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListRegionsRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListServiceEntriesRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListServiceEntriesRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/ListServiceRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/ListServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/MoveAuthorizationRuleToDNSServiceRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/MoveAuthorizationRuleToDNSServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/MoveGroupAuthorizationRuleToDNSServiceRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/MoveGroupAuthorizationRuleToDNSServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/OpenIoTCloudConnectorServiceRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/OpenIoTCloudConnectorServiceRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/RemoveIoTCloudConnectorFromGroupRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/RemoveIoTCloudConnectorFromGroupRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/SubmitDiagnoseTaskForSingleCardRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/CreateIpMappingRuleRequest.py`

 * *Files 18% similar despite different names*

```diff
@@ -15,53 +15,48 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RpcRequest
 
-class SubmitDiagnoseTaskForSingleCardRequest(RpcRequest):
+class CreateIpMappingRuleRequest(RpcRequest):
 
 	def __init__(self):
-		RpcRequest.__init__(self, 'IoTCC', '2021-05-13', 'SubmitDiagnoseTaskForSingleCard','IoTCC')
+		RpcRequest.__init__(self, 'IoTCC', '2021-05-13', 'CreateIpMappingRule','IoTCC')
 		self.set_method('POST')
 
-	def get_DestinationType(self): # String
-		return self.get_query_params().get('DestinationType')
+	def get_ClientToken(self): # String
+		return self.get_query_params().get('ClientToken')
 
-	def set_DestinationType(self, DestinationType):  # String
-		self.add_query_param('DestinationType', DestinationType)
-	def get_Destination(self): # String
-		return self.get_query_params().get('Destination')
-
-	def set_Destination(self, Destination):  # String
-		self.add_query_param('Destination', Destination)
-	def get_Source(self): # String
-		return self.get_query_params().get('Source')
-
-	def set_Source(self, Source):  # String
-		self.add_query_param('Source', Source)
-	def get_ResourceUid(self): # Long
-		return self.get_query_params().get('ResourceUid')
-
-	def set_ResourceUid(self, ResourceUid):  # Long
-		self.add_query_param('ResourceUid', ResourceUid)
-	def get_SourceType(self): # String
-		return self.get_query_params().get('SourceType')
-
-	def set_SourceType(self, SourceType):  # String
-		self.add_query_param('SourceType', SourceType)
-	def get_EndTime(self): # Long
-		return self.get_query_params().get('EndTime')
-
-	def set_EndTime(self, EndTime):  # Long
-		self.add_query_param('EndTime', EndTime)
-	def get_BeginTime(self): # Long
-		return self.get_query_params().get('BeginTime')
+	def set_ClientToken(self, ClientToken):  # String
+		self.add_query_param('ClientToken', ClientToken)
+	def get_IpMappingRuleName(self): # String
+		return self.get_query_params().get('IpMappingRuleName')
+
+	def set_IpMappingRuleName(self, IpMappingRuleName):  # String
+		self.add_query_param('IpMappingRuleName', IpMappingRuleName)
+	def get_DryRun(self): # Boolean
+		return self.get_query_params().get('DryRun')
+
+	def set_DryRun(self, DryRun):  # Boolean
+		self.add_query_param('DryRun', DryRun)
+	def get_IpMappingRuleDescription(self): # String
+		return self.get_query_params().get('IpMappingRuleDescription')
+
+	def set_IpMappingRuleDescription(self, IpMappingRuleDescription):  # String
+		self.add_query_param('IpMappingRuleDescription', IpMappingRuleDescription)
+	def get_DestinationIp(self): # String
+		return self.get_query_params().get('DestinationIp')
 
-	def set_BeginTime(self, BeginTime):  # Long
-		self.add_query_param('BeginTime', BeginTime)
+	def set_DestinationIp(self, DestinationIp):  # String
+		self.add_query_param('DestinationIp', DestinationIp)
 	def get_IoTCloudConnectorId(self): # String
 		return self.get_query_params().get('IoTCloudConnectorId')
 
 	def set_IoTCloudConnectorId(self, IoTCloudConnectorId):  # String
 		self.add_query_param('IoTCloudConnectorId', IoTCloudConnectorId)
+	def get_MappingIp(self): # String
+		return self.get_query_params().get('MappingIp')
+
+	def set_MappingIp(self, MappingIp):  # String
+		self.add_query_param('MappingIp', MappingIp)
```

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateAuthorizationRuleAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateAuthorizationRuleAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateConnectionPoolAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateConnectionPoolAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateDNSServiceRuleAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateDNSServiceRuleAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateGroupAuthorizationRuleAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateGroupAuthorizationRuleAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateGroupDNSServiceRuleAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateGroupDNSServiceRuleAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorGroupAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateIoTCloudConnectorGroupAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateServiceAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateServiceAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/aliyunsdkiotcc/request/v20210513/UpdateServiceEntryAttributeRequest.py` & `aliyun-python-sdk-iotcc-2.0.5/aliyunsdkiotcc/request/v20210513/UpdateServiceEntryAttributeRequest.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-iotcc-2.0.4/setup.py` & `aliyun-python-sdk-iotcc-2.0.5/setup.py`

 * *Files identical despite different names*

