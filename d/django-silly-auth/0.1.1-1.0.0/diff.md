# Comparing `tmp/django-silly-auth-0.1.1.tar.gz` & `tmp/django-silly-auth-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-silly-auth-0.1.1.tar", last modified: Mon Apr 10 01:49:29 2023, max compression
+gzip compressed data, was "django-silly-auth-1.0.0.tar", last modified: Mon Apr 10 01:50:56 2023, max compression
```

## Comparing `django-silly-auth-0.1.1.tar` & `django-silly-auth-1.0.0.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:49:29.480914 django-silly-auth-0.1.1/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-0.1.1/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1550 2023-04-10 01:49:29.480914 django-silly-auth-0.1.1/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      940 2023-04-10 01:22:43.000000 django-silly-auth-0.1.1/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:49:29.464914 django-silly-auth-0.1.1/django_silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-04-10 01:45:52.000000 django-silly-auth-0.1.1/django_silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4730 2023-04-10 01:39:52.000000 django-silly-auth-0.1.1/django_silly_auth/config.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5726 2023-04-10 01:39:27.000000 django-silly-auth-0.1.1/django_silly_auth/forms.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2468 2023-04-10 01:38:49.000000 django-silly-auth-0.1.1/django_silly_auth/mixins.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5164 2023-04-10 01:38:31.000000 django-silly-auth-0.1.1/django_silly_auth/serializers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:49:29.468914 django-silly-auth-0.1.1/django_silly_auth/templates/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:44:50.000000 django-silly-auth-0.1.1/django_silly_auth/templates/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:49:29.468914 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:44:57.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/_base.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:49:29.468914 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/_test/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:45:22.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/_test/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4265 2023-04-10 01:17:29.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/_test/_base.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      175 2023-04-04 22:34:28.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/_test/_test.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      274 2023-04-04 20:59:42.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/_test/_users.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:49:29.472914 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:45:14.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      515 2023-04-05 04:15:11.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/account.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      528 2023-04-05 04:15:11.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/change_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      539 2023-04-05 04:15:11.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/change_username.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      328 2023-04-05 04:15:11.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/index.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1045 2023-04-06 16:37:59.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/login.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-05 04:15:11.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      527 2023-04-06 16:37:59.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      800 2023-04-06 16:37:59.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/reset_password.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1094 2023-04-06 17:29:58.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/signup.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:49:29.476914 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/emails/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:45:06.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/emails/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      238 2023-04-10 01:22:43.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      238 2023-03-31 12:20:50.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:49:29.476914 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/silly/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:46:56.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/silly/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      462 2023-04-10 01:22:43.000000 django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4424 2023-04-10 01:37:32.000000 django-silly-auth-0.1.1/django_silly_auth/urls.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3696 2023-04-10 01:37:25.000000 django-silly-auth-0.1.1/django_silly_auth/utils.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:49:29.476914 django-silly-auth-0.1.1/django_silly_auth/views/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:44:30.000000 django-silly-auth-0.1.1/django_silly_auth/views/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2978 2023-04-10 01:44:09.000000 django-silly-auth-0.1.1/django_silly_auth/views/api_custom_login.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      325 2023-04-10 01:42:31.000000 django-silly-auth-0.1.1/django_silly_auth/views/api_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5123 2023-04-10 01:43:11.000000 django-silly-auth-0.1.1/django_silly_auth/views/api_views_if_drf.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    13103 2023-04-10 01:42:03.000000 django-silly-auth-0.1.1/django_silly_auth/views/classics.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1756 2023-04-10 01:41:23.000000 django-silly-auth-0.1.1/django_silly_auth/views/silly_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-10 01:40:40.000000 django-silly-auth-0.1.1/django_silly_auth/views/test_views.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:49:29.468914 django-silly-auth-0.1.1/django_silly_auth.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1550 2023-04-10 01:49:29.000000 django-silly-auth-0.1.1/django_silly_auth.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2058 2023-04-10 01:49:29.000000 django-silly-auth-0.1.1/django_silly_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-10 01:49:29.000000 django-silly-auth-0.1.1/django_silly_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-04-10 01:49:29.000000 django-silly-auth-0.1.1/django_silly_auth.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-04-10 01:49:29.000000 django-silly-auth-0.1.1/django_silly_auth.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-10 01:49:29.480914 django-silly-auth-0.1.1/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1952 2023-04-10 01:47:20.000000 django-silly-auth-0.1.1/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.348334 django-silly-auth-1.0.0/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.0.0/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1550 2023-04-10 01:50:56.348334 django-silly-auth-1.0.0/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      940 2023-04-10 01:22:43.000000 django-silly-auth-1.0.0/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.328333 django-silly-auth-1.0.0/django_silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-04-10 01:50:14.000000 django-silly-auth-1.0.0/django_silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4730 2023-04-10 01:39:52.000000 django-silly-auth-1.0.0/django_silly_auth/config.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5726 2023-04-10 01:39:27.000000 django-silly-auth-1.0.0/django_silly_auth/forms.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2468 2023-04-10 01:38:49.000000 django-silly-auth-1.0.0/django_silly_auth/mixins.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5164 2023-04-10 01:38:31.000000 django-silly-auth-1.0.0/django_silly_auth/serializers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.336334 django-silly-auth-1.0.0/django_silly_auth/templates/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:44:50.000000 django-silly-auth-1.0.0/django_silly_auth/templates/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.336334 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:44:57.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_base.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.340334 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_test/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:45:22.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_test/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4265 2023-04-10 01:17:29.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_test/_base.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      175 2023-04-04 22:34:28.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_test/_test.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      274 2023-04-04 20:59:42.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_test/_users.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.344334 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:45:14.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      515 2023-04-05 04:15:11.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/account.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      528 2023-04-05 04:15:11.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/change_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      539 2023-04-05 04:15:11.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/change_username.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      328 2023-04-05 04:15:11.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/index.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1045 2023-04-06 16:37:59.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/login.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-05 04:15:11.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      527 2023-04-06 16:37:59.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      800 2023-04-06 16:37:59.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/reset_password.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1094 2023-04-06 17:29:58.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/signup.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.344334 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/emails/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:45:06.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/emails/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      238 2023-04-10 01:22:43.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      238 2023-03-31 12:20:50.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.344334 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/silly/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:46:56.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/silly/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      462 2023-04-10 01:22:43.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4424 2023-04-10 01:37:32.000000 django-silly-auth-1.0.0/django_silly_auth/urls.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3696 2023-04-10 01:37:25.000000 django-silly-auth-1.0.0/django_silly_auth/utils.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.348334 django-silly-auth-1.0.0/django_silly_auth/views/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:44:30.000000 django-silly-auth-1.0.0/django_silly_auth/views/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2978 2023-04-10 01:44:09.000000 django-silly-auth-1.0.0/django_silly_auth/views/api_custom_login.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      325 2023-04-10 01:42:31.000000 django-silly-auth-1.0.0/django_silly_auth/views/api_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5123 2023-04-10 01:43:11.000000 django-silly-auth-1.0.0/django_silly_auth/views/api_views_if_drf.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    13103 2023-04-10 01:42:03.000000 django-silly-auth-1.0.0/django_silly_auth/views/classics.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1756 2023-04-10 01:41:23.000000 django-silly-auth-1.0.0/django_silly_auth/views/silly_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-10 01:40:40.000000 django-silly-auth-1.0.0/django_silly_auth/views/test_views.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.336334 django-silly-auth-1.0.0/django_silly_auth.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1550 2023-04-10 01:50:56.000000 django-silly-auth-1.0.0/django_silly_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2058 2023-04-10 01:50:56.000000 django-silly-auth-1.0.0/django_silly_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-10 01:50:56.000000 django-silly-auth-1.0.0/django_silly_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-04-10 01:50:56.000000 django-silly-auth-1.0.0/django_silly_auth.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-04-10 01:50:56.000000 django-silly-auth-1.0.0/django_silly_auth.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-10 01:50:56.348334 django-silly-auth-1.0.0/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1952 2023-04-10 01:47:20.000000 django-silly-auth-1.0.0/setup.py
```

### Comparing `django-silly-auth-0.1.1/LICENSE.md` & `django-silly-auth-1.0.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/PKG-INFO` & `django-silly-auth-1.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 0.1.1
+Version: 1.0.0
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
```

### Comparing `django-silly-auth-0.1.1/README.md` & `django-silly-auth-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/config.py` & `django-silly-auth-1.0.0/django_silly_auth/config.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/forms.py` & `django-silly-auth-1.0.0/django_silly_auth/forms.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/mixins.py` & `django-silly-auth-1.0.0/django_silly_auth/mixins.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/serializers.py` & `django-silly-auth-1.0.0/django_silly_auth/serializers.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/_base.html` & `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_base.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/_test/_base.html` & `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_test/_base.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/account.html` & `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/account.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/change_email.html` & `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/change_email.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/change_username.html` & `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/change_username.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/login.html` & `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/login.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/request_password_reset.html` & `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/request_password_reset.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html` & `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/reset_password.html` & `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/reset_password.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/templates/silly_auth/classic/signup.html` & `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/signup.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/urls.py` & `django-silly-auth-1.0.0/django_silly_auth/urls.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/utils.py` & `django-silly-auth-1.0.0/django_silly_auth/utils.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/views/api_custom_login.py` & `django-silly-auth-1.0.0/django_silly_auth/views/api_custom_login.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/views/api_views_if_drf.py` & `django-silly-auth-1.0.0/django_silly_auth/views/api_views_if_drf.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/views/classics.py` & `django-silly-auth-1.0.0/django_silly_auth/views/classics.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/views/silly_views.py` & `django-silly-auth-1.0.0/django_silly_auth/views/silly_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth/views/test_views.py` & `django-silly-auth-1.0.0/django_silly_auth/views/test_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/django_silly_auth.egg-info/PKG-INFO` & `django-silly-auth-1.0.0/django_silly_auth.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 0.1.1
+Version: 1.0.0
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
```

### Comparing `django-silly-auth-0.1.1/django_silly_auth.egg-info/SOURCES.txt` & `django-silly-auth-1.0.0/django_silly_auth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-silly-auth-0.1.1/setup.py` & `django-silly-auth-1.0.0/setup.py`

 * *Files identical despite different names*

