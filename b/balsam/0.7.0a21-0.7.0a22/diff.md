# Comparing `tmp/balsam-0.7.0a21.tar.gz` & `tmp/balsam-0.7.0a22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "balsam-0.7.0a21.tar", last modified: Mon Feb  6 23:35:30 2023, max compression
+gzip compressed data, was "balsam-0.7.0a22.tar", last modified: Mon Apr 10 20:36:58 2023, max compression
```

## Comparing `balsam-0.7.0a21.tar` & `balsam-0.7.0a22.tar`

### file list

```diff
@@ -1,267 +1,271 @@
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.451175 balsam-0.7.0a21/
--rw-r--r--   0 turam      (501) staff       (20)      813 2023-02-06 23:35:30.451283 balsam-0.7.0a21/PKG-INFO
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.396866 balsam-0.7.0a21/balsam/
--rw-r--r--   0 turam      (501) staff       (20)       91 2023-02-06 22:58:44.000000 balsam-0.7.0a21/balsam/__init__.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.400087 balsam-0.7.0a21/balsam/_api/
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/_api/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)    17893 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/_api/app.py
--rw-r--r--   0 turam      (501) staff       (20)    15182 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/_api/bases.py
--rw-r--r--   0 turam      (501) staff       (20)    10519 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/_api/manager.py
--rw-r--r--   0 turam      (501) staff       (20)     7943 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/_api/model.py
--rw-r--r--   0 turam      (501) staff       (20)    68175 2023-02-06 23:24:19.000000 balsam-0.7.0a21/balsam/_api/models.py
--rw-r--r--   0 turam      (501) staff       (20)     6273 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/_api/query.py
--rw-r--r--   0 turam      (501) staff       (20)     1862 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/analytics.py
--rw-r--r--   0 turam      (501) staff       (20)     1523 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/api.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.402250 balsam-0.7.0a21/balsam/client/
--rw-r--r--   0 turam      (501) staff       (20)      404 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/client/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     5307 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/client/encoders.py
--rw-r--r--   0 turam      (501) staff       (20)     5284 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/client/requests_client.py
--rw-r--r--   0 turam      (501) staff       (20)     4132 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/client/requests_oauth.py
--rw-r--r--   0 turam      (501) staff       (20)     3025 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/client/requests_password.py
--rw-r--r--   0 turam      (501) staff       (20)     3515 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/client/rest_base_client.py
--rw-r--r--   0 turam      (501) staff       (20)      185 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/client/urls.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.404538 balsam-0.7.0a21/balsam/cmdline/
--rw-r--r--   0 turam      (501) staff       (20)     1655 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/cmdline/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     5820 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/cmdline/_launcher.py
--rw-r--r--   0 turam      (501) staff       (20)     2022 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/cmdline/app.py
--rw-r--r--   0 turam      (501) staff       (20)    12179 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/cmdline/job.py
--rw-r--r--   0 turam      (501) staff       (20)       89 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/cmdline/launcher.py
--rw-r--r--   0 turam      (501) staff       (20)     2175 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/cmdline/login.py
--rw-r--r--   0 turam      (501) staff       (20)     4781 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/cmdline/scheduler.py
--rw-r--r--   0 turam      (501) staff       (20)     5292 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/cmdline/server.py
--rw-r--r--   0 turam      (501) staff       (20)     7128 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/cmdline/site.py
--rw-r--r--   0 turam      (501) staff       (20)     8490 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/cmdline/utils.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.405241 balsam-0.7.0a21/balsam/config/
--rw-r--r--   0 turam      (501) staff       (20)      177 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)    17080 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/config.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.405784 balsam-0.7.0a21/balsam/config/defaults/
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.406325 balsam-0.7.0a21/balsam/config/defaults/alcf_cooley/
--rw-r--r--   0 turam      (501) staff       (20)      721 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/alcf_cooley/job-template.sh
--rw-r--r--   0 turam      (501) staff       (20)      667 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/alcf_cooley/settings.yml
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.406816 balsam-0.7.0a21/balsam/config/defaults/alcf_polaris/
--rw-r--r--   0 turam      (501) staff       (20)      672 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/alcf_polaris/job-template.sh
--rw-r--r--   0 turam      (501) staff       (20)      753 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/alcf_polaris/settings.yml
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.407347 balsam-0.7.0a21/balsam/config/defaults/alcf_sunspot/
--rw-r--r--   0 turam      (501) staff       (20)      740 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/alcf_sunspot/job-template.sh
--rw-r--r--   0 turam      (501) staff       (20)      506 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/alcf_sunspot/settings.yml
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.407947 balsam-0.7.0a21/balsam/config/defaults/alcf_theta/
--rw-r--r--   0 turam      (501) staff       (20)      937 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/alcf_theta/job-template.sh
--rw-r--r--   0 turam      (501) staff       (20)      896 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/alcf_theta/settings.yml
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.408426 balsam-0.7.0a21/balsam/config/defaults/alcf_thetagpu/
--rw-r--r--   0 turam      (501) staff       (20)     1623 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/alcf_thetagpu/job-template.sh
--rw-r--r--   0 turam      (501) staff       (20)      766 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/alcf_thetagpu/settings.yml
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.408923 balsam-0.7.0a21/balsam/config/defaults/nersc_corihaswell/
--rw-r--r--   0 turam      (501) staff       (20)      597 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/nersc_corihaswell/job-template.sh
--rw-r--r--   0 turam      (501) staff       (20)      852 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/nersc_corihaswell/settings.yml
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.409593 balsam-0.7.0a21/balsam/config/defaults/nersc_coriknl/
--rw-r--r--   0 turam      (501) staff       (20)      481 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/nersc_coriknl/job-template.sh
--rw-r--r--   0 turam      (501) staff       (20)      829 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/nersc_coriknl/settings.yml
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.410138 balsam-0.7.0a21/balsam/config/defaults/nersc_perlmutter/
--rw-r--r--   0 turam      (501) staff       (20)      593 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/nersc_perlmutter/job-template.sh
--rw-r--r--   0 turam      (501) staff       (20)      852 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/nersc_perlmutter/settings.yml
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.410694 balsam-0.7.0a21/balsam/config/defaults/olcf_summit/
--rw-r--r--   0 turam      (501) staff       (20)      733 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/olcf_summit/job-template.sh
--rw-r--r--   0 turam      (501) staff       (20)      800 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/olcf_summit/settings.yml
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.411196 balsam-0.7.0a21/balsam/config/defaults/osx/
--rw-r--r--   0 turam      (501) staff       (20)      858 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/osx/job-template.sh
--rw-r--r--   0 turam      (501) staff       (20)      691 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/osx/settings.yml
--rw-r--r--   0 turam      (501) staff       (20)     6198 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/settings.yml.j2
--rw-r--r--   0 turam      (501) staff       (20)      609 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/defaults/validate.py
--rw-r--r--   0 turam      (501) staff       (20)     4045 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/config/site_builder.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.411420 balsam-0.7.0a21/balsam/platform/
--rw-r--r--   0 turam      (501) staff       (20)       74 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/__init__.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.414245 balsam-0.7.0a21/balsam/platform/app_run/
--rw-r--r--   0 turam      (501) staff       (20)      545 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/app_run/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     6429 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/app_run/app_run.py
--rw-r--r--   0 turam      (501) staff       (20)      727 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/app_run/mpich.py
--rw-r--r--   0 turam      (501) staff       (20)      701 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/app_run/openmpi.py
--rw-r--r--   0 turam      (501) staff       (20)     1168 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/app_run/perlmutter.py
--rw-r--r--   0 turam      (501) staff       (20)      735 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/app_run/polaris.py
--rw-r--r--   0 turam      (501) staff       (20)      754 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/app_run/slurm.py
--rw-r--r--   0 turam      (501) staff       (20)     1213 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/app_run/summit.py
--rw-r--r--   0 turam      (501) staff       (20)     1273 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/app_run/sunspot.py
--rw-r--r--   0 turam      (501) staff       (20)      973 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/app_run/theta.py
--rw-r--r--   0 turam      (501) staff       (20)      865 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/app_run/theta_gpu.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.417400 balsam-0.7.0a21/balsam/platform/compute_node/
--rw-r--r--   0 turam      (501) staff       (20)      702 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/compute_node/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)      933 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/platform/compute_node/alcf_cooley_node.py
--rw-r--r--   0 turam      (501) staff       (20)     1897 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/platform/compute_node/alcf_polaris_node.py
--rw-r--r--   0 turam      (501) staff       (20)     1675 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/platform/compute_node/alcf_sunspot_node.py
--rw-r--r--   0 turam      (501) staff       (20)     1970 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/platform/compute_node/alcf_thetagpu_node.py
--rw-r--r--   0 turam      (501) staff       (20)     1100 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/platform/compute_node/alcf_thetaknl_node.py
--rw-r--r--   0 turam      (501) staff       (20)     3481 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/platform/compute_node/compute_node.py
--rw-r--r--   0 turam      (501) staff       (20)      978 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/platform/compute_node/default.py
--rw-r--r--   0 turam      (501) staff       (20)     1751 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/platform/compute_node/nersc_corihas_node.py
--rw-r--r--   0 turam      (501) staff       (20)     1578 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/platform/compute_node/nersc_coriknl_node.py
--rw-r--r--   0 turam      (501) staff       (20)     1769 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/platform/compute_node/nersc_perlmutter_gpu.py
--rw-r--r--   0 turam      (501) staff       (20)      975 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/platform/compute_node/summit_node.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.419183 balsam-0.7.0a21/balsam/platform/scheduler/
--rw-r--r--   0 turam      (501) staff       (20)      617 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/scheduler/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)    11606 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/scheduler/cobalt_sched.py
--rw-r--r--   0 turam      (501) staff       (20)     4142 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/scheduler/local.py
--rw-r--r--   0 turam      (501) staff       (20)     8917 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/scheduler/lsf_sched.py
--rw-r--r--   0 turam      (501) staff       (20)    14063 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/scheduler/pbs_sched.py
--rw-r--r--   0 turam      (501) staff       (20)     6090 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/scheduler/scheduler.py
--rw-r--r--   0 turam      (501) staff       (20)    11722 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/scheduler/slurm_sched.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.419904 balsam-0.7.0a21/balsam/platform/transfer/
--rw-r--r--   0 turam      (501) staff       (20)      292 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/transfer/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     6185 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/transfer/globus_transfer.py
--rw-r--r--   0 turam      (501) staff       (20)     1439 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/platform/transfer/transfer.py
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/py.typed
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/querytest.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.422983 balsam-0.7.0a21/balsam/schemas/
--rw-r--r--   0 turam      (501) staff       (20)     2629 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/schemas/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)    15400 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/schemas/api_generator.py
--rw-r--r--   0 turam      (501) staff       (20)     3377 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/schemas/apps.py
--rw-r--r--   0 turam      (501) staff       (20)     3928 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/schemas/batchjob.py
--rw-r--r--   0 turam      (501) staff       (20)     9284 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/schemas/job.py
--rw-r--r--   0 turam      (501) staff       (20)      615 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/schemas/logevent.py
--rw-r--r--   0 turam      (501) staff       (20)     2107 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/schemas/serializer.py
--rw-r--r--   0 turam      (501) staff       (20)     1418 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/schemas/session.py
--rw-r--r--   0 turam      (501) staff       (20)     3836 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/schemas/site.py
--rw-r--r--   0 turam      (501) staff       (20)     1966 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/schemas/transfer.py
--rw-r--r--   0 turam      (501) staff       (20)      156 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/schemas/user.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.424804 balsam-0.7.0a21/balsam/server/
--rw-r--r--   0 turam      (501) staff       (20)      335 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/__init__.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.426490 balsam-0.7.0a21/balsam/server/auth/
--rw-r--r--   0 turam      (501) staff       (20)     1227 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/auth/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     6381 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/auth/authorization_code_login.py
--rw-r--r--   0 turam      (501) staff       (20)     1146 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/auth/db_sessions.py
--rw-r--r--   0 turam      (501) staff       (20)     4696 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/auth/device_code_login.py
--rw-r--r--   0 turam      (501) staff       (20)     2137 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/auth/password_login.py
--rw-r--r--   0 turam      (501) staff       (20)      288 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/auth/password_utils.py
--rw-r--r--   0 turam      (501) staff       (20)     1832 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/auth/token.py
--rw-r--r--   0 turam      (501) staff       (20)     3201 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/conf.py
--rw-r--r--   0 turam      (501) staff       (20)      703 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/gunicorn.conf.example.py
--rw-r--r--   0 turam      (501) staff       (20)      703 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/gunicorn.conf.py
--rw-r--r--   0 turam      (501) staff       (20)     1307 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/gunicorn_logger.py
--rw-r--r--   0 turam      (501) staff       (20)     2852 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/main.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.427255 balsam-0.7.0a21/balsam/server/models/
--rw-r--r--   0 turam      (501) staff       (20)      345 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/models/__init__.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.427667 balsam-0.7.0a21/balsam/server/models/alembic/
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/models/alembic/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)      501 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/models/alembic/env.py
--rw-r--r--   0 turam      (501) staff       (20)     1013 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/models/base.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.429703 balsam-0.7.0a21/balsam/server/models/crud/
--rw-r--r--   0 turam      (501) staff       (20)      210 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/models/crud/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     2607 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/models/crud/apps.py
--rw-r--r--   0 turam      (501) staff       (20)     3794 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/models/crud/batch_jobs.py
--rw-r--r--   0 turam      (501) staff       (20)      723 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/models/crud/events.py
--rw-r--r--   0 turam      (501) staff       (20)    15568 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/models/crud/jobs.py
--rw-r--r--   0 turam      (501) staff       (20)     8288 2023-02-06 23:04:00.000000 balsam-0.7.0a21/balsam/server/models/crud/sessions.py
--rw-r--r--   0 turam      (501) staff       (20)     2109 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/models/crud/sites.py
--rw-r--r--   0 turam      (501) staff       (20)     3517 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/models/crud/transfers.py
--rw-r--r--   0 turam      (501) staff       (20)     3471 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/models/crud/users.py
--rw-r--r--   0 turam      (501) staff       (20)     8618 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/models/tables.py
--rw-r--r--   0 turam      (501) staff       (20)     1635 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/pubsub.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.431993 balsam-0.7.0a21/balsam/server/routers/
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/routers/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     2620 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/routers/apps.py
--rw-r--r--   0 turam      (501) staff       (20)     3355 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/routers/batch_jobs.py
--rw-r--r--   0 turam      (501) staff       (20)      849 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/routers/events.py
--rw-r--r--   0 turam      (501) staff       (20)    13164 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/routers/filters.py
--rw-r--r--   0 turam      (501) staff       (20)     4723 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/routers/jobs.py
--rw-r--r--   0 turam      (501) staff       (20)     2481 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/routers/sessions.py
--rw-r--r--   0 turam      (501) staff       (20)     2737 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/routers/sites.py
--rw-r--r--   0 turam      (501) staff       (20)     2364 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/routers/transfers.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.433101 balsam-0.7.0a21/balsam/server/utils/
--rw-r--r--   0 turam      (501) staff       (20)      162 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/utils/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     1237 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/utils/log.py
--rw-r--r--   0 turam      (501) staff       (20)     1222 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/utils/paginator.py
--rw-r--r--   0 turam      (501) staff       (20)     1798 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/utils/timer.py
--rw-r--r--   0 turam      (501) staff       (20)     1317 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/server/utils/user_tools.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.433324 balsam-0.7.0a21/balsam/shared_apps/
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/shared_apps/__init__.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.433680 balsam-0.7.0a21/balsam/shared_apps/alcf_cooley/
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/shared_apps/alcf_cooley/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     2184 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/shared_apps/alcf_cooley/parsl.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.434079 balsam-0.7.0a21/balsam/shared_apps/alcf_theta/
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/shared_apps/alcf_theta/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     1276 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/shared_apps/alcf_theta/xpcs.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.434795 balsam-0.7.0a21/balsam/shared_apps/demo/
--rw-r--r--   0 turam      (501) staff       (20)       80 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/shared_apps/demo/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)      176 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/shared_apps/demo/adder.py
--rw-r--r--   0 turam      (501) staff       (20)      143 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/shared_apps/demo/hello.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.435204 balsam-0.7.0a21/balsam/shared_apps/olcf_summit/
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/shared_apps/olcf_summit/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     1358 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/shared_apps/olcf_summit/xpcs.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.436172 balsam-0.7.0a21/balsam/site/
--rw-r--r--   0 turam      (501) staff       (20)      273 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     9323 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/job_source.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.438482 balsam-0.7.0a21/balsam/site/launcher/
--rw-r--r--   0 turam      (501) staff       (20)       59 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/launcher/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)    11131 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/launcher/_mpi_mode.py
--rw-r--r--   0 turam      (501) staff       (20)     9553 2023-02-06 23:24:19.000000 balsam-0.7.0a21/balsam/site/launcher/_serial_mode_master.py
--rw-r--r--   0 turam      (501) staff       (20)     9934 2023-02-06 23:24:06.000000 balsam-0.7.0a21/balsam/site/launcher/_serial_mode_worker.py
--rw-r--r--   0 turam      (501) staff       (20)      168 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/launcher/mpi_mode.py
--rw-r--r--   0 turam      (501) staff       (20)     4639 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/launcher/node_manager.py
--rw-r--r--   0 turam      (501) staff       (20)     2943 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/launcher/python_runner.py
--rw-r--r--   0 turam      (501) staff       (20)     1106 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/launcher/serial_mode.py
--rw-r--r--   0 turam      (501) staff       (20)      684 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/launcher/util.py
--rw-r--r--   0 turam      (501) staff       (20)     2341 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/script_template.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.442031 balsam-0.7.0a21/balsam/site/service/
--rw-r--r--   0 turam      (501) staff       (20)      435 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/service/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     7132 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/service/elastic_queue.py
--rw-r--r--   0 turam      (501) staff       (20)     3102 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/service/file_cleaner.py
--rw-r--r--   0 turam      (501) staff       (20)     2796 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/service/main.py
--rw-r--r--   0 turam      (501) staff       (20)     7643 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/service/processing.py
--rw-r--r--   0 turam      (501) staff       (20)     2143 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/service/queue_maintainer.py
--rw-r--r--   0 turam      (501) staff       (20)     7467 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/service/scheduler.py
--rw-r--r--   0 turam      (501) staff       (20)      953 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/service/service_base.py
--rw-r--r--   0 turam      (501) staff       (20)     8358 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/service/transfer.py
--rw-r--r--   0 turam      (501) staff       (20)     3413 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/status_updater.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.442712 balsam-0.7.0a21/balsam/site/util/
--rw-r--r--   0 turam      (501) staff       (20)       49 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/util/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     3142 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/site/util/mp_queue.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.444498 balsam-0.7.0a21/balsam/util/
--rw-r--r--   0 turam      (501) staff       (20)      350 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/util/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)    12040 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/util/globus_auth.py
--rw-r--r--   0 turam      (501) staff       (20)     4910 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/util/log.py
--rw-r--r--   0 turam      (501) staff       (20)    12046 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/util/postgres.py
--rw-r--r--   0 turam      (501) staff       (20)      719 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/util/process.py
--rw-r--r--   0 turam      (501) staff       (20)     1032 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/util/sighandler.py
--rw-r--r--   0 turam      (501) staff       (20)      833 2023-02-06 22:51:07.000000 balsam-0.7.0a21/balsam/util/time_parser.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.398210 balsam-0.7.0a21/balsam.egg-info/
--rw-r--r--   0 turam      (501) staff       (20)      813 2023-02-06 23:35:30.000000 balsam-0.7.0a21/balsam.egg-info/PKG-INFO
--rw-r--r--   0 turam      (501) staff       (20)     7307 2023-02-06 23:35:30.000000 balsam-0.7.0a21/balsam.egg-info/SOURCES.txt
--rw-r--r--   0 turam      (501) staff       (20)        1 2023-02-06 23:35:30.000000 balsam-0.7.0a21/balsam.egg-info/dependency_links.txt
--rw-r--r--   0 turam      (501) staff       (20)       47 2023-02-06 23:35:30.000000 balsam-0.7.0a21/balsam.egg-info/entry_points.txt
--rw-r--r--   0 turam      (501) staff       (20)      331 2023-02-06 23:35:30.000000 balsam-0.7.0a21/balsam.egg-info/requires.txt
--rw-r--r--   0 turam      (501) staff       (20)       13 2023-02-06 23:35:30.000000 balsam-0.7.0a21/balsam.egg-info/top_level.txt
--rw-r--r--   0 turam      (501) staff       (20)      173 2023-02-06 22:51:07.000000 balsam-0.7.0a21/pyproject.toml
--rw-r--r--   0 turam      (501) staff       (20)     2531 2023-02-06 23:35:30.451950 balsam-0.7.0a21/setup.cfg
--rw-r--r--   0 turam      (501) staff       (20)     1634 2023-02-06 22:51:07.000000 balsam-0.7.0a21/setup.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.394986 balsam-0.7.0a21/tests/
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.445110 balsam-0.7.0a21/tests/api/
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/api/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/api/conftest.py
--rw-r--r--   0 turam      (501) staff       (20)    41857 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/api/test_api.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.447561 balsam-0.7.0a21/tests/benchmark/
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/benchmark/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     3366 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/benchmark/batch_simulation.py
--rw-r--r--   0 turam      (501) staff       (20)     3486 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/benchmark/batch_simulation_cori.py
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/benchmark/conftest.py
--rw-r--r--   0 turam      (501) staff       (20)     4083 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/benchmark/eig_backlog.py
--rw-r--r--   0 turam      (501) staff       (20)     4336 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/benchmark/eig_scaling.py
--rw-r--r--   0 turam      (501) staff       (20)     8614 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/benchmark/job_producer.py
--rw-r--r--   0 turam      (501) staff       (20)    10085 2023-02-06 23:04:00.000000 balsam-0.7.0a21/tests/benchmark/locustfile.py
--rw-r--r--   0 turam      (501) staff       (20)     2954 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/benchmark/populate_eig.py
--rw-r--r--   0 turam      (501) staff       (20)      382 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/benchmark/random-eig.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.449613 balsam-0.7.0a21/tests/server/
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/server/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)     1646 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/server/conftest.py
--rw-r--r--   0 turam      (501) staff       (20)     2778 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/server/test_apps.py
--rw-r--r--   0 turam      (501) staff       (20)      609 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/server/test_auth.py
--rw-r--r--   0 turam      (501) staff       (20)    11869 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/server/test_batchjobs.py
--rw-r--r--   0 turam      (501) staff       (20)    41008 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/server/test_jobs.py
--rw-r--r--   0 turam      (501) staff       (20)     2350 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/server/test_sites.py
--rw-r--r--   0 turam      (501) staff       (20)     3749 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/server/util.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.450180 balsam-0.7.0a21/tests/site_integration/
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/site_integration/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/site_integration/conftest.py
--rw-r--r--   0 turam      (501) staff       (20)     6149 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/site_integration/test_integration.py
-drwxr-xr-x   0 turam      (501) staff       (20)        0 2023-02-06 23:35:30.451002 balsam-0.7.0a21/tests/units/
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/units/__init__.py
--rw-r--r--   0 turam      (501) staff       (20)        0 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/units/conftest.py
--rw-r--r--   0 turam      (501) staff       (20)     2153 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/units/test_mpi_launcher.py
--rw-r--r--   0 turam      (501) staff       (20)       31 2023-02-06 22:51:07.000000 balsam-0.7.0a21/tests/units/test_scheduler.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/
+-rw-r--r--   0 turam     (2517) users      (100)      813 2023-04-10 20:36:58.000000 balsam-0.7.0a22/PKG-INFO
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/
+-rw-r--r--   0 turam     (2517) users      (100)       91 2023-04-10 20:33:59.000000 balsam-0.7.0a22/balsam/__init__.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/_api/
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/_api/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)    17893 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/_api/app.py
+-rw-r--r--   0 turam     (2517) users      (100)    15182 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/_api/bases.py
+-rw-r--r--   0 turam     (2517) users      (100)    10519 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/_api/manager.py
+-rw-r--r--   0 turam     (2517) users      (100)     7943 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/_api/model.py
+-rw-r--r--   0 turam     (2517) users      (100)    68189 2023-04-10 20:29:37.000000 balsam-0.7.0a22/balsam/_api/models.py
+-rw-r--r--   0 turam     (2517) users      (100)     6273 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/_api/query.py
+-rw-r--r--   0 turam     (2517) users      (100)     1862 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/analytics.py
+-rw-r--r--   0 turam     (2517) users      (100)     1523 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/api.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/client/
+-rw-r--r--   0 turam     (2517) users      (100)      404 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/client/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     5307 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/client/encoders.py
+-rw-r--r--   0 turam     (2517) users      (100)     5306 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/client/requests_client.py
+-rw-r--r--   0 turam     (2517) users      (100)     4132 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/client/requests_oauth.py
+-rw-r--r--   0 turam     (2517) users      (100)     3025 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/client/requests_password.py
+-rw-r--r--   0 turam     (2517) users      (100)     3515 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/client/rest_base_client.py
+-rw-r--r--   0 turam     (2517) users      (100)      185 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/client/urls.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/cmdline/
+-rw-r--r--   0 turam     (2517) users      (100)     1655 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/cmdline/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     5820 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/cmdline/_launcher.py
+-rw-r--r--   0 turam     (2517) users      (100)     2022 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/cmdline/app.py
+-rw-r--r--   0 turam     (2517) users      (100)    12179 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/cmdline/job.py
+-rw-r--r--   0 turam     (2517) users      (100)       89 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/cmdline/launcher.py
+-rw-r--r--   0 turam     (2517) users      (100)     2175 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/cmdline/login.py
+-rw-r--r--   0 turam     (2517) users      (100)     4781 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/cmdline/scheduler.py
+-rw-r--r--   0 turam     (2517) users      (100)     5292 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/cmdline/server.py
+-rw-r--r--   0 turam     (2517) users      (100)     7128 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/cmdline/site.py
+-rw-r--r--   0 turam     (2517) users      (100)     8490 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/cmdline/utils.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/config/
+-rw-r--r--   0 turam     (2517) users      (100)      177 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)    17080 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/config.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/config/defaults/
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_cooley/
+-rw-r--r--   0 turam     (2517) users      (100)      721 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_cooley/job-template.sh
+-rw-r--r--   0 turam     (2517) users      (100)      667 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_cooley/settings.yml
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_polaris/
+-rw-r--r--   0 turam     (2517) users      (100)      672 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_polaris/job-template.sh
+-rw-r--r--   0 turam     (2517) users      (100)      847 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_polaris/settings.yml
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_sunspot/
+-rw-r--r--   0 turam     (2517) users      (100)      740 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_sunspot/job-template.sh
+-rw-r--r--   0 turam     (2517) users      (100)      506 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_sunspot/settings.yml
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_theta/
+-rw-r--r--   0 turam     (2517) users      (100)      937 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_theta/job-template.sh
+-rw-r--r--   0 turam     (2517) users      (100)      896 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_theta/settings.yml
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_thetagpu/
+-rw-r--r--   0 turam     (2517) users      (100)     1623 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_thetagpu/job-template.sh
+-rw-r--r--   0 turam     (2517) users      (100)      766 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/alcf_thetagpu/settings.yml
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/config/defaults/nersc_corihaswell/
+-rw-r--r--   0 turam     (2517) users      (100)      597 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/nersc_corihaswell/job-template.sh
+-rw-r--r--   0 turam     (2517) users      (100)      852 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/nersc_corihaswell/settings.yml
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/config/defaults/nersc_coriknl/
+-rw-r--r--   0 turam     (2517) users      (100)      481 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/nersc_coriknl/job-template.sh
+-rw-r--r--   0 turam     (2517) users      (100)      829 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/nersc_coriknl/settings.yml
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/config/defaults/nersc_perlmuttercpu/
+-rw-r--r--   0 turam     (2517) users      (100)      593 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/nersc_perlmuttercpu/job-template.sh
+-rw-r--r--   0 turam     (2517) users      (100)      750 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/nersc_perlmuttercpu/settings.yml
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/config/defaults/nersc_perlmuttergpu/
+-rw-r--r--   0 turam     (2517) users      (100)      593 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/nersc_perlmuttergpu/job-template.sh
+-rw-r--r--   0 turam     (2517) users      (100)      750 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/nersc_perlmuttergpu/settings.yml
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/config/defaults/olcf_summit/
+-rw-r--r--   0 turam     (2517) users      (100)      733 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/olcf_summit/job-template.sh
+-rw-r--r--   0 turam     (2517) users      (100)      800 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/olcf_summit/settings.yml
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/config/defaults/osx/
+-rw-r--r--   0 turam     (2517) users      (100)      858 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/osx/job-template.sh
+-rw-r--r--   0 turam     (2517) users      (100)      691 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/osx/settings.yml
+-rw-r--r--   0 turam     (2517) users      (100)     6268 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/settings.yml.j2
+-rw-r--r--   0 turam     (2517) users      (100)      609 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/defaults/validate.py
+-rw-r--r--   0 turam     (2517) users      (100)     4045 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/config/site_builder.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/platform/
+-rw-r--r--   0 turam     (2517) users      (100)       74 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/__init__.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/platform/app_run/
+-rw-r--r--   0 turam     (2517) users      (100)      539 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/app_run/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     6429 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/app_run/app_run.py
+-rw-r--r--   0 turam     (2517) users      (100)      727 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/app_run/mpich.py
+-rw-r--r--   0 turam     (2517) users      (100)      701 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/app_run/openmpi.py
+-rw-r--r--   0 turam     (2517) users      (100)     1344 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/app_run/perlmutter.py
+-rw-r--r--   0 turam     (2517) users      (100)      735 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/app_run/polaris.py
+-rw-r--r--   0 turam     (2517) users      (100)      754 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/app_run/slurm.py
+-rw-r--r--   0 turam     (2517) users      (100)     1213 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/app_run/summit.py
+-rw-r--r--   0 turam     (2517) users      (100)     1273 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/app_run/sunspot.py
+-rw-r--r--   0 turam     (2517) users      (100)      973 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/app_run/theta.py
+-rw-r--r--   0 turam     (2517) users      (100)      865 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/app_run/theta_gpu.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/platform/compute_node/
+-rw-r--r--   0 turam     (2517) users      (100)      692 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/compute_node/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)      933 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/compute_node/alcf_cooley_node.py
+-rw-r--r--   0 turam     (2517) users      (100)     1897 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/compute_node/alcf_polaris_node.py
+-rw-r--r--   0 turam     (2517) users      (100)     1675 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/compute_node/alcf_sunspot_node.py
+-rw-r--r--   0 turam     (2517) users      (100)     1970 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/compute_node/alcf_thetagpu_node.py
+-rw-r--r--   0 turam     (2517) users      (100)     1100 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/compute_node/alcf_thetaknl_node.py
+-rw-r--r--   0 turam     (2517) users      (100)     3481 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/compute_node/compute_node.py
+-rw-r--r--   0 turam     (2517) users      (100)      978 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/compute_node/default.py
+-rw-r--r--   0 turam     (2517) users      (100)     1751 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/compute_node/nersc_corihas_node.py
+-rw-r--r--   0 turam     (2517) users      (100)     1578 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/compute_node/nersc_coriknl_node.py
+-rw-r--r--   0 turam     (2517) users      (100)     1760 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/compute_node/nersc_perlmutter.py
+-rw-r--r--   0 turam     (2517) users      (100)      975 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/compute_node/summit_node.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/platform/scheduler/
+-rw-r--r--   0 turam     (2517) users      (100)      617 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/scheduler/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)    11606 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/scheduler/cobalt_sched.py
+-rw-r--r--   0 turam     (2517) users      (100)     4142 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/scheduler/local.py
+-rw-r--r--   0 turam     (2517) users      (100)     8917 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/scheduler/lsf_sched.py
+-rw-r--r--   0 turam     (2517) users      (100)    14722 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/scheduler/pbs_sched.py
+-rw-r--r--   0 turam     (2517) users      (100)     6090 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/scheduler/scheduler.py
+-rw-r--r--   0 turam     (2517) users      (100)    11722 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/scheduler/slurm_sched.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/platform/transfer/
+-rw-r--r--   0 turam     (2517) users      (100)      292 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/transfer/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     6185 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/transfer/globus_transfer.py
+-rw-r--r--   0 turam     (2517) users      (100)     1439 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/platform/transfer/transfer.py
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/py.typed
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/querytest.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/schemas/
+-rw-r--r--   0 turam     (2517) users      (100)     2629 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/schemas/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)    15400 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/schemas/api_generator.py
+-rw-r--r--   0 turam     (2517) users      (100)     3377 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/schemas/apps.py
+-rw-r--r--   0 turam     (2517) users      (100)     3928 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/schemas/batchjob.py
+-rw-r--r--   0 turam     (2517) users      (100)     9284 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/schemas/job.py
+-rw-r--r--   0 turam     (2517) users      (100)      615 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/schemas/logevent.py
+-rw-r--r--   0 turam     (2517) users      (100)     2107 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/schemas/serializer.py
+-rw-r--r--   0 turam     (2517) users      (100)     1418 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/schemas/session.py
+-rw-r--r--   0 turam     (2517) users      (100)     3836 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/schemas/site.py
+-rw-r--r--   0 turam     (2517) users      (100)     1966 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/schemas/transfer.py
+-rw-r--r--   0 turam     (2517) users      (100)      156 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/schemas/user.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/server/
+-rw-r--r--   0 turam     (2517) users      (100)      335 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/__init__.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/server/auth/
+-rw-r--r--   0 turam     (2517) users      (100)     1227 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/auth/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     6381 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/auth/authorization_code_login.py
+-rw-r--r--   0 turam     (2517) users      (100)     1146 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/auth/db_sessions.py
+-rw-r--r--   0 turam     (2517) users      (100)     4696 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/auth/device_code_login.py
+-rw-r--r--   0 turam     (2517) users      (100)     2137 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/auth/password_login.py
+-rw-r--r--   0 turam     (2517) users      (100)      288 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/auth/password_utils.py
+-rw-r--r--   0 turam     (2517) users      (100)     1832 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/auth/token.py
+-rw-r--r--   0 turam     (2517) users      (100)     3201 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/conf.py
+-rw-r--r--   0 turam     (2517) users      (100)      703 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/gunicorn.conf.example.py
+-rw-r--r--   0 turam     (2517) users      (100)      703 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/gunicorn.conf.py
+-rw-r--r--   0 turam     (2517) users      (100)     1307 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/gunicorn_logger.py
+-rw-r--r--   0 turam     (2517) users      (100)     2852 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/main.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/server/models/
+-rw-r--r--   0 turam     (2517) users      (100)      345 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/models/__init__.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/server/models/alembic/
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/models/alembic/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)      501 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/models/alembic/env.py
+-rw-r--r--   0 turam     (2517) users      (100)     1013 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/models/base.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/server/models/crud/
+-rw-r--r--   0 turam     (2517) users      (100)      210 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/models/crud/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     2607 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/models/crud/apps.py
+-rw-r--r--   0 turam     (2517) users      (100)     3794 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/models/crud/batch_jobs.py
+-rw-r--r--   0 turam     (2517) users      (100)      723 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/models/crud/events.py
+-rw-r--r--   0 turam     (2517) users      (100)    15568 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/models/crud/jobs.py
+-rw-r--r--   0 turam     (2517) users      (100)     8288 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/models/crud/sessions.py
+-rw-r--r--   0 turam     (2517) users      (100)     2109 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/models/crud/sites.py
+-rw-r--r--   0 turam     (2517) users      (100)     3517 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/models/crud/transfers.py
+-rw-r--r--   0 turam     (2517) users      (100)     3471 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/models/crud/users.py
+-rw-r--r--   0 turam     (2517) users      (100)     8618 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/models/tables.py
+-rw-r--r--   0 turam     (2517) users      (100)     1635 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/pubsub.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/server/routers/
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/routers/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     2620 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/routers/apps.py
+-rw-r--r--   0 turam     (2517) users      (100)     3355 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/routers/batch_jobs.py
+-rw-r--r--   0 turam     (2517) users      (100)      849 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/routers/events.py
+-rw-r--r--   0 turam     (2517) users      (100)    13164 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/routers/filters.py
+-rw-r--r--   0 turam     (2517) users      (100)     4723 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/routers/jobs.py
+-rw-r--r--   0 turam     (2517) users      (100)     2481 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/routers/sessions.py
+-rw-r--r--   0 turam     (2517) users      (100)     2737 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/routers/sites.py
+-rw-r--r--   0 turam     (2517) users      (100)     2364 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/routers/transfers.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/server/utils/
+-rw-r--r--   0 turam     (2517) users      (100)      162 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/utils/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     1237 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/utils/log.py
+-rw-r--r--   0 turam     (2517) users      (100)     1222 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/utils/paginator.py
+-rw-r--r--   0 turam     (2517) users      (100)     1798 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/utils/timer.py
+-rw-r--r--   0 turam     (2517) users      (100)     1317 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/server/utils/user_tools.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/shared_apps/
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/shared_apps/__init__.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/shared_apps/alcf_cooley/
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/shared_apps/alcf_cooley/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     2184 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/shared_apps/alcf_cooley/parsl.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/shared_apps/alcf_theta/
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/shared_apps/alcf_theta/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     1276 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/shared_apps/alcf_theta/xpcs.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/shared_apps/demo/
+-rw-r--r--   0 turam     (2517) users      (100)       80 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/shared_apps/demo/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)      176 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/shared_apps/demo/adder.py
+-rw-r--r--   0 turam     (2517) users      (100)      143 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/shared_apps/demo/hello.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/shared_apps/olcf_summit/
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/shared_apps/olcf_summit/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     1358 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/shared_apps/olcf_summit/xpcs.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/site/
+-rw-r--r--   0 turam     (2517) users      (100)      273 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     9323 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/job_source.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/site/launcher/
+-rw-r--r--   0 turam     (2517) users      (100)       59 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/launcher/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)    11131 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/launcher/_mpi_mode.py
+-rw-r--r--   0 turam     (2517) users      (100)     9553 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/launcher/_serial_mode_master.py
+-rw-r--r--   0 turam     (2517) users      (100)     9934 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/launcher/_serial_mode_worker.py
+-rw-r--r--   0 turam     (2517) users      (100)      168 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/launcher/mpi_mode.py
+-rw-r--r--   0 turam     (2517) users      (100)     4639 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/launcher/node_manager.py
+-rw-r--r--   0 turam     (2517) users      (100)     2943 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/launcher/python_runner.py
+-rw-r--r--   0 turam     (2517) users      (100)     1106 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/launcher/serial_mode.py
+-rw-r--r--   0 turam     (2517) users      (100)      684 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/launcher/util.py
+-rw-r--r--   0 turam     (2517) users      (100)     2341 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/script_template.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/site/service/
+-rw-r--r--   0 turam     (2517) users      (100)      435 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/service/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     7132 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/service/elastic_queue.py
+-rw-r--r--   0 turam     (2517) users      (100)     3102 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/service/file_cleaner.py
+-rw-r--r--   0 turam     (2517) users      (100)     2796 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/service/main.py
+-rw-r--r--   0 turam     (2517) users      (100)     7643 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/service/processing.py
+-rw-r--r--   0 turam     (2517) users      (100)     2143 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/service/queue_maintainer.py
+-rw-r--r--   0 turam     (2517) users      (100)     7467 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/service/scheduler.py
+-rw-r--r--   0 turam     (2517) users      (100)      953 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/service/service_base.py
+-rw-r--r--   0 turam     (2517) users      (100)     8358 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/service/transfer.py
+-rw-r--r--   0 turam     (2517) users      (100)     3413 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/status_updater.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/site/util/
+-rw-r--r--   0 turam     (2517) users      (100)       49 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/util/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     3142 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/site/util/mp_queue.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam/util/
+-rw-r--r--   0 turam     (2517) users      (100)      350 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/util/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)    12040 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/util/globus_auth.py
+-rw-r--r--   0 turam     (2517) users      (100)     4910 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/util/log.py
+-rw-r--r--   0 turam     (2517) users      (100)    12046 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/util/postgres.py
+-rw-r--r--   0 turam     (2517) users      (100)      719 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/util/process.py
+-rw-r--r--   0 turam     (2517) users      (100)     1032 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/util/sighandler.py
+-rw-r--r--   0 turam     (2517) users      (100)      833 2023-04-10 20:29:11.000000 balsam-0.7.0a22/balsam/util/time_parser.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam.egg-info/
+-rw-r--r--   0 turam     (2517) users      (100)      813 2023-04-10 20:36:57.000000 balsam-0.7.0a22/balsam.egg-info/PKG-INFO
+-rw-r--r--   0 turam     (2517) users      (100)     7447 2023-04-10 20:36:58.000000 balsam-0.7.0a22/balsam.egg-info/SOURCES.txt
+-rw-r--r--   0 turam     (2517) users      (100)        1 2023-04-10 20:36:57.000000 balsam-0.7.0a22/balsam.egg-info/dependency_links.txt
+-rw-r--r--   0 turam     (2517) users      (100)       47 2023-04-10 20:36:57.000000 balsam-0.7.0a22/balsam.egg-info/entry_points.txt
+-rw-r--r--   0 turam     (2517) users      (100)      331 2023-04-10 20:36:57.000000 balsam-0.7.0a22/balsam.egg-info/requires.txt
+-rw-r--r--   0 turam     (2517) users      (100)       13 2023-04-10 20:36:57.000000 balsam-0.7.0a22/balsam.egg-info/top_level.txt
+-rw-r--r--   0 turam     (2517) users      (100)      173 2023-04-10 20:29:11.000000 balsam-0.7.0a22/pyproject.toml
+-rw-r--r--   0 turam     (2517) users      (100)     2531 2023-04-10 20:36:58.000000 balsam-0.7.0a22/setup.cfg
+-rw-r--r--   0 turam     (2517) users      (100)     1634 2023-04-10 20:29:11.000000 balsam-0.7.0a22/setup.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/tests/
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/tests/api/
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:11.000000 balsam-0.7.0a22/tests/api/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:11.000000 balsam-0.7.0a22/tests/api/conftest.py
+-rw-r--r--   0 turam     (2517) users      (100)    41857 2023-04-10 20:29:11.000000 balsam-0.7.0a22/tests/api/test_api.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/tests/benchmark/
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:11.000000 balsam-0.7.0a22/tests/benchmark/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     3366 2023-04-10 20:29:11.000000 balsam-0.7.0a22/tests/benchmark/batch_simulation.py
+-rw-r--r--   0 turam     (2517) users      (100)     3486 2023-04-10 20:29:11.000000 balsam-0.7.0a22/tests/benchmark/batch_simulation_cori.py
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:11.000000 balsam-0.7.0a22/tests/benchmark/conftest.py
+-rw-r--r--   0 turam     (2517) users      (100)     4083 2023-04-10 20:29:11.000000 balsam-0.7.0a22/tests/benchmark/eig_backlog.py
+-rw-r--r--   0 turam     (2517) users      (100)     4336 2023-04-10 20:29:11.000000 balsam-0.7.0a22/tests/benchmark/eig_scaling.py
+-rw-r--r--   0 turam     (2517) users      (100)     8614 2023-04-10 20:29:11.000000 balsam-0.7.0a22/tests/benchmark/job_producer.py
+-rw-r--r--   0 turam     (2517) users      (100)    10085 2023-04-10 20:29:11.000000 balsam-0.7.0a22/tests/benchmark/locustfile.py
+-rw-r--r--   0 turam     (2517) users      (100)     2954 2023-04-10 20:29:11.000000 balsam-0.7.0a22/tests/benchmark/populate_eig.py
+-rw-r--r--   0 turam     (2517) users      (100)      382 2023-04-10 20:29:11.000000 balsam-0.7.0a22/tests/benchmark/random-eig.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/tests/server/
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/server/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)     1646 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/server/conftest.py
+-rw-r--r--   0 turam     (2517) users      (100)     2778 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/server/test_apps.py
+-rw-r--r--   0 turam     (2517) users      (100)      609 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/server/test_auth.py
+-rw-r--r--   0 turam     (2517) users      (100)    11869 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/server/test_batchjobs.py
+-rw-r--r--   0 turam     (2517) users      (100)    41008 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/server/test_jobs.py
+-rw-r--r--   0 turam     (2517) users      (100)     2350 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/server/test_sites.py
+-rw-r--r--   0 turam     (2517) users      (100)     3749 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/server/util.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/tests/site_integration/
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/site_integration/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/site_integration/conftest.py
+-rw-r--r--   0 turam     (2517) users      (100)     6149 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/site_integration/test_integration.py
+-rw-r--r--   0 turam     (2517) users      (100)     1991 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/test_platform.py
+drwxr-xr-x   0 turam     (2517) users      (100)        0 2023-04-10 20:36:58.000000 balsam-0.7.0a22/tests/units/
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/units/__init__.py
+-rw-r--r--   0 turam     (2517) users      (100)        0 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/units/conftest.py
+-rw-r--r--   0 turam     (2517) users      (100)     2153 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/units/test_mpi_launcher.py
+-rw-r--r--   0 turam     (2517) users      (100)       31 2023-04-10 20:29:12.000000 balsam-0.7.0a22/tests/units/test_scheduler.py
```

### Comparing `balsam-0.7.0a21/PKG-INFO` & `balsam-0.7.0a22/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsam
-Version: 0.7.0a21
+Version: 0.7.0a22
 Summary: HPC Workflows & Edge Service
 Home-page: https://balsam.readthedocs.io
 Author: Misha Salim, Thomas Uram, J. Taylor Childers
 Author-email: turam@anl.gov
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/argonne-lcf/balsam
 Project-URL: Documentation, https://argonne-lcf.github.io/balsam
```

### Comparing `balsam-0.7.0a21/balsam/_api/app.py` & `balsam-0.7.0a22/balsam/_api/app.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/_api/bases.py` & `balsam-0.7.0a22/balsam/_api/bases.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/_api/manager.py` & `balsam-0.7.0a22/balsam/_api/manager.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/_api/model.py` & `balsam-0.7.0a22/balsam/_api/model.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/_api/models.py` & `balsam-0.7.0a22/balsam/_api/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# This file was auto-generated via /Users/turam/opt/miniconda3/bin/python balsam/schemas/api_generator.py
-# [git rev ce4bdce]
+# This file was auto-generated via /home/turam/miniconda3/bin/python balsam/schemas/api_generator.py
+# [git rev 7634992]
 # Do *not* make changes to the API by changing this file!
 
 import datetime
 import pathlib
 import typing
 import uuid
 from typing import Any, List, Optional, Union
@@ -761,15 +761,15 @@
     objects: "BatchJobManager"
 
     num_nodes = Field[int]()
     wall_time_min = Field[int]()
     job_mode = Field[balsam.schemas.batchjob.JobMode]()
     optional_params = Field[typing.Dict[str, str]]()
     filter_tags = Field[typing.Dict[str, str]]()
-    partitions = Field[typing.Optional[typing.List[balsam.schemas.batchjob.BatchJobPartition]]]()
+    partitions = Field[Optional[typing.Union[typing.List[balsam.schemas.batchjob.BatchJobPartition], None]]]()
     site_id = Field[int]()
     project = Field[str]()
     queue = Field[str]()
     scheduler_id = Field[Optional[int]]()
     state = Field[Optional[balsam.schemas.batchjob.BatchJobState]]()
     status_info = Field[Optional[typing.Dict[str, str]]]()
     start_time = Field[Optional[datetime.datetime]]()
@@ -782,15 +782,15 @@
         wall_time_min: int,
         job_mode: balsam.schemas.batchjob.JobMode,
         site_id: int,
         project: str,
         queue: str,
         optional_params: Optional[typing.Dict[str, str]] = None,
         filter_tags: Optional[typing.Dict[str, str]] = None,
-        partitions: Optional[typing.Optional[typing.List[balsam.schemas.batchjob.BatchJobPartition]]] = None,
+        partitions: Optional[typing.Union[typing.List[balsam.schemas.batchjob.BatchJobPartition], None]] = None,
         **kwargs: Any,
     ) -> None:
         """
         Construct a new BatchJob object.  You must eventually call the save() method or
         pass a BatchJob list into BatchJob.objects.bulk_create().
 
         num_nodes:       Requested number of nodes for this allocation
@@ -914,15 +914,15 @@
         wall_time_min: int,
         job_mode: balsam.schemas.batchjob.JobMode,
         site_id: int,
         project: str,
         queue: str,
         optional_params: Optional[typing.Dict[str, str]] = None,
         filter_tags: Optional[typing.Dict[str, str]] = None,
-        partitions: Optional[typing.Optional[typing.List[balsam.schemas.batchjob.BatchJobPartition]]] = None,
+        partitions: Optional[typing.Union[typing.List[balsam.schemas.batchjob.BatchJobPartition], None]] = None,
     ) -> BatchJob:
         """
         Create a new BatchJob object and save it to the API in one step.
 
         num_nodes:       Requested number of nodes for this allocation
         wall_time_min:   Requested wall clock time for this allocation
         job_mode:        Balsam launcher execution mode (if single partition)
```

### Comparing `balsam-0.7.0a21/balsam/_api/query.py` & `balsam-0.7.0a22/balsam/_api/query.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/analytics.py` & `balsam-0.7.0a22/balsam/analytics.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/api.py` & `balsam-0.7.0a22/balsam/api.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/client/encoders.py` & `balsam-0.7.0a22/balsam/client/encoders.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/client/requests_client.py` & `balsam-0.7.0a22/balsam/client/requests_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         while True:
             try:
                 logger.debug(f"{http_method}: {absolute_url} {params if params else ''}")
                 response = self._do_request(absolute_url, http_method, params, json, data)
             except requests.Timeout as exc:
                 logger.warning(f"Attempt Retry of Timed-out request {http_method} {absolute_url}")
                 self.backoff(exc)
-            except requests.ConnectionError as exc:
+            except (requests.ConnectionError, requests.HTTPError) as exc:
                 logger.warning(f"Attempt retry ({self._attempt} of {self.retry_count}) of connection: {exc}")
                 self.backoff(exc)
             else:
                 try:
                     return response.json()  # type: ignore
                 except (ValueError, JSONDecodeError):
                     if http_method != "DELETE":
```

### Comparing `balsam-0.7.0a21/balsam/client/requests_oauth.py` & `balsam-0.7.0a22/balsam/client/requests_oauth.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/client/requests_password.py` & `balsam-0.7.0a22/balsam/client/requests_password.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/client/rest_base_client.py` & `balsam-0.7.0a22/balsam/client/rest_base_client.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/cmdline/__init__.py` & `balsam-0.7.0a22/balsam/cmdline/__init__.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/cmdline/_launcher.py` & `balsam-0.7.0a22/balsam/cmdline/_launcher.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/cmdline/app.py` & `balsam-0.7.0a22/balsam/cmdline/app.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/cmdline/job.py` & `balsam-0.7.0a22/balsam/cmdline/job.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/cmdline/login.py` & `balsam-0.7.0a22/balsam/cmdline/login.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/cmdline/scheduler.py` & `balsam-0.7.0a22/balsam/cmdline/scheduler.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/cmdline/server.py` & `balsam-0.7.0a22/balsam/cmdline/server.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/cmdline/site.py` & `balsam-0.7.0a22/balsam/cmdline/site.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/cmdline/utils.py` & `balsam-0.7.0a22/balsam/cmdline/utils.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/config.py` & `balsam-0.7.0a22/balsam/config/config.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/alcf_cooley/job-template.sh` & `balsam-0.7.0a22/balsam/config/defaults/alcf_cooley/job-template.sh`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/alcf_cooley/settings.yml` & `balsam-0.7.0a22/balsam/config/defaults/alcf_cooley/settings.yml`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/alcf_polaris/job-template.sh` & `balsam-0.7.0a22/balsam/config/defaults/alcf_polaris/job-template.sh`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/alcf_polaris/settings.yml` & `balsam-0.7.0a22/balsam/config/defaults/alcf_polaris/settings.yml`

 * *Files 23% similar despite different names*

```diff
@@ -14,14 +14,18 @@
         max_nodes: 2
         max_queued_jobs: 100
         max_walltime: 60
     prod:
         max_nodes: 496
         max_queued_jobs: 100
         max_walltime: 1440
+    preemptable:
+        max_nodes: 10
+        max_queued_jobs: 20
+        max_walltime: 4320
 
 allowed_projects:
 - datascience
 
 optional_batch_job_params:
     mig_count: "0"  # Use -x mig_count='2' (or '3' or '7') to split GPUs N-ways
```

### Comparing `balsam-0.7.0a21/balsam/config/defaults/alcf_sunspot/job-template.sh` & `balsam-0.7.0a22/balsam/config/defaults/alcf_sunspot/job-template.sh`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/alcf_theta/job-template.sh` & `balsam-0.7.0a22/balsam/config/defaults/alcf_theta/job-template.sh`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/alcf_theta/settings.yml` & `balsam-0.7.0a22/balsam/config/defaults/alcf_theta/settings.yml`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/alcf_thetagpu/job-template.sh` & `balsam-0.7.0a22/balsam/config/defaults/alcf_thetagpu/job-template.sh`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/alcf_thetagpu/settings.yml` & `balsam-0.7.0a22/balsam/config/defaults/alcf_thetagpu/settings.yml`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/nersc_corihaswell/job-template.sh` & `balsam-0.7.0a22/balsam/config/defaults/nersc_corihaswell/job-template.sh`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/nersc_corihaswell/settings.yml` & `balsam-0.7.0a22/balsam/config/defaults/nersc_corihaswell/settings.yml`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/nersc_coriknl/settings.yml` & `balsam-0.7.0a22/balsam/config/defaults/nersc_coriknl/settings.yml`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/nersc_perlmutter/job-template.sh` & `balsam-0.7.0a22/balsam/config/defaults/nersc_perlmuttergpu/job-template.sh`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/nersc_perlmutter/settings.yml` & `balsam-0.7.0a22/balsam/config/defaults/nersc_perlmuttercpu/settings.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,26 @@
-title: "Perlmutter-GPU (NERSC)"
+title: "Perlmutter-CPU (NERSC)"
 
-compute_node: balsam.platform.compute_node.PerlmutterGPUNode
-mpi_app_launcher: balsam.platform.app_run.PerlmutterGPURun
+compute_node: balsam.platform.compute_node.PerlmutterNode
+mpi_app_launcher: balsam.platform.app_run.PerlmutterRun
 local_app_launcher: balsam.platform.app_run.LocalAppRun
 mpirun_allows_node_packing: true # mpi_app_launcher supports multiple concurrent runs per node
 serial_mode_startup_params: {}
 
 scheduler_class: balsam.platform.scheduler.SlurmScheduler
 allowed_queues:
     regular:
-        max_nodes: 128
+        max_nodes: 3072
         max_queued_jobs: 5000
-        max_walltime: 2880
+        max_walltime: 720
     debug:
-        max_nodes: 64
+        max_nodes: 8
         max_queued_jobs: 5
         max_walltime: 30
-    premium:
-        max_nodes: 1772
-        max_queued_jobs: 5
-        max_walltime: 2880
 
 allowed_projects:
-- m3676
-- m1759_g
+    - ntrain
 
 optional_batch_job_params:
     reservation: ""
 
-globus_endpoint_id: 9d6d99eb-6d04-11e5-ba46-22000b92c6ec # The local Globus endpoint ID
+globus_endpoint_id: 6bdc7956-fc0f-4ad2-989c-7aa5ee643a79 # The local Globus endpoint ID
```

### Comparing `balsam-0.7.0a21/balsam/config/defaults/olcf_summit/job-template.sh` & `balsam-0.7.0a22/balsam/config/defaults/olcf_summit/job-template.sh`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/olcf_summit/settings.yml` & `balsam-0.7.0a22/balsam/config/defaults/olcf_summit/settings.yml`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/osx/job-template.sh` & `balsam-0.7.0a22/balsam/config/defaults/osx/job-template.sh`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/osx/settings.yml` & `balsam-0.7.0a22/balsam/config/defaults/osx/settings.yml`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/defaults/settings.yml.j2` & `balsam-0.7.0a22/balsam/config/defaults/settings.yml.j2`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 transfers:
     # Trusted transfer locations
     # The site will only transfer data to/from remote locations given here
     # Given as a set of {site_alias}: {protocol}//{address} pairs
     transfer_locations:
         olcf_dtn: globus://ef1a9560-7ca1-11e5-992c-22000b96db58
         cori_dtn: globus://9d6d99eb-6d04-11e5-ba46-22000b92c6ec
+        perlmutter_dtn: globus://6bdc7956-fc0f-4ad2-989c-7aa5ee643a79
         theta_dtn: globus://08925f04-569f-11e7-bef8-22000b9a448b
         aps_dtn: globus://1c85525e-8948-11e9-8e6a-029d279f7e24
         als_dtn: globus://c7c11b22-e127-11e8-8c91-0a1d4c5c824a
 
     globus_endpoint_id: {{ globus_endpoint_id or "null" }} # The local Globus endpoint ID
     max_concurrent_transfers: 5 # How many TransferTasks can run at a time
     transfer_batch_size: 100 # Maximum number of items per TransferTask
```

### Comparing `balsam-0.7.0a21/balsam/config/defaults/validate.py` & `balsam-0.7.0a22/balsam/config/defaults/validate.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/config/site_builder.py` & `balsam-0.7.0a22/balsam/config/site_builder.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/app_run/__init__.py` & `balsam-0.7.0a22/balsam/platform/app_run/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from .app_run import AppRun, LocalAppRun
 from .mpich import MPICHRun
 from .openmpi import OpenMPIRun
-from .perlmutter import PerlmutterGPURun
+from .perlmutter import PerlmutterRun
 from .polaris import PolarisRun
 from .slurm import SlurmRun
 from .summit import SummitJsrun
 from .sunspot import SunspotRun
 from .theta import ThetaAprun
 from .theta_gpu import ThetaGPURun
 
@@ -16,9 +16,9 @@
     "SlurmRun",
     "OpenMPIRun",
     "PolarisRun",
     "ThetaGPURun",
     "MPICHRun",
     "SummitJsrun",
     "SunspotRun",
-    "PerlmutterGPURun",
+    "PerlmutterRun",
 ]
```

### Comparing `balsam-0.7.0a21/balsam/platform/app_run/app_run.py` & `balsam-0.7.0a22/balsam/platform/app_run/app_run.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/app_run/mpich.py` & `balsam-0.7.0a22/balsam/platform/app_run/mpich.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/app_run/openmpi.py` & `balsam-0.7.0a22/balsam/platform/app_run/openmpi.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/app_run/perlmutter.py` & `balsam-0.7.0a22/balsam/platform/app_run/slurm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,46 +1,31 @@
 import time
 
 from .app_run import SubprocessAppRun
 
 
-class PerlmutterGPURun(SubprocessAppRun):
+class SlurmRun(SubprocessAppRun):
     """
     https://slurm.schedmd.com/srun.html
     """
 
     def _build_cmdline(self) -> str:
         node_ids = [h for h in self._node_spec.hostnames]
         num_nodes = str(len(node_ids))
-        num_ranks = self.get_num_ranks()
-        if num_ranks == 1:
-            network_args = ["--gres=craynetwork:0"]
-        else:
-            network_args = []
-
-        if self._gpus_per_rank > 0:
-            gpu_args = ["--gpus-per-task", self._gpus_per_rank]
-        else:
-            gpu_args = []
-
         args = [
             "srun",
-            *network_args,
             "-n",
             self.get_num_ranks(),
             "--ntasks-per-node",
             self._ranks_per_node,
-            *gpu_args,
             "--nodelist",
             ",".join(node_ids),
             "--nodes",
             num_nodes,
             "--cpus-per-task",
             self.get_cpus_per_rank(),
-            "--mem=40G",
-            "--overlap",
             self._cmdline,
         ]
         return " ".join(str(arg) for arg in args)
 
     def _pre_popen(self) -> None:
         time.sleep(0.01)
```

### Comparing `balsam-0.7.0a21/balsam/platform/app_run/polaris.py` & `balsam-0.7.0a22/balsam/platform/app_run/polaris.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/app_run/summit.py` & `balsam-0.7.0a22/balsam/platform/app_run/summit.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/app_run/sunspot.py` & `balsam-0.7.0a22/balsam/platform/app_run/sunspot.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/app_run/theta.py` & `balsam-0.7.0a22/balsam/platform/app_run/theta.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/app_run/theta_gpu.py` & `balsam-0.7.0a22/balsam/platform/app_run/theta_gpu.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/compute_node/__init__.py` & `balsam-0.7.0a22/balsam/platform/compute_node/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 from .alcf_sunspot_node import SunspotNode
 from .alcf_thetagpu_node import ThetaGPUNode
 from .alcf_thetaknl_node import ThetaKNLNode
 from .compute_node import ComputeNode
 from .default import DefaultNode
 from .nersc_corihas_node import CoriHaswellNode
 from .nersc_coriknl_node import CoriKNLNode
-from .nersc_perlmutter_gpu import PerlmutterGPUNode
+from .nersc_perlmutter import PerlmutterNode
 from .summit_node import SummitNode
 
 __all__ = [
     "DefaultNode",
     "ThetaKNLNode",
     "SummitNode",
     "ThetaGPUNode",
     "CooleyNode",
     "CoriHaswellNode",
     "CoriKNLNode",
-    "PerlmutterGPUNode",
+    "PerlmutterNode",
     "PolarisNode",
     "SunspotNode",
     "ComputeNode",
 ]
```

### Comparing `balsam-0.7.0a21/balsam/platform/compute_node/alcf_cooley_node.py` & `balsam-0.7.0a22/balsam/platform/compute_node/alcf_cooley_node.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/compute_node/alcf_polaris_node.py` & `balsam-0.7.0a22/balsam/platform/compute_node/alcf_polaris_node.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/compute_node/alcf_sunspot_node.py` & `balsam-0.7.0a22/balsam/platform/compute_node/alcf_sunspot_node.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/compute_node/alcf_thetagpu_node.py` & `balsam-0.7.0a22/balsam/platform/compute_node/alcf_thetagpu_node.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/compute_node/alcf_thetaknl_node.py` & `balsam-0.7.0a22/balsam/platform/compute_node/alcf_thetaknl_node.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/compute_node/compute_node.py` & `balsam-0.7.0a22/balsam/platform/compute_node/compute_node.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/compute_node/default.py` & `balsam-0.7.0a22/balsam/platform/compute_node/default.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/compute_node/nersc_corihas_node.py` & `balsam-0.7.0a22/balsam/platform/compute_node/nersc_corihas_node.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/compute_node/nersc_coriknl_node.py` & `balsam-0.7.0a22/balsam/platform/compute_node/nersc_coriknl_node.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/compute_node/nersc_perlmutter_gpu.py` & `balsam-0.7.0a22/balsam/platform/compute_node/nersc_perlmutter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import os
 from typing import List, Optional, Union
 
 from .compute_node import ComputeNode
 
 
-class PerlmutterGPUNode(ComputeNode):
+class PerlmutterNode(ComputeNode):
     cpu_ids = list(range(64))
     gpu_ids: List[Union[int, str]] = list(range(4))
 
     @classmethod
-    def get_job_nodelist(cls) -> List["PerlmutterGPUNode"]:
+    def get_job_nodelist(cls) -> List["PerlmutterNode"]:
         """
         Get all compute nodes allocated in the current job context
         """
         nodelist_str = os.environ["SLURM_NODELIST"]
         # string like: nid[02529,02878,03047,03290,03331,03813,11847-11848]
         # or like: nid0[3038-3039,8241-8246]
         # or like: nid00[858-861]
@@ -46,8 +46,8 @@
             return int(id)
         return None
 
 
 if __name__ == "__main__":
     if "SLURM_NODELIST" not in os.environ:
         os.environ["SLURM_NODELIST"] = "nid0[3038-3039,8241-8246]"
-    print([str(x) for x in PerlmutterGPUNode.get_job_nodelist()])
+    print([str(x) for x in PerlmutterNode.get_job_nodelist()])
```

### Comparing `balsam-0.7.0a21/balsam/platform/compute_node/summit_node.py` & `balsam-0.7.0a22/balsam/platform/compute_node/summit_node.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/scheduler/__init__.py` & `balsam-0.7.0a22/balsam/platform/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/scheduler/cobalt_sched.py` & `balsam-0.7.0a22/balsam/platform/scheduler/cobalt_sched.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/scheduler/local.py` & `balsam-0.7.0a22/balsam/platform/scheduler/local.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/scheduler/lsf_sched.py` & `balsam-0.7.0a22/balsam/platform/scheduler/lsf_sched.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/scheduler/pbs_sched.py` & `balsam-0.7.0a22/balsam/platform/scheduler/pbs_sched.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,21 +143,15 @@
             "doe",
             str(script_path),
         ]
         return args
 
     @staticmethod
     def _render_status_args(project: Optional[str], user: Optional[str], queue: Optional[str]) -> List[str]:
-        args = [PBSScheduler.status_exe]
-        args += "-f -F json".split()
-        # if user is not None:
-        #     args += ["-u", user]
-        if queue is not None:
-            args += ["-q", queue]
-        return args
+        pass
 
     @staticmethod
     def _render_delete_args(job_id: Union[int, str]) -> List[str]:
         return [PBSScheduler.delete_exe, str(job_id)]
 
     @staticmethod
     def _render_backfill_args() -> List[str]:
@@ -168,14 +162,37 @@
         try:
             return int(submit_output.split(".")[0])
         except Exception as exc:
             # Catch errors here and handle
             logger.warning(f"Exception: {exc}")
             raise
 
+    @classmethod
+    def get_statuses(
+        cls,
+        project: Optional[str] = None,
+        user: Optional[str] = getpass.getuser(),
+        queue: Optional[str] = None,
+    ) -> Dict[int, SchedulerJobStatus]:
+        # First call qstat to get user job ids
+        args = [PBSScheduler.status_exe]
+        stdout = scheduler_subproc(args)
+        stdout_lines = [s for s in stdout.split("\n") if str(user) in s]
+        if len(stdout_lines) == 0:
+            return {}  # if there are no jobs in the queue return an empty dictionary
+        user_job_ids = [s.split(".")[0] for s in stdout_lines]
+
+        # Next call qstat to get job jsons
+        args = [PBSScheduler.status_exe]
+        args += user_job_ids
+        args += "-f -F json".split()
+        stdout = scheduler_subproc(args)
+        stat_dict = cls._parse_status_output(stdout)
+        return stat_dict
+
     @staticmethod
     def _parse_status_output(raw_output: str) -> Dict[int, SchedulerJobStatus]:
         # TODO: this can be much more efficient with a compiled regex findall()
         # logger.info(f"json status output {raw_output}")
         username = getpass.getuser()
         j = json.loads(raw_output)
         date_format = "%a %b %d %H:%M:%S %Y"
```

### Comparing `balsam-0.7.0a21/balsam/platform/scheduler/scheduler.py` & `balsam-0.7.0a22/balsam/platform/scheduler/scheduler.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/scheduler/slurm_sched.py` & `balsam-0.7.0a22/balsam/platform/scheduler/slurm_sched.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/transfer/globus_transfer.py` & `balsam-0.7.0a22/balsam/platform/transfer/globus_transfer.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/platform/transfer/transfer.py` & `balsam-0.7.0a22/balsam/platform/transfer/transfer.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/schemas/__init__.py` & `balsam-0.7.0a22/balsam/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/schemas/api_generator.py` & `balsam-0.7.0a22/balsam/schemas/api_generator.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/schemas/apps.py` & `balsam-0.7.0a22/balsam/schemas/apps.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/schemas/batchjob.py` & `balsam-0.7.0a22/balsam/schemas/batchjob.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/schemas/job.py` & `balsam-0.7.0a22/balsam/schemas/job.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/schemas/logevent.py` & `balsam-0.7.0a22/balsam/schemas/logevent.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/schemas/serializer.py` & `balsam-0.7.0a22/balsam/schemas/serializer.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/schemas/session.py` & `balsam-0.7.0a22/balsam/schemas/session.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/schemas/site.py` & `balsam-0.7.0a22/balsam/schemas/site.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/schemas/transfer.py` & `balsam-0.7.0a22/balsam/schemas/transfer.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/auth/__init__.py` & `balsam-0.7.0a22/balsam/server/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/auth/authorization_code_login.py` & `balsam-0.7.0a22/balsam/server/auth/authorization_code_login.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/auth/db_sessions.py` & `balsam-0.7.0a22/balsam/server/auth/db_sessions.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/auth/device_code_login.py` & `balsam-0.7.0a22/balsam/server/auth/device_code_login.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/auth/password_login.py` & `balsam-0.7.0a22/balsam/server/auth/password_login.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/auth/token.py` & `balsam-0.7.0a22/balsam/server/auth/token.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/conf.py` & `balsam-0.7.0a22/balsam/server/conf.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/gunicorn.conf.example.py` & `balsam-0.7.0a22/balsam/server/gunicorn.conf.example.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/gunicorn.conf.py` & `balsam-0.7.0a22/balsam/server/gunicorn.conf.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/gunicorn_logger.py` & `balsam-0.7.0a22/balsam/server/gunicorn_logger.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/main.py` & `balsam-0.7.0a22/balsam/server/main.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/models/base.py` & `balsam-0.7.0a22/balsam/server/models/base.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/models/crud/apps.py` & `balsam-0.7.0a22/balsam/server/models/crud/apps.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/models/crud/batch_jobs.py` & `balsam-0.7.0a22/balsam/server/models/crud/batch_jobs.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/models/crud/events.py` & `balsam-0.7.0a22/balsam/server/models/crud/events.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/models/crud/jobs.py` & `balsam-0.7.0a22/balsam/server/models/crud/jobs.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/models/crud/sessions.py` & `balsam-0.7.0a22/balsam/server/models/crud/sessions.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/models/crud/sites.py` & `balsam-0.7.0a22/balsam/server/models/crud/sites.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/models/crud/transfers.py` & `balsam-0.7.0a22/balsam/server/models/crud/transfers.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/models/crud/users.py` & `balsam-0.7.0a22/balsam/server/models/crud/users.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/models/tables.py` & `balsam-0.7.0a22/balsam/server/models/tables.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/pubsub.py` & `balsam-0.7.0a22/balsam/server/pubsub.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/routers/apps.py` & `balsam-0.7.0a22/balsam/server/routers/apps.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/routers/batch_jobs.py` & `balsam-0.7.0a22/balsam/server/routers/batch_jobs.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/routers/events.py` & `balsam-0.7.0a22/balsam/server/routers/events.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/routers/filters.py` & `balsam-0.7.0a22/balsam/server/routers/filters.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/routers/jobs.py` & `balsam-0.7.0a22/balsam/server/routers/jobs.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/routers/sessions.py` & `balsam-0.7.0a22/balsam/server/routers/sessions.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/routers/sites.py` & `balsam-0.7.0a22/balsam/server/routers/sites.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/routers/transfers.py` & `balsam-0.7.0a22/balsam/server/routers/transfers.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/utils/log.py` & `balsam-0.7.0a22/balsam/server/utils/log.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/utils/paginator.py` & `balsam-0.7.0a22/balsam/server/utils/paginator.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/utils/timer.py` & `balsam-0.7.0a22/balsam/server/utils/timer.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/server/utils/user_tools.py` & `balsam-0.7.0a22/balsam/server/utils/user_tools.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/shared_apps/alcf_cooley/parsl.py` & `balsam-0.7.0a22/balsam/shared_apps/alcf_cooley/parsl.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/shared_apps/alcf_theta/xpcs.py` & `balsam-0.7.0a22/balsam/shared_apps/alcf_theta/xpcs.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/shared_apps/olcf_summit/xpcs.py` & `balsam-0.7.0a22/balsam/shared_apps/olcf_summit/xpcs.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/job_source.py` & `balsam-0.7.0a22/balsam/site/job_source.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/launcher/_mpi_mode.py` & `balsam-0.7.0a22/balsam/site/launcher/_mpi_mode.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/launcher/_serial_mode_master.py` & `balsam-0.7.0a22/balsam/site/launcher/_serial_mode_master.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/launcher/_serial_mode_worker.py` & `balsam-0.7.0a22/balsam/site/launcher/_serial_mode_worker.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/launcher/node_manager.py` & `balsam-0.7.0a22/balsam/site/launcher/node_manager.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/launcher/python_runner.py` & `balsam-0.7.0a22/balsam/site/launcher/python_runner.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/launcher/serial_mode.py` & `balsam-0.7.0a22/balsam/site/launcher/serial_mode.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/launcher/util.py` & `balsam-0.7.0a22/balsam/site/launcher/util.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/script_template.py` & `balsam-0.7.0a22/balsam/site/script_template.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/service/elastic_queue.py` & `balsam-0.7.0a22/balsam/site/service/elastic_queue.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/service/file_cleaner.py` & `balsam-0.7.0a22/balsam/site/service/file_cleaner.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/service/main.py` & `balsam-0.7.0a22/balsam/site/service/main.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/service/processing.py` & `balsam-0.7.0a22/balsam/site/service/processing.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/service/queue_maintainer.py` & `balsam-0.7.0a22/balsam/site/service/queue_maintainer.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/service/scheduler.py` & `balsam-0.7.0a22/balsam/site/service/scheduler.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/service/service_base.py` & `balsam-0.7.0a22/balsam/site/service/service_base.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/service/transfer.py` & `balsam-0.7.0a22/balsam/site/service/transfer.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/status_updater.py` & `balsam-0.7.0a22/balsam/site/status_updater.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/site/util/mp_queue.py` & `balsam-0.7.0a22/balsam/site/util/mp_queue.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/util/globus_auth.py` & `balsam-0.7.0a22/balsam/util/globus_auth.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/util/log.py` & `balsam-0.7.0a22/balsam/util/log.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/util/postgres.py` & `balsam-0.7.0a22/balsam/util/postgres.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/util/process.py` & `balsam-0.7.0a22/balsam/util/process.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/util/sighandler.py` & `balsam-0.7.0a22/balsam/util/sighandler.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam/util/time_parser.py` & `balsam-0.7.0a22/balsam/util/time_parser.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/balsam.egg-info/PKG-INFO` & `balsam-0.7.0a22/balsam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: balsam
-Version: 0.7.0a21
+Version: 0.7.0a22
 Summary: HPC Workflows & Edge Service
 Home-page: https://balsam.readthedocs.io
 Author: Misha Salim, Thomas Uram, J. Taylor Childers
 Author-email: turam@anl.gov
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/argonne-lcf/balsam
 Project-URL: Documentation, https://argonne-lcf.github.io/balsam
```

### Comparing `balsam-0.7.0a21/balsam.egg-info/SOURCES.txt` & `balsam-0.7.0a22/balsam.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -51,16 +51,18 @@
 balsam/config/defaults/alcf_theta/settings.yml
 balsam/config/defaults/alcf_thetagpu/job-template.sh
 balsam/config/defaults/alcf_thetagpu/settings.yml
 balsam/config/defaults/nersc_corihaswell/job-template.sh
 balsam/config/defaults/nersc_corihaswell/settings.yml
 balsam/config/defaults/nersc_coriknl/job-template.sh
 balsam/config/defaults/nersc_coriknl/settings.yml
-balsam/config/defaults/nersc_perlmutter/job-template.sh
-balsam/config/defaults/nersc_perlmutter/settings.yml
+balsam/config/defaults/nersc_perlmuttercpu/job-template.sh
+balsam/config/defaults/nersc_perlmuttercpu/settings.yml
+balsam/config/defaults/nersc_perlmuttergpu/job-template.sh
+balsam/config/defaults/nersc_perlmuttergpu/settings.yml
 balsam/config/defaults/olcf_summit/job-template.sh
 balsam/config/defaults/olcf_summit/settings.yml
 balsam/config/defaults/osx/job-template.sh
 balsam/config/defaults/osx/settings.yml
 balsam/platform/__init__.py
 balsam/platform/app_run/__init__.py
 balsam/platform/app_run/app_run.py
@@ -79,15 +81,15 @@
 balsam/platform/compute_node/alcf_sunspot_node.py
 balsam/platform/compute_node/alcf_thetagpu_node.py
 balsam/platform/compute_node/alcf_thetaknl_node.py
 balsam/platform/compute_node/compute_node.py
 balsam/platform/compute_node/default.py
 balsam/platform/compute_node/nersc_corihas_node.py
 balsam/platform/compute_node/nersc_coriknl_node.py
-balsam/platform/compute_node/nersc_perlmutter_gpu.py
+balsam/platform/compute_node/nersc_perlmutter.py
 balsam/platform/compute_node/summit_node.py
 balsam/platform/scheduler/__init__.py
 balsam/platform/scheduler/cobalt_sched.py
 balsam/platform/scheduler/local.py
 balsam/platform/scheduler/lsf_sched.py
 balsam/platform/scheduler/pbs_sched.py
 balsam/platform/scheduler/scheduler.py
@@ -185,14 +187,15 @@
 balsam/util/__init__.py
 balsam/util/globus_auth.py
 balsam/util/log.py
 balsam/util/postgres.py
 balsam/util/process.py
 balsam/util/sighandler.py
 balsam/util/time_parser.py
+tests/test_platform.py
 tests/api/__init__.py
 tests/api/conftest.py
 tests/api/test_api.py
 tests/benchmark/__init__.py
 tests/benchmark/batch_simulation.py
 tests/benchmark/batch_simulation_cori.py
 tests/benchmark/conftest.py
```

### Comparing `balsam-0.7.0a21/setup.cfg` & `balsam-0.7.0a22/setup.cfg`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/setup.py` & `balsam-0.7.0a22/setup.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/api/test_api.py` & `balsam-0.7.0a22/tests/api/test_api.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/benchmark/batch_simulation.py` & `balsam-0.7.0a22/tests/benchmark/batch_simulation.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/benchmark/batch_simulation_cori.py` & `balsam-0.7.0a22/tests/benchmark/batch_simulation_cori.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/benchmark/eig_backlog.py` & `balsam-0.7.0a22/tests/benchmark/eig_backlog.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/benchmark/eig_scaling.py` & `balsam-0.7.0a22/tests/benchmark/eig_scaling.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/benchmark/job_producer.py` & `balsam-0.7.0a22/tests/benchmark/job_producer.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/benchmark/locustfile.py` & `balsam-0.7.0a22/tests/benchmark/locustfile.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/benchmark/populate_eig.py` & `balsam-0.7.0a22/tests/benchmark/populate_eig.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/server/conftest.py` & `balsam-0.7.0a22/tests/server/conftest.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/server/test_apps.py` & `balsam-0.7.0a22/tests/server/test_apps.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/server/test_auth.py` & `balsam-0.7.0a22/tests/server/test_auth.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/server/test_batchjobs.py` & `balsam-0.7.0a22/tests/server/test_batchjobs.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/server/test_jobs.py` & `balsam-0.7.0a22/tests/server/test_jobs.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/server/test_sites.py` & `balsam-0.7.0a22/tests/server/test_sites.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/server/util.py` & `balsam-0.7.0a22/tests/server/util.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/site_integration/test_integration.py` & `balsam-0.7.0a22/tests/site_integration/test_integration.py`

 * *Files identical despite different names*

### Comparing `balsam-0.7.0a21/tests/units/test_mpi_launcher.py` & `balsam-0.7.0a22/tests/units/test_mpi_launcher.py`

 * *Files identical despite different names*

