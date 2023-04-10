# Comparing `tmp/aliyun-python-sdk-sae-1.4.0.0.tar.gz` & `tmp/aliyun-python-sdk-sae-1.5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aliyun-python-sdk-sae-1.4.0.0.tar", last modified: Wed May  6 06:17:29 2020, max compression
+gzip compressed data, was "dist/aliyun-python-sdk-sae-1.5.0.0.tar", last modified: Mon Sep 14 02:59:17 2020, max compression
```

## Comparing `aliyun-python-sdk-sae-1.4.0.0.tar` & `aliyun-python-sdk-sae-1.5.0.0.tar`

### file list

```diff
@@ -1,73 +1,78 @@
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-05-06 06:17:29.000000 aliyun-python-sdk-sae-1.4.0.0/
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/MANIFEST.in
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-05-06 06:17:29.000000 aliyun-python-sdk-sae-1.4.0.0/aliyun_python_sdk_sae.egg-info/
--rw-rw-r--   0 admin     (1017) admin     (1017)        1 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyun_python_sdk_sae.egg-info/dependency_links.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)       13 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyun_python_sdk_sae.egg-info/top_level.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)       31 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyun_python_sdk_sae.egg-info/requires.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)     3649 2020-05-06 06:17:29.000000 aliyun-python-sdk-sae-1.4.0.0/aliyun_python_sdk_sae.egg-info/SOURCES.txt
--rw-rw-r--   0 admin     (1017) admin     (1017)     1539 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyun_python_sdk_sae.egg-info/PKG-INFO
--rw-rw-r--   0 admin     (1017) admin     (1017)       38 2020-05-06 06:17:29.000000 aliyun-python-sdk-sae-1.4.0.0/setup.cfg
--rw-rw-r--   0 admin     (1017) admin     (1017)      527 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/README.rst
--rw-rw-r--   0 admin     (1017) admin     (1017)     1539 2020-05-06 06:17:29.000000 aliyun-python-sdk-sae-1.4.0.0/PKG-INFO
--rw-rw-r--   0 admin     (1017) admin     (1017)     2452 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/setup.py
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-05-06 06:17:29.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/
--rw-rw-r--   0 admin     (1017) admin     (1017)       23 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/__init__.py
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-05-06 06:17:29.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/__init__.py
-drwxrwxr-x   0 admin     (1017) admin     (1017)        0 2020-05-06 06:17:29.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/
--rw-rw-r--   0 admin     (1017) admin     (1017)     1360 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeInstanceSpecificationsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1465 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/StartApplicationRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1492 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DeleteNamespaceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1554 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/AbortAndRollbackChangeOrderRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2308 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/UpdateIngressRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1912 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/CreateNamespaceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1509 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeInstanceLogRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1493 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeNamespaceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     6711 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/CreateApplicationRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2312 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListNamespaceChangeOrdersRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1481 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListConsumedServicesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1530 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeChangeOrderRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1754 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeNamespaceListRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1780 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/RescaleApplicationVerticallyRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1537 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeNamespaceResourcesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1462 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/StopApplicationRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2129 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListApplicationsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)        0 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/__init__.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1685 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/RestartApplicationRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1797 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListLogConfigsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1636 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListIngressesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1830 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeApplicationGroupsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1338 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeEdasContainersRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1521 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/AbortChangeOrderRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2463 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/CreateIngressRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2240 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/RollbackApplicationRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1669 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ConfirmPipelineBatchRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1484 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListPublishedServicesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1960 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListTagResourcesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1482 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeIngressRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1466 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeApplicationSlbsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1993 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeApplicationInstancesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2618 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListAppEventsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1761 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/UnbindSlbRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1480 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/QueryResourceStaticsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1656 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/UpdateNamespaceVpcRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1492 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeApplicationStatusRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1653 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/UpdateApplicationVswitchesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1664 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/BatchStopApplicationsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1481 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DeleteIngressRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1471 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DeleteApplicationRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1604 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeComponentsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1462 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListAppVersionsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1977 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/UntagResourcesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1655 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeApplicationImageRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1787 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/TagResourcesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1656 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeNamespacesRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1911 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/UpdateNamespaceRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2249 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListChangeOrdersRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     6049 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DeployApplicationRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1667 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/BatchStartApplicationsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1314 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeRegionsRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     2135 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/BindSlbRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1658 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeApplicationConfigRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1845 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/RescaleApplicationRequest.py
--rw-rw-r--   0 admin     (1017) admin     (1017)     1088 2020-05-06 06:17:28.000000 aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1539 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      527 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyun_python_sdk_sae.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1539 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyun_python_sdk_sae.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3941 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyun_python_sdk_sae.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyun_python_sdk_sae.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyun_python_sdk_sae.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       13 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyun_python_sdk_sae.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/
+-rw-r--r--   0 root         (0) root         (0)       23 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1088 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/endpoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/
+-rw-r--r--   0 root         (0) root         (0)     1567 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/AbortAndRollbackChangeOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1534 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/AbortChangeOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/BatchStartApplicationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1677 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/BatchStopApplicationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2148 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/BindSlbRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1682 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ConfirmPipelineBatchRequest.py
+-rw-r--r--   0 root         (0) root         (0)     8222 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/CreateApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1962 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/CreateConfigMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2476 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/CreateIngressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1925 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/CreateNamespaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1484 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DeleteApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1514 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DeleteConfigMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DeleteIngressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DeleteNamespaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     7358 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DeployApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeApplicationConfigRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1843 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeApplicationGroupsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeApplicationImageRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2006 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeApplicationInstancesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeApplicationSlbsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1505 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeApplicationStatusRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1543 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeChangeOrderRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeComponentsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1515 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeConfigMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1351 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeEdasContainersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1495 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeIngressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1522 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeInstanceLogRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1373 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeInstanceSpecificationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeNamespaceListRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1506 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeNamespaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1550 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeNamespaceResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeNamespacesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1327 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeRegionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2631 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListAppEventsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListAppVersionsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2142 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListApplicationsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2262 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListChangeOrdersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1494 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListConsumedServicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1649 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListIngressesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1810 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListLogConfigsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2325 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListNamespaceChangeOrdersRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1544 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListNamespacedConfigMapsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListPublishedServicesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1973 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListTagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1493 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/QueryResourceStaticsRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1858 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/RescaleApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/RescaleApplicationVerticallyRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/RestartApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2253 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/RollbackApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1478 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/StartApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1475 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/StopApplicationRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1800 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/TagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1774 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/UnbindSlbRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1990 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/UntagResourcesRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1698 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/UpdateAppSecurityGroupRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1825 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/UpdateConfigMapRequest.py
+-rw-r--r--   0 root         (0) root         (0)     2321 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/UpdateIngressRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1924 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/UpdateNamespaceRequest.py
+-rw-r--r--   0 root         (0) root         (0)     1669 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/UpdateNamespaceVpcRequest.py
+-rw-r--r--   0 root         (0) root         (0)        0 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       38 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2452 2020-09-14 02:59:17.000000 aliyun-python-sdk-sae-1.5.0.0/setup.py
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyun_python_sdk_sae.egg-info/SOURCES.txt` & `aliyun-python-sdk-sae-1.5.0.0/aliyun_python_sdk_sae.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,31 @@
 aliyunsdksae/request/v20190506/AbortAndRollbackChangeOrderRequest.py
 aliyunsdksae/request/v20190506/AbortChangeOrderRequest.py
 aliyunsdksae/request/v20190506/BatchStartApplicationsRequest.py
 aliyunsdksae/request/v20190506/BatchStopApplicationsRequest.py
 aliyunsdksae/request/v20190506/BindSlbRequest.py
 aliyunsdksae/request/v20190506/ConfirmPipelineBatchRequest.py
 aliyunsdksae/request/v20190506/CreateApplicationRequest.py
+aliyunsdksae/request/v20190506/CreateConfigMapRequest.py
 aliyunsdksae/request/v20190506/CreateIngressRequest.py
 aliyunsdksae/request/v20190506/CreateNamespaceRequest.py
 aliyunsdksae/request/v20190506/DeleteApplicationRequest.py
+aliyunsdksae/request/v20190506/DeleteConfigMapRequest.py
 aliyunsdksae/request/v20190506/DeleteIngressRequest.py
 aliyunsdksae/request/v20190506/DeleteNamespaceRequest.py
 aliyunsdksae/request/v20190506/DeployApplicationRequest.py
 aliyunsdksae/request/v20190506/DescribeApplicationConfigRequest.py
 aliyunsdksae/request/v20190506/DescribeApplicationGroupsRequest.py
 aliyunsdksae/request/v20190506/DescribeApplicationImageRequest.py
 aliyunsdksae/request/v20190506/DescribeApplicationInstancesRequest.py
 aliyunsdksae/request/v20190506/DescribeApplicationSlbsRequest.py
 aliyunsdksae/request/v20190506/DescribeApplicationStatusRequest.py
 aliyunsdksae/request/v20190506/DescribeChangeOrderRequest.py
 aliyunsdksae/request/v20190506/DescribeComponentsRequest.py
+aliyunsdksae/request/v20190506/DescribeConfigMapRequest.py
 aliyunsdksae/request/v20190506/DescribeEdasContainersRequest.py
 aliyunsdksae/request/v20190506/DescribeIngressRequest.py
 aliyunsdksae/request/v20190506/DescribeInstanceLogRequest.py
 aliyunsdksae/request/v20190506/DescribeInstanceSpecificationsRequest.py
 aliyunsdksae/request/v20190506/DescribeNamespaceListRequest.py
 aliyunsdksae/request/v20190506/DescribeNamespaceRequest.py
 aliyunsdksae/request/v20190506/DescribeNamespaceResourcesRequest.py
@@ -43,24 +46,26 @@
 aliyunsdksae/request/v20190506/ListAppVersionsRequest.py
 aliyunsdksae/request/v20190506/ListApplicationsRequest.py
 aliyunsdksae/request/v20190506/ListChangeOrdersRequest.py
 aliyunsdksae/request/v20190506/ListConsumedServicesRequest.py
 aliyunsdksae/request/v20190506/ListIngressesRequest.py
 aliyunsdksae/request/v20190506/ListLogConfigsRequest.py
 aliyunsdksae/request/v20190506/ListNamespaceChangeOrdersRequest.py
+aliyunsdksae/request/v20190506/ListNamespacedConfigMapsRequest.py
 aliyunsdksae/request/v20190506/ListPublishedServicesRequest.py
 aliyunsdksae/request/v20190506/ListTagResourcesRequest.py
 aliyunsdksae/request/v20190506/QueryResourceStaticsRequest.py
 aliyunsdksae/request/v20190506/RescaleApplicationRequest.py
 aliyunsdksae/request/v20190506/RescaleApplicationVerticallyRequest.py
 aliyunsdksae/request/v20190506/RestartApplicationRequest.py
 aliyunsdksae/request/v20190506/RollbackApplicationRequest.py
 aliyunsdksae/request/v20190506/StartApplicationRequest.py
 aliyunsdksae/request/v20190506/StopApplicationRequest.py
 aliyunsdksae/request/v20190506/TagResourcesRequest.py
 aliyunsdksae/request/v20190506/UnbindSlbRequest.py
 aliyunsdksae/request/v20190506/UntagResourcesRequest.py
-aliyunsdksae/request/v20190506/UpdateApplicationVswitchesRequest.py
+aliyunsdksae/request/v20190506/UpdateAppSecurityGroupRequest.py
+aliyunsdksae/request/v20190506/UpdateConfigMapRequest.py
 aliyunsdksae/request/v20190506/UpdateIngressRequest.py
 aliyunsdksae/request/v20190506/UpdateNamespaceRequest.py
 aliyunsdksae/request/v20190506/UpdateNamespaceVpcRequest.py
 aliyunsdksae/request/v20190506/__init__.py
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyun_python_sdk_sae.egg-info/PKG-INFO` & `aliyun-python-sdk-sae-1.5.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-sae
-Version: 1.4.0.0
+Version: 1.5.0.0
 Summary: The sae module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-sae
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/README.rst` & `aliyun-python-sdk-sae-1.5.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-sae-1.4.0.0/PKG-INFO` & `aliyun-python-sdk-sae-1.5.0.0/aliyun_python_sdk_sae.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: aliyun-python-sdk-sae
-Version: 1.4.0.0
+Version: 1.5.0.0
 Summary: The sae module of Aliyun Python sdk.
 Home-page: http://develop.aliyun.com/sdk/python
 Author: Aliyun
 Author-email: aliyun-developers-efficiency@list.alibaba-inc.com
 License: Apache
 Description: =============================================================
         aliyun-python-sdk-sae
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/setup.py` & `aliyun-python-sdk-sae-1.5.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeInstanceSpecificationsRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeInstanceSpecificationsRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DescribeInstanceSpecificationsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeInstanceSpecifications')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeInstanceSpecifications','serverless')
 		self.set_uri_pattern('/pop/v1/paas/quota/instanceSpecifications')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/StartApplicationRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/StartApplicationRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class StartApplicationRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'StartApplication')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'StartApplication','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/startApplication')
 		self.set_method('PUT')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DeleteNamespaceRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeNamespaceRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
-class DeleteNamespaceRequest(RoaRequest):
+class DescribeNamespaceRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DeleteNamespace')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeNamespace','serverless')
 		self.set_uri_pattern('/pop/v1/paas/namespace')
-		self.set_method('DELETE')
+		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_NamespaceId(self):
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/AbortAndRollbackChangeOrderRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/AbortAndRollbackChangeOrderRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class AbortAndRollbackChangeOrderRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'AbortAndRollbackChangeOrder')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'AbortAndRollbackChangeOrder','serverless')
 		self.set_uri_pattern('/pop/v1/sam/changeorder/AbortAndRollbackChangeOrder')
 		self.set_method('PUT')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/UpdateIngressRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/UpdateIngressRequest.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class UpdateIngressRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'UpdateIngress')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'UpdateIngress','serverless')
 		self.set_uri_pattern('/pop/v1/sam/ingress/Ingress')
 		self.set_method('PUT')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -47,18 +47,18 @@
 	def get_Description(self):
 		return self.get_query_params().get('Description')
 
 	def set_Description(self,Description):
 		self.add_query_param('Description',Description)
 
 	def get_Rules(self):
-		return self.get_query_params().get('Rules')
+		return self.get_body_params().get('Rules')
 
 	def set_Rules(self,Rules):
-		self.add_query_param('Rules',Rules)
+		self.add_body_params('Rules', Rules)
 
 	def get_CertId(self):
 		return self.get_query_params().get('CertId')
 
 	def set_CertId(self,CertId):
 		self.add_query_param('CertId',CertId)
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/CreateNamespaceRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/CreateNamespaceRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class CreateNamespaceRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'CreateNamespace')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'CreateNamespace','serverless')
 		self.set_uri_pattern('/pop/v1/paas/namespace')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeInstanceLogRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeInstanceLogRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DescribeInstanceLogRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeInstanceLog')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeInstanceLog','serverless')
 		self.set_uri_pattern('/pop/v1/sam/instance/describeInstanceLog')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeNamespaceRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DeleteNamespaceRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
-class DescribeNamespaceRequest(RoaRequest):
+class DeleteNamespaceRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeNamespace')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DeleteNamespace','serverless')
 		self.set_uri_pattern('/pop/v1/paas/namespace')
-		self.set_method('GET')
+		self.set_method('DELETE')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_NamespaceId(self):
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/CreateApplicationRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/CreateApplicationRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class CreateApplicationRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'CreateApplication')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'CreateApplication','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/createApplication')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -82,26 +82,44 @@
 
 	def get_MountHost(self):
 		return self.get_query_params().get('MountHost')
 
 	def set_MountHost(self,MountHost):
 		self.add_query_param('MountHost',MountHost)
 
+	def get_AutoConfig(self):
+		return self.get_query_params().get('AutoConfig')
+
+	def set_AutoConfig(self,AutoConfig):
+		self.add_query_param('AutoConfig',AutoConfig)
+
 	def get_Liveness(self):
 		return self.get_query_params().get('Liveness')
 
 	def set_Liveness(self,Liveness):
 		self.add_query_param('Liveness',Liveness)
 
+	def get_SecurityGroupId(self):
+		return self.get_query_params().get('SecurityGroupId')
+
+	def set_SecurityGroupId(self,SecurityGroupId):
+		self.add_query_param('SecurityGroupId',SecurityGroupId)
+
 	def get_Envs(self):
 		return self.get_query_params().get('Envs')
 
 	def set_Envs(self,Envs):
 		self.add_query_param('Envs',Envs)
 
+	def get_PhpArmsConfigLocation(self):
+		return self.get_query_params().get('PhpArmsConfigLocation')
+
+	def set_PhpArmsConfigLocation(self,PhpArmsConfigLocation):
+		self.add_query_param('PhpArmsConfigLocation',PhpArmsConfigLocation)
+
 	def get_PackageVersion(self):
 		return self.get_query_params().get('PackageVersion')
 
 	def set_PackageVersion(self,PackageVersion):
 		self.add_query_param('PackageVersion',PackageVersion)
 
 	def get_CustomHostAlias(self):
@@ -148,14 +166,32 @@
 
 	def get_PackageUrl(self):
 		return self.get_query_params().get('PackageUrl')
 
 	def set_PackageUrl(self,PackageUrl):
 		self.add_query_param('PackageUrl',PackageUrl)
 
+	def get_TerminationGracePeriodSeconds(self):
+		return self.get_query_params().get('TerminationGracePeriodSeconds')
+
+	def set_TerminationGracePeriodSeconds(self,TerminationGracePeriodSeconds):
+		self.add_query_param('TerminationGracePeriodSeconds',TerminationGracePeriodSeconds)
+
+	def get_ConfigMapMountDesc(self):
+		return self.get_body_params().get('ConfigMapMountDesc')
+
+	def set_ConfigMapMountDesc(self,ConfigMapMountDesc):
+		self.add_body_params('ConfigMapMountDesc', ConfigMapMountDesc)
+
+	def get_PhpConfig(self):
+		return self.get_body_params().get('PhpConfig')
+
+	def set_PhpConfig(self,PhpConfig):
+		self.add_body_params('PhpConfig', PhpConfig)
+
 	def get_PreStop(self):
 		return self.get_query_params().get('PreStop')
 
 	def set_PreStop(self,PreStop):
 		self.add_query_param('PreStop',PreStop)
 
 	def get_Replicas(self):
@@ -214,12 +250,18 @@
 
 	def get_PackageType(self):
 		return self.get_query_params().get('PackageType')
 
 	def set_PackageType(self,PackageType):
 		self.add_query_param('PackageType',PackageType)
 
+	def get_PhpConfigLocation(self):
+		return self.get_query_params().get('PhpConfigLocation')
+
+	def set_PhpConfigLocation(self,PhpConfigLocation):
+		self.add_query_param('PhpConfigLocation',PhpConfigLocation)
+
 	def get_PostStart(self):
 		return self.get_query_params().get('PostStart')
 
 	def set_PostStart(self,PostStart):
 		self.add_query_param('PostStart',PostStart)
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListNamespaceChangeOrdersRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListNamespaceChangeOrdersRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class ListNamespaceChangeOrdersRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListNamespaceChangeOrders')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListNamespaceChangeOrders','serverless')
 		self.set_uri_pattern('/pop/v1/sam/changeorder/listNamespaceChangeOrders')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListConsumedServicesRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListConsumedServicesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class ListConsumedServicesRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListConsumedServices')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListConsumedServices','serverless')
 		self.set_uri_pattern('/pop/v1/sam/service/listConsumedServices')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeChangeOrderRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeConfigMapRequest.py`

 * *Files 14% similar despite different names*

```diff
@@ -16,24 +16,24 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
-class DescribeChangeOrderRequest(RoaRequest):
+class DescribeConfigMapRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeChangeOrder')
-		self.set_uri_pattern('/pop/v1/sam/changeorder/DescribeChangeOrder')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeConfigMap','serverless')
+		self.set_uri_pattern('/pop/v1/sam/configmap/configMap')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_ChangeOrderId(self):
-		return self.get_query_params().get('ChangeOrderId')
+	def get_ConfigMapId(self):
+		return self.get_query_params().get('ConfigMapId')
 
-	def set_ChangeOrderId(self,ChangeOrderId):
-		self.add_query_param('ChangeOrderId',ChangeOrderId)
+	def set_ConfigMapId(self,ConfigMapId):
+		self.add_query_param('ConfigMapId',ConfigMapId)
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeNamespaceListRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeNamespaceListRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DescribeNamespaceListRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeNamespaceList')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeNamespaceList','serverless')
 		self.set_uri_pattern('/pop/v1/sam/namespace/describeNamespaceList')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/RescaleApplicationVerticallyRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/RescaleApplicationVerticallyRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class RescaleApplicationVerticallyRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'RescaleApplicationVertically')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'RescaleApplicationVertically','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/rescaleApplicationVertically')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeNamespaceResourcesRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeNamespaceResourcesRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DescribeNamespaceResourcesRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeNamespaceResources')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeNamespaceResources','serverless')
 		self.set_uri_pattern('/pop/v1/sam/namespace/describeNamespaceResources')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/StopApplicationRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeApplicationSlbsRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
-class StopApplicationRequest(RoaRequest):
+class DescribeApplicationSlbsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'StopApplication')
-		self.set_uri_pattern('/pop/v1/sam/app/stopApplication')
-		self.set_method('PUT')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeApplicationSlbs','serverless')
+		self.set_uri_pattern('/pop/v1/sam/app/slb')
+		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_AppId(self):
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListApplicationsRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListApplicationsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class ListApplicationsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListApplications')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListApplications','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/listApplications')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/RestartApplicationRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/RestartApplicationRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class RestartApplicationRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'RestartApplication')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'RestartApplication','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/restartApplication')
 		self.set_method('PUT')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListLogConfigsRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListLogConfigsRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class ListLogConfigsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListLogConfigs')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListLogConfigs','serverless')
 		self.set_uri_pattern('/pop/v1/sam/log/listLogConfigs')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListIngressesRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListIngressesRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class ListIngressesRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListIngresses')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListIngresses','serverless')
 		self.set_uri_pattern('/pop/v1/sam/ingress/IngressList')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeApplicationGroupsRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeApplicationGroupsRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DescribeApplicationGroupsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeApplicationGroups')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeApplicationGroups','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/describeApplicationGroups')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeEdasContainersRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeEdasContainersRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DescribeEdasContainersRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeEdasContainers')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeEdasContainers','serverless')
 		self.set_uri_pattern('/pop/v1/sam/resource/edasContainers')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/AbortChangeOrderRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeChangeOrderRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
-class AbortChangeOrderRequest(RoaRequest):
+class DescribeChangeOrderRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'AbortChangeOrder')
-		self.set_uri_pattern('/pop/v1/sam/changeorder/AbortChangeOrder')
-		self.set_method('PUT')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeChangeOrder','serverless')
+		self.set_uri_pattern('/pop/v1/sam/changeorder/DescribeChangeOrder')
+		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_ChangeOrderId(self):
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/CreateIngressRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/CreateIngressRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class CreateIngressRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'CreateIngress')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'CreateIngress','serverless')
 		self.set_uri_pattern('/pop/v1/sam/ingress/Ingress')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -53,18 +53,18 @@
 	def get_Description(self):
 		return self.get_query_params().get('Description')
 
 	def set_Description(self,Description):
 		self.add_query_param('Description',Description)
 
 	def get_Rules(self):
-		return self.get_query_params().get('Rules')
+		return self.get_body_params().get('Rules')
 
 	def set_Rules(self,Rules):
-		self.add_query_param('Rules',Rules)
+		self.add_body_params('Rules', Rules)
 
 	def get_CertId(self):
 		return self.get_query_params().get('CertId')
 
 	def set_CertId(self,CertId):
 		self.add_query_param('CertId',CertId)
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/RollbackApplicationRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/RollbackApplicationRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class RollbackApplicationRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'RollbackApplication')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'RollbackApplication','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/rollbackApplication')
 		self.set_method('PUT')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ConfirmPipelineBatchRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ConfirmPipelineBatchRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class ConfirmPipelineBatchRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ConfirmPipelineBatch')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ConfirmPipelineBatch','serverless')
 		self.set_uri_pattern('/pop/v1/sam/changeorder/ConfirmPipelineBatch')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListPublishedServicesRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListPublishedServicesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class ListPublishedServicesRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListPublishedServices')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListPublishedServices','serverless')
 		self.set_uri_pattern('/pop/v1/sam/service/listPublishedServices')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListTagResourcesRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListTagResourcesRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class ListTagResourcesRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListTagResources')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListTagResources','serverless')
 		self.set_uri_pattern('/tags')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeIngressRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeIngressRequest.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DescribeIngressRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeIngress')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeIngress','serverless')
 		self.set_uri_pattern('/pop/v1/sam/ingress/Ingress')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeApplicationSlbsRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/QueryResourceStaticsRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
-class DescribeApplicationSlbsRequest(RoaRequest):
+class QueryResourceStaticsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeApplicationSlbs')
-		self.set_uri_pattern('/pop/v1/sam/app/slb')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'QueryResourceStatics','serverless')
+		self.set_uri_pattern('/pop/v1/paas/quota/queryResourceStatics')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeApplicationInstancesRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeApplicationInstancesRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DescribeApplicationInstancesRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeApplicationInstances')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeApplicationInstances','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/describeApplicationInstances')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListAppEventsRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListAppEventsRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class ListAppEventsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListAppEvents')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListAppEvents','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/listAppEvents')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/UnbindSlbRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/UnbindSlbRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class UnbindSlbRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'UnbindSlb')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'UnbindSlb','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/slb')
 		self.set_method('DELETE')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/QueryResourceStaticsRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListAppVersionsRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
-class QueryResourceStaticsRequest(RoaRequest):
+class ListAppVersionsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'QueryResourceStatics')
-		self.set_uri_pattern('/pop/v1/paas/quota/queryResourceStatics')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListAppVersions','serverless')
+		self.set_uri_pattern('/pop/v1/sam/app/listAppVersions')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/UpdateNamespaceVpcRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/UpdateNamespaceVpcRequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class UpdateNamespaceVpcRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'UpdateNamespaceVpc')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'UpdateNamespaceVpc','serverless')
 		self.set_uri_pattern('/pop/v1/sam/namespace/updateNamespaceVpc')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeApplicationStatusRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeApplicationStatusRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DescribeApplicationStatusRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeApplicationStatus')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeApplicationStatus','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/describeApplicationStatus')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/UpdateApplicationVswitchesRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/UpdateAppSecurityGroupRequest.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,30 +16,30 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
-class UpdateApplicationVswitchesRequest(RoaRequest):
+class UpdateAppSecurityGroupRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'UpdateApplicationVswitches')
-		self.set_uri_pattern('/pop/v1/sam/app/updateAppVswitches')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'UpdateAppSecurityGroup','serverless')
+		self.set_uri_pattern('/pop/v1/sam/app/updateAppSecurityGroup')
 		self.set_method('PUT')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
-	def get_VSwitchId(self):
-		return self.get_query_params().get('VSwitchId')
-
-	def set_VSwitchId(self,VSwitchId):
-		self.add_query_param('VSwitchId',VSwitchId)
-
 	def get_AppId(self):
 		return self.get_query_params().get('AppId')
 
 	def set_AppId(self,AppId):
-		self.add_query_param('AppId',AppId)
+		self.add_query_param('AppId',AppId)
+
+	def get_SecurityGroupId(self):
+		return self.get_query_params().get('SecurityGroupId')
+
+	def set_SecurityGroupId(self,SecurityGroupId):
+		self.add_query_param('SecurityGroupId',SecurityGroupId)
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/BatchStopApplicationsRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/BatchStopApplicationsRequest.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class BatchStopApplicationsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'BatchStopApplications')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'BatchStopApplications','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/batchStopApplications')
 		self.set_method('PUT')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DeleteIngressRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DeleteIngressRequest.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DeleteIngressRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DeleteIngress')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DeleteIngress','serverless')
 		self.set_uri_pattern('/pop/v1/sam/ingress/Ingress')
 		self.set_method('DELETE')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DeleteApplicationRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DeleteApplicationRequest.py`

 * *Files 8% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DeleteApplicationRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DeleteApplication')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DeleteApplication','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/deleteApplication')
 		self.set_method('DELETE')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeComponentsRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeComponentsRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DescribeComponentsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeComponents')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeComponents','serverless')
 		self.set_uri_pattern('/pop/v1/sam/resource/components')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListAppVersionsRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/StopApplicationRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
-class ListAppVersionsRequest(RoaRequest):
+class StopApplicationRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListAppVersions')
-		self.set_uri_pattern('/pop/v1/sam/app/listAppVersions')
-		self.set_method('GET')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'StopApplication','serverless')
+		self.set_uri_pattern('/pop/v1/sam/app/stopApplication')
+		self.set_method('PUT')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
 
 	def get_AppId(self):
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/UntagResourcesRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/UntagResourcesRequest.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class UntagResourcesRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'UntagResources')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'UntagResources','serverless')
 		self.set_uri_pattern('/tags')
 		self.set_method('DELETE')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeApplicationImageRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeApplicationImageRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DescribeApplicationImageRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeApplicationImage')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeApplicationImage','serverless')
 		self.set_uri_pattern('/pop/v1/sam/container/describeApplicationImage')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/TagResourcesRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/TagResourcesRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class TagResourcesRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'TagResources')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'TagResources','serverless')
 		self.set_uri_pattern('/tags')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeNamespacesRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeNamespacesRequest.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DescribeNamespacesRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeNamespaces')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeNamespaces','serverless')
 		self.set_uri_pattern('/pop/v1/paas/namespaces')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/UpdateNamespaceRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/UpdateNamespaceRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class UpdateNamespaceRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'UpdateNamespace')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'UpdateNamespace','serverless')
 		self.set_uri_pattern('/pop/v1/paas/namespace')
 		self.set_method('PUT')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/ListChangeOrdersRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/ListChangeOrdersRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class ListChangeOrdersRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListChangeOrders')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'ListChangeOrders','serverless')
 		self.set_uri_pattern('/pop/v1/sam/changeorder/ListChangeOrders')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DeployApplicationRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DeployApplicationRequest.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DeployApplicationRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DeployApplication')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DeployApplication','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/deployApplication')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
 
@@ -46,14 +46,20 @@
 
 	def get_JarStartArgs(self):
 		return self.get_query_params().get('JarStartArgs')
 
 	def set_JarStartArgs(self,JarStartArgs):
 		self.add_query_param('JarStartArgs',JarStartArgs)
 
+	def get_EnableAhas(self):
+		return self.get_query_params().get('EnableAhas')
+
+	def set_EnableAhas(self,EnableAhas):
+		self.add_query_param('EnableAhas',EnableAhas)
+
 	def get_SlsConfigs(self):
 		return self.get_query_params().get('SlsConfigs')
 
 	def set_SlsConfigs(self,SlsConfigs):
 		self.add_query_param('SlsConfigs',SlsConfigs)
 
 	def get_CommandArgs(self):
@@ -94,14 +100,20 @@
 
 	def get_Envs(self):
 		return self.get_query_params().get('Envs')
 
 	def set_Envs(self,Envs):
 		self.add_query_param('Envs',Envs)
 
+	def get_PhpArmsConfigLocation(self):
+		return self.get_query_params().get('PhpArmsConfigLocation')
+
+	def set_PhpArmsConfigLocation(self,PhpArmsConfigLocation):
+		self.add_query_param('PhpArmsConfigLocation',PhpArmsConfigLocation)
+
 	def get_PackageVersion(self):
 		return self.get_query_params().get('PackageVersion')
 
 	def set_PackageVersion(self,PackageVersion):
 		self.add_query_param('PackageVersion',PackageVersion)
 
 	def get_CustomHostAlias(self):
@@ -130,14 +142,32 @@
 
 	def get_PackageUrl(self):
 		return self.get_query_params().get('PackageUrl')
 
 	def set_PackageUrl(self,PackageUrl):
 		self.add_query_param('PackageUrl',PackageUrl)
 
+	def get_TerminationGracePeriodSeconds(self):
+		return self.get_query_params().get('TerminationGracePeriodSeconds')
+
+	def set_TerminationGracePeriodSeconds(self,TerminationGracePeriodSeconds):
+		self.add_query_param('TerminationGracePeriodSeconds',TerminationGracePeriodSeconds)
+
+	def get_ConfigMapMountDesc(self):
+		return self.get_body_params().get('ConfigMapMountDesc')
+
+	def set_ConfigMapMountDesc(self,ConfigMapMountDesc):
+		self.add_body_params('ConfigMapMountDesc', ConfigMapMountDesc)
+
+	def get_PhpConfig(self):
+		return self.get_body_params().get('PhpConfig')
+
+	def set_PhpConfig(self,PhpConfig):
+		self.add_body_params('PhpConfig', PhpConfig)
+
 	def get_PreStop(self):
 		return self.get_query_params().get('PreStop')
 
 	def set_PreStop(self,PreStop):
 		self.add_query_param('PreStop',PreStop)
 
 	def get_Command(self):
@@ -184,12 +214,18 @@
 
 	def get_ImageUrl(self):
 		return self.get_query_params().get('ImageUrl')
 
 	def set_ImageUrl(self,ImageUrl):
 		self.add_query_param('ImageUrl',ImageUrl)
 
+	def get_PhpConfigLocation(self):
+		return self.get_query_params().get('PhpConfigLocation')
+
+	def set_PhpConfigLocation(self,PhpConfigLocation):
+		self.add_query_param('PhpConfigLocation',PhpConfigLocation)
+
 	def get_PostStart(self):
 		return self.get_query_params().get('PostStart')
 
 	def set_PostStart(self,PostStart):
 		self.add_query_param('PostStart',PostStart)
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/BatchStartApplicationsRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/BatchStartApplicationsRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class BatchStartApplicationsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'BatchStartApplications')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'BatchStartApplications','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/batchStartApplications')
 		self.set_method('PUT')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeRegionsRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeRegionsRequest.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,14 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DescribeRegionsRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeRegions')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeRegions','serverless')
 		self.set_uri_pattern('/pop/v1/paas/regionConfig')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/BindSlbRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/BindSlbRequest.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class BindSlbRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'BindSlb')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'BindSlb','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/slb')
 		self.set_method('POST')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/DescribeApplicationConfigRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/DescribeApplicationConfigRequest.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class DescribeApplicationConfigRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeApplicationConfig')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'DescribeApplicationConfig','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/describeApplicationConfig')
 		self.set_method('GET')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/request/v20190506/RescaleApplicationRequest.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/request/v20190506/RescaleApplicationRequest.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 from aliyunsdkcore.request import RoaRequest
 from aliyunsdksae.endpoint import endpoint_data
 
 class RescaleApplicationRequest(RoaRequest):
 
 	def __init__(self):
-		RoaRequest.__init__(self, 'sae', '2019-05-06', 'RescaleApplication')
+		RoaRequest.__init__(self, 'sae', '2019-05-06', 'RescaleApplication','serverless')
 		self.set_uri_pattern('/pop/v1/sam/app/rescaleApplication')
 		self.set_method('PUT')
 		if hasattr(self, "endpoint_map"):
 			setattr(self, "endpoint_map", endpoint_data.getEndpointMap())
 		if hasattr(self, "endpoint_regional"):
 			setattr(self, "endpoint_regional", endpoint_data.getEndpointRegional())
```

### Comparing `aliyun-python-sdk-sae-1.4.0.0/aliyunsdksae/endpoint.py` & `aliyun-python-sdk-sae-1.5.0.0/aliyunsdksae/endpoint.py`

 * *Files identical despite different names*

