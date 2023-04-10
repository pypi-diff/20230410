# Comparing `tmp/qiskit-ibm-provider-0.5.1.tar.gz` & `tmp/qiskit-ibm-provider-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/qiskit-ibm-provider-0.5.1.tar", last modified: Tue Apr  4 19:46:45 2023, max compression
+gzip compressed data, was "dist/qiskit-ibm-provider-0.5.2.tar", last modified: Mon Apr 10 21:25:21 2023, max compression
```

## Comparing `qiskit-ibm-provider-0.5.1.tar` & `qiskit-ibm-provider-0.5.2.tar`

### file list

```diff
@@ -1,196 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/VERSION.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/accounts/
--rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/accounts/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/accounts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/accounts/management.py
--rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/accounts/storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/client_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/runtime_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/websocket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/program_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/root.py
--rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/utils/data_mapper.py
--rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/apiconstants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/hub_group_project.py
--rw-r--r--   0 runner    (1001) docker     (123)    36424 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/ibm_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)    28562 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/ibm_backend_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/ibm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/ibm_qubit_properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    32324 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/ibm_circuit_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    48879 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/ibm_composite_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/ibm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/job_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/queueinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/sub_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/backend_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/config_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/backend_update.py
--rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/gates_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/jobs_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/qubits_widget.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/proxies/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/proxies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/proxies/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/
--rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/binary_io/
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/binary_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38998 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/binary_io/circuits.py
--rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/binary_io/schedules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/binary_io/value.py
--rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/formats.py
--rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/type_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py
--rw-r--r--   0 runner    (1001) docker     (123)    23298 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py
--rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/backend_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/backend_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/converters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/hgp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/json_decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/qobj_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/colormaps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/device_layouts.py
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/interactive/
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/interactive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/interactive/error_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/interactive/gate_map.py
--rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6584 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/qiskit_ibm_provider.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/contextmanagers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/test/e2e/
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/e2e/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/e2e/test_real_devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/e2e/test_tutorials.py
--rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/fake_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/http_server.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/ibm_test_case.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/test/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/test_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6689 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/test_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/test_basic_server_paths.py
--rw-r--r--   0 runner    (1001) docker     (123)    38625 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/test_composite_job.py
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/test_filter_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/test_ibm_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20848 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/test_ibm_job.py
--rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/test_ibm_job_attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/test_ibm_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/test_ibm_qasm_simulator.py
--rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/test_jupyter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/test_proxies.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/integration/test_websocket_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/jobtestcase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/proxy_server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/test/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/test/unit/mock/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/mock/fake_account_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/mock/fake_provider.py
--rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)    22433 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/test_ibm_job_states.py
--rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/test_ibm_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/test_websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/test/unit/transpiler/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/transpiler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/basis/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/basis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/scheduling/
--rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/scheduling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/scheduling/control_flow_test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py
--rw-r--r--   0 runner    (1001) docker     (123)    58260 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/scheduling/test_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/scheduling/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-04 19:46:45.000000 qiskit-ibm-provider-0.5.1/test/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/unit/utils/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-04 19:46:35.000000 qiskit-ibm-provider-0.5.1/test/ws_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11416 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5072 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/VERSION.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4547 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/
+-rw-r--r--   0 runner    (1001) docker     (123)      712 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5325 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7443 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2888 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1248 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/client_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6235 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9375 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/runtime_ws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7521 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/websocket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1955 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/program_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4139 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/root.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/utils/data_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13683 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/apiconstants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/hub_group_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37988 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29558 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_backend_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25047 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_qubit_properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32324 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/ibm_circuit_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48879 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/ibm_composite_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7480 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/ibm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3429 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/job_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6792 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/queueinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4792 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/sub_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)     2507 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3277 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/backend_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4386 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/config_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/backend_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8069 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12078 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      714 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3341 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4713 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/gates_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10137 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/jobs_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3586 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/qubits_widget.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/proxies/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/proxies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/proxies/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38998 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/circuits.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16213 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/schedules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12505 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7833 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/formats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9707 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11718 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/type_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     1039 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      840 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23601 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23298 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2497 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28286 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10053 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7415 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/backend_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/backend_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/hgp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10657 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4789 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/json_decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/qobj_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9215 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/colormaps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2689 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/device_layouts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16827 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/error_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/gate_map.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4465 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6370 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6610 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4797 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/contextmanagers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4997 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/e2e/
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/e2e/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8769 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/e2e/test_real_devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/e2e/test_tutorials.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18373 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/fake_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/http_server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/ibm_test_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7818 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_basic_server_paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38625 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_composite_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_filter_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6022 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_ibm_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20848 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_ibm_job.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15401 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_ibm_job_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12946 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_ibm_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7297 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_ibm_qasm_simulator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5181 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_jupyter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_proxies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8803 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/integration/test_websocket_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/jobtestcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2072 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/proxy_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/unit/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4080 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/mock/fake_account_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3514 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/mock/fake_provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18671 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6047 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/test_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22540 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/test_ibm_job_states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8029 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/test_ibm_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5074 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/test_websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/basis/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/basis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/
+-rw-r--r--   0 runner    (1001) docker     (123)      477 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1362 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/control_flow_test_case.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26825 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    58260 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/test_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:25:21.000000 qiskit-ibm-provider-0.5.2/test/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/unit/utils/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3738 2023-04-10 21:25:10.000000 qiskit-ibm-provider-0.5.2/test/ws_server.py
```

### Comparing `qiskit-ibm-provider-0.5.1/LICENSE.txt` & `qiskit-ibm-provider-0.5.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/PKG-INFO` & `qiskit-ibm-provider-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-provider
-Version: 0.5.1
+Version: 0.5.2
 Summary: Qiskit IBM Quantum Provider for accessing the quantum devices and simulators at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-provider
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-provider/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-provider-0.5.1/README.md` & `qiskit-ibm-provider-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/accounts/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/accounts/account.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/accounts/exceptions.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/accounts/management.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/management.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/accounts/storage.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/accounts/storage.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/auth.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/client_parameters.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/client_parameters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/account.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/auth.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/auth.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/base.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/runtime.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/runtime.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/runtime_ws.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/runtime_ws.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/version.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/clients/websocket.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/clients/websocket.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/exceptions.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/backend.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/backend.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/base.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/base.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/job.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/program_job.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/program_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/root.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/root.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/runtime.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/runtime.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/utils/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/rest/utils/data_mapper.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/rest/utils/data_mapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/api/session.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/api/session.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/apiconstants.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/apiconstants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/exceptions.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/hub_group_project.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/hub_group_project.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/ibm_backend.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -486,14 +486,20 @@
         )
 
         run_config_dict["circuits"] = circuits
         if not program_id.startswith(QASM3RUNNERPROGRAMID):
             # Transpiling in circuit-runner is deprecated.
             run_config_dict["skip_transpilation"] = True
 
+        if isinstance(circuits, (QuantumCircuit, Schedule)):
+            circuits = [circuits]
+        for circ in circuits:
+            if isinstance(circ, QuantumCircuit):
+                self.check_faulty(circ)
+
         return self._runtime_run(
             program_id=program_id,
             inputs=run_config_dict,
             options=options,
             job_tags=job_tags,
         )
 
@@ -794,14 +800,50 @@
 
         return circuits
 
     def get_translation_stage_plugin(self) -> str:
         """Return the default translation stage plugin name for IBM backends."""
         return "ibm_dynamic_circuits"
 
+    def check_faulty(self, circuit: QuantumCircuit) -> None:
+        """Check if the input circuit uses faulty qubits or edges.
+
+        Args:
+            circuit: Circuit to check.
+
+        Raises:
+            ValueError: If an instruction operating on a faulty qubit or edge is found.
+        """
+        if not self.properties():
+            return
+
+        faulty_qubits = self.properties().faulty_qubits()
+        faulty_gates = self.properties().faulty_gates()
+        faulty_edges = [
+            tuple(gate.qubits) for gate in faulty_gates if len(gate.qubits) > 1
+        ]
+
+        for instr in circuit.data:
+            if instr.operation.name == "barrier":
+                continue
+            qubit_indices = tuple(circuit.find_bit(x).index for x in instr.qubits)
+
+            for circ_qubit in qubit_indices:
+                if circ_qubit in faulty_qubits:
+                    raise ValueError(
+                        f"Circuit {circuit.name} contains instruction "
+                        f"{instr} operating on a faulty qubit {circ_qubit}."
+                    )
+
+            if len(qubit_indices) == 2 and qubit_indices in faulty_edges:
+                raise ValueError(
+                    f"Circuit {circuit.name} contains instruction "
+                    f"{instr} operating on a faulty edge {qubit_indices}"
+                )
+
 
 class IBMRetiredBackend(IBMBackend):
     """Backend class interfacing with an IBM Quantum device no longer available."""
 
     def __init__(
         self,
         configuration: Union[QasmBackendConfiguration, PulseBackendConfiguration],
```

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/ibm_backend_service.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_backend_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,41 +153,45 @@
 
         Returns:
             The list of available backends that match the filter.
 
         Raises:
             IBMBackendValueError: If only one or two parameters from `hub`, `group`,
                 `project` are specified.
+            QiskitBackendNotFoundError: If the backend is not found in any instance.
         """
         backends: List[IBMBackend] = []
-        if instance:
+        if name:
+            if name not in self._backends:
+                raise QiskitBackendNotFoundError("No backend matches the criteria")
+            if not self._backends[name] or instance != self._backends[name]._instance:
+                self._set_backend_config(name)
+                self._backends[name] = self._create_backend_obj(
+                    self._backend_configs[name], instance, self._provider._get_hgps()
+                )
+            backends.append(self._backends[name])
+        elif instance:
             hgp = self._provider._get_hgp(instance=instance)
             for backend_name in hgp.backends.keys():
                 if (
                     not self._backends[backend_name]
                     or instance != self._backends[backend_name]._instance
                 ):
                     self._set_backend_config(backend_name, instance)
                     self._backends[backend_name] = self._create_backend_obj(
                         self._backend_configs[backend_name], instance
                     )
                 backends.append(self._backends[backend_name])
-        elif name:
-            if not self._backends[name]:
-                self._set_backend_config(name, instance)
-                self._backends[name] = self._create_backend_obj(
-                    self._backend_configs[name], instance
-                )
-            backends.append(self._backends[name])
         else:
+            hgps = self._provider._get_hgps()
             for backend_name, backend_config in self._backends.items():
                 if not backend_config:
-                    self._set_backend_config(backend_name, instance)
+                    self._set_backend_config(backend_name)
                     self._backends[backend_name] = self._create_backend_obj(
-                        self._backend_configs[backend_name], instance
+                        self._backend_configs[backend_name], hgps=hgps
                     )
                 backends.append(self._backends[backend_name])
         # Special handling of the `name` parameter, to support alias resolution.
         if name:
             aliases = self._aliased_backend_names()
             aliases.update(self._deprecated_backend_names())
             name = aliases.get(name, name)
@@ -668,23 +672,41 @@
             )
             self._backend_configs[backend_name] = config
 
     def _create_backend_obj(
         self,
         config: Union[QasmBackendConfiguration, PulseBackendConfiguration],
         instance: Optional[str] = None,
+        hgps: Optional[List] = None,
     ) -> IBMBackend:
         """Given a backend configuration return the backend object.
 
         Args:
             config: backend configuration.
             instance: the current h/g/p.
         Returns:
             A backend object.
+        Raises:
+            QiskitBackendNotFoundError: if the backend is not in the hgp passed in.
         """
+        if not instance:
+            for hgp in hgps:
+                if config.backend_name in hgp.backends:
+                    instance = to_instance_format(hgp._hub, hgp._group, hgp._project)
+                    break
+
+        elif (
+            config.backend_name
+            not in self._provider._get_hgp(instance=instance).backends
+        ):
+            raise QiskitBackendNotFoundError(
+                f"Backend {config.backend_name} is not in "
+                f"{instance}: please try a different hub/group/project."
+            )
+
         return ibm_backend.IBMBackend(
             instance=instance,
             configuration=config,
             api_client=AccountClient(self._provider._client_params),
             provider=self._provider,
         )
```

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/ibm_provider.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/ibm_qubit_properties.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/ibm_qubit_properties.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/constants.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/exceptions.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/ibm_circuit_job.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/ibm_circuit_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/ibm_composite_job.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/ibm_composite_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/ibm_job.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/ibm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/job_monitor.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/job_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/queueinfo.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/queueinfo.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/sub_job.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/sub_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/job/utils.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/job/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/backend_info.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/backend_info.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/config_widget.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/config_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/backend_update.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/backend_update.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/backend_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/constants.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/constants.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/dashboard.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/dashboard.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/job_widgets.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/provider_buttons.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/utils.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/dashboard/watcher_monitor.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/gates_widget.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/gates_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/jobs_widget.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/jobs_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/jupyter/qubits_widget.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/jupyter/qubits_widget.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/proxies/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/proxies/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/proxies/configuration.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/proxies/configuration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/binary_io/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/binary_io/circuits.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/circuits.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/binary_io/schedules.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/schedules.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/binary_io/value.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/binary_io/value.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/common.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/common.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/exceptions.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/formats.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/formats.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/interface.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/interface.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/qpy/type_keys.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/qpy/type_keys.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/basis/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/basis/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/basis/convert_id_to_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/block_base_padder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/dynamical_decoupling.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/pad_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/scheduler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/passes/scheduling/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/transpiler/plugin.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/transpiler/plugin.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/backend_converter.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/backend_converter.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/backend_decoder.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/backend_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/converters.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/converters.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/hgp.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/hgp.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/json.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/json.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/json_decoder.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/json_decoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/json_encoder.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/options.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/options.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/qobj_utils.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/qobj_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/utils/utils.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/utils/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/version.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/version.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/colormaps.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/colormaps.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/device_layouts.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/device_layouts.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/exceptions.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/exceptions.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/interactive/__init__.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/interactive/error_map.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/error_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/interactive/gate_map.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/gate_map.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider/visualization/interactive/plotly_wrapper.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider.egg-info/PKG-INFO` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-ibm-provider
-Version: 0.5.1
+Version: 0.5.2
 Summary: Qiskit IBM Quantum Provider for accessing the quantum devices and simulators at IBM
 Home-page: https://github.com/Qiskit/qiskit-ibm-provider
 Author: Qiskit Development Team
 Author-email: hello@qiskit.org
 License: Apache 2.0
 Project-URL: Bug Tracker, https://github.com/Qiskit/qiskit-ibm-provider/issues
 Project-URL: Documentation, https://qiskit.org/documentation/
```

### Comparing `qiskit-ibm-provider-0.5.1/qiskit_ibm_provider.egg-info/SOURCES.txt` & `qiskit-ibm-provider-0.5.2/qiskit_ibm_provider.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 test/integration/test_ibm_qasm_simulator.py
 test/integration/test_jupyter.py
 test/integration/test_proxies.py
 test/integration/test_serialization.py
 test/integration/test_websocket_integration.py
 test/unit/__init__.py
 test/unit/test_account.py
+test/unit/test_backend.py
 test/unit/test_ibm_job_states.py
 test/unit/test_ibm_logger.py
 test/unit/test_serialization.py
 test/unit/test_websocket.py
 test/unit/mock/__init__.py
 test/unit/mock/fake_account_client.py
 test/unit/mock/fake_provider.py
```

### Comparing `qiskit-ibm-provider-0.5.1/setup.cfg` & `qiskit-ibm-provider-0.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/setup.py` & `qiskit-ibm-provider-0.5.2/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/__init__.py` & `qiskit-ibm-provider-0.5.2/test/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/account.py` & `qiskit-ibm-provider-0.5.2/test/account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/contextmanagers.py` & `qiskit-ibm-provider-0.5.2/test/contextmanagers.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/decorators.py` & `qiskit-ibm-provider-0.5.2/test/decorators.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/e2e/test_real_devices.py` & `qiskit-ibm-provider-0.5.2/test/e2e/test_real_devices.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/e2e/test_tutorials.py` & `qiskit-ibm-provider-0.5.2/test/e2e/test_tutorials.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/fake_account_client.py` & `qiskit-ibm-provider-0.5.2/test/fake_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/http_server.py` & `qiskit-ibm-provider-0.5.2/test/http_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/ibm_test_case.py` & `qiskit-ibm-provider-0.5.2/test/ibm_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/integration/test_account_client.py` & `qiskit-ibm-provider-0.5.2/test/integration/test_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/integration/test_backend.py` & `qiskit-ibm-provider-0.5.2/test/integration/test_backend.py`

 * *Files 19% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 """IBMBackend Test."""
 
 from unittest import SkipTest, mock, skip
 from unittest.mock import patch
 
 from qiskit import QuantumCircuit, transpile
 from qiskit.providers.models import QasmBackendConfiguration
+from qiskit.providers.exceptions import QiskitBackendNotFoundError
 from qiskit.test.reference_circuits import ReferenceCircuits
 
 from qiskit_ibm_provider import IBMBackend, IBMProvider
 from qiskit_ibm_provider.ibm_qubit_properties import IBMQubitProperties
 from ..decorators import (
     IntegrationTestDependencies,
     integration_test_setup_with_backend,
@@ -162,7 +163,28 @@
         circ = QuantumCircuit(2)
         circ.id(0)
         circ.id(1)
         tqc = transpile(circ, self.backend)
         op_counts = tqc.count_ops()
         self.assertNotIn("id", op_counts)
         self.assertIn("delay", op_counts)
+
+    def test_backend_wrong_instance(self):
+        """Test that an error is raised when retrieving a backend not in the instance."""
+        backends = self.dependencies.provider.backends()
+        hgps = self.dependencies.provider._hgps.values()
+        if len(hgps) >= 2:
+            for hgp in hgps:
+                backend_names = list(hgp._backends)
+                for backend in backends:
+                    if backend.name not in backend_names:
+                        with self.assertRaises(QiskitBackendNotFoundError):
+                            self.dependencies.provider.get_backend(
+                                backend.name,
+                                instance=f"{hgp._hub}/{hgp._group}/{hgp._project}",
+                            )
+                        return
+
+    def test_retrieve_backend_not_exist(self):
+        """Test that an error is raised when retrieving a backend that does not exist."""
+        with self.assertRaises(QiskitBackendNotFoundError):
+            self.dependencies.provider.get_backend("nonexistent_backend")
```

### Comparing `qiskit-ibm-provider-0.5.1/test/integration/test_basic_server_paths.py` & `qiskit-ibm-provider-0.5.2/test/integration/test_basic_server_paths.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/integration/test_composite_job.py` & `qiskit-ibm-provider-0.5.2/test/integration/test_composite_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/integration/test_filter_backends.py` & `qiskit-ibm-provider-0.5.2/test/integration/test_filter_backends.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/integration/test_ibm_integration.py` & `qiskit-ibm-provider-0.5.2/test/integration/test_ibm_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/integration/test_ibm_job.py` & `qiskit-ibm-provider-0.5.2/test/integration/test_ibm_job.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/integration/test_ibm_job_attributes.py` & `qiskit-ibm-provider-0.5.2/test/integration/test_ibm_job_attributes.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/integration/test_ibm_provider.py` & `qiskit-ibm-provider-0.5.2/test/integration/test_ibm_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/integration/test_ibm_qasm_simulator.py` & `qiskit-ibm-provider-0.5.2/test/integration/test_ibm_qasm_simulator.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/integration/test_jupyter.py` & `qiskit-ibm-provider-0.5.2/test/integration/test_jupyter.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/integration/test_proxies.py` & `qiskit-ibm-provider-0.5.2/test/integration/test_proxies.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/integration/test_serialization.py` & `qiskit-ibm-provider-0.5.2/test/integration/test_serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/integration/test_websocket_integration.py` & `qiskit-ibm-provider-0.5.2/test/integration/test_websocket_integration.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/jobtestcase.py` & `qiskit-ibm-provider-0.5.2/test/jobtestcase.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/proxy_server.py` & `qiskit-ibm-provider-0.5.2/test/proxy_server.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/unit/mock/fake_account_client.py` & `qiskit-ibm-provider-0.5.2/test/unit/mock/fake_account_client.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/unit/mock/fake_provider.py` & `qiskit-ibm-provider-0.5.2/test/unit/mock/fake_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/unit/test_account.py` & `qiskit-ibm-provider-0.5.2/test/unit/test_account.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/unit/test_ibm_job_states.py` & `qiskit-ibm-provider-0.5.2/test/unit/test_ibm_job_states.py`

 * *Files 1% similar despite different names*

```diff
@@ -518,14 +518,17 @@
             "backend_name": backend_name,
             "backend_version": "0.0.0",
             "operational": True,
             "pending_jobs": 0,
             "status_msg": "active",
         }
 
+    def backend_properties(self, *args, **kwargs):  # pylint: disable=unused-argument
+        return None
+
     def job_type(self, job_id: str) -> str:
         if job_id[0] != "c" and len(job_id) == 24:
             return "IQX"
         return "RUNTIME"
 
 
 class UnknownStatusAPI(BaseFakeAPI):
```

### Comparing `qiskit-ibm-provider-0.5.1/test/unit/test_ibm_logger.py` & `qiskit-ibm-provider-0.5.2/test/unit/test_ibm_logger.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/unit/test_serialization.py` & `qiskit-ibm-provider-0.5.2/test/unit/test_serialization.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/unit/test_websocket.py` & `qiskit-ibm-provider-0.5.2/test/unit/test_websocket.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py` & `qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/basis/test_convert_id_to_delay.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/scheduling/control_flow_test_case.py` & `qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/control_flow_test_case.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py` & `qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/test_dynamical_decoupling.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/scheduling/test_scheduler.py` & `qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/test_scheduler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/unit/transpiler/passes/scheduling/test_utils.py` & `qiskit-ibm-provider-0.5.2/test/unit/transpiler/passes/scheduling/test_utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/unit/utils/ws_handler.py` & `qiskit-ibm-provider-0.5.2/test/unit/utils/ws_handler.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/utils.py` & `qiskit-ibm-provider-0.5.2/test/utils.py`

 * *Files identical despite different names*

### Comparing `qiskit-ibm-provider-0.5.1/test/ws_server.py` & `qiskit-ibm-provider-0.5.2/test/ws_server.py`

 * *Files identical despite different names*

