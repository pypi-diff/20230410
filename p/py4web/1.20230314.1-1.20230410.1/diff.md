# Comparing `tmp/py4web-1.20230314.1.tar.gz` & `tmp/py4web-1.20230410.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py4web-1.20230314.1.tar", last modified: Wed Mar 15 06:49:10 2023, max compression
+gzip compressed data, was "py4web-1.20230410.1.tar", last modified: Mon Apr 10 07:02:21 2023, max compression
```

## Comparing `py4web-1.20230314.1.tar` & `py4web-1.20230410.1.tar`

### file list

```diff
@@ -1,62 +1,63 @@
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-03-15 06:49:10.241840 py4web-1.20230314.1/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      826 2023-03-15 06:49:10.241840 py4web-1.20230314.1/PKG-INFO
--rw-r--r--   0 massimo   (1000) massimo   (1000)     7120 2022-01-11 05:54:38.000000 py4web-1.20230314.1/README.rst
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-03-15 06:49:10.221840 py4web-1.20230314.1/py4web/
--rw-r--r--   0 massimo   (1000) massimo   (1000)      721 2023-03-15 06:48:50.000000 py4web-1.20230314.1/py4web/__init__.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-03-15 06:49:10.233840 py4web-1.20230314.1/py4web/assets/
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  2990703 2023-03-12 23:37:24.000000 py4web-1.20230314.1/py4web/assets/py4web.app._dashboard.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)   182307 2023-03-12 23:37:24.000000 py4web-1.20230314.1/py4web/assets/py4web.app._default.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  4278467 2023-03-12 23:37:25.000000 py4web-1.20230314.1/py4web/assets/py4web.app._documentation.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      409 2023-03-12 23:37:25.000000 py4web-1.20230314.1/py4web/assets/py4web.app._minimal.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    16674 2023-03-12 23:37:24.000000 py4web-1.20230314.1/py4web/assets/py4web.app._scaffold.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)  1386132 2023-03-12 23:37:25.000000 py4web-1.20230314.1/py4web/assets/py4web.app.showcase.zip
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    66585 2023-02-13 05:02:28.000000 py4web-1.20230314.1/py4web/core.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     7510 2022-06-30 06:41:15.000000 py4web-1.20230314.1/py4web/server_adapters.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-03-15 06:49:10.237840 py4web-1.20230314.1/py4web/utils/
--rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2019-07-23 06:20:41.000000 py4web-1.20230314.1/py4web/utils/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    69365 2023-03-15 03:30:17.000000 py4web-1.20230314.1/py4web/utils/auth.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-03-15 06:49:10.241840 py4web-1.20230314.1/py4web/utils/auth_plugins/
--rw-r--r--   0 massimo   (1000) massimo   (1000)     5976 2023-02-26 23:32:27.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/__init__.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      801 2022-03-20 01:46:38.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/basic_auth_plugin.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)     8154 2022-03-15 04:37:19.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/cas_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1444 2022-03-20 01:46:38.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/email_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    35385 2022-03-20 01:46:38.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/ldap_plugin.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)     3563 2022-03-14 19:17:56.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/newsamlplugin.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)     1759 2022-02-21 23:58:14.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/oauth2discord.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      654 2020-10-10 04:20:35.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/oauth2facebook.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      512 2023-02-26 23:31:59.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/oauth2github.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      524 2020-10-10 04:20:35.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/oauth2google.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      489 2020-10-10 04:20:35.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/oauth2okta.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2084 2022-03-20 01:46:38.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/oauth2server.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6090 2022-03-20 01:46:38.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     5051 2022-03-20 01:46:38.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/pam.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      187 2020-10-10 04:20:35.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/pam_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6672 2022-03-20 01:46:38.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/saml2_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2848 2022-03-20 01:46:38.000000 py4web-1.20230314.1/py4web/utils/auth_plugins/x509_auth_plugin.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      857 2022-03-20 01:46:38.000000 py4web-1.20230314.1/py4web/utils/cors.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1628 2023-01-11 05:50:14.000000 py4web-1.20230314.1/py4web/utils/dbstore.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     2075 2022-03-20 01:46:38.000000 py4web-1.20230314.1/py4web/utils/downloader.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3142 2022-03-20 01:46:38.000000 py4web-1.20230314.1/py4web/utils/factories.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    36017 2023-03-15 06:47:05.000000 py4web-1.20230314.1/py4web/utils/form.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    63643 2023-03-12 23:35:32.000000 py4web-1.20230314.1/py4web/utils/grid.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1651 2022-06-08 06:27:50.000000 py4web-1.20230314.1/py4web/utils/jsonrpc.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    34865 2022-11-11 06:40:11.000000 py4web-1.20230314.1/py4web/utils/mailer.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     9196 2022-06-03 04:17:49.000000 py4web-1.20230314.1/py4web/utils/misc.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)      502 2020-09-13 06:17:02.000000 py4web-1.20230314.1/py4web/utils/param.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)    18269 2022-03-20 01:46:38.000000 py4web-1.20230314.1/py4web/utils/populate.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1694 2022-05-31 06:26:42.000000 py4web-1.20230314.1/py4web/utils/publisher.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)    70958 2022-03-14 20:46:56.000000 py4web-1.20230314.1/py4web/utils/scheduler.py
--rw-r--r--   0 massimo   (1000) massimo   (1000)    70958 2022-03-14 20:46:56.000000 py4web-1.20230314.1/py4web/utils/scheduler_old.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     3728 2022-03-20 01:46:38.000000 py4web-1.20230314.1/py4web/utils/security.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)      158 2022-03-20 01:46:38.000000 py4web-1.20230314.1/py4web/utils/tags.py
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     6425 2022-09-24 20:59:44.000000 py4web-1.20230314.1/py4web/utils/url_signer.py
-drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-03-15 06:49:10.221840 py4web-1.20230314.1/py4web.egg-info/
--rw-r--r--   0 massimo   (1000) massimo   (1000)      826 2023-03-15 06:49:10.000000 py4web-1.20230314.1/py4web.egg-info/PKG-INFO
--rw-r--r--   0 massimo   (1000) massimo   (1000)     1701 2023-03-15 06:49:10.000000 py4web-1.20230314.1/py4web.egg-info/SOURCES.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2023-03-15 06:49:10.000000 py4web-1.20230314.1/py4web.egg-info/dependency_links.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)       44 2023-03-15 06:49:10.000000 py4web-1.20230314.1/py4web.egg-info/entry_points.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2020-09-07 23:01:39.000000 py4web-1.20230314.1/py4web.egg-info/not-zip-safe
--rw-r--r--   0 massimo   (1000) massimo   (1000)      215 2023-03-15 06:49:10.000000 py4web-1.20230314.1/py4web.egg-info/requires.txt
--rw-r--r--   0 massimo   (1000) massimo   (1000)        7 2023-03-15 06:49:10.000000 py4web-1.20230314.1/py4web.egg-info/top_level.txt
--rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-03-15 06:49:10.241840 py4web-1.20230314.1/setup.cfg
--rw-rw-r--   0 massimo   (1000) massimo   (1000)     1758 2023-03-12 23:37:12.000000 py4web-1.20230314.1/setup.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-10 07:02:21.236715 py4web-1.20230410.1/
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      826 2023-04-10 07:02:21.236715 py4web-1.20230410.1/PKG-INFO
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     7120 2022-01-11 05:54:38.000000 py4web-1.20230410.1/README.rst
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-10 07:02:21.220715 py4web-1.20230410.1/py4web/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      721 2023-04-10 07:01:33.000000 py4web-1.20230410.1/py4web/__init__.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-10 07:02:21.228715 py4web-1.20230410.1/py4web/assets/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)  2990826 2023-04-10 05:21:53.000000 py4web-1.20230410.1/py4web/assets/py4web.app._dashboard.zip
+-rw-r--r--   0 massimo   (1000) massimo   (1000)   182307 2023-04-10 05:16:03.000000 py4web-1.20230410.1/py4web/assets/py4web.app._default.zip
+-rw-r--r--   0 massimo   (1000) massimo   (1000)  4278028 2023-04-10 05:21:53.000000 py4web-1.20230410.1/py4web/assets/py4web.app._documentation.zip
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      409 2023-04-10 04:54:48.000000 py4web-1.20230410.1/py4web/assets/py4web.app._minimal.zip
+-rw-r--r--   0 massimo   (1000) massimo   (1000)    16674 2023-04-10 04:54:48.000000 py4web-1.20230410.1/py4web/assets/py4web.app._scaffold.zip
+-rw-r--r--   0 massimo   (1000) massimo   (1000)  1386102 2023-04-10 05:21:53.000000 py4web-1.20230410.1/py4web/assets/py4web.app.showcase.zip
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    66864 2023-04-08 17:57:31.000000 py4web-1.20230410.1/py4web/core.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     7510 2022-06-30 06:41:15.000000 py4web-1.20230410.1/py4web/server_adapters.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-10 07:02:21.236715 py4web-1.20230410.1/py4web/utils/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2019-07-23 06:20:41.000000 py4web-1.20230410.1/py4web/utils/__init__.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)    69664 2023-04-10 05:23:42.000000 py4web-1.20230410.1/py4web/utils/auth.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-10 07:02:21.236715 py4web-1.20230410.1/py4web/utils/auth_plugins/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     6207 2023-04-10 03:57:23.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/__init__.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      798 2023-04-10 01:56:10.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/basic_auth_plugin.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     8154 2022-03-15 04:37:19.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/cas_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1441 2023-04-10 01:56:10.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/email_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    35513 2023-04-10 03:57:06.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/ldap_plugin.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     3563 2022-03-14 19:17:56.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/newsamlplugin.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1759 2022-02-21 23:58:14.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/oauth2discord.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      654 2020-10-10 04:20:35.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/oauth2facebook.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      514 2023-04-10 03:57:06.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/oauth2github.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      524 2020-10-10 04:20:35.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/oauth2google.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      489 2020-10-10 04:20:35.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/oauth2okta.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2084 2022-03-20 01:46:38.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/oauth2server.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6090 2022-03-20 01:46:38.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/oauth2wpminiorange.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     5051 2022-03-20 01:46:38.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/pam.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      187 2023-04-10 01:56:10.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/pam_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6672 2022-03-20 01:46:38.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/saml2_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2848 2022-03-20 01:46:38.000000 py4web-1.20230410.1/py4web/utils/auth_plugins/x509_auth_plugin.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      857 2022-03-20 01:46:38.000000 py4web-1.20230410.1/py4web/utils/cors.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1628 2023-01-11 05:50:14.000000 py4web-1.20230410.1/py4web/utils/dbstore.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2075 2022-03-20 01:46:38.000000 py4web-1.20230410.1/py4web/utils/downloader.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3142 2022-03-20 01:46:38.000000 py4web-1.20230410.1/py4web/utils/factories.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    35864 2023-03-17 04:41:37.000000 py4web-1.20230410.1/py4web/utils/form.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    68937 2023-04-10 02:55:45.000000 py4web-1.20230410.1/py4web/utils/grid.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1651 2022-06-08 06:27:50.000000 py4web-1.20230410.1/py4web/utils/jsonrpc.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    34865 2022-11-11 06:40:11.000000 py4web-1.20230410.1/py4web/utils/mailer.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     9196 2022-06-03 04:17:49.000000 py4web-1.20230410.1/py4web/utils/misc.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      502 2020-09-13 06:17:02.000000 py4web-1.20230410.1/py4web/utils/param.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)    18269 2022-03-20 01:46:38.000000 py4web-1.20230410.1/py4web/utils/populate.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1694 2022-05-31 06:26:42.000000 py4web-1.20230410.1/py4web/utils/publisher.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     2225 2023-03-19 21:28:12.000000 py4web-1.20230410.1/py4web/utils/recaptcha.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)    70958 2022-03-14 20:46:56.000000 py4web-1.20230410.1/py4web/utils/scheduler.py
+-rw-r--r--   0 massimo   (1000) massimo   (1000)    70958 2022-03-14 20:46:56.000000 py4web-1.20230410.1/py4web/utils/scheduler_old.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     3728 2022-03-20 01:46:38.000000 py4web-1.20230410.1/py4web/utils/security.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)      158 2022-03-20 01:46:38.000000 py4web-1.20230410.1/py4web/utils/tags.py
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     6425 2022-09-24 20:59:44.000000 py4web-1.20230410.1/py4web/utils/url_signer.py
+drwxrwxr-x   0 massimo   (1000) massimo   (1000)        0 2023-04-10 07:02:21.220715 py4web-1.20230410.1/py4web.egg-info/
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      826 2023-04-10 07:02:21.000000 py4web-1.20230410.1/py4web.egg-info/PKG-INFO
+-rw-r--r--   0 massimo   (1000) massimo   (1000)     1727 2023-04-10 07:02:21.000000 py4web-1.20230410.1/py4web.egg-info/SOURCES.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2023-04-10 07:02:21.000000 py4web-1.20230410.1/py4web.egg-info/dependency_links.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)       44 2023-04-10 07:02:21.000000 py4web-1.20230410.1/py4web.egg-info/entry_points.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        1 2020-09-07 23:01:39.000000 py4web-1.20230410.1/py4web.egg-info/not-zip-safe
+-rw-r--r--   0 massimo   (1000) massimo   (1000)      215 2023-04-10 07:02:21.000000 py4web-1.20230410.1/py4web.egg-info/requires.txt
+-rw-r--r--   0 massimo   (1000) massimo   (1000)        7 2023-04-10 07:02:21.000000 py4web-1.20230410.1/py4web.egg-info/top_level.txt
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)       38 2023-04-10 07:02:21.236715 py4web-1.20230410.1/setup.cfg
+-rw-rw-r--   0 massimo   (1000) massimo   (1000)     1758 2023-03-12 23:37:12.000000 py4web-1.20230410.1/setup.py
```

### Comparing `py4web-1.20230314.1/PKG-INFO` & `py4web-1.20230410.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: py4web
-Version: 1.20230314.1
+Version: 1.20230410.1
 Summary: Experimental py4web (a better web2py)
 Home-page: https://github.com/web2py/py4web
 Author: Massimo Di Pierro
 Author-email: massimo.dipierro@gmail.com
 Maintainer: Massimo Di Pierro
 Maintainer-email: massimo.dipierro@gmail.com
 License: BSD
```

### Comparing `py4web-1.20230314.1/README.rst` & `py4web-1.20230410.1/README.rst`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/__init__.py` & `py4web-1.20230410.1/py4web/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import sys
 
 __author__ = "Massimo Di Pierro <massimo.dipierro@gmail.com>"
 __license__ = "BSDv3"
-__version__ = "1.20230314.1"
+__version__ = "1.20230410.1"
 
 
 def _maybe_gevent():
     for arg in sys.argv[1:]:
         if "gevent" in arg.lower():
             from gevent import monkey
```

### Comparing `py4web-1.20230314.1/py4web/assets/py4web.app._dashboard.zip` & `py4web-1.20230410.1/py4web/assets/py4web.app._dashboard.zip`

 * *Files 16% similar despite different names*

#### zipinfo {}

```diff
@@ -1,380 +1,380 @@
-Zip file size: 2990703 bytes, number of entries: 378
--rw-r--r--  3.0 unx     3965 tx defN 21-Sep-27 06:28 utils.py
--rw-rw-r--  3.0 unx     8304 tx defN 22-Apr-13 06:23 static/components/mtable.js
--rw-r--r--  3.0 unx     7597 tx defN 21-Sep-27 06:28 static/components/mtable.html
--rw-r--r--  3.0 unx    12025 bx defN 19-Jul-23 06:13 static/images/alert-red.gif
--rw-r--r--  3.0 unx    12305 bx defN 19-Jul-23 06:13 static/images/alert-blue.gif
--rw-r--r--  3.0 unx    13366 bx defN 19-Jul-23 06:13 static/images/alert-orange.gif
--rw-r--r--  3.0 unx  1010153 bx defN 19-Jul-23 06:13 static/images/widget.gif
--rw-r--r--  3.0 unx     7927 bx defN 19-Jul-23 06:13 static/images/forkme.png
--rw-r--r--  3.0 unx    13380 bx defN 19-Jul-23 06:13 static/images/alert-yellow.gif
--rw-r--r--  3.0 unx    11068 bx defN 19-Jul-23 06:13 static/images/alert-green.gif
--rw-r--r--  3.0 unx     5744 tx defN 22-Jul-19 13:20 static/css/future.css
--rw-r--r--  3.0 unx      708 tx defN 20-May-17 22:15 static/css/gitlog.min.css
+Zip file size: 2990826 bytes, number of entries: 378
+-rw-rw-r--  3.0 unx     3965 tx defN 21-Sep-27 06:28 utils.py
+-rw-r--r--  3.0 unx     8304 tx defN 22-Apr-13 06:23 static/components/mtable.js
+-rw-rw-r--  3.0 unx     7597 tx defN 21-Sep-27 06:28 static/components/mtable.html
 -rw-r--r--  3.0 unx    10442 tx defN 22-May-01 19:25 static/js/index.js
--rw-r--r--  3.0 unx     3362 tx defN 21-Jul-30 14:11 static/js/translations.js
--rw-r--r--  3.0 unx    68547 tx defN 19-Jul-23 06:13 static/js/sugar.min.js
--rw-r--r--  3.0 unx     8947 tx defN 19-Jul-23 06:33 static/js/ace/mode-d.js
--rw-r--r--  3.0 unx   470435 tx defN 19-Jul-23 06:33 static/js/ace/mode-php.js
--rw-r--r--  3.0 unx     6495 tx defN 19-Jul-23 06:33 static/js/ace/mode-rust.js
--rw-r--r--  3.0 unx     4933 tx defN 19-Jul-23 06:33 static/js/ace/mode-elm.js
--rw-r--r--  3.0 unx     3840 tx defN 19-Jul-23 06:33 static/js/ace/ext-elastic_tabstops_lite.js
--rw-r--r--  3.0 unx    58909 tx defN 19-Jul-23 06:33 static/js/ace/mode-curly.js
--rw-r--r--  3.0 unx     2791 tx defN 19-Jul-23 06:33 static/js/ace/theme-mono_industrial.js
--rw-r--r--  3.0 unx     2585 tx defN 19-Jul-23 06:33 static/js/ace/theme-textmate.js
--rw-r--r--  3.0 unx     2712 tx defN 19-Jul-23 06:33 static/js/ace/theme-chrome.js
--rw-r--r--  3.0 unx    62955 tx defN 19-Jul-23 06:33 static/js/ace/mode-rhtml.js
--rw-r--r--  3.0 unx     5005 tx defN 19-Jul-23 06:33 static/js/ace/mode-r.js
--rw-r--r--  3.0 unx     1762 tx defN 19-Jul-23 06:33 static/js/ace/mode-ada.js
--rw-r--r--  3.0 unx     4559 tx defN 19-Jul-23 06:33 static/js/ace/mode-pascal.js
--rw-r--r--  3.0 unx    30624 tx defN 19-Jul-23 06:33 static/js/ace/mode-ftl.js
--rw-r--r--  3.0 unx     3818 tx defN 19-Jul-23 06:33 static/js/ace/ext-beautify.js
--rw-r--r--  3.0 unx     1464 tx defN 19-Jul-23 06:35 static/js/ace/mode-gcode.js
--rw-r--r--  3.0 unx  1177601 tx defN 19-Jul-23 06:35 static/js/ace/worker-xquery.js
--rw-r--r--  3.0 unx    49991 tx defN 19-Jul-23 06:33 static/js/ace/mode-jade.js
--rw-r--r--  3.0 unx    20085 tx defN 19-Jul-23 06:33 static/js/ace/mode-less.js
--rw-r--r--  3.0 unx    63640 tx defN 19-Jul-23 06:33 static/js/ace/mode-autohotkey.js
--rw-r--r--  3.0 unx     3189 tx defN 19-Jul-23 06:33 static/js/ace/mode-mipsassembler.js
--rw-r--r--  3.0 unx     2819 tx defN 19-Jul-23 06:33 static/js/ace/ext-static_highlight.js
--rw-r--r--  3.0 unx        0 bx stor 19-Jul-23 06:13 static/js/ace/mode-text.js
--rw-r--r--  3.0 unx     2409 tx defN 19-Jul-23 06:35 static/js/ace/mode-diff.js
--rw-r--r--  3.0 unx     2236 tx defN 19-Jul-23 06:35 static/js/ace/mode-space.js
--rw-r--r--  3.0 unx     2313 tx defN 19-Jul-23 06:33 static/js/ace/mode-cobol.js
--rw-r--r--  3.0 unx     4193 tx defN 19-Jul-23 06:33 static/js/ace/ext-split.js
--rw-r--r--  3.0 unx     3024 tx defN 19-Jul-23 06:33 static/js/ace/mode-rst.js
--rw-r--r--  3.0 unx     3031 tx defN 19-Jul-23 06:33 static/js/ace/theme-tomorrow_night_blue.js
--rw-r--r--  3.0 unx    40358 tx defN 19-Jul-23 06:33 static/js/ace/mode-mask.js
--rw-r--r--  3.0 unx    16415 tx defN 19-Jul-23 06:33 static/js/ace/mode-sqlserver.js
--rw-r--r--  3.0 unx     3994 tx defN 19-Jul-23 06:35 static/js/ace/mode-yaml.js
--rw-r--r--  3.0 unx     2556 tx defN 19-Jul-23 06:33 static/js/ace/theme-tomorrow.js
--rw-r--r--  3.0 unx    20545 tx defN 19-Jul-23 06:33 static/js/ace/mode-actionscript.js
--rw-r--r--  3.0 unx    61525 tx defN 19-Jul-23 06:33 static/js/ace/mode-twig.js
--rw-r--r--  3.0 unx     6913 tx defN 19-Jul-23 06:33 static/js/ace/mode-golang.js
--rw-r--r--  3.0 unx    32911 tx defN 19-Jul-23 06:33 static/js/ace/worker-json.js
--rw-r--r--  3.0 unx     3729 tx defN 19-Jul-23 06:33 static/js/ace/ext-modelist.js
--rw-r--r--  3.0 unx     2087 tx defN 19-Jul-23 06:33 static/js/ace/mode-textile.js
--rw-r--r--  3.0 unx     6120 tx defN 19-Jul-23 06:35 static/js/ace/mode-tcl.js
--rw-r--r--  3.0 unx    61356 tx defN 19-Jul-23 06:35 static/js/ace/mode-smarty.js
--rw-r--r--  3.0 unx     3138 tx defN 19-Jul-23 06:35 static/js/ace/theme-dreamweaver.js
--rw-r--r--  3.0 unx     4104 bx defN 19-Jul-23 06:33 static/js/ace/mode-c9search.js
--rw-r--r--  3.0 unx    11837 tx defN 19-Jul-23 06:33 static/js/ace/mode-kotlin.js
--rw-r--r--  3.0 unx     2312 tx defN 19-Jul-23 06:33 static/js/ace/theme-solarized_dark.js
--rw-r--r--  3.0 unx    55541 tx defN 19-Jul-23 06:35 static/js/ace/worker-xml.js
--rw-r--r--  3.0 unx     2844 tx defN 19-Jul-23 06:33 static/js/ace/mode-eiffel.js
--rw-r--r--  3.0 unx   140879 tx defN 19-Jul-23 06:33 static/js/ace/worker-css.js
--rw-r--r--  3.0 unx     2081 tx defN 19-Jul-23 06:33 static/js/ace/theme-clouds.js
--rw-r--r--  3.0 unx    21273 tx defN 19-Jul-23 06:33 static/js/ace/mode-sjs.js
--rw-r--r--  3.0 unx     8226 tx defN 19-Jul-23 06:35 static/js/ace/mode-dockerfile.js
--rw-r--r--  3.0 unx     3658 tx defN 19-Jul-23 06:33 static/js/ace/mode-scheme.js
--rw-r--r--  3.0 unx    19962 tx defN 19-Jul-23 06:33 static/js/ace/mode-live_script.js
--rw-r--r--  3.0 unx   232939 tx defN 19-Jul-23 06:33 static/js/ace/mode-jsoniq.js
--rw-r--r--  3.0 unx     6540 tx defN 19-Jul-23 06:33 static/js/ace/mode-haxe.js
--rw-r--r--  3.0 unx    20269 tx defN 19-Jul-23 06:33 static/js/ace/mode-wollok.js
--rw-r--r--  3.0 unx     3126 tx defN 19-Jul-23 06:33 static/js/ace/theme-katzenmilch.js
--rw-r--r--  3.0 unx     6476 tx defN 19-Jul-23 06:33 static/js/ace/theme-iplastic.js
--rw-r--r--  3.0 unx     7382 tx defN 19-Jul-23 06:33 static/js/ace/mode-perl.js
--rw-r--r--  3.0 unx    24465 tx defN 19-Jul-23 06:33 static/js/ace/keybinding-emacs.js
--rw-r--r--  3.0 unx    15753 tx defN 19-Jul-23 06:33 static/js/ace/mode-elixir.js
--rw-r--r--  3.0 unx     2380 tx defN 19-Jul-23 06:33 static/js/ace/mode-gherkin.js
--rw-r--r--  3.0 unx    21805 tx defN 19-Jul-23 06:33 static/js/ace/mode-java.js
--rw-r--r--  3.0 unx    34689 tx defN 19-Jul-23 06:33 static/js/ace/mode-jsp.js
--rw-r--r--  3.0 unx     2892 tx defN 19-Jul-23 06:33 static/js/ace/theme-sqlserver.js
--rw-r--r--  3.0 unx     8840 tx defN 19-Jul-23 06:33 static/js/ace/mode-csharp.js
--rw-r--r--  3.0 unx    20332 tx defN 19-Jul-23 06:35 static/js/ace/mode-gobstones.js
--rw-r--r--  3.0 unx     8367 tx defN 19-Jul-23 06:33 static/js/ace/mode-prolog.js
--rw-r--r--  3.0 unx     2499 tx defN 19-Jul-23 06:33 static/js/ace/theme-twilight.js
--rw-r--r--  3.0 unx     1099 tx defN 19-Jul-23 06:33 static/js/ace/mode-properties.js
--rw-r--r--  3.0 unx    62630 tx defN 19-Jul-23 06:33 static/js/ace/mode-velocity.js
--rw-r--r--  3.0 unx    12235 tx defN 19-Jul-23 06:33 static/js/ace/mode-stylus.js
--rw-r--r--  3.0 unx    57890 tx defN 19-Jul-23 06:33 static/js/ace/mode-html.js
--rw-r--r--  3.0 unx   164518 tx defN 19-Jul-23 06:33 static/js/ace/worker-javascript.js
--rw-r--r--  3.0 unx    32692 tx defN 19-Jul-23 06:33 static/js/ace/mode-powershell.js
--rw-r--r--  3.0 unx     5970 tx defN 19-Jul-23 06:33 static/js/ace/mode-hjson.js
--rw-r--r--  3.0 unx     3874 tx defN 19-Jul-23 06:33 static/js/ace/mode-latex.js
--rw-r--r--  3.0 unx     1918 tx defN 19-Jul-23 06:33 static/js/ace/theme-xcode.js
--rw-r--r--  3.0 unx    15600 tx defN 19-Jul-23 06:33 static/js/ace/mode-ocaml.js
--rw-r--r--  3.0 unx     8028 tx defN 19-Jul-23 06:33 static/js/ace/mode-clojure.js
--rw-r--r--  3.0 unx     6554 tx defN 19-Jul-23 06:33 static/js/ace/mode-makefile.js
--rw-r--r--  3.0 unx   190654 tx defN 19-Jul-23 06:33 static/js/ace/worker-coffee.js
--rw-r--r--  3.0 unx     5399 tx defN 19-Jul-23 06:35 static/js/ace/mode-applescript.js
--rw-r--r--  3.0 unx     7595 tx defN 19-Jul-23 06:33 static/js/ace/mode-dot.js
--rw-r--r--  3.0 unx      143 tx defN 19-Jul-23 06:33 static/js/ace/snippets/objectivec.js
--rw-r--r--  3.0 unx      607 tx defN 19-Jul-23 06:33 static/js/ace/snippets/gobstones.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/kotlin.js
--rw-r--r--  3.0 unx      128 tx defN 19-Jul-23 06:33 static/js/ace/snippets/hjson.js
--rw-r--r--  3.0 unx      147 tx defN 19-Jul-23 06:33 static/js/ace/snippets/assembly_x86.js
--rw-r--r--  3.0 unx    21279 tx defN 19-Jul-23 06:33 static/js/ace/snippets/ruby.js
--rw-r--r--  3.0 unx      135 tx defN 19-Jul-23 06:33 static/js/ace/snippets/logiql.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/text.js
--rw-r--r--  3.0 unx      141 tx defN 19-Jul-23 06:33 static/js/ace/snippets/html_ruby.js
--rw-r--r--  3.0 unx     6763 tx defN 19-Jul-23 06:33 static/js/ace/snippets/php.js
--rw-r--r--  3.0 unx      198 tx defN 19-Jul-23 06:33 static/js/ace/snippets/makefile.js
--rw-r--r--  3.0 unx      139 tx defN 19-Jul-23 06:33 static/js/ace/snippets/vbscript.js
--rw-r--r--  3.0 unx      297 tx defN 19-Jul-23 06:33 static/js/ace/snippets/snippets.js
--rw-r--r--  3.0 unx      448 tx defN 19-Jul-23 06:33 static/js/ace/snippets/haml.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/json.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/svg.js
--rw-r--r--  3.0 unx      370 tx defN 19-Jul-23 06:33 static/js/ace/snippets/drools.js
--rw-r--r--  3.0 unx     1975 tx defN 19-Jul-23 06:33 static/js/ace/snippets/haskell.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/vhdl.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/gcode.js
--rw-r--r--  3.0 unx     3574 tx defN 19-Jul-23 06:33 static/js/ace/snippets/erlang.js
--rw-r--r--  3.0 unx      135 tx defN 19-Jul-23 06:33 static/js/ace/snippets/matlab.js
--rw-r--r--  3.0 unx      143 tx defN 19-Jul-23 06:33 static/js/ace/snippets/properties.js
--rw-r--r--  3.0 unx     1219 tx defN 19-Jul-23 06:33 static/js/ace/snippets/io.js
--rw-r--r--  3.0 unx     1716 tx defN 19-Jul-23 06:33 static/js/ace/snippets/xquery.js
--rw-r--r--  3.0 unx      164 tx defN 19-Jul-23 06:33 static/js/ace/snippets/razor.js
--rw-r--r--  3.0 unx      143 tx defN 19-Jul-23 06:33 static/js/ace/snippets/typescript.js
--rw-r--r--  3.0 unx      151 tx defN 19-Jul-23 06:33 static/js/ace/snippets/mips_assembler.js
--rw-r--r--  3.0 unx      540 tx defN 19-Jul-23 06:33 static/js/ace/snippets/textile.js
--rw-r--r--  3.0 unx     5513 tx defN 19-Jul-23 06:33 static/js/ace/snippets/perl.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/mel.js
--rw-r--r--  3.0 unx      145 tx defN 19-Jul-23 06:33 static/js/ace/snippets/applescript.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/less.js
--rw-r--r--  3.0 unx      134 tx defN 19-Jul-23 06:33 static/js/ace/snippets/live_script.js
--rw-r--r--  3.0 unx     2233 tx defN 19-Jul-23 06:33 static/js/ace/snippets/coffee.js
--rw-r--r--  3.0 unx      126 tx defN 19-Jul-23 06:33 static/js/ace/snippets/bro.js
--rw-r--r--  3.0 unx      135 tx defN 19-Jul-23 06:33 static/js/ace/snippets/prolog.js
--rw-r--r--  3.0 unx      651 tx defN 19-Jul-23 06:33 static/js/ace/snippets/velocity.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/ini.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/rdoc.js
--rw-r--r--  3.0 unx     2973 tx defN 19-Jul-23 06:33 static/js/ace/snippets/actionscript.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/cirru.js
--rw-r--r--  3.0 unx    18271 tx defN 19-Jul-23 06:33 static/js/ace/snippets/html.js
--rw-r--r--  3.0 unx      135 tx defN 19-Jul-23 06:33 static/js/ace/snippets/groovy.js
--rw-r--r--  3.0 unx    35423 tx defN 19-Jul-23 06:33 static/js/ace/snippets/lsl.js
--rw-r--r--  3.0 unx     2630 tx defN 19-Jul-23 06:33 static/js/ace/snippets/r.js
--rw-r--r--  3.0 unx      143 tx defN 19-Jul-23 06:33 static/js/ace/snippets/plain_text.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/mysql.js
--rw-r--r--  3.0 unx    19650 tx defN 19-Jul-23 06:33 static/js/ace/snippets/css.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/pgsql.js
--rw-r--r--  3.0 unx      135 tx defN 19-Jul-23 06:33 static/js/ace/snippets/lucene.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/ocaml.js
--rw-r--r--  3.0 unx     4322 tx defN 19-Jul-23 06:33 static/js/ace/snippets/java.js
--rw-r--r--  3.0 unx      139 tx defN 19-Jul-23 06:33 static/js/ace/snippets/mushcode.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/dot.js
--rw-r--r--  3.0 unx      137 tx defN 19-Jul-23 06:33 static/js/ace/snippets/verilog.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/twig.js
--rw-r--r--  3.0 unx      135 tx defN 19-Jul-23 06:33 static/js/ace/snippets/eiffel.js
--rw-r--r--  3.0 unx      143 tx defN 19-Jul-23 06:33 static/js/ace/snippets/dockerfile.js
--rw-r--r--  3.0 unx      942 tx defN 19-Jul-23 06:33 static/js/ace/snippets/sql.js
--rw-r--r--  3.0 unx      137 tx defN 19-Jul-23 06:33 static/js/ace/snippets/fortran.js
--rw-r--r--  3.0 unx     1690 tx defN 19-Jul-23 06:33 static/js/ace/snippets/tcl.js
--rw-r--r--  3.0 unx      135 tx defN 19-Jul-23 06:33 static/js/ace/snippets/golang.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/curly.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/lean.js
--rw-r--r--  3.0 unx     2778 tx defN 19-Jul-23 06:33 static/js/ace/snippets/jsp.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/ejs.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/swig.js
--rw-r--r--  3.0 unx      147 tx defN 19-Jul-23 06:33 static/js/ace/snippets/soy_template.js
--rw-r--r--  3.0 unx      141 tx defN 19-Jul-23 06:33 static/js/ace/snippets/gitignore.js
--rw-r--r--  3.0 unx      135 tx defN 19-Jul-23 06:33 static/js/ace/snippets/pascal.js
--rw-r--r--  3.0 unx     1263 tx defN 19-Jul-23 06:33 static/js/ace/snippets/wollok.js
--rw-r--r--  3.0 unx     2663 tx defN 19-Jul-23 06:33 static/js/ace/snippets/c_cpp.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/haxe.js
--rw-r--r--  3.0 unx      137 tx defN 19-Jul-23 06:33 static/js/ace/snippets/gherkin.js
--rw-r--r--  3.0 unx     3672 tx defN 19-Jul-23 06:33 static/js/ace/snippets/python.js
--rw-r--r--  3.0 unx      270 tx defN 19-Jul-23 06:33 static/js/ace/snippets/maze.js
--rw-r--r--  3.0 unx      143 tx defN 19-Jul-23 06:33 static/js/ace/snippets/autohotkey.js
--rw-r--r--  3.0 unx      135 tx defN 19-Jul-23 06:33 static/js/ace/snippets/scheme.js
--rw-r--r--  3.0 unx      947 tx defN 19-Jul-23 06:33 static/js/ace/snippets/abc.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/scss.js
--rw-r--r--  3.0 unx      145 tx defN 19-Jul-23 06:33 static/js/ace/snippets/html_elixir.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/latex.js
--rw-r--r--  3.0 unx      127 tx defN 19-Jul-23 06:33 static/js/ace/snippets/nsis.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/sjs.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/jsx.js
--rw-r--r--  3.0 unx     3636 tx defN 19-Jul-23 06:33 static/js/ace/snippets/tex.js
--rw-r--r--  3.0 unx     3127 tx defN 19-Jul-23 06:33 static/js/ace/snippets/vala.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/tsx.js
--rw-r--r--  3.0 unx      442 tx defN 19-Jul-23 06:33 static/js/ace/snippets/rst.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/scala.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/yaml.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/ada.js
--rw-r--r--  3.0 unx      141 tx defN 19-Jul-23 06:33 static/js/ace/snippets/batchfile.js
--rw-r--r--  3.0 unx      135 tx defN 19-Jul-23 06:33 static/js/ace/snippets/smarty.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/praat.js
--rw-r--r--  3.0 unx      139 tx defN 19-Jul-23 06:33 static/js/ace/snippets/asciidoc.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/swift.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/scad.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/elm.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/glsl.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/mask.js
--rw-r--r--  3.0 unx      508 tx defN 19-Jul-23 06:33 static/js/ace/snippets/lua.js
--rw-r--r--  3.0 unx      139 tx defN 19-Jul-23 06:33 static/js/ace/snippets/c9search.js
--rw-r--r--  3.0 unx      551 tx defN 19-Jul-23 06:33 static/js/ace/snippets/diff.js
--rw-r--r--  3.0 unx     2040 tx defN 19-Jul-23 06:33 static/js/ace/snippets/clojure.js
--rw-r--r--  3.0 unx      143 tx defN 19-Jul-23 06:33 static/js/ace/snippets/livescript.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/rust.js
--rw-r--r--  3.0 unx      143 tx defN 19-Jul-23 06:33 static/js/ace/snippets/powershell.js
--rw-r--r--  3.0 unx     1716 tx defN 19-Jul-23 06:33 static/js/ace/snippets/jsoniq.js
--rw-r--r--  3.0 unx      125 tx defN 19-Jul-23 06:33 static/js/ace/snippets/d.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/toml.js
--rw-r--r--  3.0 unx      135 tx defN 19-Jul-23 06:33 static/js/ace/snippets/csharp.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/lisp.js
--rw-r--r--  3.0 unx     2139 tx defN 19-Jul-23 06:33 static/js/ace/snippets/sqlserver.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/nix.js
--rw-r--r--  3.0 unx     1319 tx defN 19-Jul-23 06:33 static/js/ace/snippets/dart.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/cobol.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/jade.js
--rw-r--r--  3.0 unx      132 tx defN 19-Jul-23 06:33 static/js/ace/snippets/protobuf.js
--rw-r--r--  3.0 unx      136 tx defN 19-Jul-23 06:33 static/js/ace/snippets/mipsassembler.js
--rw-r--r--  3.0 unx      135 tx defN 19-Jul-23 06:33 static/js/ace/snippets/liquid.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/jack.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/rhtml.js
--rw-r--r--  3.0 unx      143 tx defN 19-Jul-23 06:33 static/js/ace/snippets/handlebars.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/xml.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/abap.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/elixir.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/forth.js
--rw-r--r--  3.0 unx      145 tx defN 19-Jul-23 06:33 static/js/ace/snippets/apache_conf.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/julia.js
--rw-r--r--  3.0 unx      149 tx defN 19-Jul-23 06:33 static/js/ace/snippets/haskell_cabal.js
--rw-r--r--  3.0 unx      135 tx defN 19-Jul-23 06:33 static/js/ace/snippets/stylus.js
--rw-r--r--  3.0 unx      131 tx defN 19-Jul-23 06:33 static/js/ace/snippets/sass.js
--rw-r--r--  3.0 unx     4000 tx defN 19-Jul-23 06:33 static/js/ace/snippets/django.js
--rw-r--r--  3.0 unx      143 tx defN 19-Jul-23 06:33 static/js/ace/snippets/coldfusion.js
--rw-r--r--  3.0 unx     3840 tx defN 19-Jul-23 06:33 static/js/ace/snippets/javascript.js
--rw-r--r--  3.0 unx     2055 tx defN 19-Jul-23 06:33 static/js/ace/snippets/sh.js
--rw-r--r--  3.0 unx      129 tx defN 19-Jul-23 06:33 static/js/ace/snippets/ftl.js
--rw-r--r--  3.0 unx      133 tx defN 19-Jul-23 06:33 static/js/ace/snippets/space.js
--rw-r--r--  3.0 unx      137 tx defN 19-Jul-23 06:33 static/js/ace/snippets/luapage.js
--rw-r--r--  3.0 unx     1973 tx defN 19-Jul-23 06:33 static/js/ace/snippets/markdown.js
--rw-r--r--  3.0 unx    96918 tx defN 19-Jul-23 06:33 static/js/ace/keybinding-vim.js
--rw-r--r--  3.0 unx     6989 tx defN 19-Jul-23 06:33 static/js/ace/mode-forth.js
--rw-r--r--  3.0 unx     7189 tx defN 19-Jul-23 06:33 static/js/ace/mode-sh.js
--rw-r--r--  3.0 unx     2572 tx defN 19-Jul-23 06:35 static/js/ace/ext-whitespace.js
--rw-r--r--  3.0 unx    13909 tx defN 19-Jul-23 06:33 static/js/ace/mode-apache_conf.js
--rw-r--r--  3.0 unx     6712 tx defN 19-Jul-23 06:33 static/js/ace/mode-mushcode.js
--rw-r--r--  3.0 unx     2204 tx defN 19-Jul-23 06:33 static/js/ace/mode-toml.js
--rw-r--r--  3.0 unx     1811 tx defN 19-Jul-23 06:33 static/js/ace/mode-sql.js
--rw-r--r--  3.0 unx     2088 tx defN 19-Jul-23 06:33 static/js/ace/mode-vhdl.js
--rw-r--r--  3.0 unx     7283 tx defN 19-Jul-23 06:33 static/js/ace/mode-lua.js
--rw-r--r--  3.0 unx     8898 tx defN 19-Jul-23 06:33 static/js/ace/mode-assembly_x86.js
--rw-r--r--  3.0 unx    13008 tx defN 19-Jul-23 06:33 static/js/ace/mode-glsl.js
--rw-r--r--  3.0 unx     2913 tx defN 19-Jul-23 06:35 static/js/ace/theme-terminal.js
--rw-r--r--  3.0 unx     3003 tx defN 19-Jul-23 06:33 static/js/ace/mode-cirru.js
--rw-r--r--  3.0 unx    22619 tx defN 19-Jul-23 06:35 static/js/ace/mode-scala.js
--rw-r--r--  3.0 unx     6965 tx defN 19-Jul-23 06:33 static/js/ace/mode-jsx.js
--rw-r--r--  3.0 unx    60415 tx defN 19-Jul-23 06:33 static/js/ace/mode-coldfusion.js
--rw-r--r--  3.0 unx    10220 tx defN 19-Jul-23 06:33 static/js/ace/mode-sass.js
--rw-r--r--  3.0 unx     2176 tx defN 19-Jul-23 06:33 static/js/ace/theme-github.js
--rw-r--r--  3.0 unx    31988 tx defN 19-Jul-23 06:35 static/js/ace/mode-svg.js
--rw-r--r--  3.0 unx    12951 tx defN 19-Jul-23 06:35 static/js/ace/mode-scss.js
--rw-r--r--  3.0 unx   354781 tx defN 19-Jul-23 06:33 static/js/ace/ace.js
--rw-r--r--  3.0 unx     2761 tx defN 19-Jul-23 06:33 static/js/ace/mode-tex.js
--rw-r--r--  3.0 unx     5665 tx defN 19-Jul-23 06:33 static/js/ace/mode-io.js
--rw-r--r--  3.0 unx    10785 tx defN 19-Jul-23 06:33 static/js/ace/mode-drools.js
--rw-r--r--  3.0 unx     2375 tx defN 19-Jul-23 06:33 static/js/ace/theme-monokai.js
--rw-r--r--  3.0 unx     2125 tx defN 19-Jul-23 06:33 static/js/ace/theme-eclipse.js
--rw-r--r--  3.0 unx    12546 tx defN 19-Jul-23 06:33 static/js/ace/mode-protobuf.js
--rw-r--r--  3.0 unx    10025 tx defN 19-Jul-23 06:33 static/js/ace/mode-ruby.js
--rw-r--r--  3.0 unx     2842 tx defN 19-Jul-23 06:33 static/js/ace/theme-chaos.js
--rw-r--r--  3.0 unx      825 tx defN 19-Jul-23 06:33 static/js/ace/ext-linking.js
--rw-r--r--  3.0 unx     1088 tx defN 19-Jul-23 06:33 static/js/ace/ext-statusbar.js
--rw-r--r--  3.0 unx   217401 tx defN 19-Jul-23 06:33 static/js/ace/worker-html.js
--rw-r--r--  3.0 unx    10035 tx defN 19-Jul-23 06:33 static/js/ace/mode-nsis.js
--rw-r--r--  3.0 unx    78297 tx defN 19-Jul-23 06:33 static/js/ace/worker-php.js
--rw-r--r--  3.0 unx    54512 tx defN 19-Jul-23 06:33 static/js/ace/mode-objectivec.js
--rw-r--r--  3.0 unx     1440 bx defN 19-Jul-23 06:33 static/js/ace/ext-spellcheck.js
--rw-r--r--  3.0 unx    18060 tx defN 19-Jul-23 06:33 static/js/ace/mode-javascript.js
--rw-r--r--  3.0 unx    10260 tx defN 19-Jul-23 06:35 static/js/ace/mode-praat.js
--rw-r--r--  3.0 unx    20567 tx defN 19-Jul-23 06:35 static/js/ace/mode-matlab.js
--rw-r--r--  3.0 unx      506 tx defN 19-Jul-23 06:33 static/js/ace/mode-plain_text.js
--rw-r--r--  3.0 unx    24939 tx defN 19-Jul-23 06:35 static/js/ace/mode-mel.js
--rw-r--r--  3.0 unx     3994 tx defN 19-Jul-23 06:33 static/js/ace/mode-rdoc.js
--rw-r--r--  3.0 unx     2820 tx defN 19-Jul-23 06:35 static/js/ace/theme-tomorrow_night.js
--rw-r--r--  3.0 unx    22440 tx defN 19-Jul-23 06:33 static/js/ace/mode-groovy.js
--rw-r--r--  3.0 unx    64800 tx defN 19-Jul-23 06:35 static/js/ace/mode-markdown.js
--rw-r--r--  3.0 unx     6523 tx defN 19-Jul-23 06:35 static/js/ace/mode-mysql.js
--rw-r--r--  3.0 unx     4856 tx defN 19-Jul-23 06:33 static/js/ace/mode-batchfile.js
--rw-r--r--  3.0 unx      899 tx defN 19-Jul-23 06:33 static/js/ace/mode-gitignore.js
--rw-r--r--  3.0 unx     7539 tx defN 19-Jul-23 06:33 static/js/ace/mode-julia.js
--rw-r--r--  3.0 unx     2296 tx defN 19-Jul-23 06:33 static/js/ace/theme-kr_theme.js
--rw-r--r--  3.0 unx      140 tx defN 19-Jul-23 06:33 static/js/ace/ext-error_marker.js
--rw-r--r--  3.0 unx     5097 tx defN 19-Jul-23 06:33 static/js/ace/mode-json.js
--rw-r--r--  3.0 unx    66385 tx defN 19-Jul-23 06:33 static/js/ace/mode-soy_template.js
--rw-r--r--  3.0 unx    12293 tx defN 19-Jul-23 06:35 static/js/ace/ext-settings_menu.js
--rw-r--r--  3.0 unx    16578 tx defN 19-Jul-23 06:33 static/js/ace/mode-vala.js
--rw-r--r--  3.0 unx     5712 tx defN 19-Jul-23 06:35 static/js/ace/mode-logiql.js
--rw-r--r--  3.0 unx     5813 tx defN 19-Jul-23 06:33 static/js/ace/mode-abap.js
--rw-r--r--  3.0 unx     1961 tx defN 19-Jul-23 06:33 static/js/ace/mode-lisp.js
--rw-r--r--  3.0 unx    14198 tx defN 19-Jul-23 06:33 static/js/ace/mode-dart.js
--rw-r--r--  3.0 unx     1470 tx defN 19-Jul-23 06:33 static/js/ace/ext-themelist.js
--rw-r--r--  3.0 unx     2248 tx defN 19-Jul-23 06:33 static/js/ace/theme-idle_fingers.js
--rw-r--r--  3.0 unx    10005 tx defN 19-Jul-23 06:33 static/js/ace/ext-searchbox.js
--rw-r--r--  3.0 unx     2710 tx defN 19-Jul-23 06:33 static/js/ace/mode-ini.js
--rw-r--r--  3.0 unx    10840 tx defN 19-Jul-23 06:33 static/js/ace/mode-c_cpp.js
--rw-r--r--  3.0 unx    47114 tx defN 19-Jul-23 06:33 static/js/ace/worker-lua.js
--rw-r--r--  3.0 unx     2812 tx defN 19-Jul-23 06:33 static/js/ace/theme-crimson_editor.js
--rw-r--r--  3.0 unx    20510 tx defN 19-Jul-23 06:33 static/js/ace/mode-tsx.js
--rw-r--r--  3.0 unx    59769 tx defN 19-Jul-23 06:33 static/js/ace/mode-handlebars.js
--rw-r--r--  3.0 unx    34464 tx defN 19-Jul-23 06:33 static/js/ace/ext-language_tools.js
--rw-r--r--  3.0 unx    20198 tx defN 19-Jul-23 06:33 static/js/ace/mode-typescript.js
--rw-r--r--  3.0 unx     5576 tx defN 19-Jul-23 06:33 static/js/ace/mode-lean.js
--rw-r--r--  3.0 unx     2689 tx defN 19-Jul-23 06:33 static/js/ace/mode-verilog.js
--rw-r--r--  3.0 unx     2204 tx defN 19-Jul-23 06:35 static/js/ace/theme-vibrant_ink.js
--rw-r--r--  3.0 unx     5764 tx defN 19-Jul-23 06:33 static/js/ace/mode-jack.js
--rw-r--r--  3.0 unx    30271 tx defN 19-Jul-23 06:33 static/js/ace/mode-liquid.js
--rw-r--r--  3.0 unx    64984 tx defN 19-Jul-23 06:33 static/js/ace/mode-razor.js
--rw-r--r--  3.0 unx     3687 tx defN 19-Jul-23 06:33 static/js/ace/mode-snippets.js
--rw-r--r--  3.0 unx     4881 tx defN 19-Jul-23 06:33 static/js/ace/mode-maze.js
--rw-r--r--  3.0 unx     9112 tx defN 19-Jul-23 06:33 static/js/ace/ext-textarea.js
--rw-r--r--  3.0 unx    11468 tx defN 19-Jul-23 06:33 static/js/ace/mode-haskell.js
--rw-r--r--  3.0 unx     6211 tx defN 19-Jul-23 06:35 static/js/ace/mode-bro.js
--rw-r--r--  3.0 unx    26620 tx defN 19-Jul-23 06:35 static/js/ace/mode-lsl.js
--rw-r--r--  3.0 unx    68412 tx defN 19-Jul-23 06:33 static/js/ace/mode-ejs.js
--rw-r--r--  3.0 unx    27779 tx defN 19-Jul-23 06:33 static/js/ace/theme-ambiance.js
--rw-r--r--  3.0 unx    11914 tx defN 19-Jul-23 06:33 static/js/ace/ext-old_ie.js
--rw-r--r--  3.0 unx     1173 tx defN 19-Jul-23 06:33 static/js/ace/mode-lucene.js
--rw-r--r--  3.0 unx     7416 tx defN 19-Jul-23 06:33 static/js/ace/mode-coffee.js
--rw-r--r--  3.0 unx    37225 tx defN 19-Jul-23 06:33 static/js/ace/mode-haml.js
--rw-r--r--  3.0 unx     2282 tx defN 19-Jul-23 06:33 static/js/ace/mode-haskell_cabal.js
--rw-r--r--  3.0 unx    18046 tx defN 19-Jul-23 06:35 static/js/ace/mode-css.js
--rw-r--r--  3.0 unx     2448 tx defN 19-Jul-23 06:33 static/js/ace/theme-merbivore_soft.js
--rw-r--r--  3.0 unx     5073 tx defN 19-Jul-23 06:35 static/js/ace/mode-vbscript.js
--rw-r--r--  3.0 unx    68741 tx defN 19-Jul-23 06:35 static/js/ace/mode-html_ruby.js
--rw-r--r--  3.0 unx    55911 tx defN 19-Jul-23 06:33 static/js/ace/mode-pgsql.js
--rw-r--r--  3.0 unx     4709 tx defN 19-Jul-23 06:33 static/js/ace/mode-abc.js
--rw-r--r--  3.0 unx     3221 tx defN 19-Jul-23 06:35 static/js/ace/theme-tomorrow_night_eighties.js
--rw-r--r--  3.0 unx    21478 tx defN 19-Jul-23 06:33 static/js/ace/ext-emmet.js
--rw-r--r--  3.0 unx    75093 tx defN 19-Jul-23 06:35 static/js/ace/mode-html_elixir.js
--rw-r--r--  3.0 unx    29711 tx defN 19-Jul-23 06:33 static/js/ace/mode-erlang.js
--rw-r--r--  3.0 unx     3640 tx defN 19-Jul-23 06:35 static/js/ace/ext-keybinding_menu.js
--rw-r--r--  3.0 unx     2240 tx defN 19-Jul-23 06:33 static/js/ace/theme-dawn.js
--rw-r--r--  3.0 unx     8159 tx defN 19-Jul-23 06:33 static/js/ace/mode-asciidoc.js
--rw-r--r--  3.0 unx     2633 tx defN 19-Jul-23 06:33 static/js/ace/theme-pastel_on_dark.js
--rw-r--r--  3.0 unx    31151 tx defN 19-Jul-23 06:33 static/js/ace/mode-swig.js
--rw-r--r--  3.0 unx     6929 tx defN 19-Jul-23 06:33 static/js/ace/mode-swift.js
--rw-r--r--  3.0 unx     4681 tx defN 19-Jul-23 06:33 static/js/ace/mode-python.js
--rw-r--r--  3.0 unx     4984 tx defN 19-Jul-23 06:33 static/js/ace/mode-livescript.js
--rw-r--r--  3.0 unx     2353 tx defN 19-Jul-23 06:33 static/js/ace/theme-cobalt.js
--rw-r--r--  3.0 unx    59262 tx defN 19-Jul-23 06:33 static/js/ace/mode-django.js
--rw-r--r--  3.0 unx   230322 tx defN 19-Jul-23 06:33 static/js/ace/mode-xquery.js
--rw-r--r--  3.0 unx     6520 tx defN 19-Jul-23 06:33 static/js/ace/mode-scad.js
--rw-r--r--  3.0 unx     2432 tx defN 19-Jul-23 06:33 static/js/ace/theme-clouds_midnight.js
--rw-r--r--  3.0 unx     6360 tx defN 19-Jul-23 06:33 static/js/ace/ext-chromevox.js
--rw-r--r--  3.0 unx     2360 tx defN 19-Jul-23 06:33 static/js/ace/theme-solarized_light.js
--rw-r--r--  3.0 unx    13129 tx defN 19-Jul-23 06:33 static/js/ace/mode-nix.js
--rw-r--r--  3.0 unx    66336 tx defN 19-Jul-23 06:33 static/js/ace/mode-luapage.js
--rw-r--r--  3.0 unx     2054 tx defN 19-Jul-23 06:33 static/js/ace/theme-kuroir.js
--rw-r--r--  3.0 unx     8428 tx defN 19-Jul-23 06:33 static/js/ace/mode-fortran.js
--rw-r--r--  3.0 unx     2236 tx defN 19-Jul-23 06:33 static/js/ace/theme-merbivore.js
--rw-r--r--  3.0 unx     3496 tx defN 19-Jul-23 06:33 static/js/ace/theme-tomorrow_night_bright.js
--rw-r--r--  3.0 unx    11847 tx defN 19-Jul-23 06:33 static/js/ace/mode-xml.js
--rw-r--r--  3.0 unx     5959 tx defN 19-Jul-23 06:33 static/js/ace/mode-mips_assembler.js
--rw-rw-r--  3.0 unx    11459 tx defN 22-Mar-20 02:03 static/js/utils.js
--rw-rw-r--  3.0 unx    14265 tx defN 22-Mar-20 01:11 static/js/axios.min.js
--rw-rw-r--  3.0 unx      493 tx defN 22-Mar-20 01:46 static/js/dbadmin.js
--rw-r--r--  3.0 unx    93670 tx defN 20-Aug-29 18:02 static/js/vue.min.js
--rw-r--r--  3.0 unx    88145 tx defN 20-Feb-10 05:20 static/js/jquery.min.js
--rw-r--r--  3.0 unx    95432 tx defN 20-May-17 22:15 static/js/highlight.min.js
+-rw-r--r--  3.0 unx     1470 tx defN 21-May-31 18:07 static/js/ace/ext-themelist.js
+-rw-r--r--  3.0 unx     8367 tx defN 21-May-31 18:07 static/js/ace/mode-prolog.js
+-rw-r--r--  3.0 unx    26620 tx defN 21-May-31 18:07 static/js/ace/mode-lsl.js
+-rw-r--r--  3.0 unx    20332 tx defN 21-May-31 18:07 static/js/ace/mode-gobstones.js
+-rw-r--r--  3.0 unx     2087 tx defN 21-May-31 18:07 static/js/ace/mode-textile.js
+-rw-r--r--  3.0 unx     2585 tx defN 21-May-31 18:07 static/js/ace/theme-textmate.js
+-rw-r--r--  3.0 unx     5712 tx defN 21-May-31 18:07 static/js/ace/mode-logiql.js
+-rw-r--r--  3.0 unx  1177601 tx defN 21-May-31 18:07 static/js/ace/worker-xquery.js
+-rw-r--r--  3.0 unx   164518 tx defN 21-May-31 18:07 static/js/ace/worker-javascript.js
+-rw-r--r--  3.0 unx     2176 tx defN 21-May-31 18:07 static/js/ace/theme-github.js
+-rw-r--r--  3.0 unx     2240 tx defN 21-May-31 18:07 static/js/ace/theme-dawn.js
+-rw-r--r--  3.0 unx     4933 tx defN 21-May-31 18:07 static/js/ace/mode-elm.js
+-rw-r--r--  3.0 unx    24939 tx defN 21-May-31 18:07 static/js/ace/mode-mel.js
+-rw-r--r--  3.0 unx    40358 tx defN 21-May-31 18:07 static/js/ace/mode-mask.js
+-rw-r--r--  3.0 unx     4193 tx defN 21-May-31 18:07 static/js/ace/ext-split.js
+-rw-r--r--  3.0 unx     5813 tx defN 21-May-31 18:07 static/js/ace/mode-abap.js
+-rw-r--r--  3.0 unx     2791 tx defN 21-May-31 18:07 static/js/ace/theme-mono_industrial.js
+-rw-r--r--  3.0 unx     1961 tx defN 21-May-31 18:07 static/js/ace/mode-lisp.js
+-rw-r--r--  3.0 unx    29711 tx defN 21-May-31 18:07 static/js/ace/mode-erlang.js
+-rw-r--r--  3.0 unx     7189 tx defN 21-May-31 18:07 static/js/ace/mode-sh.js
+-rw-r--r--  3.0 unx    68412 tx defN 21-May-31 18:07 static/js/ace/mode-ejs.js
+-rw-r--r--  3.0 unx   190654 tx defN 21-May-31 18:07 static/js/ace/worker-coffee.js
+-rw-r--r--  3.0 unx    37225 tx defN 21-May-31 18:07 static/js/ace/mode-haml.js
+-rw-r--r--  3.0 unx     1464 tx defN 21-May-31 18:07 static/js/ace/mode-gcode.js
+-rw-r--r--  3.0 unx     2820 tx defN 21-May-31 18:07 static/js/ace/theme-tomorrow_night.js
+-rw-r--r--  3.0 unx     3640 tx defN 21-May-31 18:07 static/js/ace/ext-keybinding_menu.js
+-rw-r--r--  3.0 unx     2892 tx defN 21-May-31 18:07 static/js/ace/theme-sqlserver.js
+-rw-r--r--  3.0 unx     2236 tx defN 21-May-31 18:07 static/js/ace/mode-space.js
+-rw-r--r--  3.0 unx     5970 tx defN 21-May-31 18:07 static/js/ace/mode-hjson.js
+-rw-r--r--  3.0 unx    12546 tx defN 21-May-31 18:07 static/js/ace/mode-protobuf.js
+-rw-r--r--  3.0 unx     3138 tx defN 21-May-31 18:07 static/js/ace/theme-dreamweaver.js
+-rw-r--r--  3.0 unx     1099 tx defN 21-May-31 18:07 static/js/ace/mode-properties.js
+-rw-r--r--  3.0 unx    14198 tx defN 21-May-31 18:07 static/js/ace/mode-dart.js
+-rw-r--r--  3.0 unx    60415 tx defN 21-May-31 18:07 static/js/ace/mode-coldfusion.js
+-rw-r--r--  3.0 unx     4709 tx defN 21-May-31 18:07 static/js/ace/mode-abc.js
+-rw-r--r--  3.0 unx    10260 tx defN 21-May-31 18:07 static/js/ace/mode-praat.js
+-rw-r--r--  3.0 unx     7539 tx defN 21-May-31 18:07 static/js/ace/mode-julia.js
+-rw-r--r--  3.0 unx     2913 tx defN 21-May-31 18:07 static/js/ace/theme-terminal.js
+-rw-r--r--  3.0 unx     2409 tx defN 21-May-31 18:07 static/js/ace/mode-diff.js
+-rw-r--r--  3.0 unx    12293 tx defN 21-May-31 18:07 static/js/ace/ext-settings_menu.js
+-rw-r--r--  3.0 unx    10785 tx defN 21-May-31 18:07 static/js/ace/mode-drools.js
+-rw-r--r--  3.0 unx    55541 tx defN 21-May-31 18:07 static/js/ace/worker-xml.js
+-rw-r--r--  3.0 unx    64984 tx defN 21-May-31 18:07 static/js/ace/mode-razor.js
+-rw-r--r--  3.0 unx    66385 tx defN 21-May-31 18:07 static/js/ace/mode-soy_template.js
+-rw-r--r--  3.0 unx    19962 tx defN 21-May-31 18:07 static/js/ace/mode-live_script.js
+-rw-r--r--  3.0 unx   230322 tx defN 21-May-31 18:07 static/js/ace/mode-xquery.js
+-rw-r--r--  3.0 unx        0 bx stor 21-May-31 18:07 static/js/ace/mode-text.js
+-rw-r--r--  3.0 unx     3994 tx defN 21-May-31 18:07 static/js/ace/mode-yaml.js
+-rw-r--r--  3.0 unx     6989 tx defN 21-May-31 18:07 static/js/ace/mode-forth.js
+-rw-r--r--  3.0 unx     2633 tx defN 21-May-31 18:07 static/js/ace/theme-pastel_on_dark.js
+-rw-r--r--  3.0 unx   354781 tx defN 21-May-31 18:07 static/js/ace/ace.js
+-rw-r--r--  3.0 unx     1762 tx defN 21-May-31 18:07 static/js/ace/mode-ada.js
+-rw-r--r--  3.0 unx     6211 tx defN 21-May-31 18:07 static/js/ace/mode-bro.js
+-rw-r--r--  3.0 unx     8898 tx defN 21-May-31 18:07 static/js/ace/mode-assembly_x86.js
+-rw-r--r--  3.0 unx    31988 tx defN 21-May-31 18:07 static/js/ace/mode-svg.js
+-rw-r--r--  3.0 unx     6913 tx defN 21-May-31 18:07 static/js/ace/mode-golang.js
+-rw-r--r--  3.0 unx    24465 tx defN 21-May-31 18:07 static/js/ace/keybinding-emacs.js
+-rw-r--r--  3.0 unx     9112 tx defN 21-May-31 18:07 static/js/ace/ext-textarea.js
+-rw-r--r--  3.0 unx     2054 tx defN 21-May-31 18:07 static/js/ace/theme-kuroir.js
+-rw-r--r--  3.0 unx    20269 tx defN 21-May-31 18:07 static/js/ace/mode-wollok.js
+-rw-r--r--  3.0 unx    20567 tx defN 21-May-31 18:07 static/js/ace/mode-matlab.js
+-rw-r--r--  3.0 unx    20085 tx defN 21-May-31 18:07 static/js/ace/mode-less.js
+-rw-r--r--  3.0 unx     2088 tx defN 21-May-31 18:07 static/js/ace/mode-vhdl.js
+-rw-r--r--  3.0 unx     2572 tx defN 21-May-31 18:07 static/js/ace/ext-whitespace.js
+-rw-r--r--  3.0 unx     8226 tx defN 21-May-31 18:07 static/js/ace/mode-dockerfile.js
+-rw-r--r--  3.0 unx     2312 tx defN 21-May-31 18:07 static/js/ace/theme-solarized_dark.js
+-rw-r--r--  3.0 unx     4984 tx defN 21-May-31 18:07 static/js/ace/mode-livescript.js
+-rw-r--r--  3.0 unx     5399 tx defN 21-May-31 18:07 static/js/ace/mode-applescript.js
+-rw-r--r--  3.0 unx    10005 tx defN 21-May-31 18:07 static/js/ace/ext-searchbox.js
+-rw-r--r--  3.0 unx     6965 tx defN 21-May-31 18:07 static/js/ace/mode-jsx.js
+-rw-r--r--  3.0 unx    66336 tx defN 21-May-31 18:07 static/js/ace/mode-luapage.js
+-rw-r--r--  3.0 unx    10840 tx defN 21-May-31 18:07 static/js/ace/mode-c_cpp.js
+-rw-r--r--  3.0 unx     7416 tx defN 21-May-31 18:07 static/js/ace/mode-coffee.js
+-rw-r--r--  3.0 unx    58909 tx defN 21-May-31 18:07 static/js/ace/mode-curly.js
+-rw-r--r--  3.0 unx    20510 tx defN 21-May-31 18:07 static/js/ace/mode-tsx.js
+-rw-r--r--  3.0 unx    13909 tx defN 21-May-31 18:07 static/js/ace/mode-apache_conf.js
+-rw-r--r--  3.0 unx    59769 tx defN 21-May-31 18:07 static/js/ace/mode-handlebars.js
+-rw-r--r--  3.0 unx     3031 tx defN 21-May-31 18:07 static/js/ace/theme-tomorrow_night_blue.js
+-rw-r--r--  3.0 unx     6476 tx defN 21-May-31 18:07 static/js/ace/theme-iplastic.js
+-rw-r--r--  3.0 unx     2296 tx defN 21-May-31 18:07 static/js/ace/theme-kr_theme.js
+-rw-r--r--  3.0 unx     2710 tx defN 21-May-31 18:07 static/js/ace/mode-ini.js
+-rw-r--r--  3.0 unx     6523 tx defN 21-May-31 18:07 static/js/ace/mode-mysql.js
+-rw-r--r--  3.0 unx     2761 tx defN 21-May-31 18:07 static/js/ace/mode-tex.js
+-rw-r--r--  3.0 unx     2499 tx defN 21-May-31 18:07 static/js/ace/theme-twilight.js
+-rw-r--r--  3.0 unx     8428 tx defN 21-May-31 18:07 static/js/ace/mode-fortran.js
+-rw-r--r--  3.0 unx     5764 tx defN 21-May-31 18:07 static/js/ace/mode-jack.js
+-rw-r--r--  3.0 unx     3818 tx defN 21-May-31 18:07 static/js/ace/ext-beautify.js
+-rw-r--r--  3.0 unx      506 tx defN 21-May-31 18:07 static/js/ace/mode-plain_text.js
+-rw-r--r--  3.0 unx     3003 tx defN 21-May-31 18:07 static/js/ace/mode-cirru.js
+-rw-r--r--  3.0 unx     3126 tx defN 21-May-31 18:07 static/js/ace/theme-katzenmilch.js
+-rw-r--r--  3.0 unx     6120 tx defN 21-May-31 18:07 static/js/ace/mode-tcl.js
+-rw-r--r--  3.0 unx    57890 tx defN 21-May-31 18:07 static/js/ace/mode-html.js
+-rw-r--r--  3.0 unx     2380 tx defN 21-May-31 18:07 static/js/ace/mode-gherkin.js
+-rw-r--r--  3.0 unx     3729 tx defN 21-May-31 18:07 static/js/ace/ext-modelist.js
+-rw-r--r--  3.0 unx     2353 tx defN 21-May-31 18:07 static/js/ace/theme-cobalt.js
+-rw-r--r--  3.0 unx    18060 tx defN 21-May-31 18:07 static/js/ace/mode-javascript.js
+-rw-r--r--  3.0 unx    16415 tx defN 21-May-31 18:07 static/js/ace/mode-sqlserver.js
+-rw-r--r--  3.0 unx     2432 tx defN 21-May-31 18:07 static/js/ace/theme-clouds_midnight.js
+-rw-r--r--  3.0 unx    20545 tx defN 21-May-31 18:07 static/js/ace/mode-actionscript.js
+-rw-r--r--  3.0 unx    30271 tx defN 21-May-31 18:07 static/js/ace/mode-liquid.js
+-rw-r--r--  3.0 unx    47114 tx defN 21-May-31 18:07 static/js/ace/worker-lua.js
+-rw-r--r--  3.0 unx     6712 tx defN 21-May-31 18:07 static/js/ace/mode-mushcode.js
+-rw-r--r--  3.0 unx    34689 tx defN 21-May-31 18:07 static/js/ace/mode-jsp.js
+-rw-r--r--  3.0 unx    49991 tx defN 21-May-31 18:07 static/js/ace/mode-jade.js
+-rw-r--r--  3.0 unx     2282 tx defN 21-May-31 18:07 static/js/ace/mode-haskell_cabal.js
+-rw-r--r--  3.0 unx     3658 tx defN 21-May-31 18:07 static/js/ace/mode-scheme.js
+-rw-r--r--  3.0 unx    20198 tx defN 21-May-31 18:07 static/js/ace/mode-typescript.js
+-rw-r--r--  3.0 unx    11914 tx defN 21-May-31 18:07 static/js/ace/ext-old_ie.js
+-rw-r--r--  3.0 unx    10035 tx defN 21-May-31 18:07 static/js/ace/mode-nsis.js
+-rw-r--r--  3.0 unx    11468 tx defN 21-May-31 18:07 static/js/ace/mode-haskell.js
+-rw-r--r--  3.0 unx      899 tx defN 21-May-31 18:07 static/js/ace/mode-gitignore.js
+-rw-r--r--  3.0 unx    62955 tx defN 21-May-31 18:07 static/js/ace/mode-rhtml.js
+-rw-r--r--  3.0 unx    27779 tx defN 21-May-31 18:07 static/js/ace/theme-ambiance.js
+-rw-r--r--  3.0 unx     6929 tx defN 21-May-31 18:07 static/js/ace/mode-swift.js
+-rw-r--r--  3.0 unx     8947 tx defN 21-May-31 18:07 static/js/ace/mode-d.js
+-rw-r--r--  3.0 unx     4559 tx defN 21-May-31 18:07 static/js/ace/mode-pascal.js
+-rw-r--r--  3.0 unx     2313 tx defN 21-May-31 18:07 static/js/ace/mode-cobol.js
+-rw-r--r--  3.0 unx     2125 tx defN 21-May-31 18:07 static/js/ace/theme-eclipse.js
+-rw-r--r--  3.0 unx    78297 tx defN 21-May-31 18:07 static/js/ace/worker-php.js
+-rw-r--r--  3.0 unx   232939 tx defN 21-May-31 18:07 static/js/ace/mode-jsoniq.js
+-rw-r--r--  3.0 unx     5665 tx defN 21-May-31 18:07 static/js/ace/mode-io.js
+-rw-r--r--  3.0 unx      825 tx defN 21-May-31 18:07 static/js/ace/ext-linking.js
+-rw-r--r--  3.0 unx     2842 tx defN 21-May-31 18:07 static/js/ace/theme-chaos.js
+-rw-r--r--  3.0 unx    32911 tx defN 21-May-31 18:07 static/js/ace/worker-json.js
+-rw-r--r--  3.0 unx     2712 tx defN 21-May-31 18:07 static/js/ace/theme-chrome.js
+-rw-r--r--  3.0 unx    32692 tx defN 21-May-31 18:07 static/js/ace/mode-powershell.js
+-rw-r--r--  3.0 unx    61356 tx defN 21-May-31 18:07 static/js/ace/mode-smarty.js
+-rw-r--r--  3.0 unx     4104 bx defN 21-May-31 18:07 static/js/ace/mode-c9search.js
+-rw-r--r--  3.0 unx     5073 tx defN 21-May-31 18:07 static/js/ace/mode-vbscript.js
+-rw-r--r--  3.0 unx    18046 tx defN 21-May-31 18:07 static/js/ace/mode-css.js
+-rw-r--r--  3.0 unx    11847 tx defN 21-May-31 18:07 static/js/ace/mode-xml.js
+-rw-r--r--  3.0 unx   140879 tx defN 21-May-31 18:07 static/js/ace/worker-css.js
+-rw-r--r--  3.0 unx    21805 tx defN 21-May-31 18:07 static/js/ace/mode-java.js
+-rw-r--r--  3.0 unx     2081 tx defN 21-May-31 18:07 static/js/ace/theme-clouds.js
+-rw-r--r--  3.0 unx     2556 tx defN 21-May-31 18:07 static/js/ace/theme-tomorrow.js
+-rw-r--r--  3.0 unx    10220 tx defN 21-May-31 18:07 static/js/ace/mode-sass.js
+-rw-r--r--  3.0 unx     6554 tx defN 21-May-31 18:07 static/js/ace/mode-makefile.js
+-rw-r--r--  3.0 unx     4856 tx defN 21-May-31 18:07 static/js/ace/mode-batchfile.js
+-rw-r--r--  3.0 unx    15753 tx defN 21-May-31 18:07 static/js/ace/mode-elixir.js
+-rw-r--r--  3.0 unx    63640 tx defN 21-May-31 18:07 static/js/ace/mode-autohotkey.js
+-rw-r--r--  3.0 unx     2248 tx defN 21-May-31 18:07 static/js/ace/theme-idle_fingers.js
+-rw-r--r--  3.0 unx    13008 tx defN 21-May-31 18:07 static/js/ace/mode-glsl.js
+-rw-r--r--  3.0 unx     4681 tx defN 21-May-31 18:07 static/js/ace/mode-python.js
+-rw-r--r--  3.0 unx    13129 tx defN 21-May-31 18:07 static/js/ace/mode-nix.js
+-rw-r--r--  3.0 unx    59262 tx defN 21-May-31 18:07 static/js/ace/mode-django.js
+-rw-r--r--  3.0 unx     7283 tx defN 21-May-31 18:07 static/js/ace/mode-lua.js
+-rw-r--r--  3.0 unx     2360 tx defN 21-May-31 18:07 static/js/ace/theme-solarized_light.js
+-rw-r--r--  3.0 unx     1918 tx defN 21-May-31 18:07 static/js/ace/theme-xcode.js
+-rw-r--r--  3.0 unx     6360 tx defN 21-May-31 18:07 static/js/ace/ext-chromevox.js
+-rw-r--r--  3.0 unx    61525 tx defN 21-May-31 18:07 static/js/ace/mode-twig.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/elm.js
+-rw-r--r--  3.0 unx      143 tx defN 21-May-31 18:07 static/js/ace/snippets/typescript.js
+-rw-r--r--  3.0 unx      143 tx defN 21-May-31 18:07 static/js/ace/snippets/handlebars.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/mysql.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/cobol.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/sass.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/haxe.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/ini.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/twig.js
+-rw-r--r--  3.0 unx     2040 tx defN 21-May-31 18:07 static/js/ace/snippets/clojure.js
+-rw-r--r--  3.0 unx      134 tx defN 21-May-31 18:07 static/js/ace/snippets/live_script.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/swift.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/ocaml.js
+-rw-r--r--  3.0 unx      143 tx defN 21-May-31 18:07 static/js/ace/snippets/plain_text.js
+-rw-r--r--  3.0 unx     3127 tx defN 21-May-31 18:07 static/js/ace/snippets/vala.js
+-rw-r--r--  3.0 unx    35423 tx defN 21-May-31 18:07 static/js/ace/snippets/lsl.js
+-rw-r--r--  3.0 unx      942 tx defN 21-May-31 18:07 static/js/ace/snippets/sql.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/less.js
+-rw-r--r--  3.0 unx     1973 tx defN 21-May-31 18:07 static/js/ace/snippets/markdown.js
+-rw-r--r--  3.0 unx      135 tx defN 21-May-31 18:07 static/js/ace/snippets/liquid.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/space.js
+-rw-r--r--  3.0 unx      135 tx defN 21-May-31 18:07 static/js/ace/snippets/golang.js
+-rw-r--r--  3.0 unx      143 tx defN 21-May-31 18:07 static/js/ace/snippets/properties.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/vhdl.js
+-rw-r--r--  3.0 unx      139 tx defN 21-May-31 18:07 static/js/ace/snippets/vbscript.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/ftl.js
+-rw-r--r--  3.0 unx     2233 tx defN 21-May-31 18:07 static/js/ace/snippets/coffee.js
+-rw-r--r--  3.0 unx      135 tx defN 21-May-31 18:07 static/js/ace/snippets/lucene.js
+-rw-r--r--  3.0 unx     1319 tx defN 21-May-31 18:07 static/js/ace/snippets/dart.js
+-rw-r--r--  3.0 unx      151 tx defN 21-May-31 18:07 static/js/ace/snippets/mips_assembler.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/pgsql.js
+-rw-r--r--  3.0 unx     2630 tx defN 21-May-31 18:07 static/js/ace/snippets/r.js
+-rw-r--r--  3.0 unx      442 tx defN 21-May-31 18:07 static/js/ace/snippets/rst.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/dot.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/xml.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/scala.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/text.js
+-rw-r--r--  3.0 unx      128 tx defN 21-May-31 18:07 static/js/ace/snippets/hjson.js
+-rw-r--r--  3.0 unx      139 tx defN 21-May-31 18:07 static/js/ace/snippets/asciidoc.js
+-rw-r--r--  3.0 unx      145 tx defN 21-May-31 18:07 static/js/ace/snippets/apache_conf.js
+-rw-r--r--  3.0 unx      164 tx defN 21-May-31 18:07 static/js/ace/snippets/razor.js
+-rw-r--r--  3.0 unx     3840 tx defN 21-May-31 18:07 static/js/ace/snippets/javascript.js
+-rw-r--r--  3.0 unx      135 tx defN 21-May-31 18:07 static/js/ace/snippets/scheme.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/curly.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/glsl.js
+-rw-r--r--  3.0 unx      370 tx defN 21-May-31 18:07 static/js/ace/snippets/drools.js
+-rw-r--r--  3.0 unx     2055 tx defN 21-May-31 18:07 static/js/ace/snippets/sh.js
+-rw-r--r--  3.0 unx      551 tx defN 21-May-31 18:07 static/js/ace/snippets/diff.js
+-rw-r--r--  3.0 unx      141 tx defN 21-May-31 18:07 static/js/ace/snippets/html_ruby.js
+-rw-r--r--  3.0 unx      126 tx defN 21-May-31 18:07 static/js/ace/snippets/bro.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/ejs.js
+-rw-r--r--  3.0 unx     1716 tx defN 21-May-31 18:07 static/js/ace/snippets/jsoniq.js
+-rw-r--r--  3.0 unx     1263 tx defN 21-May-31 18:07 static/js/ace/snippets/wollok.js
+-rw-r--r--  3.0 unx      135 tx defN 21-May-31 18:07 static/js/ace/snippets/smarty.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/json.js
+-rw-r--r--  3.0 unx     2663 tx defN 21-May-31 18:07 static/js/ace/snippets/c_cpp.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/gcode.js
+-rw-r--r--  3.0 unx      141 tx defN 21-May-31 18:07 static/js/ace/snippets/batchfile.js
+-rw-r--r--  3.0 unx    19650 tx defN 21-May-31 18:07 static/js/ace/snippets/css.js
+-rw-r--r--  3.0 unx     5513 tx defN 21-May-31 18:07 static/js/ace/snippets/perl.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/nix.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/abap.js
+-rw-r--r--  3.0 unx    18271 tx defN 21-May-31 18:07 static/js/ace/snippets/html.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/lisp.js
+-rw-r--r--  3.0 unx      137 tx defN 21-May-31 18:07 static/js/ace/snippets/verilog.js
+-rw-r--r--  3.0 unx      947 tx defN 21-May-31 18:07 static/js/ace/snippets/abc.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/kotlin.js
+-rw-r--r--  3.0 unx      508 tx defN 21-May-31 18:07 static/js/ace/snippets/lua.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/jsx.js
+-rw-r--r--  3.0 unx      139 tx defN 21-May-31 18:07 static/js/ace/snippets/c9search.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/mask.js
+-rw-r--r--  3.0 unx      147 tx defN 21-May-31 18:07 static/js/ace/snippets/assembly_x86.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/jack.js
+-rw-r--r--  3.0 unx      297 tx defN 21-May-31 18:07 static/js/ace/snippets/snippets.js
+-rw-r--r--  3.0 unx      136 tx defN 21-May-31 18:07 static/js/ace/snippets/mipsassembler.js
+-rw-r--r--  3.0 unx     4000 tx defN 21-May-31 18:07 static/js/ace/snippets/django.js
+-rw-r--r--  3.0 unx      448 tx defN 21-May-31 18:07 static/js/ace/snippets/haml.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/scad.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/elixir.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/toml.js
+-rw-r--r--  3.0 unx    21279 tx defN 21-May-31 18:07 static/js/ace/snippets/ruby.js
+-rw-r--r--  3.0 unx      143 tx defN 21-May-31 18:07 static/js/ace/snippets/coldfusion.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/praat.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/forth.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/mel.js
+-rw-r--r--  3.0 unx      135 tx defN 21-May-31 18:07 static/js/ace/snippets/groovy.js
+-rw-r--r--  3.0 unx      135 tx defN 21-May-31 18:07 static/js/ace/snippets/prolog.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/rdoc.js
+-rw-r--r--  3.0 unx      137 tx defN 21-May-31 18:07 static/js/ace/snippets/luapage.js
+-rw-r--r--  3.0 unx     2973 tx defN 21-May-31 18:07 static/js/ace/snippets/actionscript.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/tsx.js
+-rw-r--r--  3.0 unx      145 tx defN 21-May-31 18:07 static/js/ace/snippets/applescript.js
+-rw-r--r--  3.0 unx      607 tx defN 21-May-31 18:07 static/js/ace/snippets/gobstones.js
+-rw-r--r--  3.0 unx     3574 tx defN 21-May-31 18:07 static/js/ace/snippets/erlang.js
+-rw-r--r--  3.0 unx     6763 tx defN 21-May-31 18:07 static/js/ace/snippets/php.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/swig.js
+-rw-r--r--  3.0 unx      135 tx defN 21-May-31 18:07 static/js/ace/snippets/pascal.js
+-rw-r--r--  3.0 unx      143 tx defN 21-May-31 18:07 static/js/ace/snippets/autohotkey.js
+-rw-r--r--  3.0 unx      139 tx defN 21-May-31 18:07 static/js/ace/snippets/mushcode.js
+-rw-r--r--  3.0 unx      135 tx defN 21-May-31 18:07 static/js/ace/snippets/logiql.js
+-rw-r--r--  3.0 unx      540 tx defN 21-May-31 18:07 static/js/ace/snippets/textile.js
+-rw-r--r--  3.0 unx      132 tx defN 21-May-31 18:07 static/js/ace/snippets/protobuf.js
+-rw-r--r--  3.0 unx      147 tx defN 21-May-31 18:07 static/js/ace/snippets/soy_template.js
+-rw-r--r--  3.0 unx      145 tx defN 21-May-31 18:07 static/js/ace/snippets/html_elixir.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/rust.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/sjs.js
+-rw-r--r--  3.0 unx      143 tx defN 21-May-31 18:07 static/js/ace/snippets/livescript.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/julia.js
+-rw-r--r--  3.0 unx      270 tx defN 21-May-31 18:07 static/js/ace/snippets/maze.js
+-rw-r--r--  3.0 unx     3636 tx defN 21-May-31 18:07 static/js/ace/snippets/tex.js
+-rw-r--r--  3.0 unx     3672 tx defN 21-May-31 18:07 static/js/ace/snippets/python.js
+-rw-r--r--  3.0 unx      141 tx defN 21-May-31 18:07 static/js/ace/snippets/gitignore.js
+-rw-r--r--  3.0 unx     2778 tx defN 21-May-31 18:07 static/js/ace/snippets/jsp.js
+-rw-r--r--  3.0 unx     1975 tx defN 21-May-31 18:07 static/js/ace/snippets/haskell.js
+-rw-r--r--  3.0 unx     1690 tx defN 21-May-31 18:07 static/js/ace/snippets/tcl.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/scss.js
+-rw-r--r--  3.0 unx     1219 tx defN 21-May-31 18:07 static/js/ace/snippets/io.js
+-rw-r--r--  3.0 unx      137 tx defN 21-May-31 18:07 static/js/ace/snippets/fortran.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/svg.js
+-rw-r--r--  3.0 unx     2139 tx defN 21-May-31 18:07 static/js/ace/snippets/sqlserver.js
+-rw-r--r--  3.0 unx      137 tx defN 21-May-31 18:07 static/js/ace/snippets/gherkin.js
+-rw-r--r--  3.0 unx      143 tx defN 21-May-31 18:07 static/js/ace/snippets/powershell.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/cirru.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/jade.js
+-rw-r--r--  3.0 unx      198 tx defN 21-May-31 18:07 static/js/ace/snippets/makefile.js
+-rw-r--r--  3.0 unx      135 tx defN 21-May-31 18:07 static/js/ace/snippets/stylus.js
+-rw-r--r--  3.0 unx      651 tx defN 21-May-31 18:07 static/js/ace/snippets/velocity.js
+-rw-r--r--  3.0 unx     1716 tx defN 21-May-31 18:07 static/js/ace/snippets/xquery.js
+-rw-r--r--  3.0 unx      135 tx defN 21-May-31 18:07 static/js/ace/snippets/csharp.js
+-rw-r--r--  3.0 unx      143 tx defN 21-May-31 18:07 static/js/ace/snippets/dockerfile.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/rhtml.js
+-rw-r--r--  3.0 unx      125 tx defN 21-May-31 18:07 static/js/ace/snippets/d.js
+-rw-r--r--  3.0 unx      133 tx defN 21-May-31 18:07 static/js/ace/snippets/latex.js
+-rw-r--r--  3.0 unx      127 tx defN 21-May-31 18:07 static/js/ace/snippets/nsis.js
+-rw-r--r--  3.0 unx      135 tx defN 21-May-31 18:07 static/js/ace/snippets/matlab.js
+-rw-r--r--  3.0 unx      143 tx defN 21-May-31 18:07 static/js/ace/snippets/objectivec.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/lean.js
+-rw-r--r--  3.0 unx     4322 tx defN 21-May-31 18:07 static/js/ace/snippets/java.js
+-rw-r--r--  3.0 unx      135 tx defN 21-May-31 18:07 static/js/ace/snippets/eiffel.js
+-rw-r--r--  3.0 unx      129 tx defN 21-May-31 18:07 static/js/ace/snippets/ada.js
+-rw-r--r--  3.0 unx      149 tx defN 21-May-31 18:07 static/js/ace/snippets/haskell_cabal.js
+-rw-r--r--  3.0 unx      131 tx defN 21-May-31 18:07 static/js/ace/snippets/yaml.js
+-rw-r--r--  3.0 unx     3840 tx defN 21-May-31 18:07 static/js/ace/ext-elastic_tabstops_lite.js
+-rw-r--r--  3.0 unx     2236 tx defN 21-May-31 18:07 static/js/ace/theme-merbivore.js
+-rw-r--r--  3.0 unx     3687 tx defN 21-May-31 18:07 static/js/ace/mode-snippets.js
+-rw-r--r--  3.0 unx     2819 tx defN 21-May-31 18:07 static/js/ace/ext-static_highlight.js
+-rw-r--r--  3.0 unx    34464 tx defN 21-May-31 18:07 static/js/ace/ext-language_tools.js
+-rw-r--r--  3.0 unx     5959 tx defN 21-May-31 18:07 static/js/ace/mode-mips_assembler.js
+-rw-r--r--  3.0 unx    22440 tx defN 21-May-31 18:07 static/js/ace/mode-groovy.js
+-rw-r--r--  3.0 unx    55911 tx defN 21-May-31 18:07 static/js/ace/mode-pgsql.js
+-rw-r--r--  3.0 unx    64800 tx defN 21-May-31 18:07 static/js/ace/mode-markdown.js
+-rw-r--r--  3.0 unx     6520 tx defN 21-May-31 18:07 static/js/ace/mode-scad.js
+-rw-r--r--  3.0 unx    12235 tx defN 21-May-31 18:07 static/js/ace/mode-stylus.js
+-rw-r--r--  3.0 unx    15600 tx defN 21-May-31 18:07 static/js/ace/mode-ocaml.js
+-rw-r--r--  3.0 unx    31151 tx defN 21-May-31 18:07 static/js/ace/mode-swig.js
+-rw-r--r--  3.0 unx     6540 tx defN 21-May-31 18:07 static/js/ace/mode-haxe.js
+-rw-r--r--  3.0 unx     4881 tx defN 21-May-31 18:07 static/js/ace/mode-maze.js
+-rw-r--r--  3.0 unx    12951 tx defN 21-May-31 18:07 static/js/ace/mode-scss.js
+-rw-r--r--  3.0 unx     6495 tx defN 21-May-31 18:07 static/js/ace/mode-rust.js
+-rw-r--r--  3.0 unx     3994 tx defN 21-May-31 18:07 static/js/ace/mode-rdoc.js
+-rw-r--r--  3.0 unx     2844 tx defN 21-May-31 18:07 static/js/ace/mode-eiffel.js
+-rw-r--r--  3.0 unx     3874 tx defN 21-May-31 18:07 static/js/ace/mode-latex.js
+-rw-r--r--  3.0 unx    22619 tx defN 21-May-31 18:07 static/js/ace/mode-scala.js
+-rw-r--r--  3.0 unx     7595 tx defN 21-May-31 18:07 static/js/ace/mode-dot.js
+-rw-r--r--  3.0 unx     7382 tx defN 21-May-31 18:07 static/js/ace/mode-perl.js
+-rw-r--r--  3.0 unx    54512 tx defN 21-May-31 18:07 static/js/ace/mode-objectivec.js
+-rw-r--r--  3.0 unx   217401 tx defN 21-May-31 18:07 static/js/ace/worker-html.js
+-rw-r--r--  3.0 unx     2448 tx defN 21-May-31 18:07 static/js/ace/theme-merbivore_soft.js
+-rw-r--r--  3.0 unx    62630 tx defN 21-May-31 18:07 static/js/ace/mode-velocity.js
+-rw-r--r--  3.0 unx     2204 tx defN 21-May-31 18:07 static/js/ace/theme-vibrant_ink.js
+-rw-r--r--  3.0 unx     8028 tx defN 21-May-31 18:07 static/js/ace/mode-clojure.js
+-rw-r--r--  3.0 unx   470435 tx defN 21-May-31 18:07 static/js/ace/mode-php.js
+-rw-r--r--  3.0 unx     2375 tx defN 21-May-31 18:07 static/js/ace/theme-monokai.js
+-rw-r--r--  3.0 unx    21478 tx defN 21-May-31 18:07 static/js/ace/ext-emmet.js
+-rw-r--r--  3.0 unx     8159 tx defN 21-May-31 18:07 static/js/ace/mode-asciidoc.js
+-rw-r--r--  3.0 unx     8840 tx defN 21-May-31 18:07 static/js/ace/mode-csharp.js
+-rw-r--r--  3.0 unx     3221 tx defN 21-May-31 18:07 static/js/ace/theme-tomorrow_night_eighties.js
+-rw-r--r--  3.0 unx     1811 tx defN 21-May-31 18:07 static/js/ace/mode-sql.js
+-rw-r--r--  3.0 unx     1440 bx defN 21-May-31 18:07 static/js/ace/ext-spellcheck.js
+-rw-r--r--  3.0 unx     3496 tx defN 21-May-31 18:07 static/js/ace/theme-tomorrow_night_bright.js
+-rw-r--r--  3.0 unx    30624 tx defN 21-May-31 18:07 static/js/ace/mode-ftl.js
+-rw-r--r--  3.0 unx    96918 tx defN 21-May-31 18:07 static/js/ace/keybinding-vim.js
+-rw-r--r--  3.0 unx     3189 tx defN 21-May-31 18:07 static/js/ace/mode-mipsassembler.js
+-rw-r--r--  3.0 unx     5005 tx defN 21-May-31 18:07 static/js/ace/mode-r.js
+-rw-r--r--  3.0 unx     5576 tx defN 21-May-31 18:07 static/js/ace/mode-lean.js
+-rw-r--r--  3.0 unx     2204 tx defN 21-May-31 18:07 static/js/ace/mode-toml.js
+-rw-r--r--  3.0 unx    68741 tx defN 21-May-31 18:07 static/js/ace/mode-html_ruby.js
+-rw-r--r--  3.0 unx     1173 tx defN 21-May-31 18:07 static/js/ace/mode-lucene.js
+-rw-r--r--  3.0 unx      140 tx defN 21-May-31 18:07 static/js/ace/ext-error_marker.js
+-rw-r--r--  3.0 unx    11837 tx defN 21-May-31 18:07 static/js/ace/mode-kotlin.js
+-rw-r--r--  3.0 unx     3024 tx defN 21-May-31 18:07 static/js/ace/mode-rst.js
+-rw-r--r--  3.0 unx    10025 tx defN 21-May-31 18:07 static/js/ace/mode-ruby.js
+-rw-r--r--  3.0 unx    16578 tx defN 21-May-31 18:07 static/js/ace/mode-vala.js
+-rw-r--r--  3.0 unx     1088 tx defN 21-May-31 18:07 static/js/ace/ext-statusbar.js
+-rw-r--r--  3.0 unx    75093 tx defN 21-May-31 18:07 static/js/ace/mode-html_elixir.js
+-rw-r--r--  3.0 unx     5097 tx defN 21-May-31 18:07 static/js/ace/mode-json.js
+-rw-r--r--  3.0 unx    21273 tx defN 21-May-31 18:07 static/js/ace/mode-sjs.js
+-rw-r--r--  3.0 unx     2812 tx defN 21-May-31 18:07 static/js/ace/theme-crimson_editor.js
+-rw-r--r--  3.0 unx     2689 tx defN 21-May-31 18:07 static/js/ace/mode-verilog.js
+-rw-r--r--  3.0 unx    95432 tx defN 21-May-31 18:07 static/js/highlight.min.js
+-rw-r--r--  3.0 unx    88145 tx defN 21-May-31 18:07 static/js/jquery.min.js
+-rw-r--r--  3.0 unx    11826 tx defN 23-Mar-19 22:18 static/js/utils.js
+-rw-r--r--  3.0 unx    93670 tx defN 21-May-31 18:07 static/js/vue.min.js
+-rw-r--r--  3.0 unx    68547 tx defN 21-May-31 18:07 static/js/sugar.min.js
+-rw-r--r--  3.0 unx    14265 tx defN 21-May-31 18:07 static/js/axios.min.js
+-rw-r--r--  3.0 unx      493 tx defN 22-Mar-20 01:46 static/js/dbadmin.js
+-rw-rw-r--  3.0 unx     3362 tx defN 21-Jul-30 14:11 static/js/translations.js
+-rw-r--r--  3.0 unx      708 tx defN 21-May-31 18:07 static/css/gitlog.min.css
+-rw-rw-r--  3.0 unx     5744 tx defN 22-Jul-19 13:20 static/css/future.css
+-rw-r--r--  3.0 unx    12305 bx defN 21-May-31 18:07 static/images/alert-blue.gif
+-rw-r--r--  3.0 unx  1010153 bx defN 21-May-31 18:07 static/images/widget.gif
+-rw-r--r--  3.0 unx    13380 bx defN 21-May-31 18:07 static/images/alert-yellow.gif
+-rw-r--r--  3.0 unx    12025 bx defN 21-May-31 18:07 static/images/alert-red.gif
+-rw-r--r--  3.0 unx    11068 bx defN 21-May-31 18:07 static/images/alert-green.gif
+-rw-r--r--  3.0 unx     7927 bx defN 21-May-31 18:07 static/images/forkme.png
+-rw-r--r--  3.0 unx    13366 bx defN 21-May-31 18:07 static/images/alert-orange.gif
+-rw-r--r--  3.0 unx        1 tx stor 21-May-31 18:07 translations/README.md
 -rw-r--r--  3.0 unx    20255 tx defN 22-May-01 20:04 __init__.py
--rw-rw-r--  3.0 unx     2994 tx defN 22-Mar-20 01:11 templates/translations.html
--rw-rw-r--  3.0 unx    13886 tx defN 22-Mar-20 01:11 templates/index.html
--rw-rw-r--  3.0 unx     4849 tx defN 22-Mar-20 01:11 templates/gitlog.html
--rw-rw-r--  3.0 unx      993 tx defN 22-Mar-20 01:11 templates/dbadmin.html
--rw-r--r--  3.0 unx     1141 tx defN 19-Jul-23 06:13 templates/ticket.html
--rw-r--r--  3.0 unx     6493 tx defN 20-Aug-05 06:58 diff2kryten.py
--rw-r--r--  3.0 unx        1 tx stor 19-Jul-23 06:13 translations/README.md
-378 files, 7987585 bytes uncompressed, 2919909 bytes compressed:  63.4%
+-rw-r--r--  3.0 unx     6493 tx defN 21-May-31 18:07 diff2kryten.py
+-rw-r--r--  3.0 unx     4849 tx defN 21-May-31 18:07 templates/gitlog.html
+-rw-r--r--  3.0 unx     1141 tx defN 21-May-31 18:07 templates/ticket.html
+-rw-rw-r--  3.0 unx      993 tx defN 21-Sep-27 06:28 templates/dbadmin.html
+-rw-rw-r--  3.0 unx     2994 tx defN 21-Jul-30 14:11 templates/translations.html
+-rw-rw-r--  3.0 unx    13886 tx defN 22-Feb-13 18:38 templates/index.html
+378 files, 7987952 bytes uncompressed, 2920032 bytes compressed:  63.5%
```

#### zipnote {}

```diff
@@ -3,1133 +3,1133 @@
 
 Filename: static/components/mtable.js
 Comment: 
 
 Filename: static/components/mtable.html
 Comment: 
 
-Filename: static/images/alert-red.gif
+Filename: static/js/index.js
 Comment: 
 
-Filename: static/images/alert-blue.gif
+Filename: static/js/ace/ext-themelist.js
 Comment: 
 
-Filename: static/images/alert-orange.gif
+Filename: static/js/ace/mode-prolog.js
 Comment: 
 
-Filename: static/images/widget.gif
+Filename: static/js/ace/mode-lsl.js
 Comment: 
 
-Filename: static/images/forkme.png
+Filename: static/js/ace/mode-gobstones.js
 Comment: 
 
-Filename: static/images/alert-yellow.gif
+Filename: static/js/ace/mode-textile.js
 Comment: 
 
-Filename: static/images/alert-green.gif
+Filename: static/js/ace/theme-textmate.js
 Comment: 
 
-Filename: static/css/future.css
+Filename: static/js/ace/mode-logiql.js
 Comment: 
 
-Filename: static/css/gitlog.min.css
+Filename: static/js/ace/worker-xquery.js
 Comment: 
 
-Filename: static/js/index.js
+Filename: static/js/ace/worker-javascript.js
 Comment: 
 
-Filename: static/js/translations.js
+Filename: static/js/ace/theme-github.js
 Comment: 
 
-Filename: static/js/sugar.min.js
+Filename: static/js/ace/theme-dawn.js
 Comment: 
 
-Filename: static/js/ace/mode-d.js
+Filename: static/js/ace/mode-elm.js
 Comment: 
 
-Filename: static/js/ace/mode-php.js
+Filename: static/js/ace/mode-mel.js
 Comment: 
 
-Filename: static/js/ace/mode-rust.js
+Filename: static/js/ace/mode-mask.js
 Comment: 
 
-Filename: static/js/ace/mode-elm.js
+Filename: static/js/ace/ext-split.js
 Comment: 
 
-Filename: static/js/ace/ext-elastic_tabstops_lite.js
+Filename: static/js/ace/mode-abap.js
 Comment: 
 
-Filename: static/js/ace/mode-curly.js
+Filename: static/js/ace/theme-mono_industrial.js
 Comment: 
 
-Filename: static/js/ace/theme-mono_industrial.js
+Filename: static/js/ace/mode-lisp.js
 Comment: 
 
-Filename: static/js/ace/theme-textmate.js
+Filename: static/js/ace/mode-erlang.js
 Comment: 
 
-Filename: static/js/ace/theme-chrome.js
+Filename: static/js/ace/mode-sh.js
 Comment: 
 
-Filename: static/js/ace/mode-rhtml.js
+Filename: static/js/ace/mode-ejs.js
 Comment: 
 
-Filename: static/js/ace/mode-r.js
+Filename: static/js/ace/worker-coffee.js
 Comment: 
 
-Filename: static/js/ace/mode-ada.js
+Filename: static/js/ace/mode-haml.js
 Comment: 
 
-Filename: static/js/ace/mode-pascal.js
+Filename: static/js/ace/mode-gcode.js
 Comment: 
 
-Filename: static/js/ace/mode-ftl.js
+Filename: static/js/ace/theme-tomorrow_night.js
 Comment: 
 
-Filename: static/js/ace/ext-beautify.js
+Filename: static/js/ace/ext-keybinding_menu.js
 Comment: 
 
-Filename: static/js/ace/mode-gcode.js
+Filename: static/js/ace/theme-sqlserver.js
 Comment: 
 
-Filename: static/js/ace/worker-xquery.js
+Filename: static/js/ace/mode-space.js
 Comment: 
 
-Filename: static/js/ace/mode-jade.js
+Filename: static/js/ace/mode-hjson.js
 Comment: 
 
-Filename: static/js/ace/mode-less.js
+Filename: static/js/ace/mode-protobuf.js
 Comment: 
 
-Filename: static/js/ace/mode-autohotkey.js
+Filename: static/js/ace/theme-dreamweaver.js
 Comment: 
 
-Filename: static/js/ace/mode-mipsassembler.js
+Filename: static/js/ace/mode-properties.js
 Comment: 
 
-Filename: static/js/ace/ext-static_highlight.js
+Filename: static/js/ace/mode-dart.js
 Comment: 
 
-Filename: static/js/ace/mode-text.js
+Filename: static/js/ace/mode-coldfusion.js
 Comment: 
 
-Filename: static/js/ace/mode-diff.js
+Filename: static/js/ace/mode-abc.js
 Comment: 
 
-Filename: static/js/ace/mode-space.js
+Filename: static/js/ace/mode-praat.js
 Comment: 
 
-Filename: static/js/ace/mode-cobol.js
+Filename: static/js/ace/mode-julia.js
 Comment: 
 
-Filename: static/js/ace/ext-split.js
+Filename: static/js/ace/theme-terminal.js
 Comment: 
 
-Filename: static/js/ace/mode-rst.js
+Filename: static/js/ace/mode-diff.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow_night_blue.js
+Filename: static/js/ace/ext-settings_menu.js
 Comment: 
 
-Filename: static/js/ace/mode-mask.js
+Filename: static/js/ace/mode-drools.js
 Comment: 
 
-Filename: static/js/ace/mode-sqlserver.js
+Filename: static/js/ace/worker-xml.js
 Comment: 
 
-Filename: static/js/ace/mode-yaml.js
+Filename: static/js/ace/mode-razor.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow.js
+Filename: static/js/ace/mode-soy_template.js
 Comment: 
 
-Filename: static/js/ace/mode-actionscript.js
+Filename: static/js/ace/mode-live_script.js
 Comment: 
 
-Filename: static/js/ace/mode-twig.js
+Filename: static/js/ace/mode-xquery.js
 Comment: 
 
-Filename: static/js/ace/mode-golang.js
+Filename: static/js/ace/mode-text.js
 Comment: 
 
-Filename: static/js/ace/worker-json.js
+Filename: static/js/ace/mode-yaml.js
 Comment: 
 
-Filename: static/js/ace/ext-modelist.js
+Filename: static/js/ace/mode-forth.js
 Comment: 
 
-Filename: static/js/ace/mode-textile.js
+Filename: static/js/ace/theme-pastel_on_dark.js
 Comment: 
 
-Filename: static/js/ace/mode-tcl.js
+Filename: static/js/ace/ace.js
 Comment: 
 
-Filename: static/js/ace/mode-smarty.js
+Filename: static/js/ace/mode-ada.js
 Comment: 
 
-Filename: static/js/ace/theme-dreamweaver.js
+Filename: static/js/ace/mode-bro.js
 Comment: 
 
-Filename: static/js/ace/mode-c9search.js
+Filename: static/js/ace/mode-assembly_x86.js
 Comment: 
 
-Filename: static/js/ace/mode-kotlin.js
+Filename: static/js/ace/mode-svg.js
 Comment: 
 
-Filename: static/js/ace/theme-solarized_dark.js
+Filename: static/js/ace/mode-golang.js
 Comment: 
 
-Filename: static/js/ace/worker-xml.js
+Filename: static/js/ace/keybinding-emacs.js
 Comment: 
 
-Filename: static/js/ace/mode-eiffel.js
+Filename: static/js/ace/ext-textarea.js
 Comment: 
 
-Filename: static/js/ace/worker-css.js
+Filename: static/js/ace/theme-kuroir.js
 Comment: 
 
-Filename: static/js/ace/theme-clouds.js
+Filename: static/js/ace/mode-wollok.js
 Comment: 
 
-Filename: static/js/ace/mode-sjs.js
+Filename: static/js/ace/mode-matlab.js
 Comment: 
 
-Filename: static/js/ace/mode-dockerfile.js
+Filename: static/js/ace/mode-less.js
 Comment: 
 
-Filename: static/js/ace/mode-scheme.js
+Filename: static/js/ace/mode-vhdl.js
 Comment: 
 
-Filename: static/js/ace/mode-live_script.js
+Filename: static/js/ace/ext-whitespace.js
 Comment: 
 
-Filename: static/js/ace/mode-jsoniq.js
+Filename: static/js/ace/mode-dockerfile.js
 Comment: 
 
-Filename: static/js/ace/mode-haxe.js
+Filename: static/js/ace/theme-solarized_dark.js
 Comment: 
 
-Filename: static/js/ace/mode-wollok.js
+Filename: static/js/ace/mode-livescript.js
 Comment: 
 
-Filename: static/js/ace/theme-katzenmilch.js
+Filename: static/js/ace/mode-applescript.js
 Comment: 
 
-Filename: static/js/ace/theme-iplastic.js
+Filename: static/js/ace/ext-searchbox.js
 Comment: 
 
-Filename: static/js/ace/mode-perl.js
+Filename: static/js/ace/mode-jsx.js
 Comment: 
 
-Filename: static/js/ace/keybinding-emacs.js
+Filename: static/js/ace/mode-luapage.js
 Comment: 
 
-Filename: static/js/ace/mode-elixir.js
+Filename: static/js/ace/mode-c_cpp.js
 Comment: 
 
-Filename: static/js/ace/mode-gherkin.js
+Filename: static/js/ace/mode-coffee.js
 Comment: 
 
-Filename: static/js/ace/mode-java.js
+Filename: static/js/ace/mode-curly.js
 Comment: 
 
-Filename: static/js/ace/mode-jsp.js
+Filename: static/js/ace/mode-tsx.js
 Comment: 
 
-Filename: static/js/ace/theme-sqlserver.js
+Filename: static/js/ace/mode-apache_conf.js
 Comment: 
 
-Filename: static/js/ace/mode-csharp.js
+Filename: static/js/ace/mode-handlebars.js
 Comment: 
 
-Filename: static/js/ace/mode-gobstones.js
+Filename: static/js/ace/theme-tomorrow_night_blue.js
 Comment: 
 
-Filename: static/js/ace/mode-prolog.js
+Filename: static/js/ace/theme-iplastic.js
 Comment: 
 
-Filename: static/js/ace/theme-twilight.js
+Filename: static/js/ace/theme-kr_theme.js
 Comment: 
 
-Filename: static/js/ace/mode-properties.js
+Filename: static/js/ace/mode-ini.js
 Comment: 
 
-Filename: static/js/ace/mode-velocity.js
+Filename: static/js/ace/mode-mysql.js
 Comment: 
 
-Filename: static/js/ace/mode-stylus.js
+Filename: static/js/ace/mode-tex.js
 Comment: 
 
-Filename: static/js/ace/mode-html.js
+Filename: static/js/ace/theme-twilight.js
 Comment: 
 
-Filename: static/js/ace/worker-javascript.js
+Filename: static/js/ace/mode-fortran.js
 Comment: 
 
-Filename: static/js/ace/mode-powershell.js
+Filename: static/js/ace/mode-jack.js
 Comment: 
 
-Filename: static/js/ace/mode-hjson.js
+Filename: static/js/ace/ext-beautify.js
 Comment: 
 
-Filename: static/js/ace/mode-latex.js
+Filename: static/js/ace/mode-plain_text.js
 Comment: 
 
-Filename: static/js/ace/theme-xcode.js
+Filename: static/js/ace/mode-cirru.js
 Comment: 
 
-Filename: static/js/ace/mode-ocaml.js
+Filename: static/js/ace/theme-katzenmilch.js
 Comment: 
 
-Filename: static/js/ace/mode-clojure.js
+Filename: static/js/ace/mode-tcl.js
 Comment: 
 
-Filename: static/js/ace/mode-makefile.js
+Filename: static/js/ace/mode-html.js
 Comment: 
 
-Filename: static/js/ace/worker-coffee.js
+Filename: static/js/ace/mode-gherkin.js
 Comment: 
 
-Filename: static/js/ace/mode-applescript.js
+Filename: static/js/ace/ext-modelist.js
 Comment: 
 
-Filename: static/js/ace/mode-dot.js
+Filename: static/js/ace/theme-cobalt.js
 Comment: 
 
-Filename: static/js/ace/snippets/objectivec.js
+Filename: static/js/ace/mode-javascript.js
 Comment: 
 
-Filename: static/js/ace/snippets/gobstones.js
+Filename: static/js/ace/mode-sqlserver.js
 Comment: 
 
-Filename: static/js/ace/snippets/kotlin.js
+Filename: static/js/ace/theme-clouds_midnight.js
 Comment: 
 
-Filename: static/js/ace/snippets/hjson.js
+Filename: static/js/ace/mode-actionscript.js
 Comment: 
 
-Filename: static/js/ace/snippets/assembly_x86.js
+Filename: static/js/ace/mode-liquid.js
 Comment: 
 
-Filename: static/js/ace/snippets/ruby.js
+Filename: static/js/ace/worker-lua.js
 Comment: 
 
-Filename: static/js/ace/snippets/logiql.js
+Filename: static/js/ace/mode-mushcode.js
 Comment: 
 
-Filename: static/js/ace/snippets/text.js
+Filename: static/js/ace/mode-jsp.js
 Comment: 
 
-Filename: static/js/ace/snippets/html_ruby.js
+Filename: static/js/ace/mode-jade.js
 Comment: 
 
-Filename: static/js/ace/snippets/php.js
+Filename: static/js/ace/mode-haskell_cabal.js
 Comment: 
 
-Filename: static/js/ace/snippets/makefile.js
+Filename: static/js/ace/mode-scheme.js
 Comment: 
 
-Filename: static/js/ace/snippets/vbscript.js
+Filename: static/js/ace/mode-typescript.js
 Comment: 
 
-Filename: static/js/ace/snippets/snippets.js
+Filename: static/js/ace/ext-old_ie.js
 Comment: 
 
-Filename: static/js/ace/snippets/haml.js
+Filename: static/js/ace/mode-nsis.js
 Comment: 
 
-Filename: static/js/ace/snippets/json.js
+Filename: static/js/ace/mode-haskell.js
 Comment: 
 
-Filename: static/js/ace/snippets/svg.js
+Filename: static/js/ace/mode-gitignore.js
 Comment: 
 
-Filename: static/js/ace/snippets/drools.js
+Filename: static/js/ace/mode-rhtml.js
 Comment: 
 
-Filename: static/js/ace/snippets/haskell.js
+Filename: static/js/ace/theme-ambiance.js
 Comment: 
 
-Filename: static/js/ace/snippets/vhdl.js
+Filename: static/js/ace/mode-swift.js
 Comment: 
 
-Filename: static/js/ace/snippets/gcode.js
+Filename: static/js/ace/mode-d.js
 Comment: 
 
-Filename: static/js/ace/snippets/erlang.js
+Filename: static/js/ace/mode-pascal.js
 Comment: 
 
-Filename: static/js/ace/snippets/matlab.js
+Filename: static/js/ace/mode-cobol.js
 Comment: 
 
-Filename: static/js/ace/snippets/properties.js
+Filename: static/js/ace/theme-eclipse.js
 Comment: 
 
-Filename: static/js/ace/snippets/io.js
+Filename: static/js/ace/worker-php.js
 Comment: 
 
-Filename: static/js/ace/snippets/xquery.js
+Filename: static/js/ace/mode-jsoniq.js
 Comment: 
 
-Filename: static/js/ace/snippets/razor.js
+Filename: static/js/ace/mode-io.js
 Comment: 
 
-Filename: static/js/ace/snippets/typescript.js
+Filename: static/js/ace/ext-linking.js
 Comment: 
 
-Filename: static/js/ace/snippets/mips_assembler.js
+Filename: static/js/ace/theme-chaos.js
 Comment: 
 
-Filename: static/js/ace/snippets/textile.js
+Filename: static/js/ace/worker-json.js
 Comment: 
 
-Filename: static/js/ace/snippets/perl.js
+Filename: static/js/ace/theme-chrome.js
 Comment: 
 
-Filename: static/js/ace/snippets/mel.js
+Filename: static/js/ace/mode-powershell.js
 Comment: 
 
-Filename: static/js/ace/snippets/applescript.js
+Filename: static/js/ace/mode-smarty.js
 Comment: 
 
-Filename: static/js/ace/snippets/less.js
+Filename: static/js/ace/mode-c9search.js
 Comment: 
 
-Filename: static/js/ace/snippets/live_script.js
+Filename: static/js/ace/mode-vbscript.js
 Comment: 
 
-Filename: static/js/ace/snippets/coffee.js
+Filename: static/js/ace/mode-css.js
 Comment: 
 
-Filename: static/js/ace/snippets/bro.js
+Filename: static/js/ace/mode-xml.js
 Comment: 
 
-Filename: static/js/ace/snippets/prolog.js
+Filename: static/js/ace/worker-css.js
 Comment: 
 
-Filename: static/js/ace/snippets/velocity.js
+Filename: static/js/ace/mode-java.js
 Comment: 
 
-Filename: static/js/ace/snippets/ini.js
+Filename: static/js/ace/theme-clouds.js
 Comment: 
 
-Filename: static/js/ace/snippets/rdoc.js
+Filename: static/js/ace/theme-tomorrow.js
 Comment: 
 
-Filename: static/js/ace/snippets/actionscript.js
+Filename: static/js/ace/mode-sass.js
 Comment: 
 
-Filename: static/js/ace/snippets/cirru.js
+Filename: static/js/ace/mode-makefile.js
 Comment: 
 
-Filename: static/js/ace/snippets/html.js
+Filename: static/js/ace/mode-batchfile.js
 Comment: 
 
-Filename: static/js/ace/snippets/groovy.js
+Filename: static/js/ace/mode-elixir.js
 Comment: 
 
-Filename: static/js/ace/snippets/lsl.js
+Filename: static/js/ace/mode-autohotkey.js
 Comment: 
 
-Filename: static/js/ace/snippets/r.js
+Filename: static/js/ace/theme-idle_fingers.js
 Comment: 
 
-Filename: static/js/ace/snippets/plain_text.js
+Filename: static/js/ace/mode-glsl.js
 Comment: 
 
-Filename: static/js/ace/snippets/mysql.js
+Filename: static/js/ace/mode-python.js
 Comment: 
 
-Filename: static/js/ace/snippets/css.js
+Filename: static/js/ace/mode-nix.js
 Comment: 
 
-Filename: static/js/ace/snippets/pgsql.js
+Filename: static/js/ace/mode-django.js
 Comment: 
 
-Filename: static/js/ace/snippets/lucene.js
+Filename: static/js/ace/mode-lua.js
 Comment: 
 
-Filename: static/js/ace/snippets/ocaml.js
+Filename: static/js/ace/theme-solarized_light.js
 Comment: 
 
-Filename: static/js/ace/snippets/java.js
+Filename: static/js/ace/theme-xcode.js
 Comment: 
 
-Filename: static/js/ace/snippets/mushcode.js
+Filename: static/js/ace/ext-chromevox.js
 Comment: 
 
-Filename: static/js/ace/snippets/dot.js
+Filename: static/js/ace/mode-twig.js
 Comment: 
 
-Filename: static/js/ace/snippets/verilog.js
+Filename: static/js/ace/snippets/elm.js
 Comment: 
 
-Filename: static/js/ace/snippets/twig.js
+Filename: static/js/ace/snippets/typescript.js
 Comment: 
 
-Filename: static/js/ace/snippets/eiffel.js
+Filename: static/js/ace/snippets/handlebars.js
 Comment: 
 
-Filename: static/js/ace/snippets/dockerfile.js
+Filename: static/js/ace/snippets/mysql.js
 Comment: 
 
-Filename: static/js/ace/snippets/sql.js
+Filename: static/js/ace/snippets/cobol.js
 Comment: 
 
-Filename: static/js/ace/snippets/fortran.js
+Filename: static/js/ace/snippets/sass.js
 Comment: 
 
-Filename: static/js/ace/snippets/tcl.js
+Filename: static/js/ace/snippets/haxe.js
 Comment: 
 
-Filename: static/js/ace/snippets/golang.js
+Filename: static/js/ace/snippets/ini.js
 Comment: 
 
-Filename: static/js/ace/snippets/curly.js
+Filename: static/js/ace/snippets/twig.js
 Comment: 
 
-Filename: static/js/ace/snippets/lean.js
+Filename: static/js/ace/snippets/clojure.js
 Comment: 
 
-Filename: static/js/ace/snippets/jsp.js
+Filename: static/js/ace/snippets/live_script.js
 Comment: 
 
-Filename: static/js/ace/snippets/ejs.js
+Filename: static/js/ace/snippets/swift.js
 Comment: 
 
-Filename: static/js/ace/snippets/swig.js
+Filename: static/js/ace/snippets/ocaml.js
 Comment: 
 
-Filename: static/js/ace/snippets/soy_template.js
+Filename: static/js/ace/snippets/plain_text.js
 Comment: 
 
-Filename: static/js/ace/snippets/gitignore.js
+Filename: static/js/ace/snippets/vala.js
 Comment: 
 
-Filename: static/js/ace/snippets/pascal.js
+Filename: static/js/ace/snippets/lsl.js
 Comment: 
 
-Filename: static/js/ace/snippets/wollok.js
+Filename: static/js/ace/snippets/sql.js
 Comment: 
 
-Filename: static/js/ace/snippets/c_cpp.js
+Filename: static/js/ace/snippets/less.js
 Comment: 
 
-Filename: static/js/ace/snippets/haxe.js
+Filename: static/js/ace/snippets/markdown.js
 Comment: 
 
-Filename: static/js/ace/snippets/gherkin.js
+Filename: static/js/ace/snippets/liquid.js
 Comment: 
 
-Filename: static/js/ace/snippets/python.js
+Filename: static/js/ace/snippets/space.js
 Comment: 
 
-Filename: static/js/ace/snippets/maze.js
+Filename: static/js/ace/snippets/golang.js
 Comment: 
 
-Filename: static/js/ace/snippets/autohotkey.js
+Filename: static/js/ace/snippets/properties.js
 Comment: 
 
-Filename: static/js/ace/snippets/scheme.js
+Filename: static/js/ace/snippets/vhdl.js
 Comment: 
 
-Filename: static/js/ace/snippets/abc.js
+Filename: static/js/ace/snippets/vbscript.js
 Comment: 
 
-Filename: static/js/ace/snippets/scss.js
+Filename: static/js/ace/snippets/ftl.js
 Comment: 
 
-Filename: static/js/ace/snippets/html_elixir.js
+Filename: static/js/ace/snippets/coffee.js
 Comment: 
 
-Filename: static/js/ace/snippets/latex.js
+Filename: static/js/ace/snippets/lucene.js
 Comment: 
 
-Filename: static/js/ace/snippets/nsis.js
+Filename: static/js/ace/snippets/dart.js
 Comment: 
 
-Filename: static/js/ace/snippets/sjs.js
+Filename: static/js/ace/snippets/mips_assembler.js
 Comment: 
 
-Filename: static/js/ace/snippets/jsx.js
+Filename: static/js/ace/snippets/pgsql.js
 Comment: 
 
-Filename: static/js/ace/snippets/tex.js
+Filename: static/js/ace/snippets/r.js
 Comment: 
 
-Filename: static/js/ace/snippets/vala.js
+Filename: static/js/ace/snippets/rst.js
 Comment: 
 
-Filename: static/js/ace/snippets/tsx.js
+Filename: static/js/ace/snippets/dot.js
 Comment: 
 
-Filename: static/js/ace/snippets/rst.js
+Filename: static/js/ace/snippets/xml.js
 Comment: 
 
 Filename: static/js/ace/snippets/scala.js
 Comment: 
 
-Filename: static/js/ace/snippets/yaml.js
+Filename: static/js/ace/snippets/text.js
 Comment: 
 
-Filename: static/js/ace/snippets/ada.js
+Filename: static/js/ace/snippets/hjson.js
 Comment: 
 
-Filename: static/js/ace/snippets/batchfile.js
+Filename: static/js/ace/snippets/asciidoc.js
 Comment: 
 
-Filename: static/js/ace/snippets/smarty.js
+Filename: static/js/ace/snippets/apache_conf.js
 Comment: 
 
-Filename: static/js/ace/snippets/praat.js
+Filename: static/js/ace/snippets/razor.js
 Comment: 
 
-Filename: static/js/ace/snippets/asciidoc.js
+Filename: static/js/ace/snippets/javascript.js
 Comment: 
 
-Filename: static/js/ace/snippets/swift.js
+Filename: static/js/ace/snippets/scheme.js
 Comment: 
 
-Filename: static/js/ace/snippets/scad.js
+Filename: static/js/ace/snippets/curly.js
 Comment: 
 
-Filename: static/js/ace/snippets/elm.js
+Filename: static/js/ace/snippets/glsl.js
 Comment: 
 
-Filename: static/js/ace/snippets/glsl.js
+Filename: static/js/ace/snippets/drools.js
 Comment: 
 
-Filename: static/js/ace/snippets/mask.js
+Filename: static/js/ace/snippets/sh.js
 Comment: 
 
-Filename: static/js/ace/snippets/lua.js
+Filename: static/js/ace/snippets/diff.js
 Comment: 
 
-Filename: static/js/ace/snippets/c9search.js
+Filename: static/js/ace/snippets/html_ruby.js
 Comment: 
 
-Filename: static/js/ace/snippets/diff.js
+Filename: static/js/ace/snippets/bro.js
 Comment: 
 
-Filename: static/js/ace/snippets/clojure.js
+Filename: static/js/ace/snippets/ejs.js
 Comment: 
 
-Filename: static/js/ace/snippets/livescript.js
+Filename: static/js/ace/snippets/jsoniq.js
 Comment: 
 
-Filename: static/js/ace/snippets/rust.js
+Filename: static/js/ace/snippets/wollok.js
 Comment: 
 
-Filename: static/js/ace/snippets/powershell.js
+Filename: static/js/ace/snippets/smarty.js
 Comment: 
 
-Filename: static/js/ace/snippets/jsoniq.js
+Filename: static/js/ace/snippets/json.js
 Comment: 
 
-Filename: static/js/ace/snippets/d.js
+Filename: static/js/ace/snippets/c_cpp.js
 Comment: 
 
-Filename: static/js/ace/snippets/toml.js
+Filename: static/js/ace/snippets/gcode.js
 Comment: 
 
-Filename: static/js/ace/snippets/csharp.js
+Filename: static/js/ace/snippets/batchfile.js
 Comment: 
 
-Filename: static/js/ace/snippets/lisp.js
+Filename: static/js/ace/snippets/css.js
 Comment: 
 
-Filename: static/js/ace/snippets/sqlserver.js
+Filename: static/js/ace/snippets/perl.js
 Comment: 
 
 Filename: static/js/ace/snippets/nix.js
 Comment: 
 
-Filename: static/js/ace/snippets/dart.js
+Filename: static/js/ace/snippets/abap.js
 Comment: 
 
-Filename: static/js/ace/snippets/cobol.js
+Filename: static/js/ace/snippets/html.js
 Comment: 
 
-Filename: static/js/ace/snippets/jade.js
+Filename: static/js/ace/snippets/lisp.js
 Comment: 
 
-Filename: static/js/ace/snippets/protobuf.js
+Filename: static/js/ace/snippets/verilog.js
 Comment: 
 
-Filename: static/js/ace/snippets/mipsassembler.js
+Filename: static/js/ace/snippets/abc.js
 Comment: 
 
-Filename: static/js/ace/snippets/liquid.js
+Filename: static/js/ace/snippets/kotlin.js
 Comment: 
 
-Filename: static/js/ace/snippets/jack.js
+Filename: static/js/ace/snippets/lua.js
 Comment: 
 
-Filename: static/js/ace/snippets/rhtml.js
+Filename: static/js/ace/snippets/jsx.js
 Comment: 
 
-Filename: static/js/ace/snippets/handlebars.js
+Filename: static/js/ace/snippets/c9search.js
 Comment: 
 
-Filename: static/js/ace/snippets/xml.js
+Filename: static/js/ace/snippets/mask.js
 Comment: 
 
-Filename: static/js/ace/snippets/abap.js
+Filename: static/js/ace/snippets/assembly_x86.js
 Comment: 
 
-Filename: static/js/ace/snippets/elixir.js
+Filename: static/js/ace/snippets/jack.js
 Comment: 
 
-Filename: static/js/ace/snippets/forth.js
+Filename: static/js/ace/snippets/snippets.js
 Comment: 
 
-Filename: static/js/ace/snippets/apache_conf.js
+Filename: static/js/ace/snippets/mipsassembler.js
 Comment: 
 
-Filename: static/js/ace/snippets/julia.js
+Filename: static/js/ace/snippets/django.js
 Comment: 
 
-Filename: static/js/ace/snippets/haskell_cabal.js
+Filename: static/js/ace/snippets/haml.js
 Comment: 
 
-Filename: static/js/ace/snippets/stylus.js
+Filename: static/js/ace/snippets/scad.js
 Comment: 
 
-Filename: static/js/ace/snippets/sass.js
+Filename: static/js/ace/snippets/elixir.js
 Comment: 
 
-Filename: static/js/ace/snippets/django.js
+Filename: static/js/ace/snippets/toml.js
 Comment: 
 
-Filename: static/js/ace/snippets/coldfusion.js
+Filename: static/js/ace/snippets/ruby.js
 Comment: 
 
-Filename: static/js/ace/snippets/javascript.js
+Filename: static/js/ace/snippets/coldfusion.js
 Comment: 
 
-Filename: static/js/ace/snippets/sh.js
+Filename: static/js/ace/snippets/praat.js
 Comment: 
 
-Filename: static/js/ace/snippets/ftl.js
+Filename: static/js/ace/snippets/forth.js
 Comment: 
 
-Filename: static/js/ace/snippets/space.js
+Filename: static/js/ace/snippets/mel.js
 Comment: 
 
-Filename: static/js/ace/snippets/luapage.js
+Filename: static/js/ace/snippets/groovy.js
 Comment: 
 
-Filename: static/js/ace/snippets/markdown.js
+Filename: static/js/ace/snippets/prolog.js
 Comment: 
 
-Filename: static/js/ace/keybinding-vim.js
+Filename: static/js/ace/snippets/rdoc.js
 Comment: 
 
-Filename: static/js/ace/mode-forth.js
+Filename: static/js/ace/snippets/luapage.js
 Comment: 
 
-Filename: static/js/ace/mode-sh.js
+Filename: static/js/ace/snippets/actionscript.js
 Comment: 
 
-Filename: static/js/ace/ext-whitespace.js
+Filename: static/js/ace/snippets/tsx.js
 Comment: 
 
-Filename: static/js/ace/mode-apache_conf.js
+Filename: static/js/ace/snippets/applescript.js
 Comment: 
 
-Filename: static/js/ace/mode-mushcode.js
+Filename: static/js/ace/snippets/gobstones.js
 Comment: 
 
-Filename: static/js/ace/mode-toml.js
+Filename: static/js/ace/snippets/erlang.js
 Comment: 
 
-Filename: static/js/ace/mode-sql.js
+Filename: static/js/ace/snippets/php.js
 Comment: 
 
-Filename: static/js/ace/mode-vhdl.js
+Filename: static/js/ace/snippets/swig.js
 Comment: 
 
-Filename: static/js/ace/mode-lua.js
+Filename: static/js/ace/snippets/pascal.js
 Comment: 
 
-Filename: static/js/ace/mode-assembly_x86.js
+Filename: static/js/ace/snippets/autohotkey.js
 Comment: 
 
-Filename: static/js/ace/mode-glsl.js
+Filename: static/js/ace/snippets/mushcode.js
 Comment: 
 
-Filename: static/js/ace/theme-terminal.js
+Filename: static/js/ace/snippets/logiql.js
 Comment: 
 
-Filename: static/js/ace/mode-cirru.js
+Filename: static/js/ace/snippets/textile.js
 Comment: 
 
-Filename: static/js/ace/mode-scala.js
+Filename: static/js/ace/snippets/protobuf.js
 Comment: 
 
-Filename: static/js/ace/mode-jsx.js
+Filename: static/js/ace/snippets/soy_template.js
 Comment: 
 
-Filename: static/js/ace/mode-coldfusion.js
+Filename: static/js/ace/snippets/html_elixir.js
 Comment: 
 
-Filename: static/js/ace/mode-sass.js
+Filename: static/js/ace/snippets/rust.js
 Comment: 
 
-Filename: static/js/ace/theme-github.js
+Filename: static/js/ace/snippets/sjs.js
 Comment: 
 
-Filename: static/js/ace/mode-svg.js
+Filename: static/js/ace/snippets/livescript.js
 Comment: 
 
-Filename: static/js/ace/mode-scss.js
+Filename: static/js/ace/snippets/julia.js
 Comment: 
 
-Filename: static/js/ace/ace.js
+Filename: static/js/ace/snippets/maze.js
 Comment: 
 
-Filename: static/js/ace/mode-tex.js
+Filename: static/js/ace/snippets/tex.js
 Comment: 
 
-Filename: static/js/ace/mode-io.js
+Filename: static/js/ace/snippets/python.js
 Comment: 
 
-Filename: static/js/ace/mode-drools.js
+Filename: static/js/ace/snippets/gitignore.js
 Comment: 
 
-Filename: static/js/ace/theme-monokai.js
+Filename: static/js/ace/snippets/jsp.js
 Comment: 
 
-Filename: static/js/ace/theme-eclipse.js
+Filename: static/js/ace/snippets/haskell.js
 Comment: 
 
-Filename: static/js/ace/mode-protobuf.js
+Filename: static/js/ace/snippets/tcl.js
 Comment: 
 
-Filename: static/js/ace/mode-ruby.js
+Filename: static/js/ace/snippets/scss.js
 Comment: 
 
-Filename: static/js/ace/theme-chaos.js
+Filename: static/js/ace/snippets/io.js
 Comment: 
 
-Filename: static/js/ace/ext-linking.js
+Filename: static/js/ace/snippets/fortran.js
 Comment: 
 
-Filename: static/js/ace/ext-statusbar.js
+Filename: static/js/ace/snippets/svg.js
 Comment: 
 
-Filename: static/js/ace/worker-html.js
+Filename: static/js/ace/snippets/sqlserver.js
 Comment: 
 
-Filename: static/js/ace/mode-nsis.js
+Filename: static/js/ace/snippets/gherkin.js
 Comment: 
 
-Filename: static/js/ace/worker-php.js
+Filename: static/js/ace/snippets/powershell.js
 Comment: 
 
-Filename: static/js/ace/mode-objectivec.js
+Filename: static/js/ace/snippets/cirru.js
 Comment: 
 
-Filename: static/js/ace/ext-spellcheck.js
+Filename: static/js/ace/snippets/jade.js
 Comment: 
 
-Filename: static/js/ace/mode-javascript.js
+Filename: static/js/ace/snippets/makefile.js
 Comment: 
 
-Filename: static/js/ace/mode-praat.js
+Filename: static/js/ace/snippets/stylus.js
 Comment: 
 
-Filename: static/js/ace/mode-matlab.js
+Filename: static/js/ace/snippets/velocity.js
 Comment: 
 
-Filename: static/js/ace/mode-plain_text.js
+Filename: static/js/ace/snippets/xquery.js
 Comment: 
 
-Filename: static/js/ace/mode-mel.js
+Filename: static/js/ace/snippets/csharp.js
 Comment: 
 
-Filename: static/js/ace/mode-rdoc.js
+Filename: static/js/ace/snippets/dockerfile.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow_night.js
+Filename: static/js/ace/snippets/rhtml.js
 Comment: 
 
-Filename: static/js/ace/mode-groovy.js
+Filename: static/js/ace/snippets/d.js
 Comment: 
 
-Filename: static/js/ace/mode-markdown.js
+Filename: static/js/ace/snippets/latex.js
 Comment: 
 
-Filename: static/js/ace/mode-mysql.js
+Filename: static/js/ace/snippets/nsis.js
 Comment: 
 
-Filename: static/js/ace/mode-batchfile.js
+Filename: static/js/ace/snippets/matlab.js
 Comment: 
 
-Filename: static/js/ace/mode-gitignore.js
+Filename: static/js/ace/snippets/objectivec.js
 Comment: 
 
-Filename: static/js/ace/mode-julia.js
+Filename: static/js/ace/snippets/lean.js
 Comment: 
 
-Filename: static/js/ace/theme-kr_theme.js
+Filename: static/js/ace/snippets/java.js
 Comment: 
 
-Filename: static/js/ace/ext-error_marker.js
+Filename: static/js/ace/snippets/eiffel.js
 Comment: 
 
-Filename: static/js/ace/mode-json.js
+Filename: static/js/ace/snippets/ada.js
 Comment: 
 
-Filename: static/js/ace/mode-soy_template.js
+Filename: static/js/ace/snippets/haskell_cabal.js
 Comment: 
 
-Filename: static/js/ace/ext-settings_menu.js
+Filename: static/js/ace/snippets/yaml.js
 Comment: 
 
-Filename: static/js/ace/mode-vala.js
+Filename: static/js/ace/ext-elastic_tabstops_lite.js
 Comment: 
 
-Filename: static/js/ace/mode-logiql.js
+Filename: static/js/ace/theme-merbivore.js
 Comment: 
 
-Filename: static/js/ace/mode-abap.js
+Filename: static/js/ace/mode-snippets.js
 Comment: 
 
-Filename: static/js/ace/mode-lisp.js
+Filename: static/js/ace/ext-static_highlight.js
 Comment: 
 
-Filename: static/js/ace/mode-dart.js
+Filename: static/js/ace/ext-language_tools.js
 Comment: 
 
-Filename: static/js/ace/ext-themelist.js
+Filename: static/js/ace/mode-mips_assembler.js
 Comment: 
 
-Filename: static/js/ace/theme-idle_fingers.js
+Filename: static/js/ace/mode-groovy.js
 Comment: 
 
-Filename: static/js/ace/ext-searchbox.js
+Filename: static/js/ace/mode-pgsql.js
 Comment: 
 
-Filename: static/js/ace/mode-ini.js
+Filename: static/js/ace/mode-markdown.js
 Comment: 
 
-Filename: static/js/ace/mode-c_cpp.js
+Filename: static/js/ace/mode-scad.js
 Comment: 
 
-Filename: static/js/ace/worker-lua.js
+Filename: static/js/ace/mode-stylus.js
 Comment: 
 
-Filename: static/js/ace/theme-crimson_editor.js
+Filename: static/js/ace/mode-ocaml.js
 Comment: 
 
-Filename: static/js/ace/mode-tsx.js
+Filename: static/js/ace/mode-swig.js
 Comment: 
 
-Filename: static/js/ace/mode-handlebars.js
+Filename: static/js/ace/mode-haxe.js
 Comment: 
 
-Filename: static/js/ace/ext-language_tools.js
+Filename: static/js/ace/mode-maze.js
 Comment: 
 
-Filename: static/js/ace/mode-typescript.js
+Filename: static/js/ace/mode-scss.js
 Comment: 
 
-Filename: static/js/ace/mode-lean.js
+Filename: static/js/ace/mode-rust.js
 Comment: 
 
-Filename: static/js/ace/mode-verilog.js
+Filename: static/js/ace/mode-rdoc.js
 Comment: 
 
-Filename: static/js/ace/theme-vibrant_ink.js
+Filename: static/js/ace/mode-eiffel.js
 Comment: 
 
-Filename: static/js/ace/mode-jack.js
+Filename: static/js/ace/mode-latex.js
 Comment: 
 
-Filename: static/js/ace/mode-liquid.js
+Filename: static/js/ace/mode-scala.js
 Comment: 
 
-Filename: static/js/ace/mode-razor.js
+Filename: static/js/ace/mode-dot.js
 Comment: 
 
-Filename: static/js/ace/mode-snippets.js
+Filename: static/js/ace/mode-perl.js
 Comment: 
 
-Filename: static/js/ace/mode-maze.js
+Filename: static/js/ace/mode-objectivec.js
 Comment: 
 
-Filename: static/js/ace/ext-textarea.js
+Filename: static/js/ace/worker-html.js
 Comment: 
 
-Filename: static/js/ace/mode-haskell.js
+Filename: static/js/ace/theme-merbivore_soft.js
 Comment: 
 
-Filename: static/js/ace/mode-bro.js
+Filename: static/js/ace/mode-velocity.js
 Comment: 
 
-Filename: static/js/ace/mode-lsl.js
+Filename: static/js/ace/theme-vibrant_ink.js
 Comment: 
 
-Filename: static/js/ace/mode-ejs.js
+Filename: static/js/ace/mode-clojure.js
 Comment: 
 
-Filename: static/js/ace/theme-ambiance.js
+Filename: static/js/ace/mode-php.js
 Comment: 
 
-Filename: static/js/ace/ext-old_ie.js
+Filename: static/js/ace/theme-monokai.js
 Comment: 
 
-Filename: static/js/ace/mode-lucene.js
+Filename: static/js/ace/ext-emmet.js
 Comment: 
 
-Filename: static/js/ace/mode-coffee.js
+Filename: static/js/ace/mode-asciidoc.js
 Comment: 
 
-Filename: static/js/ace/mode-haml.js
+Filename: static/js/ace/mode-csharp.js
 Comment: 
 
-Filename: static/js/ace/mode-haskell_cabal.js
+Filename: static/js/ace/theme-tomorrow_night_eighties.js
 Comment: 
 
-Filename: static/js/ace/mode-css.js
+Filename: static/js/ace/mode-sql.js
 Comment: 
 
-Filename: static/js/ace/theme-merbivore_soft.js
+Filename: static/js/ace/ext-spellcheck.js
 Comment: 
 
-Filename: static/js/ace/mode-vbscript.js
+Filename: static/js/ace/theme-tomorrow_night_bright.js
 Comment: 
 
-Filename: static/js/ace/mode-html_ruby.js
+Filename: static/js/ace/mode-ftl.js
 Comment: 
 
-Filename: static/js/ace/mode-pgsql.js
+Filename: static/js/ace/keybinding-vim.js
 Comment: 
 
-Filename: static/js/ace/mode-abc.js
+Filename: static/js/ace/mode-mipsassembler.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow_night_eighties.js
+Filename: static/js/ace/mode-r.js
 Comment: 
 
-Filename: static/js/ace/ext-emmet.js
+Filename: static/js/ace/mode-lean.js
 Comment: 
 
-Filename: static/js/ace/mode-html_elixir.js
+Filename: static/js/ace/mode-toml.js
 Comment: 
 
-Filename: static/js/ace/mode-erlang.js
+Filename: static/js/ace/mode-html_ruby.js
 Comment: 
 
-Filename: static/js/ace/ext-keybinding_menu.js
+Filename: static/js/ace/mode-lucene.js
 Comment: 
 
-Filename: static/js/ace/theme-dawn.js
+Filename: static/js/ace/ext-error_marker.js
 Comment: 
 
-Filename: static/js/ace/mode-asciidoc.js
+Filename: static/js/ace/mode-kotlin.js
 Comment: 
 
-Filename: static/js/ace/theme-pastel_on_dark.js
+Filename: static/js/ace/mode-rst.js
 Comment: 
 
-Filename: static/js/ace/mode-swig.js
+Filename: static/js/ace/mode-ruby.js
 Comment: 
 
-Filename: static/js/ace/mode-swift.js
+Filename: static/js/ace/mode-vala.js
 Comment: 
 
-Filename: static/js/ace/mode-python.js
+Filename: static/js/ace/ext-statusbar.js
 Comment: 
 
-Filename: static/js/ace/mode-livescript.js
+Filename: static/js/ace/mode-html_elixir.js
 Comment: 
 
-Filename: static/js/ace/theme-cobalt.js
+Filename: static/js/ace/mode-json.js
 Comment: 
 
-Filename: static/js/ace/mode-django.js
+Filename: static/js/ace/mode-sjs.js
 Comment: 
 
-Filename: static/js/ace/mode-xquery.js
+Filename: static/js/ace/theme-crimson_editor.js
 Comment: 
 
-Filename: static/js/ace/mode-scad.js
+Filename: static/js/ace/mode-verilog.js
 Comment: 
 
-Filename: static/js/ace/theme-clouds_midnight.js
+Filename: static/js/highlight.min.js
 Comment: 
 
-Filename: static/js/ace/ext-chromevox.js
+Filename: static/js/jquery.min.js
 Comment: 
 
-Filename: static/js/ace/theme-solarized_light.js
+Filename: static/js/utils.js
 Comment: 
 
-Filename: static/js/ace/mode-nix.js
+Filename: static/js/vue.min.js
 Comment: 
 
-Filename: static/js/ace/mode-luapage.js
+Filename: static/js/sugar.min.js
 Comment: 
 
-Filename: static/js/ace/theme-kuroir.js
+Filename: static/js/axios.min.js
 Comment: 
 
-Filename: static/js/ace/mode-fortran.js
+Filename: static/js/dbadmin.js
 Comment: 
 
-Filename: static/js/ace/theme-merbivore.js
+Filename: static/js/translations.js
 Comment: 
 
-Filename: static/js/ace/theme-tomorrow_night_bright.js
+Filename: static/css/gitlog.min.css
 Comment: 
 
-Filename: static/js/ace/mode-xml.js
+Filename: static/css/future.css
 Comment: 
 
-Filename: static/js/ace/mode-mips_assembler.js
+Filename: static/images/alert-blue.gif
 Comment: 
 
-Filename: static/js/utils.js
+Filename: static/images/widget.gif
 Comment: 
 
-Filename: static/js/axios.min.js
+Filename: static/images/alert-yellow.gif
 Comment: 
 
-Filename: static/js/dbadmin.js
+Filename: static/images/alert-red.gif
 Comment: 
 
-Filename: static/js/vue.min.js
+Filename: static/images/alert-green.gif
 Comment: 
 
-Filename: static/js/jquery.min.js
+Filename: static/images/forkme.png
 Comment: 
 
-Filename: static/js/highlight.min.js
+Filename: static/images/alert-orange.gif
 Comment: 
 
-Filename: __init__.py
+Filename: translations/README.md
 Comment: 
 
-Filename: templates/translations.html
+Filename: __init__.py
 Comment: 
 
-Filename: templates/index.html
+Filename: diff2kryten.py
 Comment: 
 
 Filename: templates/gitlog.html
 Comment: 
 
-Filename: templates/dbadmin.html
+Filename: templates/ticket.html
 Comment: 
 
-Filename: templates/ticket.html
+Filename: templates/dbadmin.html
 Comment: 
 
-Filename: diff2kryten.py
+Filename: templates/translations.html
 Comment: 
 
-Filename: translations/README.md
+Filename: templates/index.html
 Comment: 
 
 Zip file comment:
```

#### static/js/utils.js

##### js-beautify {}

```diff
@@ -19,14 +19,26 @@
     return JSON.parse(JSON.stringify(data));
 };
 
 Q.eval = function(text) {
     return eval('(' + text + ')');
 };
 
+// Given a url retuns an object with parsed query string
+Q.get_query = function(source) {
+    source = source || window.location.search.substring(1);
+    var vars = {},
+        items = source.split('&');
+    items.map(function(item) {
+        var pair = item.split('=');
+        vars[decodeURIComponent(pair[0])] = decodeURIComponent(pair[1]);
+    });
+    return vars;
+};
+
 // a wrapper for fetch return a promise
 Q.ajax = function(method, url, data, headers) {
     var options = {
         method: method,
         referrerPolicy: 'no-referrer',
     }
     if (data) {
```

### Comparing `py4web-1.20230314.1/py4web/assets/py4web.app._default.zip` & `py4web-1.20230410.1/py4web/assets/py4web.app._default.zip`

 * *Files 1% similar despite different names*

#### zipinfo {}

```diff
@@ -1,5 +1,5 @@
 Zip file size: 182307 bytes, number of entries: 3
--rw-r--r--  3.0 unx   181425 bx defN 21-May-09 01:57 static/images/logo.png
+-rw-rw-r--  3.0 unx   181425 bx defN 21-May-09 01:57 static/images/logo.png
 -rw-r--r--  3.0 unx      135 tx defN 19-Dec-25 18:43 __init__.py
--rw-rw-r--  3.0 unx     1799 tx defN 22-Jun-06 01:49 templates/index.html
+-rw-r--r--  3.0 unx     1799 tx defN 22-Jun-06 01:49 templates/index.html
 3 files, 183359 bytes uncompressed, 181795 bytes compressed:  0.9%
```

### Comparing `py4web-1.20230314.1/py4web/assets/py4web.app._documentation.zip` & `py4web-1.20230410.1/py4web/assets/py4web.app._documentation.zip`

 * *Files 3% similar despite different names*

#### zipinfo {}

```diff
@@ -1,151 +1,151 @@
-Zip file size: 4278467 bytes, number of entries: 149
--rw-rw-r--  3.0 unx   111365 tx defN 23-Mar-08 00:13 static/en/chapter-10.html
--rw-rw-r--  3.0 unx    53835 tx defN 23-Mar-08 00:13 static/en/chapter-14.html
--rw-rw-r--  3.0 unx    45218 tx defN 23-Mar-08 00:13 static/en/chapter-03.html
--rw-rw-r--  3.0 unx    42205 tx defN 23-Mar-08 00:13 static/en/chapter-05.html
--rw-rw-r--  3.0 unx    85076 tx defN 23-Mar-08 00:13 static/en/chapter-16.html
--rw-rw-r--  3.0 unx    94538 tx defN 23-Mar-08 00:13 static/en/chapter-06.html
--rw-rw-r--  3.0 unx    19643 tx defN 23-Mar-08 00:13 static/en/index.html
--rw-rw-r--  3.0 unx    63229 tx defN 23-Mar-08 00:13 static/en/chapter-09.html
--rw-rw-r--  3.0 unx     1804 tx defN 23-Jan-03 04:34 static/en/_static/tabs.css
--rw-rw-r--  3.0 unx      427 tx defN 23-Mar-08 00:13 static/en/_static/documentation_options.js
--rw-rw-r--  3.0 unx     4231 tx defN 23-Jan-03 04:34 static/en/_static/tabs.js
--rw-rw-r--  3.0 unx     4712 tx defN 23-Jan-03 04:34 static/en/_static/sphinx_highlight.js
--rw-rw-r--  3.0 unx       90 bx defN 23-Jan-03 04:34 static/en/_static/minus.png
--rw-rw-r--  3.0 unx       90 bx defN 23-Jan-03 04:34 static/en/_static/plus.png
--rw-rw-r--  3.0 unx     4758 tx defN 23-Mar-08 00:13 static/en/_static/language_data.js
--rw-rw-r--  3.0 unx     4819 tx defN 23-Mar-08 00:13 static/en/_static/pygments.css
--rw-rw-r--  3.0 unx   181425 bx defN 21-May-09 02:00 static/en/_static/logo.png
--rw-rw-r--  3.0 unx    18215 tx defN 23-Jan-03 04:34 static/en/_static/searchtools.js
--rw-rw-r--  3.0 unx   131657 tx defN 23-Jan-03 04:34 static/en/_static/css/theme.css
--rw-rw-r--  3.0 unx     1456 tx defN 20-Nov-16 04:06 static/en/_static/css/toggle.css
--rw-rw-r--  3.0 unx     3229 tx defN 23-Jan-03 04:34 static/en/_static/css/badge_only.css
--rw-rw-r--  3.0 unx     6515 tx defN 20-Nov-16 04:06 static/en/_static/css/dark.css
--rw-rw-r--  3.0 unx     4370 tx defN 23-Jan-03 04:34 static/en/_static/js/html5shiv-printshiv.min.js
+Zip file size: 4278028 bytes, number of entries: 149
+-rw-r--r--  3.0 unx    15311 tx defN 23-Mar-08 00:13 static/en/chapter-01.html
+-rw-r--r--  3.0 unx     6736 tx defN 23-Mar-08 00:13 static/en/search.html
+-rw-r--r--  3.0 unx    11689 tx defN 23-Mar-08 00:13 static/en/chapter-04.html
+-rw-r--r--  3.0 unx     1804 tx defN 23-Jan-03 04:34 static/en/_static/tabs.css
+-rw-r--r--  3.0 unx    18215 tx defN 23-Jan-03 04:34 static/en/_static/searchtools.js
 -rw-rw-r--  3.0 unx      934 tx defN 23-Jan-03 04:34 static/en/_static/js/badge_only.js
--rw-rw-r--  3.0 unx     1333 tx defN 20-Nov-16 04:06 static/en/_static/js/toggle.js
--rw-rw-r--  3.0 unx     5023 tx defN 23-Jan-03 04:34 static/en/_static/js/theme.js
 -rw-rw-r--  3.0 unx     2734 tx defN 23-Jan-03 04:34 static/en/_static/js/html5shiv.min.js
+-rw-r--r--  3.0 unx     5023 tx defN 23-Jan-03 04:34 static/en/_static/js/theme.js
+-rw-rw-r--  3.0 unx     4370 tx defN 23-Jan-03 04:34 static/en/_static/js/html5shiv-printshiv.min.js
+-rw-rw-r--  3.0 unx     1333 tx defN 20-Nov-16 04:06 static/en/_static/js/toggle.js
+-rw-r--r--  3.0 unx     4712 tx defN 23-Jan-03 04:34 static/en/_static/sphinx_highlight.js
 -rw-rw-r--  3.0 unx      286 bx stor 23-Jan-03 04:34 static/en/_static/file.png
--rw-rw-r--  3.0 unx     4472 tx defN 23-Jan-03 04:34 static/en/_static/doctools.js
--rw-rw-r--  3.0 unx    14813 tx defN 23-Mar-08 00:13 static/en/_static/basic.css
--rw-rw-r--  3.0 unx    42864 tx defN 23-Mar-08 00:13 static/en/chapter-15.html
--rw-rw-r--  3.0 unx   189399 tx defN 23-Mar-08 00:13 static/en/chapter-12.html
--rw-rw-r--  3.0 unx    91787 tx defN 23-Mar-08 00:13 static/en/searchindex.js
--rw-rw-r--  3.0 unx    19496 tx defN 23-Mar-08 00:13 static/en/chapter-02.html
--rw-rw-r--  3.0 unx    11181 tx defN 23-Mar-08 00:13 static/en/chapter-11.html
--rw-rw-r--  3.0 unx    15311 tx defN 23-Mar-08 00:13 static/en/chapter-01.html
--rw-rw-r--  3.0 unx     6461 tx defN 23-Mar-08 00:13 static/en/genindex.html
+-rw-r--r--  3.0 unx     4819 tx defN 23-Mar-08 00:13 static/en/_static/pygments.css
+-rw-r--r--  3.0 unx     4758 tx defN 23-Mar-08 00:13 static/en/_static/language_data.js
+-rw-rw-r--  3.0 unx       90 bx defN 23-Jan-03 04:34 static/en/_static/minus.png
+-rw-r--r--  3.0 unx   181425 bx defN 21-May-09 02:00 static/en/_static/logo.png
+-rw-rw-r--  3.0 unx       90 bx defN 23-Jan-03 04:34 static/en/_static/plus.png
+-rw-r--r--  3.0 unx   131657 tx defN 23-Jan-03 04:34 static/en/_static/css/theme.css
+-rw-r--r--  3.0 unx     3229 tx defN 23-Jan-03 04:34 static/en/_static/css/badge_only.css
+-rw-rw-r--  3.0 unx     6515 tx defN 20-Nov-16 04:06 static/en/_static/css/dark.css
+-rw-rw-r--  3.0 unx     1456 tx defN 20-Nov-16 04:06 static/en/_static/css/toggle.css
+-rw-r--r--  3.0 unx    14813 tx defN 23-Mar-08 00:13 static/en/_static/basic.css
+-rw-r--r--  3.0 unx      427 tx defN 23-Mar-08 00:13 static/en/_static/documentation_options.js
+-rw-r--r--  3.0 unx     4472 tx defN 23-Jan-03 04:34 static/en/_static/doctools.js
+-rw-r--r--  3.0 unx     4231 tx defN 23-Jan-03 04:34 static/en/_static/tabs.js
+-rw-r--r--  3.0 unx    91787 tx defN 23-Mar-08 00:13 static/en/searchindex.js
+-rw-rw-r--  3.0 unx     6515 tx defN 20-Nov-16 04:06 static/en/dark.css
+-rw-r--r--  3.0 unx    11181 tx defN 23-Mar-08 00:13 static/en/chapter-11.html
+-rw-r--r--  3.0 unx    18809 tx defN 23-Apr-10 02:55 static/en/chapter-02.html
+-rw-r--r--  3.0 unx    85076 tx defN 23-Mar-08 00:13 static/en/chapter-16.html
+-rw-r--r--  3.0 unx     6461 tx defN 23-Mar-08 00:13 static/en/genindex.html
+-rw-r--r--  3.0 unx    50484 tx defN 23-Mar-08 00:13 static/en/chapter-13.html
+-rw-r--r--  3.0 unx   111365 tx defN 23-Mar-08 00:13 static/en/chapter-10.html
+-rw-r--r--  3.0 unx    53835 tx defN 23-Mar-08 00:13 static/en/chapter-14.html
+-rw-r--r--  3.0 unx    45218 tx defN 23-Mar-08 00:13 static/en/chapter-03.html
 -rw-rw-r--  3.0 unx     1456 tx defN 20-Nov-16 04:06 static/en/toggle.css
--rw-rw-r--  3.0 unx   129072 tx defN 23-Mar-08 00:13 static/en/chapter-08.html
--rw-rw-r--  3.0 unx    11257 bx defN 21-Jul-27 13:10 static/en/_images/form1.png
--rw-rw-r--  3.0 unx   154315 bx defN 21-Jan-10 04:31 static/en/_images/dashboard_ticket.png
--rw-rw-r--  3.0 unx    37805 bx defN 21-Sep-06 04:36 static/en/_images/form3.png
--rw-rw-r--  3.0 unx   174817 bx defN 21-Jan-10 04:31 static/en/_images/dashboard_edit.png
--rw-rw-r--  3.0 unx    40409 bx defN 21-Sep-06 04:36 static/en/_images/form2.png
--rw-rw-r--  3.0 unx    41285 bx defN 21-Dec-17 06:10 static/en/_images/grid.png
--rw-rw-r--  3.0 unx    29268 bx defN 21-Oct-04 03:32 static/en/_images/restapi2.png
+-rw-r--r--  3.0 unx   499752 tx defN 23-Mar-08 00:13 static/en/chapter-07.html
+-rw-r--r--  3.0 unx   189399 tx defN 23-Mar-08 00:13 static/en/chapter-12.html
+-rw-r--r--  3.0 unx   129072 tx defN 23-Mar-08 00:13 static/en/chapter-08.html
+-rw-r--r--  3.0 unx    94538 tx defN 23-Mar-08 00:13 static/en/chapter-06.html
+-rw-r--r--  3.0 unx    63229 tx defN 23-Mar-08 00:13 static/en/chapter-09.html
+-rw-r--r--  3.0 unx    42205 tx defN 23-Mar-08 00:13 static/en/chapter-05.html
+-rw-r--r--  3.0 unx    19643 tx defN 23-Mar-08 00:13 static/en/index.html
+-rw-r--r--  3.0 unx    40745 bx defN 21-Dec-17 06:10 static/en/_images/grid_bulmacss.png
+-rw-r--r--  3.0 unx    40478 bx defN 21-Jan-10 04:31 static/en/_images/command.png
+-rw-r--r--  3.0 unx    40467 bx defN 21-May-01 16:15 static/en/_images/dashboard_new_app.png
+-rw-r--r--  3.0 unx   174817 bx defN 21-Jan-10 04:31 static/en/_images/dashboard_edit.png
+-rw-r--r--  3.0 unx    37805 bx defN 21-Sep-06 04:36 static/en/_images/form3.png
+-rw-r--r--  3.0 unx    39765 bx defN 21-Sep-06 04:36 static/en/_images/form5.png
+-rw-r--r--  3.0 unx    30536 bx defN 21-Oct-04 03:32 static/en/_images/restapi.png
+-rw-r--r--  3.0 unx    40409 bx defN 21-Sep-06 04:36 static/en/_images/form2.png
+-rw-r--r--  3.0 unx    30931 bx defN 21-Dec-04 05:46 static/en/_images/tags2.png
+-rw-r--r--  3.0 unx   181425 bx defN 21-May-09 02:00 static/en/_images/logo.png
+-rw-r--r--  3.0 unx    50011 bx defN 21-Nov-01 01:08 static/en/_images/first_run.png
 -rw-rw-r--  3.0 unx    16627 bx defN 21-Mar-10 07:17 static/en/_images/simple_counter.png
--rw-rw-r--  3.0 unx    30536 bx defN 21-Oct-04 03:32 static/en/_images/restapi.png
--rw-rw-r--  3.0 unx    39765 bx defN 21-Sep-06 04:36 static/en/_images/form5.png
--rw-rw-r--  3.0 unx    86267 bx defN 21-Jan-10 04:31 static/en/_images/dashboard_login.png
--rw-rw-r--  3.0 unx   147429 bx defN 21-Jan-10 04:31 static/en/_images/dashboard_restapi.png
--rw-rw-r--  3.0 unx   135864 bx defN 21-Jan-10 04:31 static/en/_images/dashboard_main.png
--rw-rw-r--  3.0 unx    58653 bx defN 22-Mar-04 05:02 static/en/_images/grid_columns.png
--rw-rw-r--  3.0 unx    40745 bx defN 21-Dec-17 06:10 static/en/_images/grid_bulmacss.png
+-rw-r--r--  3.0 unx    86267 bx defN 21-Jan-10 04:31 static/en/_images/dashboard_login.png
 -rw-rw-r--  3.0 unx    12086 bx defN 21-Jan-10 04:31 static/en/_images/_scaffold.png
--rw-rw-r--  3.0 unx   181425 bx defN 21-May-09 02:00 static/en/_images/logo.png
--rw-rw-r--  3.0 unx    52898 bx defN 21-Jan-10 04:31 static/en/_images/dashboard.png
--rw-rw-r--  3.0 unx    30931 bx defN 21-Dec-04 05:46 static/en/_images/tags2.png
--rw-rw-r--  3.0 unx    46250 bx defN 21-Sep-06 04:36 static/en/_images/form4.png
--rw-rw-r--  3.0 unx    53747 bx defN 21-Jan-10 04:31 static/en/_images/dashboard_error.png
--rw-rw-r--  3.0 unx    44559 bx defN 21-Dec-17 06:10 static/en/_images/grid_nocss.png
--rw-rw-r--  3.0 unx    24753 bx defN 21-Dec-04 05:46 static/en/_images/tags_db.png
--rw-rw-r--  3.0 unx    40467 bx defN 21-May-01 16:15 static/en/_images/dashboard_new_app.png
--rw-rw-r--  3.0 unx    77606 bx defN 21-Jan-10 04:31 static/en/_images/main_page.png
--rw-rw-r--  3.0 unx    40478 bx defN 21-Jan-10 04:31 static/en/_images/command.png
--rw-rw-r--  3.0 unx    50011 bx defN 21-Nov-01 01:08 static/en/_images/first_run.png
--rw-rw-r--  3.0 unx    38066 bx defN 21-Sep-06 04:36 static/en/_images/form6.png
--rw-rw-r--  3.0 unx     6515 tx defN 20-Nov-16 04:06 static/en/dark.css
--rw-rw-r--  3.0 unx   499752 tx defN 23-Mar-08 00:13 static/en/chapter-07.html
--rw-rw-r--  3.0 unx    11689 tx defN 23-Mar-08 00:13 static/en/chapter-04.html
--rw-rw-r--  3.0 unx     6736 tx defN 23-Mar-08 00:13 static/en/search.html
--rw-rw-r--  3.0 unx    50484 tx defN 23-Mar-08 00:13 static/en/chapter-13.html
--rw-rw-r--  3.0 unx      248 tx defN 23-Mar-08 00:27 static/index.html
--rw-rw-r--  3.0 unx   104888 tx defN 23-Mar-08 00:20 static/pt/chapter-10.html
--rw-rw-r--  3.0 unx    54454 tx defN 23-Mar-08 00:20 static/pt/chapter-14.html
--rw-rw-r--  3.0 unx    44515 tx defN 23-Mar-08 00:20 static/pt/chapter-03.html
--rw-rw-r--  3.0 unx    40952 tx defN 23-Mar-08 00:20 static/pt/chapter-05.html
--rw-rw-r--  3.0 unx    85195 tx defN 23-Mar-08 00:20 static/pt/chapter-16.html
--rw-rw-r--  3.0 unx    93158 tx defN 23-Mar-08 00:20 static/pt/chapter-06.html
--rw-rw-r--  3.0 unx    19655 tx defN 23-Mar-08 00:20 static/pt/index.html
--rw-rw-r--  3.0 unx    61156 tx defN 23-Mar-08 00:20 static/pt/chapter-09.html
--rw-rw-r--  3.0 unx     1804 tx defN 23-Jan-03 04:34 static/pt/_static/tabs.css
--rw-rw-r--  3.0 unx      427 tx defN 23-Mar-08 00:20 static/pt/_static/documentation_options.js
--rw-rw-r--  3.0 unx     4231 tx defN 23-Jan-03 04:34 static/pt/_static/tabs.js
--rw-rw-r--  3.0 unx     4712 tx defN 23-Jan-03 04:34 static/pt/_static/sphinx_highlight.js
--rw-rw-r--  3.0 unx       90 bx defN 23-Jan-03 04:34 static/pt/_static/minus.png
--rw-rw-r--  3.0 unx     2412 tx defN 23-Jan-03 04:34 static/pt/_static/translations.js
--rw-rw-r--  3.0 unx       90 bx defN 23-Jan-03 04:34 static/pt/_static/plus.png
--rw-rw-r--  3.0 unx    14417 tx defN 23-Mar-08 00:20 static/pt/_static/language_data.js
--rw-rw-r--  3.0 unx     4819 tx defN 23-Mar-08 00:20 static/pt/_static/pygments.css
--rw-rw-r--  3.0 unx   181425 bx defN 21-May-09 02:00 static/pt/_static/logo.png
--rw-rw-r--  3.0 unx     8133 tx defN 23-Jan-03 04:34 static/pt/_static/base-stemmer.js
--rw-rw-r--  3.0 unx    18215 tx defN 23-Jan-03 04:34 static/pt/_static/searchtools.js
--rw-rw-r--  3.0 unx   131657 tx defN 23-Jan-03 04:34 static/pt/_static/css/theme.css
--rw-rw-r--  3.0 unx     1456 tx defN 20-Nov-16 04:06 static/pt/_static/css/toggle.css
--rw-rw-r--  3.0 unx     3229 tx defN 23-Jan-03 04:34 static/pt/_static/css/badge_only.css
--rw-rw-r--  3.0 unx     6515 tx defN 20-Nov-16 04:06 static/pt/_static/css/dark.css
--rw-rw-r--  3.0 unx    26718 tx defN 23-Jan-03 04:34 static/pt/_static/portuguese-stemmer.js
--rw-rw-r--  3.0 unx     4370 tx defN 23-Jan-03 04:34 static/pt/_static/js/html5shiv-printshiv.min.js
+-rw-r--r--  3.0 unx    77606 bx defN 21-Jan-10 04:31 static/en/_images/main_page.png
+-rw-r--r--  3.0 unx    41285 bx defN 21-Dec-17 06:10 static/en/_images/grid.png
+-rw-r--r--  3.0 unx   135864 bx defN 21-Jan-10 04:31 static/en/_images/dashboard_main.png
+-rw-r--r--  3.0 unx    44559 bx defN 21-Dec-17 06:10 static/en/_images/grid_nocss.png
+-rw-r--r--  3.0 unx    24753 bx defN 21-Dec-04 05:46 static/en/_images/tags_db.png
+-rw-r--r--  3.0 unx    46250 bx defN 21-Sep-06 04:36 static/en/_images/form4.png
+-rw-rw-r--  3.0 unx    11257 bx defN 21-Jul-27 13:10 static/en/_images/form1.png
+-rw-r--r--  3.0 unx   154315 bx defN 21-Jan-10 04:31 static/en/_images/dashboard_ticket.png
+-rw-r--r--  3.0 unx   147429 bx defN 21-Jan-10 04:31 static/en/_images/dashboard_restapi.png
+-rw-r--r--  3.0 unx    52898 bx defN 21-Jan-10 04:31 static/en/_images/dashboard.png
+-rw-r--r--  3.0 unx    58653 bx defN 22-Mar-04 05:02 static/en/_images/grid_columns.png
+-rw-r--r--  3.0 unx    38066 bx defN 21-Sep-06 04:36 static/en/_images/form6.png
+-rw-r--r--  3.0 unx    29268 bx defN 21-Oct-04 03:32 static/en/_images/restapi2.png
+-rw-r--r--  3.0 unx    53747 bx defN 21-Jan-10 04:31 static/en/_images/dashboard_error.png
+-rw-r--r--  3.0 unx    42864 tx defN 23-Mar-08 00:13 static/en/chapter-15.html
+-rw-r--r--  3.0 unx    15700 tx defN 23-Mar-08 00:20 static/pt/chapter-01.html
+-rw-r--r--  3.0 unx     6874 tx defN 23-Mar-08 00:20 static/pt/search.html
+-rw-r--r--  3.0 unx    11850 tx defN 23-Mar-08 00:20 static/pt/chapter-04.html
+-rw-r--r--  3.0 unx     1804 tx defN 23-Jan-03 04:34 static/pt/_static/tabs.css
+-rw-r--r--  3.0 unx    18215 tx defN 23-Jan-03 04:34 static/pt/_static/searchtools.js
 -rw-rw-r--  3.0 unx      934 tx defN 23-Jan-03 04:34 static/pt/_static/js/badge_only.js
--rw-rw-r--  3.0 unx     1333 tx defN 20-Nov-16 04:06 static/pt/_static/js/toggle.js
--rw-rw-r--  3.0 unx     5023 tx defN 23-Jan-03 04:34 static/pt/_static/js/theme.js
 -rw-rw-r--  3.0 unx     2734 tx defN 23-Jan-03 04:34 static/pt/_static/js/html5shiv.min.js
+-rw-r--r--  3.0 unx     5023 tx defN 23-Jan-03 04:34 static/pt/_static/js/theme.js
+-rw-rw-r--  3.0 unx     4370 tx defN 23-Jan-03 04:34 static/pt/_static/js/html5shiv-printshiv.min.js
+-rw-rw-r--  3.0 unx     1333 tx defN 20-Nov-16 04:06 static/pt/_static/js/toggle.js
+-rw-r--r--  3.0 unx     4712 tx defN 23-Jan-03 04:34 static/pt/_static/sphinx_highlight.js
 -rw-rw-r--  3.0 unx      286 bx stor 23-Jan-03 04:34 static/pt/_static/file.png
--rw-rw-r--  3.0 unx     4472 tx defN 23-Jan-03 04:34 static/pt/_static/doctools.js
--rw-rw-r--  3.0 unx    14813 tx defN 23-Mar-08 00:20 static/pt/_static/basic.css
--rw-rw-r--  3.0 unx    43020 tx defN 23-Mar-08 00:20 static/pt/chapter-15.html
--rw-rw-r--  3.0 unx   189086 tx defN 23-Mar-08 00:20 static/pt/chapter-12.html
--rw-rw-r--  3.0 unx   126019 tx defN 23-Mar-08 00:20 static/pt/searchindex.js
--rw-rw-r--  3.0 unx    20128 tx defN 23-Mar-08 00:20 static/pt/chapter-02.html
--rw-rw-r--  3.0 unx    11474 tx defN 23-Mar-08 00:20 static/pt/chapter-11.html
--rw-rw-r--  3.0 unx    15700 tx defN 23-Mar-08 00:20 static/pt/chapter-01.html
--rw-rw-r--  3.0 unx     6595 tx defN 23-Mar-08 00:20 static/pt/genindex.html
+-rw-r--r--  3.0 unx     4819 tx defN 23-Mar-08 00:20 static/pt/_static/pygments.css
+-rw-r--r--  3.0 unx    14417 tx defN 23-Mar-08 00:20 static/pt/_static/language_data.js
+-rw-rw-r--  3.0 unx       90 bx defN 23-Jan-03 04:34 static/pt/_static/minus.png
+-rw-r--r--  3.0 unx     8133 tx defN 23-Jan-03 04:34 static/pt/_static/base-stemmer.js
+-rw-r--r--  3.0 unx   181425 bx defN 21-May-09 02:00 static/pt/_static/logo.png
+-rw-rw-r--  3.0 unx       90 bx defN 23-Jan-03 04:34 static/pt/_static/plus.png
+-rw-r--r--  3.0 unx   131657 tx defN 23-Jan-03 04:34 static/pt/_static/css/theme.css
+-rw-r--r--  3.0 unx     3229 tx defN 23-Jan-03 04:34 static/pt/_static/css/badge_only.css
+-rw-rw-r--  3.0 unx     6515 tx defN 20-Nov-16 04:06 static/pt/_static/css/dark.css
+-rw-rw-r--  3.0 unx     1456 tx defN 20-Nov-16 04:06 static/pt/_static/css/toggle.css
+-rw-r--r--  3.0 unx    14813 tx defN 23-Mar-08 00:20 static/pt/_static/basic.css
+-rw-r--r--  3.0 unx      427 tx defN 23-Mar-08 00:20 static/pt/_static/documentation_options.js
+-rw-r--r--  3.0 unx    26718 tx defN 23-Jan-03 04:34 static/pt/_static/portuguese-stemmer.js
+-rw-r--r--  3.0 unx     4472 tx defN 23-Jan-03 04:34 static/pt/_static/doctools.js
+-rw-r--r--  3.0 unx     4231 tx defN 23-Jan-03 04:34 static/pt/_static/tabs.js
+-rw-r--r--  3.0 unx     2412 tx defN 23-Jan-03 04:34 static/pt/_static/translations.js
+-rw-r--r--  3.0 unx   126019 tx defN 23-Mar-08 00:20 static/pt/searchindex.js
+-rw-rw-r--  3.0 unx     6515 tx defN 20-Nov-16 04:06 static/pt/dark.css
+-rw-r--r--  3.0 unx    11474 tx defN 23-Mar-08 00:20 static/pt/chapter-11.html
+-rw-r--r--  3.0 unx    19344 tx defN 23-Apr-10 02:55 static/pt/chapter-02.html
+-rw-r--r--  3.0 unx    85195 tx defN 23-Mar-08 00:20 static/pt/chapter-16.html
+-rw-r--r--  3.0 unx     6595 tx defN 23-Mar-08 00:20 static/pt/genindex.html
+-rw-r--r--  3.0 unx    50433 tx defN 23-Mar-08 00:20 static/pt/chapter-13.html
+-rw-r--r--  3.0 unx   104888 tx defN 23-Mar-08 00:20 static/pt/chapter-10.html
+-rw-r--r--  3.0 unx    54454 tx defN 23-Mar-08 00:20 static/pt/chapter-14.html
+-rw-r--r--  3.0 unx    44515 tx defN 23-Mar-08 00:20 static/pt/chapter-03.html
 -rw-rw-r--  3.0 unx     1456 tx defN 20-Nov-16 04:06 static/pt/toggle.css
--rw-rw-r--  3.0 unx   128984 tx defN 23-Mar-08 00:20 static/pt/chapter-08.html
--rw-rw-r--  3.0 unx    11257 bx defN 21-Jul-27 13:10 static/pt/_images/form1.png
--rw-rw-r--  3.0 unx   154315 bx defN 21-Jan-10 04:31 static/pt/_images/dashboard_ticket.png
--rw-rw-r--  3.0 unx    37805 bx defN 21-Sep-06 04:36 static/pt/_images/form3.png
--rw-rw-r--  3.0 unx   174817 bx defN 21-Jan-10 04:31 static/pt/_images/dashboard_edit.png
--rw-rw-r--  3.0 unx    40409 bx defN 21-Sep-06 04:36 static/pt/_images/form2.png
--rw-rw-r--  3.0 unx    41285 bx defN 21-Dec-17 06:10 static/pt/_images/grid.png
--rw-rw-r--  3.0 unx    29268 bx defN 21-Oct-04 03:32 static/pt/_images/restapi2.png
+-rw-r--r--  3.0 unx   464287 tx defN 23-Mar-08 00:20 static/pt/chapter-07.html
+-rw-r--r--  3.0 unx   189086 tx defN 23-Mar-08 00:20 static/pt/chapter-12.html
+-rw-r--r--  3.0 unx   128984 tx defN 23-Mar-08 00:20 static/pt/chapter-08.html
+-rw-r--r--  3.0 unx    93158 tx defN 23-Mar-08 00:20 static/pt/chapter-06.html
+-rw-r--r--  3.0 unx    61156 tx defN 23-Mar-08 00:20 static/pt/chapter-09.html
+-rw-r--r--  3.0 unx    40952 tx defN 23-Mar-08 00:20 static/pt/chapter-05.html
+-rw-r--r--  3.0 unx    19655 tx defN 23-Mar-08 00:20 static/pt/index.html
+-rw-r--r--  3.0 unx    40745 bx defN 21-Dec-17 06:10 static/pt/_images/grid_bulmacss.png
+-rw-r--r--  3.0 unx    40478 bx defN 21-Jan-10 04:31 static/pt/_images/command.png
+-rw-r--r--  3.0 unx    40467 bx defN 21-May-01 16:15 static/pt/_images/dashboard_new_app.png
+-rw-r--r--  3.0 unx   174817 bx defN 21-Jan-10 04:31 static/pt/_images/dashboard_edit.png
+-rw-r--r--  3.0 unx    37805 bx defN 21-Sep-06 04:36 static/pt/_images/form3.png
+-rw-r--r--  3.0 unx    39765 bx defN 21-Sep-06 04:36 static/pt/_images/form5.png
+-rw-r--r--  3.0 unx    30536 bx defN 21-Oct-04 03:32 static/pt/_images/restapi.png
+-rw-r--r--  3.0 unx    40409 bx defN 21-Sep-06 04:36 static/pt/_images/form2.png
+-rw-r--r--  3.0 unx    30931 bx defN 21-Dec-04 05:46 static/pt/_images/tags2.png
+-rw-r--r--  3.0 unx   181425 bx defN 21-May-09 02:00 static/pt/_images/logo.png
+-rw-r--r--  3.0 unx    50011 bx defN 21-Nov-01 01:08 static/pt/_images/first_run.png
 -rw-rw-r--  3.0 unx    16627 bx defN 21-Mar-10 07:17 static/pt/_images/simple_counter.png
--rw-rw-r--  3.0 unx    30536 bx defN 21-Oct-04 03:32 static/pt/_images/restapi.png
--rw-rw-r--  3.0 unx    39765 bx defN 21-Sep-06 04:36 static/pt/_images/form5.png
--rw-rw-r--  3.0 unx    86267 bx defN 21-Jan-10 04:31 static/pt/_images/dashboard_login.png
--rw-rw-r--  3.0 unx   147429 bx defN 21-Jan-10 04:31 static/pt/_images/dashboard_restapi.png
--rw-rw-r--  3.0 unx   135864 bx defN 21-Jan-10 04:31 static/pt/_images/dashboard_main.png
--rw-rw-r--  3.0 unx    58653 bx defN 22-Mar-04 05:02 static/pt/_images/grid_columns.png
--rw-rw-r--  3.0 unx    40745 bx defN 21-Dec-17 06:10 static/pt/_images/grid_bulmacss.png
--rw-rw-r--  3.0 unx    12086 bx defN 21-Jan-10 04:31 static/pt/_images/_scaffold.png
--rw-rw-r--  3.0 unx   181425 bx defN 21-May-09 02:00 static/pt/_images/logo.png
--rw-rw-r--  3.0 unx    52898 bx defN 21-Jan-10 04:31 static/pt/_images/dashboard.png
--rw-rw-r--  3.0 unx    30931 bx defN 21-Dec-04 05:46 static/pt/_images/tags2.png
--rw-rw-r--  3.0 unx    46250 bx defN 21-Sep-06 04:36 static/pt/_images/form4.png
--rw-rw-r--  3.0 unx    53747 bx defN 21-Jan-10 04:31 static/pt/_images/dashboard_error.png
--rw-rw-r--  3.0 unx    44559 bx defN 21-Dec-17 06:10 static/pt/_images/grid_nocss.png
--rw-rw-r--  3.0 unx    24753 bx defN 21-Dec-04 05:46 static/pt/_images/tags_db.png
--rw-rw-r--  3.0 unx    40467 bx defN 21-May-01 16:15 static/pt/_images/dashboard_new_app.png
--rw-rw-r--  3.0 unx    77606 bx defN 21-Jan-10 04:31 static/pt/_images/main_page.png
--rw-rw-r--  3.0 unx    40478 bx defN 21-Jan-10 04:31 static/pt/_images/command.png
--rw-rw-r--  3.0 unx    50011 bx defN 21-Nov-01 01:08 static/pt/_images/first_run.png
--rw-rw-r--  3.0 unx    38066 bx defN 21-Sep-06 04:36 static/pt/_images/form6.png
--rw-rw-r--  3.0 unx     6515 tx defN 20-Nov-16 04:06 static/pt/dark.css
--rw-rw-r--  3.0 unx   464287 tx defN 23-Mar-08 00:20 static/pt/chapter-07.html
--rw-rw-r--  3.0 unx    11850 tx defN 23-Mar-08 00:20 static/pt/chapter-04.html
--rw-rw-r--  3.0 unx     6874 tx defN 23-Mar-08 00:20 static/pt/search.html
--rw-rw-r--  3.0 unx    50433 tx defN 23-Mar-08 00:20 static/pt/chapter-13.html
+-rw-r--r--  3.0 unx    86267 bx defN 21-Jan-10 04:31 static/pt/_images/dashboard_login.png
+-rw-r--r--  3.0 unx    12086 bx defN 21-Jan-10 04:31 static/pt/_images/_scaffold.png
+-rw-r--r--  3.0 unx    77606 bx defN 21-Jan-10 04:31 static/pt/_images/main_page.png
+-rw-r--r--  3.0 unx    41285 bx defN 21-Dec-17 06:10 static/pt/_images/grid.png
+-rw-r--r--  3.0 unx   135864 bx defN 21-Jan-10 04:31 static/pt/_images/dashboard_main.png
+-rw-r--r--  3.0 unx    44559 bx defN 21-Dec-17 06:10 static/pt/_images/grid_nocss.png
+-rw-r--r--  3.0 unx    24753 bx defN 21-Dec-04 05:46 static/pt/_images/tags_db.png
+-rw-r--r--  3.0 unx    46250 bx defN 21-Sep-06 04:36 static/pt/_images/form4.png
+-rw-rw-r--  3.0 unx    11257 bx defN 21-Jul-27 13:10 static/pt/_images/form1.png
+-rw-r--r--  3.0 unx   154315 bx defN 21-Jan-10 04:31 static/pt/_images/dashboard_ticket.png
+-rw-r--r--  3.0 unx   147429 bx defN 21-Jan-10 04:31 static/pt/_images/dashboard_restapi.png
+-rw-r--r--  3.0 unx    52898 bx defN 21-Jan-10 04:31 static/pt/_images/dashboard.png
+-rw-r--r--  3.0 unx    58653 bx defN 22-Mar-04 05:02 static/pt/_images/grid_columns.png
+-rw-r--r--  3.0 unx    38066 bx defN 21-Sep-06 04:36 static/pt/_images/form6.png
+-rw-r--r--  3.0 unx    29268 bx defN 21-Oct-04 03:32 static/pt/_images/restapi2.png
+-rw-r--r--  3.0 unx    53747 bx defN 21-Jan-10 04:31 static/pt/_images/dashboard_error.png
+-rw-r--r--  3.0 unx    43020 tx defN 23-Mar-08 00:20 static/pt/chapter-15.html
+-rw-rw-r--  3.0 unx      248 tx defN 23-Mar-08 00:27 static/index.html
 -rw-r--r--  3.0 unx      112 tx defN 20-Apr-13 01:13 __init__.py
-149 files, 7502412 bytes uncompressed, 4250707 bytes compressed:  43.3%
+149 files, 7500941 bytes uncompressed, 4250268 bytes compressed:  43.3%
```

#### zipnote {}

```diff
@@ -1,448 +1,448 @@
-Filename: static/en/chapter-10.html
-Comment: 
-
-Filename: static/en/chapter-14.html
+Filename: static/en/chapter-01.html
 Comment: 
 
-Filename: static/en/chapter-03.html
+Filename: static/en/search.html
 Comment: 
 
-Filename: static/en/chapter-05.html
+Filename: static/en/chapter-04.html
 Comment: 
 
-Filename: static/en/chapter-16.html
+Filename: static/en/_static/tabs.css
 Comment: 
 
-Filename: static/en/chapter-06.html
+Filename: static/en/_static/searchtools.js
 Comment: 
 
-Filename: static/en/index.html
+Filename: static/en/_static/js/badge_only.js
 Comment: 
 
-Filename: static/en/chapter-09.html
+Filename: static/en/_static/js/html5shiv.min.js
 Comment: 
 
-Filename: static/en/_static/tabs.css
+Filename: static/en/_static/js/theme.js
 Comment: 
 
-Filename: static/en/_static/documentation_options.js
+Filename: static/en/_static/js/html5shiv-printshiv.min.js
 Comment: 
 
-Filename: static/en/_static/tabs.js
+Filename: static/en/_static/js/toggle.js
 Comment: 
 
 Filename: static/en/_static/sphinx_highlight.js
 Comment: 
 
-Filename: static/en/_static/minus.png
+Filename: static/en/_static/file.png
 Comment: 
 
-Filename: static/en/_static/plus.png
+Filename: static/en/_static/pygments.css
 Comment: 
 
 Filename: static/en/_static/language_data.js
 Comment: 
 
-Filename: static/en/_static/pygments.css
+Filename: static/en/_static/minus.png
 Comment: 
 
 Filename: static/en/_static/logo.png
 Comment: 
 
-Filename: static/en/_static/searchtools.js
+Filename: static/en/_static/plus.png
 Comment: 
 
 Filename: static/en/_static/css/theme.css
 Comment: 
 
-Filename: static/en/_static/css/toggle.css
-Comment: 
-
 Filename: static/en/_static/css/badge_only.css
 Comment: 
 
 Filename: static/en/_static/css/dark.css
 Comment: 
 
-Filename: static/en/_static/js/html5shiv-printshiv.min.js
+Filename: static/en/_static/css/toggle.css
 Comment: 
 
-Filename: static/en/_static/js/badge_only.js
+Filename: static/en/_static/basic.css
 Comment: 
 
-Filename: static/en/_static/js/toggle.js
+Filename: static/en/_static/documentation_options.js
 Comment: 
 
-Filename: static/en/_static/js/theme.js
+Filename: static/en/_static/doctools.js
 Comment: 
 
-Filename: static/en/_static/js/html5shiv.min.js
+Filename: static/en/_static/tabs.js
 Comment: 
 
-Filename: static/en/_static/file.png
+Filename: static/en/searchindex.js
 Comment: 
 
-Filename: static/en/_static/doctools.js
+Filename: static/en/dark.css
 Comment: 
 
-Filename: static/en/_static/basic.css
+Filename: static/en/chapter-11.html
 Comment: 
 
-Filename: static/en/chapter-15.html
+Filename: static/en/chapter-02.html
 Comment: 
 
-Filename: static/en/chapter-12.html
+Filename: static/en/chapter-16.html
 Comment: 
 
-Filename: static/en/searchindex.js
+Filename: static/en/genindex.html
 Comment: 
 
-Filename: static/en/chapter-02.html
+Filename: static/en/chapter-13.html
 Comment: 
 
-Filename: static/en/chapter-11.html
+Filename: static/en/chapter-10.html
 Comment: 
 
-Filename: static/en/chapter-01.html
+Filename: static/en/chapter-14.html
 Comment: 
 
-Filename: static/en/genindex.html
+Filename: static/en/chapter-03.html
 Comment: 
 
 Filename: static/en/toggle.css
 Comment: 
 
-Filename: static/en/chapter-08.html
+Filename: static/en/chapter-07.html
 Comment: 
 
-Filename: static/en/_images/form1.png
+Filename: static/en/chapter-12.html
 Comment: 
 
-Filename: static/en/_images/dashboard_ticket.png
+Filename: static/en/chapter-08.html
 Comment: 
 
-Filename: static/en/_images/form3.png
+Filename: static/en/chapter-06.html
 Comment: 
 
-Filename: static/en/_images/dashboard_edit.png
+Filename: static/en/chapter-09.html
 Comment: 
 
-Filename: static/en/_images/form2.png
+Filename: static/en/chapter-05.html
 Comment: 
 
-Filename: static/en/_images/grid.png
+Filename: static/en/index.html
 Comment: 
 
-Filename: static/en/_images/restapi2.png
+Filename: static/en/_images/grid_bulmacss.png
 Comment: 
 
-Filename: static/en/_images/simple_counter.png
+Filename: static/en/_images/command.png
 Comment: 
 
-Filename: static/en/_images/restapi.png
+Filename: static/en/_images/dashboard_new_app.png
 Comment: 
 
-Filename: static/en/_images/form5.png
+Filename: static/en/_images/dashboard_edit.png
 Comment: 
 
-Filename: static/en/_images/dashboard_login.png
+Filename: static/en/_images/form3.png
 Comment: 
 
-Filename: static/en/_images/dashboard_restapi.png
+Filename: static/en/_images/form5.png
 Comment: 
 
-Filename: static/en/_images/dashboard_main.png
+Filename: static/en/_images/restapi.png
 Comment: 
 
-Filename: static/en/_images/grid_columns.png
+Filename: static/en/_images/form2.png
 Comment: 
 
-Filename: static/en/_images/grid_bulmacss.png
+Filename: static/en/_images/tags2.png
 Comment: 
 
-Filename: static/en/_images/_scaffold.png
+Filename: static/en/_images/logo.png
 Comment: 
 
-Filename: static/en/_images/logo.png
+Filename: static/en/_images/first_run.png
 Comment: 
 
-Filename: static/en/_images/dashboard.png
+Filename: static/en/_images/simple_counter.png
 Comment: 
 
-Filename: static/en/_images/tags2.png
+Filename: static/en/_images/dashboard_login.png
 Comment: 
 
-Filename: static/en/_images/form4.png
+Filename: static/en/_images/_scaffold.png
 Comment: 
 
-Filename: static/en/_images/dashboard_error.png
+Filename: static/en/_images/main_page.png
 Comment: 
 
-Filename: static/en/_images/grid_nocss.png
+Filename: static/en/_images/grid.png
 Comment: 
 
-Filename: static/en/_images/tags_db.png
+Filename: static/en/_images/dashboard_main.png
 Comment: 
 
-Filename: static/en/_images/dashboard_new_app.png
+Filename: static/en/_images/grid_nocss.png
 Comment: 
 
-Filename: static/en/_images/main_page.png
+Filename: static/en/_images/tags_db.png
 Comment: 
 
-Filename: static/en/_images/command.png
+Filename: static/en/_images/form4.png
 Comment: 
 
-Filename: static/en/_images/first_run.png
+Filename: static/en/_images/form1.png
 Comment: 
 
-Filename: static/en/_images/form6.png
+Filename: static/en/_images/dashboard_ticket.png
 Comment: 
 
-Filename: static/en/dark.css
+Filename: static/en/_images/dashboard_restapi.png
 Comment: 
 
-Filename: static/en/chapter-07.html
+Filename: static/en/_images/dashboard.png
 Comment: 
 
-Filename: static/en/chapter-04.html
+Filename: static/en/_images/grid_columns.png
 Comment: 
 
-Filename: static/en/search.html
+Filename: static/en/_images/form6.png
 Comment: 
 
-Filename: static/en/chapter-13.html
+Filename: static/en/_images/restapi2.png
 Comment: 
 
-Filename: static/index.html
+Filename: static/en/_images/dashboard_error.png
 Comment: 
 
-Filename: static/pt/chapter-10.html
+Filename: static/en/chapter-15.html
 Comment: 
 
-Filename: static/pt/chapter-14.html
+Filename: static/pt/chapter-01.html
 Comment: 
 
-Filename: static/pt/chapter-03.html
+Filename: static/pt/search.html
 Comment: 
 
-Filename: static/pt/chapter-05.html
+Filename: static/pt/chapter-04.html
 Comment: 
 
-Filename: static/pt/chapter-16.html
+Filename: static/pt/_static/tabs.css
 Comment: 
 
-Filename: static/pt/chapter-06.html
+Filename: static/pt/_static/searchtools.js
 Comment: 
 
-Filename: static/pt/index.html
+Filename: static/pt/_static/js/badge_only.js
 Comment: 
 
-Filename: static/pt/chapter-09.html
+Filename: static/pt/_static/js/html5shiv.min.js
 Comment: 
 
-Filename: static/pt/_static/tabs.css
+Filename: static/pt/_static/js/theme.js
 Comment: 
 
-Filename: static/pt/_static/documentation_options.js
+Filename: static/pt/_static/js/html5shiv-printshiv.min.js
 Comment: 
 
-Filename: static/pt/_static/tabs.js
+Filename: static/pt/_static/js/toggle.js
 Comment: 
 
 Filename: static/pt/_static/sphinx_highlight.js
 Comment: 
 
-Filename: static/pt/_static/minus.png
+Filename: static/pt/_static/file.png
 Comment: 
 
-Filename: static/pt/_static/translations.js
+Filename: static/pt/_static/pygments.css
 Comment: 
 
-Filename: static/pt/_static/plus.png
+Filename: static/pt/_static/language_data.js
 Comment: 
 
-Filename: static/pt/_static/language_data.js
+Filename: static/pt/_static/minus.png
 Comment: 
 
-Filename: static/pt/_static/pygments.css
+Filename: static/pt/_static/base-stemmer.js
 Comment: 
 
 Filename: static/pt/_static/logo.png
 Comment: 
 
-Filename: static/pt/_static/base-stemmer.js
+Filename: static/pt/_static/plus.png
 Comment: 
 
-Filename: static/pt/_static/searchtools.js
+Filename: static/pt/_static/css/theme.css
 Comment: 
 
-Filename: static/pt/_static/css/theme.css
+Filename: static/pt/_static/css/badge_only.css
+Comment: 
+
+Filename: static/pt/_static/css/dark.css
 Comment: 
 
 Filename: static/pt/_static/css/toggle.css
 Comment: 
 
-Filename: static/pt/_static/css/badge_only.css
+Filename: static/pt/_static/basic.css
 Comment: 
 
-Filename: static/pt/_static/css/dark.css
+Filename: static/pt/_static/documentation_options.js
 Comment: 
 
 Filename: static/pt/_static/portuguese-stemmer.js
 Comment: 
 
-Filename: static/pt/_static/js/html5shiv-printshiv.min.js
+Filename: static/pt/_static/doctools.js
 Comment: 
 
-Filename: static/pt/_static/js/badge_only.js
+Filename: static/pt/_static/tabs.js
 Comment: 
 
-Filename: static/pt/_static/js/toggle.js
+Filename: static/pt/_static/translations.js
 Comment: 
 
-Filename: static/pt/_static/js/theme.js
+Filename: static/pt/searchindex.js
 Comment: 
 
-Filename: static/pt/_static/js/html5shiv.min.js
+Filename: static/pt/dark.css
 Comment: 
 
-Filename: static/pt/_static/file.png
+Filename: static/pt/chapter-11.html
 Comment: 
 
-Filename: static/pt/_static/doctools.js
+Filename: static/pt/chapter-02.html
 Comment: 
 
-Filename: static/pt/_static/basic.css
+Filename: static/pt/chapter-16.html
 Comment: 
 
-Filename: static/pt/chapter-15.html
+Filename: static/pt/genindex.html
 Comment: 
 
-Filename: static/pt/chapter-12.html
+Filename: static/pt/chapter-13.html
 Comment: 
 
-Filename: static/pt/searchindex.js
+Filename: static/pt/chapter-10.html
 Comment: 
 
-Filename: static/pt/chapter-02.html
+Filename: static/pt/chapter-14.html
 Comment: 
 
-Filename: static/pt/chapter-11.html
+Filename: static/pt/chapter-03.html
 Comment: 
 
-Filename: static/pt/chapter-01.html
+Filename: static/pt/toggle.css
 Comment: 
 
-Filename: static/pt/genindex.html
+Filename: static/pt/chapter-07.html
 Comment: 
 
-Filename: static/pt/toggle.css
+Filename: static/pt/chapter-12.html
 Comment: 
 
 Filename: static/pt/chapter-08.html
 Comment: 
 
-Filename: static/pt/_images/form1.png
+Filename: static/pt/chapter-06.html
 Comment: 
 
-Filename: static/pt/_images/dashboard_ticket.png
+Filename: static/pt/chapter-09.html
 Comment: 
 
-Filename: static/pt/_images/form3.png
+Filename: static/pt/chapter-05.html
 Comment: 
 
-Filename: static/pt/_images/dashboard_edit.png
+Filename: static/pt/index.html
 Comment: 
 
-Filename: static/pt/_images/form2.png
+Filename: static/pt/_images/grid_bulmacss.png
 Comment: 
 
-Filename: static/pt/_images/grid.png
+Filename: static/pt/_images/command.png
 Comment: 
 
-Filename: static/pt/_images/restapi2.png
+Filename: static/pt/_images/dashboard_new_app.png
 Comment: 
 
-Filename: static/pt/_images/simple_counter.png
+Filename: static/pt/_images/dashboard_edit.png
 Comment: 
 
-Filename: static/pt/_images/restapi.png
+Filename: static/pt/_images/form3.png
 Comment: 
 
 Filename: static/pt/_images/form5.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_login.png
+Filename: static/pt/_images/restapi.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_restapi.png
+Filename: static/pt/_images/form2.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_main.png
+Filename: static/pt/_images/tags2.png
 Comment: 
 
-Filename: static/pt/_images/grid_columns.png
+Filename: static/pt/_images/logo.png
 Comment: 
 
-Filename: static/pt/_images/grid_bulmacss.png
+Filename: static/pt/_images/first_run.png
 Comment: 
 
-Filename: static/pt/_images/_scaffold.png
+Filename: static/pt/_images/simple_counter.png
 Comment: 
 
-Filename: static/pt/_images/logo.png
+Filename: static/pt/_images/dashboard_login.png
 Comment: 
 
-Filename: static/pt/_images/dashboard.png
+Filename: static/pt/_images/_scaffold.png
 Comment: 
 
-Filename: static/pt/_images/tags2.png
+Filename: static/pt/_images/main_page.png
 Comment: 
 
-Filename: static/pt/_images/form4.png
+Filename: static/pt/_images/grid.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_error.png
+Filename: static/pt/_images/dashboard_main.png
 Comment: 
 
 Filename: static/pt/_images/grid_nocss.png
 Comment: 
 
 Filename: static/pt/_images/tags_db.png
 Comment: 
 
-Filename: static/pt/_images/dashboard_new_app.png
+Filename: static/pt/_images/form4.png
 Comment: 
 
-Filename: static/pt/_images/main_page.png
+Filename: static/pt/_images/form1.png
 Comment: 
 
-Filename: static/pt/_images/command.png
+Filename: static/pt/_images/dashboard_ticket.png
 Comment: 
 
-Filename: static/pt/_images/first_run.png
+Filename: static/pt/_images/dashboard_restapi.png
 Comment: 
 
-Filename: static/pt/_images/form6.png
+Filename: static/pt/_images/dashboard.png
 Comment: 
 
-Filename: static/pt/dark.css
+Filename: static/pt/_images/grid_columns.png
 Comment: 
 
-Filename: static/pt/chapter-07.html
+Filename: static/pt/_images/form6.png
 Comment: 
 
-Filename: static/pt/chapter-04.html
+Filename: static/pt/_images/restapi2.png
 Comment: 
 
-Filename: static/pt/search.html
+Filename: static/pt/_images/dashboard_error.png
 Comment: 
 
-Filename: static/pt/chapter-13.html
+Filename: static/pt/chapter-15.html
+Comment: 
+
+Filename: static/index.html
 Comment: 
 
 Filename: __init__.py
 Comment: 
 
 Zip file comment:
```

#### static/en/chapter-02.html

```diff
@@ -45,15 +45,14 @@
               <p class="caption" role="heading"><span class="caption-text">Contents:</span></p>
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="chapter-01.html">What is py4web?</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">Help, resources and hints</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#resources">Resources</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#this-manual">This manual</a></li>
 <li class="toctree-l3"><a class="reference internal" href="#the-google-group">The Google group</a></li>
-<li class="toctree-l3"><a class="reference internal" href="#the-chat-on-irc">The chat on IRC</a></li>
 <li class="toctree-l3"><a class="reference internal" href="#the-discord-server">The Discord server</a></li>
 <li class="toctree-l3"><a class="reference internal" href="#tutorials-and-video">Tutorials and video</a></li>
 <li class="toctree-l3"><a class="reference internal" href="#the-sources-on-github">The sources on GitHub</a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#hints-and-tips">Hints and tips</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#prerequisites">Prerequisites</a></li>
@@ -116,20 +115,14 @@
 <h3>This manual<a class="headerlink" href="#this-manual" title="Permalink to this heading"></a></h3>
 <p>This manual is the Reference Manual for py4web. It’s available online at <a class="reference external" href="https://py4web.com/_documentation/static/index.html">https://py4web.com/_documentation/static/index.html</a>, where you’ll also find the PDF and EBOOK version, in multiple languages. It written in RestructuredText and generated using Sphinx.</p>
 </section>
 <section id="the-google-group">
 <h3>The Google group<a class="headerlink" href="#the-google-group" title="Permalink to this heading"></a></h3>
 <p>There is a dedicated mailing list hosted on Google Groups, see <a class="reference external" href="https://groups.google.com/g/py4web">https://groups.google.com/g/py4web</a>. This is the main source of discussions for developers and simple users. For any problem you should face, this is the right place to search for a hint or a solution.</p>
 </section>
-<section id="the-chat-on-irc">
-<h3>The chat on IRC<a class="headerlink" href="#the-chat-on-irc" title="Permalink to this heading"></a></h3>
-<p>We also use to chat sometime on IRC (Internet Relay Chat, which is an old-style text only chat). You can freely join us at <a class="reference external" href="https://webchat.freenode.net/#py4web">https://webchat.freenode.net/#py4web</a>.
-From time to time we also use it to host a scheduled public chat, where you can write and read live questions to developers.
-Transcripts of them are then available on the mailing list.</p>
-</section>
 <section id="the-discord-server">
 <h3>The Discord server<a class="headerlink" href="#the-discord-server" title="Permalink to this heading"></a></h3>
 <p>For quick questions and chats you can also use the free <a class="reference external" href="https://discord.gg/xCzQ9KTk3W">Discord server dedicated to py4web</a>. You could usually find many py4web developers hanging out in the channel.</p>
 </section>
 <section id="tutorials-and-video">
 <h3>Tutorials and video<a class="headerlink" href="#tutorials-and-video" title="Permalink to this heading"></a></h3>
 <p>There are many tutorials and videos available. Here are some of them:</p>
```

##### html2text {}

```diff
@@ -12,15 +12,14 @@
 [q                   ]
 Contents:
     * What_is_py4web?
     * Help,_resources_and_hints
           o Resources
                 # This_manual
                 # The_Google_group
-                # The_chat_on_IRC
                 # The_Discord_server
                 # Tutorials_and_video
                 # The_sources_on_GitHub
           o Hints_and_tips
                 # Prerequisites
                 # A_modern_python_workplace
                 # Debugging_py4web_with_VScode
@@ -60,21 +59,14 @@
 
 **** The Google groupï ****
 There is a dedicated mailing list hosted on Google Groups, see https://
 groups.google.com/g/py4web. This is the main source of discussions for
 developers and simple users. For any problem you should face, this is the right
 place to search for a hint or a solution.
 
-**** The chat on IRCï ****
-We also use to chat sometime on IRC (Internet Relay Chat, which is an old-style
-text only chat). You can freely join us at https://webchat.freenode.net/
-#py4web. From time to time we also use it to host a scheduled public chat,
-where you can write and read live questions to developers. Transcripts of them
-are then available on the mailing list.
-
 **** The Discord serverï ****
 For quick questions and chats you can also use the free Discord_server
 dedicated_to_py4web. You could usually find many py4web developers hanging out
 in the channel.
 
 **** Tutorials and videoï ****
 There are many tutorials and videos available. Here are some of them:
```

#### static/pt/chapter-02.html

```diff
@@ -46,15 +46,14 @@
               <p class="caption" role="heading"><span class="caption-text">Conteúdo:</span></p>
 <ul class="current">
 <li class="toctree-l1"><a class="reference internal" href="chapter-01.html">O que é py4web?</a></li>
 <li class="toctree-l1 current"><a class="current reference internal" href="#">Ajuda, recursos e dicas</a><ul>
 <li class="toctree-l2"><a class="reference internal" href="#resources">Recursos</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#this-manual">Este manual</a></li>
 <li class="toctree-l3"><a class="reference internal" href="#the-google-group">O grupo Google</a></li>
-<li class="toctree-l3"><a class="reference internal" href="#the-chat-on-irc">O bate-papo no IRC</a></li>
 <li class="toctree-l3"><a class="reference internal" href="#the-discord-server">The Discord server</a></li>
 <li class="toctree-l3"><a class="reference internal" href="#tutorials-and-video">Tutoriais e vídeo</a></li>
 <li class="toctree-l3"><a class="reference internal" href="#the-sources-on-github">As fontes no GitHub</a></li>
 </ul>
 </li>
 <li class="toctree-l2"><a class="reference internal" href="#hints-and-tips">Dicas e sugestões</a><ul>
 <li class="toctree-l3"><a class="reference internal" href="#prerequisites">Pré-requisitos</a></li>
@@ -115,18 +114,14 @@
 <h3>Este manual<a class="headerlink" href="#this-manual" title="Permalink to this heading"></a></h3>
 <p>This manual is the Reference Manual for py4web. It’s available online at <a class="reference external" href="https://py4web.com/_documentation/static/index.html">https://py4web.com/_documentation/static/index.html</a>, where you’ll also find the PDF and EBOOK version, in multiple languages. It written in RestructuredText and generated using Sphinx.</p>
 </section>
 <section id="the-google-group">
 <h3>O grupo Google<a class="headerlink" href="#the-google-group" title="Permalink to this heading"></a></h3>
 <p>Existe uma lista de discussão dedicado hospedado no Google Groups, consulte <a class="reference external" href="https://groups.google.com/g/py4web">https://groups.google.com/g/py4web</a>. Esta é a principal fonte de discussões para desenvolvedores e usuários simples. Para qualquer problema que você deve enfrentar, este é o lugar certo para procurar uma dica ou uma solução.</p>
 </section>
-<section id="the-chat-on-irc">
-<h3>O bate-papo no IRC<a class="headerlink" href="#the-chat-on-irc" title="Permalink to this heading"></a></h3>
-<p>Nós também usamos para conversar em algum momento no IRC (Internet Relay Chat, que é um texto de estilo antigo única chat). Você pode se juntar a nós livremente no <a class="reference external" href="https://webchat.freenode.net/#py4web">https://webchat.freenode.net/#py4web</a>. De vez em quando nós também usá-lo para hospedar um bate-papo pública agendada, onde você pode escrever e ler perguntas ao vivo para os desenvolvedores. Transcrições deles são, então, disponível na lista de discussão.</p>
-</section>
 <section id="the-discord-server">
 <h3>The Discord server<a class="headerlink" href="#the-discord-server" title="Permalink to this heading"></a></h3>
 <p>For quick questions and chats you can also use the free <a class="reference external" href="https://discord.gg/xCzQ9KTk3W">Discord server dedicated to py4web</a>. You could usually find many py4web developers hanging out in the channel.</p>
 </section>
 <section id="tutorials-and-video">
 <h3>Tutoriais e vídeo<a class="headerlink" href="#tutorials-and-video" title="Permalink to this heading"></a></h3>
 <p>There are many tutorials and videos available. Here are some of them:</p>
```

##### html2text {}

```diff
@@ -12,15 +12,14 @@
 [q                   ]
 ConteÃºdo:
     * O_que_Ã©_py4web?
     * Ajuda,_recursos_e_dicas
           o Recursos
                 # Este_manual
                 # O_grupo_Google
-                # O_bate-papo_no_IRC
                 # The_Discord_server
                 # Tutoriais_e_vÃ­deo
                 # As_fontes_no_GitHub
           o Dicas_e_sugestÃµes
                 # PrÃ©-requisitos
                 # Um_local_de_trabalho_python_moderna
                 # DepuraÃ§Ã£o_py4web_com_VScode
@@ -60,22 +59,14 @@
 
 **** O grupo Googleï ****
 Existe uma lista de discussÃ£o dedicado hospedado no Google Groups, consulte
 https://groups.google.com/g/py4web. Esta Ã© a principal fonte de discussÃµes
 para desenvolvedores e usuÃ¡rios simples. Para qualquer problema que vocÃª deve
 enfrentar, este Ã© o lugar certo para procurar uma dica ou uma soluÃ§Ã£o.
 
-**** O bate-papo no IRCï ****
-NÃ³s tambÃ©m usamos para conversar em algum momento no IRC (Internet Relay
-Chat, que Ã© um texto de estilo antigo Ãºnica chat). VocÃª pode se juntar a
-nÃ³s livremente no https://webchat.freenode.net/#py4web. De vez em quando nÃ³s
-tambÃ©m usÃ¡-lo para hospedar um bate-papo pÃºblica agendada, onde vocÃª pode
-escrever e ler perguntas ao vivo para os desenvolvedores. TranscriÃ§Ãµes deles
-sÃ£o, entÃ£o, disponÃ­vel na lista de discussÃ£o.
-
 **** The Discord serverï ****
 For quick questions and chats you can also use the free Discord_server
 dedicated_to_py4web. You could usually find many py4web developers hanging out
 in the channel.
 
 **** Tutoriais e vÃ­deoï ****
 There are many tutorials and videos available. Here are some of them:
```

### Comparing `py4web-1.20230314.1/py4web/assets/py4web.app._scaffold.zip` & `py4web-1.20230410.1/py4web/assets/py4web.app._scaffold.zip`

 * *Files 5% similar despite different names*

#### zipinfo {}

```diff
@@ -1,17 +1,17 @@
 Zip file size: 16674 bytes, number of entries: 15
--rw-r--r--  3.0 unx     7744 tx defN 23-Feb-26 23:36 common.py
--rw-r--r--  3.0 unx     3002 tx defN 23-Feb-26 23:34 settings.py
+-rw-r--r--  3.0 unx      254 tx defN 19-Dec-25 18:43 models.py
+-rw-r--r--  3.0 unx    11826 tx defN 23-Mar-19 22:19 static/js/utils.js
+-rw-rw-r--  3.0 unx    11431 tx defN 21-Jul-27 13:10 static/css/no.css
 -rw-r--r--  3.0 unx        1 tx stor 20-Aug-30 01:41 static/README.md
--rw-r--r--  3.0 unx    11431 tx defN 21-Jul-27 13:10 static/css/no.css
--rw-rw-r--  3.0 unx    11826 tx defN 22-Mar-20 01:46 static/js/utils.js
--rw-r--r--  3.0 unx      852 tx defN 21-Jul-27 13:10 tasks.py
+-rw-rw-r--  3.0 unx      852 tx defN 21-Jul-27 13:10 tasks.py
+-rw-r--r--  3.0 unx       97 tx defN 19-Oct-02 04:12 translations/it.json
 -rw-r--r--  3.0 unx      375 tx defN 20-Apr-13 01:13 __init__.py
--rw-r--r--  3.0 unx      254 tx defN 19-Dec-25 18:43 models.py
+-rw-r--r--  3.0 unx     1470 tx defN 22-Mar-20 01:46 controllers.py
+-rw-r--r--  3.0 unx     3002 tx defN 23-Feb-26 23:34 settings.py
+-rw-r--r--  3.0 unx      278 tx defN 20-Oct-24 20:45 templates/auth.html
 -rw-r--r--  3.0 unx      103 tx defN 20-May-18 00:26 templates/index.html
--rw-r--r--  3.0 unx        1 tx stor 19-Jul-23 06:13 templates/README.md
 -rw-r--r--  3.0 unx      264 tx defN 20-May-18 00:26 templates/generic.html
--rw-r--r--  3.0 unx     2860 tx defN 21-Oct-04 03:32 templates/layout.html
--rw-r--r--  3.0 unx      278 tx defN 20-Oct-24 20:45 templates/auth.html
--rw-rw-r--  3.0 unx     1470 tx defN 22-Mar-20 01:46 controllers.py
--rw-r--r--  3.0 unx       97 tx defN 19-Oct-02 04:12 translations/it.json
+-rw-rw-r--  3.0 unx     2860 tx defN 21-Oct-04 03:32 templates/layout.html
+-rw-r--r--  3.0 unx        1 tx stor 19-Jul-23 06:13 templates/README.md
+-rw-rw-r--  3.0 unx     7744 tx defN 23-Feb-26 23:36 common.py
 15 files, 40558 bytes uncompressed, 14264 bytes compressed:  64.8%
```

#### zipnote {}

```diff
@@ -1,46 +1,46 @@
-Filename: common.py
-Comment: 
-
-Filename: settings.py
+Filename: models.py
 Comment: 
 
-Filename: static/README.md
+Filename: static/js/utils.js
 Comment: 
 
 Filename: static/css/no.css
 Comment: 
 
-Filename: static/js/utils.js
+Filename: static/README.md
 Comment: 
 
 Filename: tasks.py
 Comment: 
 
+Filename: translations/it.json
+Comment: 
+
 Filename: __init__.py
 Comment: 
 
-Filename: models.py
+Filename: controllers.py
 Comment: 
 
-Filename: templates/index.html
+Filename: settings.py
 Comment: 
 
-Filename: templates/README.md
+Filename: templates/auth.html
 Comment: 
 
-Filename: templates/generic.html
+Filename: templates/index.html
 Comment: 
 
-Filename: templates/layout.html
+Filename: templates/generic.html
 Comment: 
 
-Filename: templates/auth.html
+Filename: templates/layout.html
 Comment: 
 
-Filename: controllers.py
+Filename: templates/README.md
 Comment: 
 
-Filename: translations/it.json
+Filename: common.py
 Comment: 
 
 Zip file comment:
```

### Comparing `py4web-1.20230314.1/py4web/assets/py4web.app.showcase.zip` & `py4web-1.20230410.1/py4web/assets/py4web.app.showcase.zip`

 * *Files 7% similar despite different names*

#### zipinfo {}

```diff
@@ -1,145 +1,145 @@
-Zip file size: 1386132 bytes, number of entries: 143
--rw-rw-r--  3.0 unx      264 tx defN 22-Jun-06 05:24 examples/session_counter.py
--rw-rw-r--  3.0 unx      396 tx defN 22-Jun-06 05:24 examples/custom_form.py
--rw-rw-r--  3.0 unx     1616 tx defN 22-Jun-06 05:24 examples/hcaptcha_form.py
--rw-rw-r--  3.0 unx      227 tx defN 22-Jun-03 05:12 examples/page_with_query.py
--rw-rw-r--  3.0 unx      125 tx defN 22-Jun-06 05:24 examples/hello_world.py
--rw-rw-r--  3.0 unx     1966 tx defN 22-Jun-06 05:24 examples/example_multiple_forms.py
--rw-rw-r--  3.0 unx      181 tx defN 22-Jun-03 05:12 examples/page_with_redirect.py
--rw-rw-r--  3.0 unx      106 tx defN 22-Jun-05 21:59 examples/page_without_template.py
--rw-rw-r--  3.0 unx      420 tx defN 22-Jun-06 05:24 examples/page_with_postback.py
--rw-rw-r--  3.0 unx      130 tx defN 22-Jun-06 05:24 examples/hello.py
--rw-rw-r--  3.0 unx      870 tx defN 22-Jun-06 05:24 examples/component_loader.py
--rw-rw-r--  3.0 unx      112 tx defN 22-Jun-03 05:12 examples/page_with_raise.py
--rw-rw-r--  3.0 unx     4809 tx defN 22-Aug-06 22:35 examples/common.py
--rw-rw-r--  3.0 unx      372 tx defN 22-Jun-06 05:24 examples/flash_example_fixture.py
--rw-rw-r--  3.0 unx      370 tx defN 22-Jun-06 05:24 examples/example_ajax_grid.py
--rw-rw-r--  3.0 unx      517 tx defN 22-Jun-11 18:53 examples/socketio.py
--rw-rw-r--  3.0 unx       88 tx defN 22-Jun-03 05:12 examples/page_with_error.py
--rw-rw-r--  3.0 unx      281 tx defN 22-Jun-03 05:12 examples/page_with_parameters.py
--rw-rw-r--  3.0 unx      145 tx defN 22-Jun-06 05:24 examples/hello_world_msg.py
--rw-rw-r--  3.0 unx     1583 tx defN 22-Jun-15 05:52 examples/example_html_grid.py
--rw-rw-r--  3.0 unx      236 tx defN 22-Jun-06 05:24 examples/example_helpers.py
--rw-rw-r--  3.0 unx      378 tx defN 22-Jun-06 05:24 examples/auth_form.py
--rw-rw-r--  3.0 unx      647 tx defN 22-Jun-06 05:24 examples/auth_forms.py
--rw-rw-r--  3.0 unx     1470 tx defN 22-Aug-09 06:04 examples/settings.py
--rw-rw-r--  3.0 unx      272 tx defN 22-Jun-11 18:53 examples/ws.py
--rw-rw-r--  3.0 unx      349 tx defN 22-Jun-06 05:24 examples/count.py
--rw-rw-r--  3.0 unx      171 tx defN 22-Jun-06 05:24 examples/page_with_template.py
--rw-rw-r--  3.0 unx      644 tx defN 22-Jun-08 06:37 examples/rpc.py
--rw-rw-r--  3.0 unx      197 tx defN 22-Jun-06 05:24 examples/session_clear.py
--rw-rw-r--  3.0 unx      375 tx defN 22-Jun-06 05:24 examples/tagsinput_form.py
--rw-rw-r--  3.0 unx      228 tx defN 22-Jun-06 05:24 examples/flash_example_naive.py
--rw-rw-r--  3.0 unx      465 tx defN 22-Jun-06 05:24 examples/update_form.py
--rw-rw-r--  3.0 unx     2617 tx defN 22-Jun-06 05:24 examples/models.py
--rw-rw-r--  3.0 unx      414 tx defN 22-Jun-06 05:24 examples/test_expose.py
--rw-rw-r--  3.0 unx     2749 tx defN 22-Jun-09 05:06 examples/rest.py
--rw-rw-r--  3.0 unx      456 tx defN 22-Jun-06 05:24 examples/create_form.py
--rwxrwxr-x  3.0 unx      422 tx defN 22-Jun-03 05:12 examples/ws_client_example.py
--rw-rw-r--  3.0 unx      255 tx defN 22-Jun-06 05:24 examples/show_a_button.py
--rw-rw-r--  3.0 unx       12 tx stor 22-Jun-03 05:12 static/hello.txt
--rw-rw-r--  3.0 unx        1 tx stor 22-Jun-03 05:12 static/ws/README.md
--rw-rw-r--  3.0 unx     5384 tx defN 22-Jun-06 05:24 static/components/grid/grid.js
--rw-rw-r--  3.0 unx     3299 tx defN 22-Jun-06 05:24 static/components/grid/grid.html
--rw-rw-r--  3.0 unx      411 tx defN 22-Jun-06 05:24 static/components/grid/grid.css
--rw-rw-r--  3.0 unx       43 tx stor 22-Jun-06 05:24 static/components/vueform/vueform.css
--rw-rw-r--  3.0 unx   257636 tx defN 22-Jun-03 05:12 static/components/vueform/luxon.js
--rw-rw-r--  3.0 unx    70115 tx defN 22-Jun-03 05:12 static/components/vueform/luxon.min.js
--rw-rw-r--  3.0 unx     3400 tx defN 22-Jun-06 05:24 static/components/vueform/vueform.html
--rw-rw-r--  3.0 unx     7263 tx defN 22-Jun-06 05:24 static/components/vueform/vueform.js
--rw-rw-r--  3.0 unx       83 tx defN 22-Jun-03 05:12 static/components/fileupload/fileupload.html
--rw-rw-r--  3.0 unx     1232 tx defN 22-Jun-03 05:12 static/components/fileupload/fileupload.js
--rw-rw-r--  3.0 unx       35 tx stor 22-Jun-03 05:12 static/components/fileupload/fileupload.css
--rw-rw-r--  3.0 unx     6013 tx defN 22-Jun-03 05:12 static/components/mtable.js
--rw-rw-r--  3.0 unx      308 tx defN 22-Jun-03 05:12 static/components/starrater/starrater.html
--rw-rw-r--  3.0 unx     1681 tx defN 22-Jun-03 05:12 static/components/starrater/starrater.js
--rw-rw-r--  3.0 unx        0 bx stor 22-Jun-03 05:12 static/components/starrater/starrater.css
--rw-rw-r--  3.0 unx     5682 tx defN 22-Jun-03 05:12 static/components/mtable.html
--rw-rw-r--  3.0 unx      977 tx defN 22-Jun-03 05:12 static/firebase-push.html
--rw-rw-r--  3.0 unx        1 tx stor 22-Jun-03 05:12 static/socketio/README.md
--rw-rw-r--  3.0 unx     9998 tx defN 22-Jun-06 05:24 static/error.html
--rw-rw-r--  3.0 unx     1903 tx defN 22-Jun-06 01:49 static/css/prism.css
--rw-rw-r--  3.0 unx    11417 tx defN 22-Jun-03 05:12 static/css/no.css
--rw-rw-r--  3.0 unx    19064 tx defN 22-Jun-06 01:41 static/css/prism.js
--rw-rw-r--  3.0 unx      496 tx defN 22-Jun-06 05:24 static/js/star_rater_vue.js
--rw-rw-r--  3.0 unx      868 tx defN 22-Jun-03 05:12 static/js/firebase-push.js
--rw-rw-r--  3.0 unx    68547 tx defN 22-Jun-03 05:12 static/js/sugar.min.js
--rw-rw-r--  3.0 unx     8311 tx defN 22-Jun-03 05:12 static/js/utils.min.js
--rw-rw-r--  3.0 unx    11826 tx defN 22-Jun-03 05:12 static/js/utils.js
--rw-rw-r--  3.0 unx    14265 tx defN 22-Jun-03 05:12 static/js/axios.min.js
--rw-rw-r--  3.0 unx    93670 tx defN 22-Jun-03 05:12 static/js/vue.min.js
--rw-rw-r--  3.0 unx    19055 tx defN 22-Jun-03 05:12 static/js/prism.js
--rw-rw-r--  3.0 unx   341462 tx defN 22-Jun-03 05:12 static/js/vue.js
--rw-rw-r--  3.0 unx     5384 tx defN 22-Jun-06 05:24 static/components-bulma/grid/grid.js
--rw-rw-r--  3.0 unx     3369 tx defN 22-Jun-06 05:24 static/components-bulma/grid/grid.html
--rw-rw-r--  3.0 unx   257636 tx defN 22-Jun-06 05:24 static/components-bulma/grid/luxon.js
--rw-rw-r--  3.0 unx      411 tx defN 22-Jun-06 05:24 static/components-bulma/grid/grid.css
--rw-rw-r--  3.0 unx       43 tx stor 22-Jun-03 05:12 static/components-bulma/vueform/vueform.css
--rw-rw-r--  3.0 unx   257636 tx defN 22-Jun-03 05:12 static/components-bulma/vueform/luxon.js
--rw-rw-r--  3.0 unx    70115 tx defN 22-Jun-03 05:12 static/components-bulma/vueform/luxon.min.js
--rw-rw-r--  3.0 unx     3400 tx defN 22-Jun-06 05:24 static/components-bulma/vueform/vueform.html
--rw-rw-r--  3.0 unx     7257 tx defN 22-Jun-06 05:24 static/components-bulma/vueform/vueform.js
--rw-rw-r--  3.0 unx       83 tx defN 22-Jun-03 05:12 static/components-bulma/fileupload/fileupload.html
--rw-rw-r--  3.0 unx     1232 tx defN 22-Jun-03 05:12 static/components-bulma/fileupload/fileupload.js
--rw-rw-r--  3.0 unx       35 tx stor 22-Jun-03 05:12 static/components-bulma/fileupload/fileupload.css
--rw-rw-r--  3.0 unx     6013 tx defN 22-Jun-03 05:12 static/components-bulma/mtable.js
--rw-rw-r--  3.0 unx      308 tx defN 22-Jun-03 05:12 static/components-bulma/starrater/starrater.html
--rw-rw-r--  3.0 unx     1687 tx defN 22-Jun-03 05:12 static/components-bulma/starrater/starrater.js
--rw-rw-r--  3.0 unx        0 bx stor 22-Jun-03 05:12 static/components-bulma/starrater/starrater.css
--rw-rw-r--  3.0 unx     5682 tx defN 22-Jun-03 05:12 static/components-bulma/mtable.html
--rw-rw-r--  3.0 unx  7330359 tx defN 22-Jun-03 05:12 static/data/uscities.json
--rw-rw-r--  3.0 unx   295408 tx defN 22-Jun-03 05:12 static/data/zip_codes.json
--rw-rw-r--  3.0 unx     4146 tx defN 22-Jun-08 07:33 __init__.py
--rw-rw-r--  3.0 unx       20 tx stor 22-Jun-03 05:12 uploads/README.md
--rw-rw-r--  3.0 unx     6784 tx defN 22-Jun-08 07:32 templates/index.html
--rw-rw-r--  3.0 unx     2172 tx defN 22-Jun-11 18:53 templates/ws/ws_index.html
--rw-rw-r--  3.0 unx      263 tx defN 22-Jun-15 05:18 templates/examples/session_counter.html
--rw-rw-r--  3.0 unx      242 tx defN 22-Jun-15 05:18 templates/examples/flash_example.html
--rw-rw-r--  3.0 unx     1711 tx defN 22-Jun-15 05:18 templates/examples/tagsinput_form.html
--rw-rw-r--  3.0 unx       26 tx stor 22-Jun-15 05:18 templates/examples/flash_example_next.html
--rw-rw-r--  3.0 unx      242 tx defN 22-Jun-15 05:18 templates/examples/forms.html
--rw-rw-r--  3.0 unx      193 tx defN 22-Jun-15 05:18 templates/examples/auth_form.html
--rw-rw-r--  3.0 unx      990 tx defN 22-Jun-15 05:18 templates/examples/custom_form.html
--rw-rw-r--  3.0 unx      305 tx defN 22-Jun-15 05:18 templates/examples/form.html
--rw-rw-r--  3.0 unx      143 tx defN 22-Jun-15 05:18 templates/examples/component_loader.html
--rw-rw-r--  3.0 unx      646 tx defN 22-Jun-15 05:18 templates/examples/auth_forms.html
--rw-rw-r--  3.0 unx      143 tx defN 22-Jun-15 05:45 templates/examples/html_grid.html
--rw-rw-r--  3.0 unx      228 tx defN 22-Jun-15 05:18 templates/examples/generic.html
--rw-rw-r--  3.0 unx       82 tx defN 22-Jun-15 05:18 templates/examples/page_with_template.html
--rw-rw-r--  3.0 unx      551 tx defN 22-Jun-15 05:18 templates/examples/auth_custom_login.html
--rw-rw-r--  3.0 unx     1025 tx defN 22-Jun-09 05:11 templates/examples/rest_info.html
--rw-rw-r--  3.0 unx      189 tx defN 22-Jun-15 05:18 templates/examples/hcaptcha_form.html
--rw-rw-r--  3.0 unx       69 tx defN 22-Jun-15 05:18 templates/examples/ajax_grid.html
--rw-rw-r--  3.0 unx     1913 tx defN 22-Jun-11 18:53 templates/socketio/socketio_index.html
--rw-rw-r--  3.0 unx      502 tx defN 22-Jun-06 05:24 templates/vue/star_rater_vue.html
--rw-rw-r--  3.0 unx      448 tx defN 22-Jun-06 05:24 templates/vue/starrating.html
--rw-rw-r--  3.0 unx      486 tx defN 22-Jun-06 05:24 templates/vue/edit_form.html
--rw-rw-r--  3.0 unx      372 tx defN 22-Jun-06 05:24 templates/vue/file_uploader.html
--rw-rw-r--  3.0 unx      544 tx defN 22-Jun-06 05:24 templates/vue/star_rater_vue_bulma.html
--rw-rw-r--  3.0 unx      488 tx defN 22-Jun-06 05:24 templates/vue/insert_form.html
--rw-rw-r--  3.0 unx      683 tx defN 22-Jun-06 05:24 templates/vue/vue_grid_and_forms.html
--rw-rw-r--  3.0 unx      392 tx defN 22-Jun-06 05:24 templates/vue/vuegrid_bulma.html
--rw-rw-r--  3.0 unx      486 tx defN 22-Jun-06 05:24 templates/vue/view_form.html
--rw-rw-r--  3.0 unx      374 tx defN 22-Jun-06 05:24 templates/vue/vuegrid.html
--rw-rw-r--  3.0 unx     2778 tx defN 22-Jun-08 06:25 templates/layout.html
--rw-rw-r--  3.0 unx      278 tx defN 22-Jun-06 05:24 templates/auth.html
--rw-rw-r--  3.0 unx     2156 tx defN 22-Jun-03 05:12 templates/layout_bulma.html
--rw-rw-r--  3.0 unx      430 tx defN 22-Jun-06 05:24 templates/show.html
--rw-rw-r--  3.0 unx      236 tx defN 22-Jun-03 05:12 translations/it.json
--rw-rw-r--  3.0 unx      196 tx defN 22-Jun-03 05:12 translations/en.json
--rw-rw-r--  3.0 unx     3031 tx defN 22-Jun-06 05:24 vue_components_examples/vue_grid_and_forms.py
--rw-rw-r--  3.0 unx     1597 tx defN 22-Jun-06 05:24 vue_components_examples/components/fileupload.py
--rw-rw-r--  3.0 unx    10333 tx defN 22-Jun-06 05:24 vue_components_examples/components/vueform.py
--rw-rw-r--  3.0 unx     7777 tx defN 22-Jun-06 05:24 vue_components_examples/components/grid.py
--rw-rw-r--  3.0 unx     7858 tx defN 22-Jun-06 05:24 vue_components_examples/components/README.md
--rw-rw-r--  3.0 unx     2078 tx defN 22-Jun-06 05:24 vue_components_examples/components/starrater.py
--rw-rw-r--  3.0 unx      324 tx defN 22-Jun-06 05:24 vue_components_examples/vue_file_uploader.py
--rw-rw-r--  3.0 unx     1215 tx defN 22-Jun-06 05:24 vue_components_examples/vue_star_rater.py
--rw-rw-r--  3.0 unx       32 tx stor 22-Jun-06 05:24 vue_components_examples/common.py
--rw-rw-r--  3.0 unx     1124 tx defN 22-Jun-06 05:24 vue_components_examples/vue_edit_form.py
--rw-rw-r--  3.0 unx      853 tx defN 22-Jun-06 05:24 vue_components_examples/vue_insert_form.py
--rw-rw-r--  3.0 unx     1149 tx defN 22-Jun-06 05:24 vue_components_examples/vue_view_form.py
--rw-rw-r--  3.0 unx       34 tx stor 22-Jun-06 05:24 vue_components_examples/settings.py
--rw-rw-r--  3.0 unx     1390 tx defN 22-Jun-06 05:24 vue_components_examples/models.py
--rw-rw-r--  3.0 unx      302 tx defN 22-Jun-06 05:24 vue_components_examples/vue_grid.py
-143 files, 9309468 bytes uncompressed, 1358974 bytes compressed:  85.4%
+Zip file size: 1386102 bytes, number of entries: 143
+-rw-r--r--  3.0 unx      181 tx defN 22-Jun-03 05:12 examples/page_with_redirect.py
+-rw-r--r--  3.0 unx      197 tx defN 22-Jun-06 05:24 examples/session_clear.py
+-rw-r--r--  3.0 unx      281 tx defN 22-Jun-03 05:12 examples/page_with_parameters.py
+-rw-r--r--  3.0 unx     2617 tx defN 22-Jun-06 05:24 examples/models.py
+-rw-r--r--  3.0 unx     1616 tx defN 22-Jun-06 05:24 examples/hcaptcha_form.py
+-rw-r--r--  3.0 unx      517 tx defN 22-Jun-11 18:53 examples/socketio.py
+-rw-r--r--  3.0 unx      255 tx defN 22-Jun-06 05:24 examples/show_a_button.py
+-rw-r--r--  3.0 unx      228 tx defN 22-Jun-06 05:24 examples/flash_example_naive.py
+-rw-r--r--  3.0 unx      372 tx defN 22-Jun-06 05:24 examples/flash_example_fixture.py
+-rw-r--r--  3.0 unx      414 tx defN 22-Jun-06 05:24 examples/test_expose.py
+-rw-r--r--  3.0 unx     2749 tx defN 22-Jun-09 05:06 examples/rest.py
+-rw-r--r--  3.0 unx     1583 tx defN 22-Jun-15 05:52 examples/example_html_grid.py
+-rw-r--r--  3.0 unx      349 tx defN 22-Jun-06 05:24 examples/count.py
+-rw-r--r--  3.0 unx      171 tx defN 22-Jun-06 05:24 examples/page_with_template.py
+-rw-r--r--  3.0 unx      396 tx defN 22-Jun-06 05:24 examples/custom_form.py
+-rw-r--r--  3.0 unx     1966 tx defN 22-Jun-06 05:24 examples/example_multiple_forms.py
+-rw-r--r--  3.0 unx      456 tx defN 22-Jun-06 05:24 examples/create_form.py
+-rw-r--r--  3.0 unx      644 tx defN 22-Jun-08 06:37 examples/rpc.py
+-rw-r--r--  3.0 unx      370 tx defN 22-Jun-06 05:24 examples/example_ajax_grid.py
+-rw-r--r--  3.0 unx      647 tx defN 22-Jun-06 05:24 examples/auth_forms.py
+-rw-r--r--  3.0 unx      465 tx defN 22-Jun-06 05:24 examples/update_form.py
+-rw-r--r--  3.0 unx      264 tx defN 22-Jun-06 05:24 examples/session_counter.py
+-rw-r--r--  3.0 unx      375 tx defN 22-Jun-06 05:24 examples/tagsinput_form.py
+-rw-r--r--  3.0 unx      870 tx defN 22-Jun-06 05:24 examples/component_loader.py
+-rw-r--r--  3.0 unx      378 tx defN 22-Jun-06 05:24 examples/auth_form.py
+-rw-r--r--  3.0 unx      227 tx defN 22-Jun-03 05:12 examples/page_with_query.py
+-rw-r--r--  3.0 unx      420 tx defN 22-Jun-06 05:24 examples/page_with_postback.py
+-rw-r--r--  3.0 unx      272 tx defN 22-Jun-11 18:53 examples/ws.py
+-rw-r--r--  3.0 unx       88 tx defN 22-Jun-03 05:12 examples/page_with_error.py
+-rw-r--r--  3.0 unx     1470 tx defN 22-Aug-09 06:04 examples/settings.py
+-rw-r--r--  3.0 unx      145 tx defN 22-Jun-06 05:24 examples/hello_world_msg.py
+-rw-r--r--  3.0 unx      106 tx defN 22-Jun-03 05:12 examples/page_without_template.py
+-rwxr--r--  3.0 unx      422 tx defN 22-Jun-03 05:12 examples/ws_client_example.py
+-rw-r--r--  3.0 unx      112 tx defN 22-Jun-03 05:12 examples/page_with_raise.py
+-rw-r--r--  3.0 unx      236 tx defN 22-Jun-06 05:24 examples/example_helpers.py
+-rw-r--r--  3.0 unx      130 tx defN 22-Jun-06 05:24 examples/hello.py
+-rw-r--r--  3.0 unx     4809 tx defN 22-Jun-06 05:24 examples/common.py
+-rw-r--r--  3.0 unx      125 tx defN 22-Jun-06 05:24 examples/hello_world.py
+-rw-r--r--  3.0 unx     6013 tx defN 22-Jun-03 05:12 static/components/mtable.js
+-rw-r--r--  3.0 unx      411 tx defN 22-Jun-05 21:13 static/components/grid/grid.css
+-rw-r--r--  3.0 unx     5384 tx defN 22-Jun-05 21:13 static/components/grid/grid.js
+-rw-r--r--  3.0 unx     3299 tx defN 22-Jun-05 21:13 static/components/grid/grid.html
+-rw-r--r--  3.0 unx     7263 tx defN 22-Jun-05 21:13 static/components/vueform/vueform.js
+-rw-r--r--  3.0 unx       43 tx stor 22-Jun-05 21:13 static/components/vueform/vueform.css
+-rw-r--r--  3.0 unx    70115 tx defN 22-Jun-03 05:12 static/components/vueform/luxon.min.js
+-rw-r--r--  3.0 unx   257636 tx defN 22-Jun-03 05:12 static/components/vueform/luxon.js
+-rw-r--r--  3.0 unx     3400 tx defN 22-Jun-05 21:13 static/components/vueform/vueform.html
+-rw-r--r--  3.0 unx        0 bx stor 22-Jun-03 05:12 static/components/starrater/starrater.css
+-rw-r--r--  3.0 unx      308 tx defN 22-Jun-03 05:12 static/components/starrater/starrater.html
+-rw-r--r--  3.0 unx     1681 tx defN 22-Jun-03 05:12 static/components/starrater/starrater.js
+-rw-r--r--  3.0 unx     5682 tx defN 22-Jun-03 05:12 static/components/mtable.html
+-rw-r--r--  3.0 unx       83 tx defN 22-Jun-03 05:12 static/components/fileupload/fileupload.html
+-rw-r--r--  3.0 unx       35 tx stor 22-Jun-03 05:12 static/components/fileupload/fileupload.css
+-rw-r--r--  3.0 unx     1232 tx defN 22-Jun-03 05:12 static/components/fileupload/fileupload.js
+-rw-r--r--  3.0 unx    19055 tx defN 22-Jun-03 05:12 static/js/prism.js
+-rw-r--r--  3.0 unx      496 tx defN 22-Jun-05 23:08 static/js/star_rater_vue.js
+-rw-r--r--  3.0 unx      868 tx defN 22-Jun-03 05:12 static/js/firebase-push.js
+-rw-r--r--  3.0 unx    11826 tx defN 22-Jun-03 05:12 static/js/utils.js
+-rw-r--r--  3.0 unx    93670 tx defN 22-Jun-03 05:12 static/js/vue.min.js
+-rw-r--r--  3.0 unx    68547 tx defN 22-Jun-03 05:12 static/js/sugar.min.js
+-rw-r--r--  3.0 unx    14265 tx defN 22-Jun-03 05:12 static/js/axios.min.js
+-rw-r--r--  3.0 unx   341462 tx defN 22-Jun-03 05:12 static/js/vue.js
+-rw-r--r--  3.0 unx     8311 tx defN 22-Jun-03 05:12 static/js/utils.min.js
+-rw-r--r--  3.0 unx     9998 tx defN 22-Jun-05 22:03 static/error.html
+-rw-r--r--  3.0 unx   295408 tx defN 22-Jun-03 05:12 static/data/zip_codes.json
+-rw-r--r--  3.0 unx  7330359 tx defN 22-Jun-03 05:12 static/data/uscities.json
+-rw-r--r--  3.0 unx      977 tx defN 22-Jun-03 05:12 static/firebase-push.html
+-rw-r--r--  3.0 unx    19064 tx defN 22-Jun-06 01:41 static/css/prism.js
+-rw-r--r--  3.0 unx     1903 tx defN 22-Jun-06 01:49 static/css/prism.css
+-rw-r--r--  3.0 unx    11417 tx defN 22-Jun-03 05:12 static/css/no.css
+-rw-r--r--  3.0 unx     6013 tx defN 22-Jun-03 05:12 static/components-bulma/mtable.js
+-rw-r--r--  3.0 unx      411 tx defN 22-Jun-05 21:13 static/components-bulma/grid/grid.css
+-rw-r--r--  3.0 unx   257636 tx defN 22-Jun-05 21:13 static/components-bulma/grid/luxon.js
+-rw-r--r--  3.0 unx     5384 tx defN 22-Jun-05 21:13 static/components-bulma/grid/grid.js
+-rw-r--r--  3.0 unx     3369 tx defN 22-Jun-05 21:13 static/components-bulma/grid/grid.html
+-rw-r--r--  3.0 unx     7257 tx defN 22-Jun-05 21:13 static/components-bulma/vueform/vueform.js
+-rw-r--r--  3.0 unx       43 tx stor 22-Jun-03 05:12 static/components-bulma/vueform/vueform.css
+-rw-r--r--  3.0 unx    70115 tx defN 22-Jun-03 05:12 static/components-bulma/vueform/luxon.min.js
+-rw-r--r--  3.0 unx   257636 tx defN 22-Jun-03 05:12 static/components-bulma/vueform/luxon.js
+-rw-r--r--  3.0 unx     3400 tx defN 22-Jun-05 21:13 static/components-bulma/vueform/vueform.html
+-rw-r--r--  3.0 unx        0 bx stor 22-Jun-03 05:12 static/components-bulma/starrater/starrater.css
+-rw-r--r--  3.0 unx      308 tx defN 22-Jun-03 05:12 static/components-bulma/starrater/starrater.html
+-rw-r--r--  3.0 unx     1687 tx defN 22-Jun-03 05:12 static/components-bulma/starrater/starrater.js
+-rw-r--r--  3.0 unx     5682 tx defN 22-Jun-03 05:12 static/components-bulma/mtable.html
+-rw-r--r--  3.0 unx       83 tx defN 22-Jun-03 05:12 static/components-bulma/fileupload/fileupload.html
+-rw-r--r--  3.0 unx       35 tx stor 22-Jun-03 05:12 static/components-bulma/fileupload/fileupload.css
+-rw-r--r--  3.0 unx     1232 tx defN 22-Jun-03 05:12 static/components-bulma/fileupload/fileupload.js
+-rw-r--r--  3.0 unx       12 tx stor 22-Jun-03 05:12 static/hello.txt
+-rw-r--r--  3.0 unx        1 tx stor 22-Jun-03 05:12 static/ws/README.md
+-rw-r--r--  3.0 unx        1 tx stor 22-Jun-03 05:12 static/socketio/README.md
+-rw-r--r--  3.0 unx      236 tx defN 22-Jun-03 05:12 translations/it.json
+-rw-r--r--  3.0 unx      196 tx defN 22-Jun-03 05:12 translations/en.json
+-rw-r--r--  3.0 unx     4146 tx defN 22-Jun-08 07:33 __init__.py
+-rw-r--r--  3.0 unx    10333 tx defN 22-Jun-05 22:35 vue_components_examples/components/vueform.py
+-rw-r--r--  3.0 unx     2078 tx defN 22-Jun-03 05:12 vue_components_examples/components/starrater.py
+-rw-r--r--  3.0 unx     1597 tx defN 22-Jun-05 21:13 vue_components_examples/components/fileupload.py
+-rw-r--r--  3.0 unx     7777 tx defN 22-Jun-05 22:49 vue_components_examples/components/grid.py
+-rw-r--r--  3.0 unx     7858 tx defN 22-Jun-05 21:35 vue_components_examples/components/README.md
+-rw-r--r--  3.0 unx     1390 tx defN 22-Jun-05 22:35 vue_components_examples/models.py
+-rw-r--r--  3.0 unx     1215 tx defN 22-Jun-05 22:35 vue_components_examples/vue_star_rater.py
+-rw-r--r--  3.0 unx      853 tx defN 22-Jun-05 22:35 vue_components_examples/vue_insert_form.py
+-rw-r--r--  3.0 unx     1149 tx defN 22-Jun-05 22:35 vue_components_examples/vue_view_form.py
+-rw-r--r--  3.0 unx      324 tx defN 22-Jun-05 21:35 vue_components_examples/vue_file_uploader.py
+-rw-r--r--  3.0 unx     3031 tx defN 22-Jun-05 22:35 vue_components_examples/vue_grid_and_forms.py
+-rw-r--r--  3.0 unx       34 tx stor 22-Jun-05 22:35 vue_components_examples/settings.py
+-rw-r--r--  3.0 unx      302 tx defN 22-Jun-05 22:23 vue_components_examples/vue_grid.py
+-rw-r--r--  3.0 unx       32 tx stor 22-Jun-05 22:35 vue_components_examples/common.py
+-rw-r--r--  3.0 unx     1124 tx defN 22-Jun-05 22:35 vue_components_examples/vue_edit_form.py
+-rw-r--r--  3.0 unx       20 tx stor 22-Jun-03 05:12 uploads/README.md
+-rw-r--r--  3.0 unx      430 tx defN 22-Jun-06 01:49 templates/show.html
+-rw-r--r--  3.0 unx      278 tx defN 22-Jun-05 22:33 templates/auth.html
+-rw-r--r--  3.0 unx      143 tx defN 22-Jun-15 05:18 templates/examples/component_loader.html
+-rw-r--r--  3.0 unx       82 tx defN 22-Jun-15 05:18 templates/examples/page_with_template.html
+-rw-r--r--  3.0 unx      869 tx defN 23-Mar-17 03:39 templates/examples/custom_form.html
+-rw-r--r--  3.0 unx      143 tx defN 22-Jun-15 05:45 templates/examples/html_grid.html
+-rw-r--r--  3.0 unx      242 tx defN 22-Jun-15 05:18 templates/examples/flash_example.html
+-rw-r--r--  3.0 unx     1025 tx defN 22-Jun-09 05:11 templates/examples/rest_info.html
+-rw-r--r--  3.0 unx      551 tx defN 22-Jun-15 05:18 templates/examples/auth_custom_login.html
+-rw-r--r--  3.0 unx      242 tx defN 22-Jun-15 05:18 templates/examples/forms.html
+-rw-r--r--  3.0 unx       69 tx defN 22-Jun-15 05:18 templates/examples/ajax_grid.html
+-rw-r--r--  3.0 unx     1711 tx defN 22-Jun-15 05:18 templates/examples/tagsinput_form.html
+-rw-r--r--  3.0 unx       26 tx stor 22-Jun-15 05:18 templates/examples/flash_example_next.html
+-rw-r--r--  3.0 unx      189 tx defN 22-Jun-15 05:18 templates/examples/hcaptcha_form.html
+-rw-r--r--  3.0 unx      193 tx defN 22-Jun-15 05:18 templates/examples/auth_form.html
+-rw-r--r--  3.0 unx      305 tx defN 22-Jun-15 05:18 templates/examples/form.html
+-rw-r--r--  3.0 unx      263 tx defN 22-Jun-15 05:18 templates/examples/session_counter.html
+-rw-r--r--  3.0 unx      646 tx defN 22-Jun-15 05:18 templates/examples/auth_forms.html
+-rw-r--r--  3.0 unx      228 tx defN 22-Jun-15 05:18 templates/examples/generic.html
+-rw-r--r--  3.0 unx     2156 tx defN 22-Jun-03 05:12 templates/layout_bulma.html
+-rw-r--r--  3.0 unx     2172 tx defN 22-Jun-11 18:53 templates/ws/ws_index.html
+-rw-r--r--  3.0 unx      502 tx defN 22-Jun-06 05:24 templates/vue/star_rater_vue.html
+-rw-r--r--  3.0 unx      488 tx defN 22-Jun-06 05:24 templates/vue/insert_form.html
+-rw-r--r--  3.0 unx      374 tx defN 22-Jun-06 05:24 templates/vue/vuegrid.html
+-rw-r--r--  3.0 unx      544 tx defN 22-Jun-06 05:24 templates/vue/star_rater_vue_bulma.html
+-rw-r--r--  3.0 unx      392 tx defN 22-Jun-06 05:24 templates/vue/vuegrid_bulma.html
+-rw-r--r--  3.0 unx      486 tx defN 22-Jun-06 05:24 templates/vue/edit_form.html
+-rw-r--r--  3.0 unx      683 tx defN 22-Jun-06 05:24 templates/vue/vue_grid_and_forms.html
+-rw-r--r--  3.0 unx      372 tx defN 22-Jun-06 05:24 templates/vue/file_uploader.html
+-rw-r--r--  3.0 unx      486 tx defN 22-Jun-06 05:24 templates/vue/view_form.html
+-rw-r--r--  3.0 unx      448 tx defN 22-Jun-06 05:24 templates/vue/starrating.html
+-rw-r--r--  3.0 unx     6784 tx defN 22-Jun-08 07:32 templates/index.html
+-rw-r--r--  3.0 unx     1913 tx defN 22-Jun-11 18:53 templates/socketio/socketio_index.html
+-rw-r--r--  3.0 unx     2778 tx defN 22-Jun-08 06:25 templates/layout.html
+143 files, 9309347 bytes uncompressed, 1358944 bytes compressed:  85.4%
```

#### zipnote {}

```diff
@@ -1,430 +1,430 @@
-Filename: examples/session_counter.py
+Filename: examples/page_with_redirect.py
 Comment: 
 
-Filename: examples/custom_form.py
+Filename: examples/session_clear.py
 Comment: 
 
-Filename: examples/hcaptcha_form.py
+Filename: examples/page_with_parameters.py
 Comment: 
 
-Filename: examples/page_with_query.py
+Filename: examples/models.py
 Comment: 
 
-Filename: examples/hello_world.py
+Filename: examples/hcaptcha_form.py
 Comment: 
 
-Filename: examples/example_multiple_forms.py
+Filename: examples/socketio.py
 Comment: 
 
-Filename: examples/page_with_redirect.py
+Filename: examples/show_a_button.py
 Comment: 
 
-Filename: examples/page_without_template.py
+Filename: examples/flash_example_naive.py
 Comment: 
 
-Filename: examples/page_with_postback.py
+Filename: examples/flash_example_fixture.py
 Comment: 
 
-Filename: examples/hello.py
+Filename: examples/test_expose.py
 Comment: 
 
-Filename: examples/component_loader.py
+Filename: examples/rest.py
 Comment: 
 
-Filename: examples/page_with_raise.py
+Filename: examples/example_html_grid.py
 Comment: 
 
-Filename: examples/common.py
+Filename: examples/count.py
 Comment: 
 
-Filename: examples/flash_example_fixture.py
+Filename: examples/page_with_template.py
 Comment: 
 
-Filename: examples/example_ajax_grid.py
+Filename: examples/custom_form.py
 Comment: 
 
-Filename: examples/socketio.py
+Filename: examples/example_multiple_forms.py
 Comment: 
 
-Filename: examples/page_with_error.py
+Filename: examples/create_form.py
 Comment: 
 
-Filename: examples/page_with_parameters.py
+Filename: examples/rpc.py
 Comment: 
 
-Filename: examples/hello_world_msg.py
+Filename: examples/example_ajax_grid.py
 Comment: 
 
-Filename: examples/example_html_grid.py
+Filename: examples/auth_forms.py
 Comment: 
 
-Filename: examples/example_helpers.py
+Filename: examples/update_form.py
 Comment: 
 
-Filename: examples/auth_form.py
+Filename: examples/session_counter.py
 Comment: 
 
-Filename: examples/auth_forms.py
+Filename: examples/tagsinput_form.py
 Comment: 
 
-Filename: examples/settings.py
+Filename: examples/component_loader.py
 Comment: 
 
-Filename: examples/ws.py
+Filename: examples/auth_form.py
 Comment: 
 
-Filename: examples/count.py
+Filename: examples/page_with_query.py
 Comment: 
 
-Filename: examples/page_with_template.py
+Filename: examples/page_with_postback.py
 Comment: 
 
-Filename: examples/rpc.py
+Filename: examples/ws.py
 Comment: 
 
-Filename: examples/session_clear.py
+Filename: examples/page_with_error.py
 Comment: 
 
-Filename: examples/tagsinput_form.py
+Filename: examples/settings.py
 Comment: 
 
-Filename: examples/flash_example_naive.py
+Filename: examples/hello_world_msg.py
 Comment: 
 
-Filename: examples/update_form.py
+Filename: examples/page_without_template.py
 Comment: 
 
-Filename: examples/models.py
+Filename: examples/ws_client_example.py
 Comment: 
 
-Filename: examples/test_expose.py
+Filename: examples/page_with_raise.py
 Comment: 
 
-Filename: examples/rest.py
+Filename: examples/example_helpers.py
 Comment: 
 
-Filename: examples/create_form.py
+Filename: examples/hello.py
 Comment: 
 
-Filename: examples/ws_client_example.py
+Filename: examples/common.py
 Comment: 
 
-Filename: examples/show_a_button.py
+Filename: examples/hello_world.py
 Comment: 
 
-Filename: static/hello.txt
+Filename: static/components/mtable.js
 Comment: 
 
-Filename: static/ws/README.md
+Filename: static/components/grid/grid.css
 Comment: 
 
 Filename: static/components/grid/grid.js
 Comment: 
 
 Filename: static/components/grid/grid.html
 Comment: 
 
-Filename: static/components/grid/grid.css
+Filename: static/components/vueform/vueform.js
 Comment: 
 
 Filename: static/components/vueform/vueform.css
 Comment: 
 
-Filename: static/components/vueform/luxon.js
+Filename: static/components/vueform/luxon.min.js
 Comment: 
 
-Filename: static/components/vueform/luxon.min.js
+Filename: static/components/vueform/luxon.js
 Comment: 
 
 Filename: static/components/vueform/vueform.html
 Comment: 
 
-Filename: static/components/vueform/vueform.js
+Filename: static/components/starrater/starrater.css
 Comment: 
 
-Filename: static/components/fileupload/fileupload.html
+Filename: static/components/starrater/starrater.html
 Comment: 
 
-Filename: static/components/fileupload/fileupload.js
+Filename: static/components/starrater/starrater.js
 Comment: 
 
-Filename: static/components/fileupload/fileupload.css
+Filename: static/components/mtable.html
 Comment: 
 
-Filename: static/components/mtable.js
+Filename: static/components/fileupload/fileupload.html
 Comment: 
 
-Filename: static/components/starrater/starrater.html
+Filename: static/components/fileupload/fileupload.css
 Comment: 
 
-Filename: static/components/starrater/starrater.js
+Filename: static/components/fileupload/fileupload.js
 Comment: 
 
-Filename: static/components/starrater/starrater.css
+Filename: static/js/prism.js
 Comment: 
 
-Filename: static/components/mtable.html
+Filename: static/js/star_rater_vue.js
 Comment: 
 
-Filename: static/firebase-push.html
+Filename: static/js/firebase-push.js
 Comment: 
 
-Filename: static/socketio/README.md
+Filename: static/js/utils.js
 Comment: 
 
-Filename: static/error.html
+Filename: static/js/vue.min.js
 Comment: 
 
-Filename: static/css/prism.css
+Filename: static/js/sugar.min.js
 Comment: 
 
-Filename: static/css/no.css
+Filename: static/js/axios.min.js
 Comment: 
 
-Filename: static/css/prism.js
+Filename: static/js/vue.js
 Comment: 
 
-Filename: static/js/star_rater_vue.js
+Filename: static/js/utils.min.js
 Comment: 
 
-Filename: static/js/firebase-push.js
+Filename: static/error.html
 Comment: 
 
-Filename: static/js/sugar.min.js
+Filename: static/data/zip_codes.json
 Comment: 
 
-Filename: static/js/utils.min.js
+Filename: static/data/uscities.json
 Comment: 
 
-Filename: static/js/utils.js
+Filename: static/firebase-push.html
 Comment: 
 
-Filename: static/js/axios.min.js
+Filename: static/css/prism.js
 Comment: 
 
-Filename: static/js/vue.min.js
+Filename: static/css/prism.css
 Comment: 
 
-Filename: static/js/prism.js
+Filename: static/css/no.css
 Comment: 
 
-Filename: static/js/vue.js
+Filename: static/components-bulma/mtable.js
 Comment: 
 
-Filename: static/components-bulma/grid/grid.js
+Filename: static/components-bulma/grid/grid.css
 Comment: 
 
-Filename: static/components-bulma/grid/grid.html
+Filename: static/components-bulma/grid/luxon.js
 Comment: 
 
-Filename: static/components-bulma/grid/luxon.js
+Filename: static/components-bulma/grid/grid.js
 Comment: 
 
-Filename: static/components-bulma/grid/grid.css
+Filename: static/components-bulma/grid/grid.html
 Comment: 
 
-Filename: static/components-bulma/vueform/vueform.css
+Filename: static/components-bulma/vueform/vueform.js
 Comment: 
 
-Filename: static/components-bulma/vueform/luxon.js
+Filename: static/components-bulma/vueform/vueform.css
 Comment: 
 
 Filename: static/components-bulma/vueform/luxon.min.js
 Comment: 
 
-Filename: static/components-bulma/vueform/vueform.html
+Filename: static/components-bulma/vueform/luxon.js
 Comment: 
 
-Filename: static/components-bulma/vueform/vueform.js
+Filename: static/components-bulma/vueform/vueform.html
 Comment: 
 
-Filename: static/components-bulma/fileupload/fileupload.html
+Filename: static/components-bulma/starrater/starrater.css
 Comment: 
 
-Filename: static/components-bulma/fileupload/fileupload.js
+Filename: static/components-bulma/starrater/starrater.html
 Comment: 
 
-Filename: static/components-bulma/fileupload/fileupload.css
+Filename: static/components-bulma/starrater/starrater.js
 Comment: 
 
-Filename: static/components-bulma/mtable.js
+Filename: static/components-bulma/mtable.html
 Comment: 
 
-Filename: static/components-bulma/starrater/starrater.html
+Filename: static/components-bulma/fileupload/fileupload.html
 Comment: 
 
-Filename: static/components-bulma/starrater/starrater.js
+Filename: static/components-bulma/fileupload/fileupload.css
 Comment: 
 
-Filename: static/components-bulma/starrater/starrater.css
+Filename: static/components-bulma/fileupload/fileupload.js
 Comment: 
 
-Filename: static/components-bulma/mtable.html
+Filename: static/hello.txt
 Comment: 
 
-Filename: static/data/uscities.json
+Filename: static/ws/README.md
 Comment: 
 
-Filename: static/data/zip_codes.json
+Filename: static/socketio/README.md
 Comment: 
 
-Filename: __init__.py
+Filename: translations/it.json
 Comment: 
 
-Filename: uploads/README.md
+Filename: translations/en.json
 Comment: 
 
-Filename: templates/index.html
+Filename: __init__.py
 Comment: 
 
-Filename: templates/ws/ws_index.html
+Filename: vue_components_examples/components/vueform.py
 Comment: 
 
-Filename: templates/examples/session_counter.html
+Filename: vue_components_examples/components/starrater.py
 Comment: 
 
-Filename: templates/examples/flash_example.html
+Filename: vue_components_examples/components/fileupload.py
 Comment: 
 
-Filename: templates/examples/tagsinput_form.html
+Filename: vue_components_examples/components/grid.py
 Comment: 
 
-Filename: templates/examples/flash_example_next.html
+Filename: vue_components_examples/components/README.md
 Comment: 
 
-Filename: templates/examples/forms.html
+Filename: vue_components_examples/models.py
 Comment: 
 
-Filename: templates/examples/auth_form.html
+Filename: vue_components_examples/vue_star_rater.py
 Comment: 
 
-Filename: templates/examples/custom_form.html
+Filename: vue_components_examples/vue_insert_form.py
 Comment: 
 
-Filename: templates/examples/form.html
+Filename: vue_components_examples/vue_view_form.py
 Comment: 
 
-Filename: templates/examples/component_loader.html
+Filename: vue_components_examples/vue_file_uploader.py
 Comment: 
 
-Filename: templates/examples/auth_forms.html
+Filename: vue_components_examples/vue_grid_and_forms.py
 Comment: 
 
-Filename: templates/examples/html_grid.html
+Filename: vue_components_examples/settings.py
 Comment: 
 
-Filename: templates/examples/generic.html
+Filename: vue_components_examples/vue_grid.py
 Comment: 
 
-Filename: templates/examples/page_with_template.html
+Filename: vue_components_examples/common.py
 Comment: 
 
-Filename: templates/examples/auth_custom_login.html
+Filename: vue_components_examples/vue_edit_form.py
 Comment: 
 
-Filename: templates/examples/rest_info.html
+Filename: uploads/README.md
 Comment: 
 
-Filename: templates/examples/hcaptcha_form.html
+Filename: templates/show.html
 Comment: 
 
-Filename: templates/examples/ajax_grid.html
+Filename: templates/auth.html
 Comment: 
 
-Filename: templates/socketio/socketio_index.html
+Filename: templates/examples/component_loader.html
 Comment: 
 
-Filename: templates/vue/star_rater_vue.html
+Filename: templates/examples/page_with_template.html
 Comment: 
 
-Filename: templates/vue/starrating.html
+Filename: templates/examples/custom_form.html
 Comment: 
 
-Filename: templates/vue/edit_form.html
+Filename: templates/examples/html_grid.html
 Comment: 
 
-Filename: templates/vue/file_uploader.html
+Filename: templates/examples/flash_example.html
 Comment: 
 
-Filename: templates/vue/star_rater_vue_bulma.html
+Filename: templates/examples/rest_info.html
 Comment: 
 
-Filename: templates/vue/insert_form.html
+Filename: templates/examples/auth_custom_login.html
 Comment: 
 
-Filename: templates/vue/vue_grid_and_forms.html
+Filename: templates/examples/forms.html
 Comment: 
 
-Filename: templates/vue/vuegrid_bulma.html
+Filename: templates/examples/ajax_grid.html
 Comment: 
 
-Filename: templates/vue/view_form.html
+Filename: templates/examples/tagsinput_form.html
 Comment: 
 
-Filename: templates/vue/vuegrid.html
+Filename: templates/examples/flash_example_next.html
 Comment: 
 
-Filename: templates/layout.html
+Filename: templates/examples/hcaptcha_form.html
 Comment: 
 
-Filename: templates/auth.html
+Filename: templates/examples/auth_form.html
 Comment: 
 
-Filename: templates/layout_bulma.html
+Filename: templates/examples/form.html
 Comment: 
 
-Filename: templates/show.html
+Filename: templates/examples/session_counter.html
 Comment: 
 
-Filename: translations/it.json
+Filename: templates/examples/auth_forms.html
 Comment: 
 
-Filename: translations/en.json
+Filename: templates/examples/generic.html
 Comment: 
 
-Filename: vue_components_examples/vue_grid_and_forms.py
+Filename: templates/layout_bulma.html
 Comment: 
 
-Filename: vue_components_examples/components/fileupload.py
+Filename: templates/ws/ws_index.html
 Comment: 
 
-Filename: vue_components_examples/components/vueform.py
+Filename: templates/vue/star_rater_vue.html
 Comment: 
 
-Filename: vue_components_examples/components/grid.py
+Filename: templates/vue/insert_form.html
 Comment: 
 
-Filename: vue_components_examples/components/README.md
+Filename: templates/vue/vuegrid.html
 Comment: 
 
-Filename: vue_components_examples/components/starrater.py
+Filename: templates/vue/star_rater_vue_bulma.html
 Comment: 
 
-Filename: vue_components_examples/vue_file_uploader.py
+Filename: templates/vue/vuegrid_bulma.html
 Comment: 
 
-Filename: vue_components_examples/vue_star_rater.py
+Filename: templates/vue/edit_form.html
 Comment: 
 
-Filename: vue_components_examples/common.py
+Filename: templates/vue/vue_grid_and_forms.html
 Comment: 
 
-Filename: vue_components_examples/vue_edit_form.py
+Filename: templates/vue/file_uploader.html
 Comment: 
 
-Filename: vue_components_examples/vue_insert_form.py
+Filename: templates/vue/view_form.html
 Comment: 
 
-Filename: vue_components_examples/vue_view_form.py
+Filename: templates/vue/starrating.html
 Comment: 
 
-Filename: vue_components_examples/settings.py
+Filename: templates/index.html
 Comment: 
 
-Filename: vue_components_examples/models.py
+Filename: templates/socketio/socketio_index.html
 Comment: 
 
-Filename: vue_components_examples/vue_grid.py
+Filename: templates/layout.html
 Comment: 
 
 Zip file comment:
```

#### templates/examples/custom_form.html

```diff
@@ -16,17 +16,14 @@
     <div class="column">
       <div class="buttons is-centered">
         [[ form.custom.submit['_class'] = 'button is-info is-large' ]]
         [[= form.custom.submit ]]
       </div>
     </div>
   </div>
-  [[ for hidden_widget in form.custom.hidden_widgets: ]]
-  [[= form.custom.hidden_widgets[hidden_widget] ]]
-  [[ pass ]]
 [[= form.custom.end ]]
 
 
 <h2 class="title">Rows</h2>
 
 <ul>
   [[for row in rows:]]
```

### Comparing `py4web-1.20230314.1/py4web/core.py` & `py4web-1.20230410.1/py4web/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -784,15 +784,16 @@
                     sys.modules[app_module], "__static_version__", None
                 )
             except KeyError:
                 static_version = None
         if static_version:
             broken_parts.insert(1, "_" + static_version)
 
-    url = prefix + "/".join(map(urllib.parse.quote, broken_parts))
+    url_prefix = os.environ.get("PY4WEB_URL_PREFIX", "")
+    url = url_prefix + prefix + "/".join(map(urllib.parse.quote, broken_parts))
     # Signs the URL if required.  Copy vars into urlvars not to modify it.
     urlvars = dict(vars) if vars else {}
     if signer:
         # Note that we need to sign the non-urlencoded URL, since
         # at verification time, it will be already URLdecoded.
         signer.sign(prefix + "/".join(broken_parts), urlvars)
     if urlvars:
@@ -1352,16 +1353,17 @@
 
             Reloader.register_route(app_name, path, {"method": "GET"}, server_static)
 
         ICECUBE.update(threadsafevariable.ThreadSafeVariable.freeze())
 
     @staticmethod
     def register_route(app_name, rule, kwargs, func):
+        url_prefix = os.environ.get("PY4WEB_URL_PREFIX", "")
         dec_func = action.catch_errors(app_name, func)
-        bottle.route(rule, **kwargs)(dec_func)
+        bottle.route(url_prefix + rule, **kwargs)(dec_func)
         filename = module2filename(func.__module__)
         methods = kwargs.get("method", ["GET"])
         if isinstance(methods, str):
             methods = [methods]
         for method in methods:
             Reloader.ROUTES[app_name].append(
                 {
@@ -1959,14 +1961,21 @@
     "-D",
     "--debug",
     is_flag=True,
     default=False,
     help="Debug switch",
     show_default=True,
 )
+@click.option(
+    "-U",
+    "--url_prefix",
+    default="",
+    help="Prefix to add to all URLs in and out",
+    show_default=True,
+)
 def run(**kwargs):
     """Run all the applications on apps_folder"""
     install_args(kwargs)
 
     from py4web import __version__
 
     click.secho(ART, fg="blue")
```

### Comparing `py4web-1.20230314.1/py4web/server_adapters.py` & `py4web-1.20230410.1/py4web/server_adapters.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/auth.py` & `py4web-1.20230410.1/py4web/utils/auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,16 +166,14 @@
             "register": "Register",
             "request": "Request",
             "sign-in": "Sign In",
             "sign-up": "Sign Up",
             "submit": "Submit",
         },
         "errors": {
-            "invalid_username": "Invalid username",
-            "invalid_email": "Invalid email",
             "registration_is_pending": "Registration is pending",
             "account_is_blocked": "Account is blocked",
             "account_needs_to_be_approved": "Account needs to be approved",
             "invalid_credentials": "Invalid Credentials",
             "invalid_token": "invalid token",
             "password_doesnt_match": "Password doesn't match",
             "invalid_current_password": "invalid current password",
@@ -205,14 +203,15 @@
         sender=None,
         use_username=True,
         use_phone_number=False,
         registration_requires_confirmation=True,
         registration_requires_approval=False,
         inject=True,
         extra_fields=None,
+        extra_form_fields=None,
         login_expiration_time=3600,  # seconds
         password_complexity="default",
         block_previous_password_num=None,
         allowed_actions=None,
         use_appname_in_redirects=None,
         password_in_db=True,
         two_factor_required=None,
@@ -260,14 +259,15 @@
         self.sender = sender
         self.route = "auth"
         self.use_username = use_username  # if False, uses email only
         self.password_in_db = password_in_db  # if False, password is never saved in db
         self.use_phone_number = use_phone_number
         # The self._link variable is not thread safe (only intended for testing)
         self.extra_auth_user_fields = extra_fields or []
+        self.extra_form_fields = extra_form_fields or {}
         self._link = None
         if db and define_tables:
             self.define_tables()
         self.plugins = {}
         self.form_source = DefaultAuthForms(self)
         self.fix_actions()
 
@@ -559,77 +559,76 @@
         in the Login form"""
         db = self.db
 
         # Default email and password in case they are None or an error will occur.
         email = "" if email is None else email
         password = "" if password is None else password
 
-        if "email_auth" in self.plugins:
-            email = email.lower()
-            if self.plugins["email_auth"].validate_credentials(email, password):
-                user = db(db.auth_user.email == email).select().first()
-                return (user, None)
-            else:
-                return None, self.param.messages["errors"].get("invalid_credentials")
-        else:
+        user = None
+        error = None
+        prevent_db_lookup = False
+        # first check if we have a plugin that can check credentials
+
+        for plugin in self.plugins.values():
+            if not hasattr(plugin, "get_login_url"):
+                prevent_db_lookup = True
+                if plugin.check_credentials(email, password):
+                    # if the creadentials are independently validated
+                    # get of create the user (if does not exist)
+                    user_info = {}
+                    user_info["sso_id"] = plugin.name + ":" + email
+                    if self.use_username or not "@" in email:
+                        user_info["username"] = email
+                    if "@" in email:
+                        user_info["email"] = email
+                    else:
+                        user_info["email"] = email + "@example.com"
+                    user = self.get_or_register_user(user_info)
+                    break
+
+        # else check against database
+        if not prevent_db_lookup:
             value = email.lower()
-            if self.use_username:
-                query = (
-                    (db.auth_user.email == value)
-                    if "@" in value
-                    else (db.auth_user.username == value)
-                )
-            else:
-                query = db.auth_user.email == value
-            user = db(query).select().first()
-            if not user:
-                if self.use_username:
-                    return (None, self.param.messages["errors"].get("invalid_username"))
-                else:
-                    return (None, self.param.messages["errors"].get("invalid_email"))
-            if (user.action_token or "").startswith("pending-registration:"):
-                return (
-                    None,
-                    self.param.messages["errors"].get("registration_is_pending"),
-                )
-            if user.action_token == "account-blocked":
-                return (None, self.param.messages["errors"].get("account_is_blocked"))
-            if user.action_token == "pending-approval":
-                return (
-                    None,
-                    self.param.messages["errors"].get("account_needs_to_be_approved"),
-                )
-            if "pam" in self.plugins or "ldap" in self.plugins:
-                plugin_name = "pam" if "pam" in self.plugins else "ldap"
-                check = self.plugins[plugin_name].check_credentials(
-                    user.username, password
-                )
-                if check:
-                    return (user, None)
-            else:
-                if CRYPT()(password)[0] == user.password:
-                    return (user, None)
-            return None, self.param.messages["errors"].get("invalid_credentials")
+            field = (
+                db.auth_user.email
+                if "@" in value or not self.use_username
+                else db.auth_user.username
+            )
+            user = db(field == value).select().first()
+            if user and not (CRYPT()(password)[0] == user.password):
+                user = None
+
+        # then check for possible login blockers
+        if not user:
+            error = "invalid_credentials"
+        elif (user["action_token"] or "").startswith("pending-registration:"):
+            error = "registration_is_pending"
+        elif user["action_token"] == "account-blocked":
+            error = "account_is_blocked"
+        elif user["action_token"] == "pending-approval":
+            error = "account_needs_to_be_approved"
+
+        # return the error or the user
+        if error:
+            return (None, self.param.messages["errors"].get(error, error))
+        return (user, None)
 
     def request_reset_password(self, email, send=True, next="", route=None):
         """Send a mail with token for changing user's password after the user's parameters are entered
         in the request_reset_password form
         """
 
         db = self.db
         value = email.lower()
-        if self.use_username:
-            query = (
-                (db.auth_user.email == value)
-                if "@" in value
-                else (db.auth_user.username == value)
-            )
-        else:
-            query = db.auth_user.email == value
-        user = db(query).select().first()
+        field = (
+            db.auth_user.email
+            if "@" in value or not self.use_username
+            else self.auth_user.username
+        )
+        user = db(field == value).select().first()
         if user and user.action_token != "account-blocked":
             token = str(uuid.uuid4())
             if next:
                 token += "/" + b16e(next)
             user.update_record(action_token="reset-password-request:" + token)
             if send:
                 self._link = link = URL(
@@ -817,15 +816,15 @@
                 return None
             # we can update all the other information provided by the SSO
             if any(user[key] != row[key] for key in user if not key == "username"):
                 row.update_record(**user)
             user["id"] = row["id"]
         # if we do not have a candidate user we need to create one
         else:
-            # we expect an email to unable to create account
+            # we expect an email to be able to create account
             if not "email" in user:
                 return None
             # if we expect a username but not provided, user email as username
             if self.use_username and "username" not in user:
                 user["username"] = user["email"]
             # create the user
             user["id"] = db.auth_user.insert(**db.auth_user._filter_fields(user))
@@ -1413,30 +1412,34 @@
 
         # if the form is submitted, before any validation
         # delete any unverified account with the same email
         if request.method == "POST":
             email = request.forms.get("email")
             if email:
                 self.auth.get_or_delete_existing_unverified_account(email)
+        extra_form_fields = self.auth.extra_form_fields.get("register", [])
+        fields += extra_form_fields
         form = Form(fields, submit_value=button_name, formstyle=self.formstyle)
         user = None
         if form.accepted:
             # notice that here the form is alrealdy validated
             if not self.auth.password_in_db:  # password must not be written in db
                 # Prioritize PAM or LDAP logins if enabled
                 if "pam" in self.auth.plugins or "ldap" in self.auth.plugins:
                     plugin_name = "pam" if "pam" in self.auth.plugins else "ldap"
                     check = self.auth.plugins[plugin_name].check_credentials(
                         form.vars["username"], form.vars["password"]
                     )
                     form.vars["password"] = ""
                     if not check:
-                        self._set_flash("Invalid username or password")
+                        self._set_flash("Invalid credentials")
                         redirect("register")
-            res = self.auth.register(form.vars, validate=False)
+            extra_names = set(field.name for field in extra_form_fields)
+            vars = {k: v for k, v in form.vars.items() if k not in extra_names}
+            res = self.auth.register(vars, validate=False)
             form.errors.update(**res.get("errors", {}))
             form.accepted = not form.errors
         if form.accepted:
             self._set_flash("user-registered")
             self._postprocessing("register", form, user)
             if self.auth.param.login_after_registration:
                 redirect("login")
@@ -1461,26 +1464,27 @@
         return form
 
     def login_buttons(self):
         """Define auth plugin type button to be displayed in login form"""
         top_buttons = []
 
         for name, plugin in self.auth.plugins.items():
+            #  do not add a button for plugin that do not delegate to url
+            if not hasattr(plugin, "get_login_url"):
+                continue
+
             url = f"/auth/plugin/{name}/login"
 
             next_url = prevent_open_redirect(request.query.get("next"))
             if next_url:
                 url = f"{url}?next={next_url}"
 
-            if (
-                name != "email_auth"
-            ):  #  do not add the top button for the email auth plugin
-                top_buttons.append(
-                    dict(label=f"{plugin.label} Login", action=name, href=url)
-                )
+            top_buttons.append(
+                dict(label=f"{plugin.label} Login", action=name, href=url)
+            )
 
         combined_div = DIV(
             *[
                 A(item["label"], _href=f"..{item['href']}", _role="button")
                 for item in top_buttons
             ]
         )
@@ -1540,28 +1544,30 @@
                 hidden=False,
                 fields=fields,
                 href="/auth/api/login",
                 submit_label=button_name,
                 additional_buttons=additional_buttons,
             )
 
+        extra_form_fields = self.auth.extra_form_fields.get("login", [])
+        fields += extra_form_fields
         form = Form(
             fields,
             submit_value=button_name,
             formstyle=self.formstyle,
         )
         user = None
         next_url = prevent_open_redirect(request.query.get("next"))
         self.auth.session["_next_login"] = next_url
         if form.submitted:
             user, error = self.auth.login(
                 form.vars.get("email", ""), form.vars.get("password", "")
             )
             form.accepted = not error
-            form.errors["email"] = error
+            form.errors["password"] = error
         if user:
             #  We will process two_factor if two_factor_send is defined and either
             #  - No two_factor_required defined
             #    OR
             #  - two_factor_required() returns True
             #  If two_factor_required exists and returns False,
             #  then this user bypasses two_factor processing
@@ -1699,14 +1705,19 @@
                 hidden=False,
                 fields=fields,
                 href="/auth/api/request_reset_password",
                 submit_label=button_name,
                 additional_buttons=additional_buttons,
             )
 
+        extra_form_fields = self.auth.extra_form_fields.get(
+            "request_reset_password", []
+        )
+        fields += extra_form_fields
+
         form = Form(
             fields,
             submit_value=button_name,
             formstyle=self.formstyle,
         )
         if form.accepted:
             email = form.vars.get("email", "")
```

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/__init__.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,30 @@
-import calendar
-import json
 import random
 import string
-import time
 import urllib
-import uuid
 
 import jwt
 import requests
 
 from py4web.core import HTTP, URL, redirect, request
 
 
+class UsernamePassword:
+
+    name = "undefined"
+
+    def __init__(self, test_mode=False):
+        self.test_mode = test_mode
+
+    def check_credentials(self, username, password):
+        if self.test_mode:
+            return password == "password"
+        raise NotImplementedError
+
+
 class SSO(object):
 
     name = "undefined"
     maps = {}
 
     ### methods that must be overwritten
 
@@ -182,10 +191,9 @@
             # fallback to old approach if "id_token" is not in the response
             token = output.get("access_token")
             headers = {"Authorization": "Bearer %s" % token}
             res = requests.get(self.userinfo_url, headers=headers)
             data = res.json()
         return data
 
-
     def revoke(self, token):
         requests.post(self.revoke_url, data=dict(token=token))
```

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/basic_auth_plugin.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/basic_auth_plugin.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
     name = "basic"
     label = "Basic"
 
     def __init__(self, server="127.0.0.1", table=None):
         self.server = server
 
-    def validate_credentials(self, username, password):
+    def check_credentials(self, username, password):
 
         """
         to use basic login with a different server
         from gluon.contrib.login_methods.basic_auth import basic_auth
         auth.settings.login_methods.append(basic_auth('http://server'))
         """
         key = base64.b64encode(username + ":" + password)
```

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/cas_plugin.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/cas_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/email_auth_plugin.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/email_auth_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     label = "Email"
 
     def __init__(self, server="smtp.gmail.com:587", domain="@gmail.com", tls_mode=None):
         self.server = server
         self.domain = domain
         self.tls_mode = tls_mode
 
-    def validate_credentials(self, username, password):
+    def check_credentials(self, username, password):
         email = username
         server = self.server
         domain = self.domain
         tls_mode = self.tls_mode
         if domain:
             if not isinstance(domain, (list, tuple)):
                 domain = [str(domain)]
```

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/ldap_plugin.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/ldap_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,21 @@
 #
 
 import logging
 import sys
 
 import ldap  # python-ldap
 import ldap.filter
-from pydal.tools.tags import Tags
+
+from . import UsernamePassword
 
 ldap.set_option(ldap.OPT_REFERRALS, 0)
 
 
-class LDAPPlugin(object):
+class LDAPPlugin(UsernamePassword):
 
     name = "ldap"
     label = "LDAP"
 
     """
     to use ldap login with MS Active Directory:
 
@@ -887,7 +888,10 @@
 
         logger.debug("User groups: %s" % ldap_groups_of_the_user)
         return list(ldap_groups_of_the_user)
 
         if filterstr[0] == "(" and filterstr[-1] == ")":  # rfc4515 syntax
             filterstr = filterstr[1:-1]  # parens added again where used
         return []
+
+    def check_credentials(self, username, password):
+        return self.is_user_in_allowed_groups(username, password)
```

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/newsamlplugin.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/newsamlplugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/oauth2discord.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/oauth2discord.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/oauth2facebook.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/oauth2facebook.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/oauth2github.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/oauth2github.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # from https://requests-oauthlib.readthedocs.io/en/latest/examples/github.html
 import requests
+
 from py4web import URL
+
 from . import OAuth2
 
 
 class OAuth2Github(OAuth2):
     name = "oauth2github"
     label = "Github"
```

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/oauth2google.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/oauth2google.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/oauth2server.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/oauth2server.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/oauth2wpminiorange.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/oauth2wpminiorange.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/pam.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/pam.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/saml2_plugin.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/saml2_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/auth_plugins/x509_auth_plugin.py` & `py4web-1.20230410.1/py4web/utils/auth_plugins/x509_auth_plugin.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/cors.py` & `py4web-1.20230410.1/py4web/utils/cors.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/dbstore.py` & `py4web-1.20230410.1/py4web/utils/dbstore.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/downloader.py` & `py4web-1.20230410.1/py4web/utils/downloader.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/factories.py` & `py4web-1.20230410.1/py4web/utils/factories.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/form.py` & `py4web-1.20230410.1/py4web/utils/form.py`

 * *Files 1% similar despite different names*

```diff
@@ -830,21 +830,18 @@
                             elif field.type == "boolean":
                                 validated_vars[field.name] = value is not None
                             else:
                                 validated_vars[field.name] = value
                             if error:
                                 self.errors[field.name] = error
                     if self.errors:
-                        print("have errors")
                         for field_name in uploaded_fields:
-                            print(field_name)
                             validated_vars[field_name] = (
                                 self.record and self.record.get(field_name) or None
                             )
-                            print(validated_vars[field_name])
                     self.vars.update(validated_vars)
                     if validation:
                         validation(self)
                     if self.record and dbio:
                         self.vars["id"] = self.record.id
                     if not self.errors:
                         for file in uploaded_files:
```

### Comparing `py4web-1.20230314.1/py4web/utils/grid.py` & `py4web-1.20230410.1/py4web/utils/grid.py`

 * *Files 8% similar despite different names*

```diff
@@ -271,14 +271,116 @@
         "grid-search-form-select": "",
         "grid-search-boolean": "padding-top: .5rem;",
         "grid-header-element": "",
         "grid-footer-element": "",
     }
 
 
+class GridClassStyleBootstrap5(GridClassStyle):
+    """The Grid style for Bootstrap 5"""
+
+    classes = {
+        "grid-wrapper": "grid-wrapper",
+        "grid-header": "grid-header clearfix pb-2",
+        "grid-new-button": "grid-new-button btn btn-outline-primary",
+        "grid-search": "grid-search float-end pb-2",
+        "grid-table-wrapper": "grid-table-wrapper table-responsive",
+        "grid-table": "grid-table table table-striped table-hover table-bordered clearfix",
+        "grid-sorter-icon-up": "grid-sort-icon-up fas fa-sort-up float-end",
+        "grid-sorter-icon-down": "grid-sort-icon-down fas fa-sort-down float-end",
+        "grid-thead": "",
+        "grid-tr": "",
+        "grid-th": "small",
+        "grid-td": "small",
+        "grid-td-buttons": "",
+        "grid-button": "grid-button btn btn-sm btn-outline-secondary",
+        "grid-details-button": "grid-details-button btn btn-sm btn-outline-secondary",
+        "grid-edit-button": "grid-edit-button btn btn-sm btn-outline-secondary",
+        "grid-delete-button": "grid-delete-button btn btn-sm btn-outline-secondary",
+        "grid-search-button": "grid-search-button btn btn-outline-info",
+        "grid-clear-button": "grid-clear-button btn btn-outline-info",
+        "grid-footer": "grid-footer pb-8",
+        "grid-info": "grid-info float-start",
+        "grid-pagination": "grid-pagination float-end",
+        "grid-pagination-button": "grid-pagination-button btn btn-sm btn-outline-primary",
+        "grid-pagination-button-current": "grid-pagination-button-current btn btn-primary btn-sm",
+        "grid-cell-type-string": "grid-cell-type-string",
+        "grid-cell-type-text": "grid-cell-type-text",
+        "grid-cell-type-boolean": "grid-cell-type-boolean text-center",
+        "grid-cell-type-float": "grid-cell-type-float",
+        "grid-cell-type-decimal": "grid-cell-type-decimal",
+        "grid-cell-type-int": "grid-cell-type-int",
+        "grid-cell-type-date": "grid-cell-type-date",
+        "grid-cell-type-time": "grid-cell-type-time",
+        "grid-cell-type-datetime": "grid-cell-type-datetime",
+        "grid-cell-type-upload": "grid-cell-type-upload",
+        "grid-cell-type-list": "grid-cell-type-list",
+        "grid-cell-type-id": "grid-cell-type-id text-center",
+        # specific for custom form
+        "grid-search-form": "grid-search-form float-end pb-2",
+        "grid-search-form-table": "grid-search-form-table",
+        "grid-search-form-tr": "grid-search-form-tr",
+        "grid-search-form-td": "grid-search-form-td pr-1",
+        "grid-search-form-input": "grid-search-form-input form-control",
+        "grid-search-form-select": "grid-search-form-input control select",
+        "grid-search-boolean": "grid-search-boolean",
+        "grid-header-element": "grid-header-element btn btn-sm",
+        "grid-footer-element": "grid-footer-element btn btn-sm",
+    }
+
+    styles = {
+        "grid-wrapper": "",
+        "grid-header": "",
+        "grid-new-button": "",
+        "grid-search": "",
+        "grid-table-wrapper": "",
+        "grid-table": "",
+        "grid-sorter-icon-up": "",
+        "grid-sorter-icon-down": "",
+        "grid-thead": "",
+        "grid-tr": "",
+        "grid-th": "text-align: center; text-transform: uppercase; vertical-align: bottom; text-decoration: none;",
+        "grid-td": "",
+        "grid-td-buttons": "white-space: nowrap; width: 1%;",
+        "grid-button": "",
+        "grid-details-button": "border-radius: 0 !important;",
+        "grid-edit-button": "border-radius: 0 !important;",
+        "grid-delete-button": "border-radius: 0 !important;",
+        "grid-search-button": "border-radius: 0 !important;",
+        "grid-clear-button": "border-radius: 0 !important;",
+        "grid-footer": "padding-top: .5em; padding-bottom: 2em;",
+        "grid-info": "",
+        "grid-pagination": "",
+        "grid-pagination-button": "margin-left: .25em; border-radius: 0 !important;",
+        "grid-pagination-button-current": "margin-left: .25em; border-radius: 0 !important;",
+        "grid-cell-type-string": "vertical-align: top; text-overflow: ellipsis;",
+        "grid-cell-type-text": "vertical-align: top; text-overflow: ellipsis;",
+        "grid-cell-type-boolean": "vertical-align: top; text-align: center",
+        "grid-cell-type-float": "vertical-align: top; text-align: right",
+        "grid-cell-type-decimal": "vertical-align: top; text-align: right",
+        "grid-cell-type-int": "vertical-align: top; text-align: center;",
+        "grid-cell-type-date": "vertical-align: top; text-align: center;",
+        "grid-cell-type-time": "vertical-align: top; text-align: center;",
+        "grid-cell-type-datetime": "vertical-align: top; text-align: center;",
+        "grid-cell-type-upload": "vertical-align: top; text-align: center;",
+        "grid-cell-type-list": "vertical-align: top; text-align: left;",
+        "grid-cell-type-id": "",
+        # specific for custom form
+        "grid-search-form": "",
+        "grid-search-form-table": "",
+        "grid-search-form-tr": "",
+        "grid-search-form-td": "",
+        "grid-search-form-input": "",
+        "grid-search-form-select": "",
+        "grid-search-boolean": "padding-top: .5rem;",
+        "grid-header-element": "",
+        "grid-footer-element": "",
+    }
+
+
 class Column:
     """class used to represent a column in a grid"""
 
     def __init__(
         self,
         name,
         represent,
@@ -659,17 +761,17 @@
                     redirect(base64.b16decode(referrer.encode("utf8")).decode("utf8"))
                 else:
                     redirect(self.endpoint)
 
         elif self.action == "delete" and self.is_deletable(record):
             db(db[self.tablename].id == self.record_id).delete()
 
-            rereffer = parse_referer(request)
+            referrer = parse_referer(request)
             url = self.endpoint + "/select"
-            if referred and referrer.query:
+            if referrer and referrer.query:
                 url += "?%s" % referrer.query
             redirect(url)
 
         elif self.action == "select":
             self.referrer = "_referrer=%s" % base64.b16encode(
                 request.url.encode("utf8")
             ).decode("utf8")
```

### Comparing `py4web-1.20230314.1/py4web/utils/jsonrpc.py` & `py4web-1.20230410.1/py4web/utils/jsonrpc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/mailer.py` & `py4web-1.20230410.1/py4web/utils/mailer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/misc.py` & `py4web-1.20230410.1/py4web/utils/misc.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/populate.py` & `py4web-1.20230410.1/py4web/utils/populate.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/publisher.py` & `py4web-1.20230410.1/py4web/utils/publisher.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/scheduler.py` & `py4web-1.20230410.1/py4web/utils/scheduler.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/scheduler_old.py` & `py4web-1.20230410.1/py4web/utils/scheduler_old.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/security.py` & `py4web-1.20230410.1/py4web/utils/security.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web/utils/url_signer.py` & `py4web-1.20230410.1/py4web/utils/url_signer.py`

 * *Files identical despite different names*

### Comparing `py4web-1.20230314.1/py4web.egg-info/PKG-INFO` & `py4web-1.20230410.1/py4web.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: py4web
-Version: 1.20230314.1
+Version: 1.20230410.1
 Summary: Experimental py4web (a better web2py)
 Home-page: https://github.com/web2py/py4web
 Author: Massimo Di Pierro
 Author-email: massimo.dipierro@gmail.com
 Maintainer: Massimo Di Pierro
 Maintainer-email: massimo.dipierro@gmail.com
 License: BSD
```

### Comparing `py4web-1.20230314.1/py4web.egg-info/SOURCES.txt` & `py4web-1.20230410.1/py4web.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 py4web/utils/grid.py
 py4web/utils/jsonrpc.py
 py4web/utils/mailer.py
 py4web/utils/misc.py
 py4web/utils/param.py
 py4web/utils/populate.py
 py4web/utils/publisher.py
+py4web/utils/recaptcha.py
 py4web/utils/scheduler.py
 py4web/utils/scheduler_old.py
 py4web/utils/security.py
 py4web/utils/tags.py
 py4web/utils/url_signer.py
 py4web/utils/auth_plugins/__init__.py
 py4web/utils/auth_plugins/basic_auth_plugin.py
```

### Comparing `py4web-1.20230314.1/setup.py` & `py4web-1.20230410.1/setup.py`

 * *Files identical despite different names*

