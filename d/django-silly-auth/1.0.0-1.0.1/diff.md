# Comparing `tmp/django-silly-auth-1.0.0.tar.gz` & `tmp/django-silly-auth-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-silly-auth-1.0.0.tar", last modified: Mon Apr 10 01:50:56 2023, max compression
+gzip compressed data, was "django-silly-auth-1.0.1.tar", last modified: Mon Apr 10 21:33:02 2023, max compression
```

## Comparing `django-silly-auth-1.0.0.tar` & `django-silly-auth-1.0.1.tar`

### file list

```diff
@@ -1,56 +1,65 @@
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.348334 django-silly-auth-1.0.0/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.0.0/LICENSE.md
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1550 2023-04-10 01:50:56.348334 django-silly-auth-1.0.0/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      940 2023-04-10 01:22:43.000000 django-silly-auth-1.0.0/README.md
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.328333 django-silly-auth-1.0.0/django_silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-04-10 01:50:14.000000 django-silly-auth-1.0.0/django_silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4730 2023-04-10 01:39:52.000000 django-silly-auth-1.0.0/django_silly_auth/config.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5726 2023-04-10 01:39:27.000000 django-silly-auth-1.0.0/django_silly_auth/forms.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2468 2023-04-10 01:38:49.000000 django-silly-auth-1.0.0/django_silly_auth/mixins.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5164 2023-04-10 01:38:31.000000 django-silly-auth-1.0.0/django_silly_auth/serializers.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.336334 django-silly-auth-1.0.0/django_silly_auth/templates/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:44:50.000000 django-silly-auth-1.0.0/django_silly_auth/templates/__init__.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.336334 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:44:57.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_base.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.340334 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_test/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:45:22.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_test/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4265 2023-04-10 01:17:29.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_test/_base.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      175 2023-04-04 22:34:28.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_test/_test.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      274 2023-04-04 20:59:42.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_test/_users.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.344334 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:45:14.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      515 2023-04-05 04:15:11.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/account.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      528 2023-04-05 04:15:11.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/change_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      539 2023-04-05 04:15:11.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/change_username.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      328 2023-04-05 04:15:11.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/index.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1045 2023-04-06 16:37:59.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/login.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-05 04:15:11.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      527 2023-04-06 16:37:59.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      800 2023-04-06 16:37:59.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/reset_password.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1094 2023-04-06 17:29:58.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/signup.html
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.344334 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/emails/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:45:06.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/emails/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      238 2023-04-10 01:22:43.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      238 2023-03-31 12:20:50.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.344334 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/silly/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:46:56.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/silly/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      462 2023-04-10 01:22:43.000000 django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     4424 2023-04-10 01:37:32.000000 django-silly-auth-1.0.0/django_silly_auth/urls.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     3696 2023-04-10 01:37:25.000000 django-silly-auth-1.0.0/django_silly_auth/utils.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.348334 django-silly-auth-1.0.0/django_silly_auth/views/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:44:30.000000 django-silly-auth-1.0.0/django_silly_auth/views/__init__.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2978 2023-04-10 01:44:09.000000 django-silly-auth-1.0.0/django_silly_auth/views/api_custom_login.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      325 2023-04-10 01:42:31.000000 django-silly-auth-1.0.0/django_silly_auth/views/api_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     5123 2023-04-10 01:43:11.000000 django-silly-auth-1.0.0/django_silly_auth/views/api_views_if_drf.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)    13103 2023-04-10 01:42:03.000000 django-silly-auth-1.0.0/django_silly_auth/views/classics.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1756 2023-04-10 01:41:23.000000 django-silly-auth-1.0.0/django_silly_auth/views/silly_views.py
--rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-10 01:40:40.000000 django-silly-auth-1.0.0/django_silly_auth/views/test_views.py
-drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:50:56.336334 django-silly-auth-1.0.0/django_silly_auth.egg-info/
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     1550 2023-04-10 01:50:56.000000 django-silly-auth-1.0.0/django_silly_auth.egg-info/PKG-INFO
--rw-rw-r--   0 byoso     (1000) byoso     (1000)     2058 2023-04-10 01:50:56.000000 django-silly-auth-1.0.0/django_silly_auth.egg-info/SOURCES.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-10 01:50:56.000000 django-silly-auth-1.0.0/django_silly_auth.egg-info/dependency_links.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-04-10 01:50:56.000000 django-silly-auth-1.0.0/django_silly_auth.egg-info/requires.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-04-10 01:50:56.000000 django-silly-auth-1.0.0/django_silly_auth.egg-info/top_level.txt
--rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-10 01:50:56.348334 django-silly-auth-1.0.0/setup.cfg
--rwxrwxr-x   0 byoso     (1000) byoso     (1000)     1952 2023-04-10 01:47:20.000000 django-silly-auth-1.0.0/setup.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.988087 django-silly-auth-1.0.1/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1072 2023-03-30 21:48:27.000000 django-silly-auth-1.0.1/LICENSE.md
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1588 2023-04-10 21:33:02.988087 django-silly-auth-1.0.1/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      978 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/README.md
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.964087 django-silly-auth-1.0.1/django_silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       51 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4641 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/config.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     6655 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/forms.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.968087 django-silly-auth-1.0.1/django_silly_auth/locale/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10385 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/locale/django.pot
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.956087 django-silly-auth-1.0.1/django_silly_auth/locale/en/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.968087 django-silly-auth-1.0.1/django_silly_auth/locale/en/LC_MESSAGES/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    10399 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/locale/en/LC_MESSAGES/django.po
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.956087 django-silly-auth-1.0.1/django_silly_auth/locale/fr/
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.968087 django-silly-auth-1.0.1/django_silly_auth/locale/fr/LC_MESSAGES/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     9661 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/locale/fr/LC_MESSAGES/django.mo
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    14409 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/locale/fr/LC_MESSAGES/django.po
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2473 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/mixins.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5326 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/serializers.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.968087 django-silly-auth-1.0.1/django_silly_auth/templates/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      141 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/templates/__init__.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.968087 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      152 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      512 2023-04-04 22:34:28.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_base.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.972087 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_test/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_test/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4497 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_test/_base.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_test/_test.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      276 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_test/_users.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.980086 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      161 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      621 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/account.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      598 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/change_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      613 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/change_username.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      388 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/index.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1156 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/login.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      570 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/request_password_reset.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      583 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      870 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/reset_password.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1147 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/signup.html
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.984087 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/emails/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      159 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/emails/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      300 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/emails/confirm_email.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      311 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/emails/request_password_reset.txt
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.984087 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/silly/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        0 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/silly/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      462 2023-04-10 01:22:43.000000 django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/silly/silly_confirm_email.html
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     4565 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/urls.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3696 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/utils.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.988087 django-silly-auth-1.0.1/django_silly_auth/views/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      137 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/views/__init__.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     3066 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/views/api_custom_login.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      325 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/views/api_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     5187 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/views/api_views_if_drf.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)    13439 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/views/classics.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1775 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/django_silly_auth/views/silly_views.py
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)      985 2023-04-10 01:52:00.000000 django-silly-auth-1.0.1/django_silly_auth/views/test_views.py
+drwxrwxr-x   0 byoso     (1000) byoso     (1000)        0 2023-04-10 21:33:02.968087 django-silly-auth-1.0.1/django_silly_auth.egg-info/
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     1588 2023-04-10 21:33:02.000000 django-silly-auth-1.0.1/django_silly_auth.egg-info/PKG-INFO
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)     2244 2023-04-10 21:33:02.000000 django-silly-auth-1.0.1/django_silly_auth.egg-info/SOURCES.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)        1 2023-04-10 21:33:02.000000 django-silly-auth-1.0.1/django_silly_auth.egg-info/dependency_links.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       13 2023-04-10 21:33:02.000000 django-silly-auth-1.0.1/django_silly_auth.egg-info/requires.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       18 2023-04-10 21:33:02.000000 django-silly-auth-1.0.1/django_silly_auth.egg-info/top_level.txt
+-rw-rw-r--   0 byoso     (1000) byoso     (1000)       38 2023-04-10 21:33:02.988087 django-silly-auth-1.0.1/setup.cfg
+-rwxrwxr-x   0 byoso     (1000) byoso     (1000)     2193 2023-04-10 21:30:12.000000 django-silly-auth-1.0.1/setup.py
```

### Comparing `django-silly-auth-1.0.0/LICENSE.md` & `django-silly-auth-1.0.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.0/PKG-INFO` & `django-silly-auth-1.0.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 1.0.0
+Version: 1.0.1
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
@@ -37,7 +37,11 @@
 # [WIKI documentation](https://github.com/byoso/django_silly_auth/wiki)
 
 ## [Read this FIRST](https://github.com/byoso/django_silly_auth/wiki/Must-read-this-few-lines-!)
 
 ### :coffee: [If you find this package usefull, consider buying me a coffee](https://www.buymeacoffee.com/byoso)
 
 
+### Changelog
+- 1.0.1: i18n fr + en
+
+
```

### Comparing `django-silly-auth-1.0.0/README.md` & `django-silly-auth-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -16,7 +16,11 @@
 <hr>
 
 # [WIKI documentation](https://github.com/byoso/django_silly_auth/wiki)
 
 ## [Read this FIRST](https://github.com/byoso/django_silly_auth/wiki/Must-read-this-few-lines-!)
 
 ### :coffee: [If you find this package usefull, consider buying me a coffee](https://www.buymeacoffee.com/byoso)
+
+
+### Changelog
+- 1.0.1: i18n fr + en
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/config.py` & `django-silly-auth-1.0.1/django_silly_auth/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,9 @@
 from django.conf import settings
 
-# django_silly_auth version
-__version__ = "0.1.1"
-
 
 class SillyAuthError(Exception):
     pass
 
 
 SILLY_AUTH_SETTINGS = {
     # Quick settings
@@ -118,9 +115,8 @@
     float(SILLY_AUTH_SETTINGS["DELETE_UNCONFIRMED_TIME"])
     assert SILLY_AUTH_SETTINGS["DELETE_UNCONFIRMED_TIME"] >= 0
 except (ValueError, AssertionError):
     raise SillyAuthError("DELETE_UNCONFIRMED_TIME must be a positive float, or 0 to set off")
 
 
 if SILLY_AUTH_SETTINGS["VERBOSE"]:
-    print(f"=== DSA Version: {__version__}")
-    print("=== DSA IMPORT django_silly_auth")
+    print("=== DSA IMPORT django_silly_auth.config")
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/forms.py` & `django-silly-auth-1.0.1/django_silly_auth/forms.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,109 +19,132 @@
 class NewPasswordForm(forms.Form):
 
     password = forms.CharField(
         max_length=64, widget=forms.PasswordInput,
         validators=[validate_password]
     )
     password2 = forms.CharField(
-        label="Confirm password",
+        label=_("Confirm password"),
         max_length=64, widget=forms.PasswordInput,
         validators=[validate_password]
     )
 
     def clean_password2(self):
         password = self.cleaned_data['password']
         password2 = self.cleaned_data['password2']
         if password != password2:
-            raise ValidationError("Passwords don't match, do it again")
+            raise ValidationError(_("The passwords you entered do not match."))
         return password2
 
 
 class NewEmailConfirmForm(forms.Form):
 
     password = forms.CharField(
         max_length=64, widget=forms.PasswordInput,
         validators=[validate_password]
     )
 
 #################### FULL CLASSIC FORMS ####################
 
+
 class LoginForm(forms.Form):
     credential = forms.CharField(
         label=_("Username or email"),
         max_length=64,
-        widget=forms.TextInput({'placeholder': _('username or email')})
+        widget=forms.TextInput({
+            'placeholder': _('Username or email'),
+        })
     )
     password = forms.CharField(
         label=_("Password"),
-        max_length=64, widget=forms.PasswordInput,
+        max_length=64,
+        widget=forms.PasswordInput(
+            {'placeholder': _('Password')}
+        ),
         validators=[validate_password]
     )
 
     def clean_login(self):
         credential = self.cleaned_data['credential']
         if "@" in credential:
             user = User.objects.filter(email=credential)
         else:
             user = User.objects.filter(username=credential)
         if not user or not user[0].is_confirmed:
-            raise ValidationError(_(f"user '{credential}' unknown or unconfirmed"))
+            raise ValidationError(_(f"User '{credential}' unknown or unconfirmed"))
         return credential
 
 
 class SignUpForm(forms.Form):
     username = forms.CharField(
         label=_("Username"),
         validators=[MinLengthValidator(4), MaxLengthValidator(64)],
         max_length=64,
+        widget=forms.TextInput({
+            'placeholder': _('Username'),
+        })
     )
     email = forms.EmailField(
         label=_("Email"),
-        validators=[EmailValidator()])
+        validators=[EmailValidator()],
+        widget=forms.EmailInput({
+            'placeholder': _('Email'),
+        }),
+        )
 
     password = forms.CharField(
         label=_("Password"),
-        max_length=64, widget=forms.PasswordInput,
-        validators=[validate_password]
+        max_length=64,
+        validators=[validate_password],
+        widget=forms.PasswordInput({
+            'placeholder': _('Password'),
+        }),
     )
     password2 = forms.CharField(
-        label="Confirm password",
-        max_length=64, widget=forms.PasswordInput,
-        validators=[validate_password]
+        label=_("Confirm password"),
+        max_length=64,
+        validators=[validate_password],
+        widget=forms.PasswordInput({
+            'placeholder': _('Password'),
+        }),
     )
 
     def clean_password2(self):
         password = self.cleaned_data['password']
         password2 = self.cleaned_data['password2']
         if password != password2:
             raise ValidationError(_("different than password"))
         return password2
 
     def clean_username(self):
         username = self.cleaned_data['username']
         if "@" in username:
-            raise ValidationError(_("'@' not allowed in a username"))
+            raise ValidationError(_("A username cannot include the symbol '@'."))
         else:
             user = User.objects.filter(username=username)
             if user:
-                raise ValidationError(_(f"'{username}' already used by someone"))
+                raise ValidationError(_(f"'{username}' is already taken by someone else."))
         return username
 
     def clean_email(self):
         email = self.cleaned_data['email']
         user = User.objects.filter(email=email)
         if user:
-            raise ValidationError(_(f"'{email}' already used."))
+            raise ValidationError(_(f"'{email}' is already taken by someone else."))
         return email
 
 
 class CredentialForm(forms.Form):
     credential = forms.CharField(
-        label=_("Email or username"),
-        validators=[])
+        label=_("Username or email"),
+        validators=[],
+        widget=forms.TextInput({
+            'placeholder': _('Username or email'),
+        }),
+        )
 
     def clean_credential(self):
         credential = self.cleaned_data['credential']
         if "@" in credential:
             user = User.objects.filter(email=credential)
         else:
             user = User.objects.filter(username=credential)
@@ -129,57 +152,70 @@
             raise ValidationError(_(f"'{credential}' unknown or unconfirmed"))
         return credential
 
 
 class ResetPasswordForm(forms.Form):
     password = forms.CharField(
         label=_("Password"),
-        max_length=64, widget=forms.PasswordInput,
+        max_length=64,
+        widget=forms.PasswordInput({
+            'placeholder': _('Password'),
+        }),
         validators=[validate_password]
     )
     password2 = forms.CharField(
         label=_("Confirm password"),
-        max_length=64, widget=forms.PasswordInput,
+        max_length=64,
+        widget=forms.PasswordInput({
+            'placeholder': _('Password'),
+        }),
         validators=[validate_password]
     )
 
     def clean_password(self):
         password = self.cleaned_data['password']
         return password
 
     def clean_password2(self):
         password = self.cleaned_data['password']
         password2 = self.cleaned_data['password2']
         if password != password2:
-            raise ValidationError(_("different than password"))
+            raise ValidationError(_("The passwords you entered do not match."))
         return password2
 
 
 class ChangeUsernameForm(forms.Form):
     username = forms.CharField(
+        label=_("New username"),
         validators=[MinLengthValidator(4), MaxLengthValidator(64)],
         max_length=64,
+        widget=forms.TextInput({
+            'placeholder': _('Username'),
+        })
     )
 
     def clean_username(self):
         username = self.cleaned_data['username']
         if "@" in username:
-            raise ValidationError(_("'@' not allowed in a username"))
+            raise ValidationError(_("A username cannot include the symbol '@'."))
         else:
             user = User.objects.filter(username=username)
             if user:
-                raise ValidationError(_(f"'{username}' is already used by someone"))
+                raise ValidationError(_(f"'{username}' is already taken by someone else."))
         return username
 
 
 class ChangeEmailForm(forms.Form):
     email = forms.EmailField(
-        label=_("New e-mail address"),
-        validators=[EmailValidator()]
+        label=_("New email address"),
+        validators=[EmailValidator()],
+        widget=forms.EmailInput({
+            'placeholder': _('Email'),
+        }),
         )
 
     def clean_email(self):
         email = self.cleaned_data['email']
         user = User.objects.filter(email=email)
         if user:
-            raise ValidationError(_(f"'{email}' already used by someone"))
+            raise ValidationError(_(f"'{email}' already taken by someone else."))
         return email
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/mixins.py` & `django-silly-auth-1.0.1/django_silly_auth/mixins.py`

 * *Files 8% similar despite different names*

```diff
@@ -69,15 +69,15 @@
             print("Token error:", e)
             return None
         return get_object_or_404(get_user_model(), id=pk)
 
     def clean(self):
         if "@" in self.username:
             raise ValidationError(
-                {'username': _("username can't contain '@' character")})
+                {'username': _("A username cannot include the symbol '@'.")})
         super().clean()
 
     def save(self, *args, **kwargs):
         # self.full_clean()
         super().save(*args, **kwargs)
 
     def __str__(self):
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/serializers.py` & `django-silly-auth-1.0.1/django_silly_auth/serializers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from django.contrib.auth import get_user_model
 from django.core import exceptions
 from django.contrib.auth.password_validation import validate_password
+from django.utils.translation import gettext_lazy as _
 
 from rest_framework import serializers
 from django_silly_auth.config import SILLY_AUTH_SETTINGS as conf
 
 if conf["VERBOSE"]:
     print("=== DSA IMPORT django_silly_auth.serializers")
 
@@ -36,15 +37,15 @@
                 password=password,
                 user=None,
                 password_validators=None)
         except exceptions.ValidationError as e:
             password_errors += list(e.messages)
 
         if "@" in username:
-            username_errors += ["A username must not contain '@'", ]
+            username_errors += [_("A username cannot include the symbol '@'."), ]
 
         if username_errors:
             errors["username"] = username_errors
         if password_errors:
             errors["password"] = password_errors
         if email_errors:
             errors["email"] = email_errors
@@ -65,15 +66,15 @@
     def validate(self, data):
         password = data.get('password')
         password2 = data.get('password2')
         errors = dict()
         password_errors = list()
 
         if password != password2:
-            password_errors += ["Passwords don't match", ]
+            password_errors += [_("The passwords you entered do not match."), ]
 
         try:
             validate_password(
                 password=password,
                 user=None,
                 password_validators=None)
 
@@ -91,15 +92,15 @@
 
     def validate(self, data):
         email = data.get('email')
         errors = dict()
         email_errors = list()
 
         if User.objects.filter(email=email).exists():
-            email_errors += ["Email already in use", ]
+            email_errors += [_("This email is already associated with an existing account."), ]
 
         if email_errors:
             errors['email'] = email_errors
             raise serializers.ValidationError(errors)
         return data
 
 
@@ -112,18 +113,18 @@
         password = data.get('password')
         errors = dict()
         credential_errors = list()
         password_errors = list()
 
         if "@" in credential:
             if not User.objects.filter(email=credential).exists():
-                credential_errors += ["Email not found", ]
+                credential_errors += [_("Email not found"), ]
         else:
             if not User.objects.filter(username=credential).exists():
-                credential_errors += ["User not found", ]
+                credential_errors += [_("User not found"), ]
 
         if credential_errors:
             errors['username'] = credential_errors
         if password_errors:
             errors['password'] = password_errors
 
         if errors:
@@ -140,28 +141,28 @@
         jwt_token = data.get('jwt_token')
         errors = dict()
         credential_errors = list()
         jwt_errors = list()
         user = None
         if "@" in credential:
             if not User.objects.filter(email=credential).exists():
-                credential_errors += ["Email not found", ]
+                credential_errors += [_("Email not found"), ]
             else:
                 user = User.objects.filter(email=credential).first()
         else:
             if not User.objects.filter(username=credential).exists():
-                credential_errors += ["User not found", ]
+                credential_errors += [_("User not found"), ]
             else:
                 user = User.objects.filter(username=credential).first()
         if credential_errors:
             errors['credential'] = credential_errors
 
         jwt_user = User.verify_jwt_token(jwt_token)
         if (user is not None and jwt_user is not None) and user != jwt_user:
-            jwt_errors += ['token does not match user']
+            jwt_errors += [_("The given token does not match the user")]
         if User.verify_jwt_token(jwt_token) is None:
-            jwt_errors += ["jwt token invalid or expired"]
+            jwt_errors += [_("jwt token invalid or expired")]
         if jwt_errors:
             errors['jwt_token'] = jwt_errors
         if errors:
             raise serializers.ValidationError(errors)
         return data
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_base.html` & `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_base.html`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/_test/_base.html` & `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/_test/_base.html`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+{% load i18n %}
 <!DOCTYPE html>
 <html>
   <head>
     <meta charset="utf-8">
     <meta name="viewport" content="width=device-width, initial-scale=1">
     <title>Password reset</title>
     <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bulma@0.9.4/css/bulma.min.css">
@@ -21,70 +22,72 @@
             <span aria-hidden="true"></span>
           </a>
         </div>
 
         <div id="navbarBasicExample" class="navbar-menu">
           <div class="navbar-start">
             <a class="navbar-item" href="{% url 'classic_index' %}">
-              Home
+              {% translate 'Home' %}
             </a>
 
             {% if user.is_authenticated %}
             <a class="navbar-item" href="{% url 'classic_account' %}">
-              Account
+              {% translate 'Account' %}
             </a>
             {% endif%}
 
             <div class="navbar-item has-dropdown is-hoverable">
               <a class="navbar-link">
-                More
+                {% translate 'More' %}
               </a>
 
               <div class="navbar-dropdown">
                 <a class="navbar-item" href="https://github.com/byoso/django_silly_auth/wiki" target="_blank">
-                  Documentation
+                  {% translate 'Documentation' %}
                 </a>
                 <a class="navbar-item" href="https://www.buymeacoffee.com/byoso" target="_blank">
-                  Buy me a coffee
+                  {% translate 'Buy me a coffee' %}
                 </a>
                 <a class="navbar-item" href="mailto:mail@mail.com">
-                  Contact
+                  {% translate 'Contact' %}
                 </a>
                 <hr class="navbar-divider">
                 <a class="navbar-item" href="https://github.com/byoso/django_silly_auth/issues" target="_blank">
-                  Report an issue
+                  {% translate 'Report an issue' %}
                 </a>
               </div>
+
             </div>
           </div>
 
           <div class="navbar-end">
             <div class="navbar-item">
               <div class="buttons">
                 {% if user.is_authenticated %}
                 <a class="button is-warning" href="{% url 'classic_logout' %}">
-                  Log out
+                  {% translate 'Log out' %}
                 </a>
                 {% else %}
                 <a class="button is-primary" href="{% url 'classic_signup' %}">
-                  <strong>Sign up</strong>
+                  <strong>{% translate 'Sign up' %}</strong>
                 </a>
                 <a class="button is-light" href="{% url 'classic_login' %}">
-                  Log in
+                  {% translate 'Log in' %}
                 </a>
                 {% endif %}
               </div>
             </div>
           </div>
+
         </div>
       </nav>
       <nav>
 
-        <a href="{% url 'test_templates_view' %}">  Test single page </a>
-        <a href="{% url 'test_users_view' %}"> :: Test Users page </a>
+        <a href="{% url 'test_templates_view' %}">  {% translate 'Test single page' %}</a>
+        <a href="{% url 'test_users_view' %}"> :: {% translate 'Test Users page' %}</a>
 
       </nav>
 
       {% if messages %}
 
         {% for message in messages %}
           <div class="notification is-{{ message.tags }}">
```

#### html2text {}

```diff
@@ -1,13 +1,17 @@
+{% load i18n %}
 
 ******_DSA_test_-_base_template_******
 
-Home {% if user.is_authenticated %} Account {% endif%}
-More
-Documentation Buy_me_a_coffee Contact
+{%_translate_'Home'_%} {% if user.is_authenticated %} {%_translate_'Account'_%}
+{% endif%}
+{% translate 'More' %}
+{%_translate_'Documentation'_%} {%_translate_'Buy_me_a_coffee'_%} {%_translate
+'Contact'_%}
 ===============================================================================
-Report_an_issue
-{% if user.is_authenticated %} Log_out {% else %} Sign_up Log_in {% endif %}
-  Test_single_page ::_Test_Users_page  {% if messages %} {% for message in
-messages %}
+{%_translate_'Report_an_issue'_%}
+{% if user.is_authenticated %} {%_translate_'Log_out'_%} {% else %} {%
+translate_'Sign_up'_%} {%_translate_'Log_in'_%} {% endif %}
+  {%_translate_'Test_single_page'_%} ::_{%_translate_'Test_Users_page'_%}  {%
+if messages %} {% for message in messages %}
  {{ message }}
 {% endfor %} {% endif %} {% block content %} {% endblock content %}
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/account.html` & `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/account.html`

 * *Files 25% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 {% extends base_template %}
 
+{% load i18n %}
+
 
 {% block content %}
 
-<h1 class="h2 subtitle">Account</h1>
+<h1 class="h2 subtitle">
+  {% translate 'Account' %}</h1>
 
 <h3>{{user.username}} - {{ user.email }}</h3>
-    secret id: {{ user.id }}
+{% translate 'id:' %}  {{ user.id }}
     <hr>
 <p>
-   <a class="button is-primary m-2" href="{% url 'classic_change_username' %}">Change my Username</a>
+   <a class="button is-primary m-2" href="{% url 'classic_change_username' %}">{% translate 'Change my Username' %}</a>
 
-   <a class="button is-primary m-2" href="{% url 'classic_change_email' %}"> Change my email </a>
+   <a class="button is-primary m-2" href="{% url 'classic_change_email' %}">{% translate 'Change my email' %} </a>
 
-   <a class="button is-primary m-2" href="{% url 'classic_request_password_reset' %}">Reset my password</a>
+   <a class="button is-primary m-2" href="{% url 'classic_reset_password_authenticated' %}">{% translate 'Change my password' %}</a>
 </p>
 
 {% endblock content %}
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/change_email.html` & `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/change_email.html`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 {% extends base_template %}
 
+{% load i18n %}
 
 {% block content %}
 
-<h1 class="h2 subtitle">Change Email</h1>
+<h1 class="h2 subtitle">{% translate 'Change Email' %}</h1>
 
-<p>Your current email: {{ user.email }}</p>
+<p>{% translate 'Your current email:' %} {{ user.email }}</p>
 
 <form method="post">
     {% csrf_token %}
 
     <p>
         {{ form.email.label }} <br>
         {{ form.email }} <br>
         {% for error in form.errors.email %}
         <span style="color: red;">{{ error }}</span>
         {% endfor %}
 
     </p>
     <p>
-        <input type="submit" class="button is-success m-2 btn btn-success" value="confirm">
+        <input type="submit" class="button is-success m-2 btn btn-success" value="{% translate 'confirm' %}">
     </p>
 
 </form>
 
 
 
 {% endblock content %}
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/change_username.html` & `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/change_username.html`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 {% extends base_template %}
 
+{% load i18n %}
 
 {% block content %}
 
-<h1 class="h2 subtitle">Change Username</h1>
+<h1 class="h2 subtitle">
+  {% translate 'Change Username' %}
+</h1>
 
-Current username: {{ user.username }} <br>
+{% translate 'Current username' %}: {{ user.username }} <br>
 
 <form method="post">
     {% csrf_token %}
 
     <p>
         {{ form.username.label }} <br>
         {{ form.username }} <br>
         {% for error in form.errors.username %}
         <span style="color: red;">{{ error }}</span>
         {% endfor %}
 
     </p>
     <p>
-        <input type="submit" class="button is-success m-2 btn btn-success" value="confirm">
+        <input type="submit" class="button is-success m-2 btn btn-success" value="{% translate 'confirm' %}">
     </p>
 
 </form>
 
 
 
 {% endblock content %}
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/login.html` & `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/login.html`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 {% extends base_template %}
 
+{% load i18n %}
+
 {% block content %}
-<h1 class="h2 subtitle">Login</h1>
+
+<h1 class="h2 subtitle">
+  {% translate 'Login' %}
+</h1>
+
 <form method="post">
   {% csrf_token %}
 
   <p>
       {{ form.credential.label }} <br>
       {{ form.credential }} <br>
       <ul>
@@ -24,24 +30,26 @@
         {% endfor %}
       </ul>
       <br>
   </p>
 
   <ul>
     <li>
-      <a href="{% url 'classic_request_password_reset' %}">I forgot my password.</a>
+      <a href="{% url 'classic_request_password_reset' %}">
+        {% translate 'I forgot my password.' %}
+      </a>
     </li>
     <li>
       <p>
         <a href="{% url 'classic_request_resend_confirmation_email' %}">
-          My account exists but is unconfirmed, please send me the confirmation email again.
+          {% translate 'My account exists but is unconfirmed, please send me the confirmation email again.' %}
         </a>
       </p>
 
     </li>
   </ul>
 
-  <input type="submit" class="button is-success m-2 btn btn-success" value="log in">
+  <input type="submit" class="button is-success m-2 btn btn-success" value="{% translate 'log in' %}">
 </form>
 
 
 {% endblock content %}
```

#### html2text {}

```diff
@@ -1,19 +1,19 @@
-{% extends base_template %} {% block content %}
-****** Login ******
+{% extends base_template %} {% load i18n %} {% block content %}
+****** {% translate 'Login' %} ******
 {% csrf_token %}
 {{ form.credential.label }}
 {{ form.credential }}
     * {% for error in form.errors.credential %}
     * {{ error }}
     * {% endfor %}
 {{ form.password.label }}
 {{ form.password }}
     * {% for error in form.errors.password %}
     * {{ error }}
     * {% endfor %}
 
-    * I_forgot_my_password.
-    * My_account_exists_but_is_unconfirmed,_please_send_me_the_confirmation
-      email_again.
-[log in]
+    * {%_translate_'I_forgot_my_password.'_%}
+    * {%_translate_'My_account_exists_but_is_unconfirmed,_please_send_me_the
+      confirmation_email_again.'_%}
+[{% translate 'log in' %}]
 {% endblock content %}
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/request_password_reset.html` & `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/request_password_reset.html`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 {% extends base_template %}
 
+{% load i18n %}
 
 {% block content %}
-<h1 class="h2 subtitle">Request password reset</h1>
+
+
+<h1 class="h2 subtitle">
+  {% translate 'Request password reset' %}</h1>
 
 <form method="post">
     {% csrf_token %}
     <p>
         {{ form.credential.label }} <br>
         {{ form.credential }} <br>
         {% for error in form.errors.credential %}
         <span style="color: red;">{{ error }}</span>
         {% endfor %}
 
     </p>
     <p>
-        <input type="submit" class="button is-warning m-2 btn btn-warning"value="send me an email">
+        <input type="submit" class="button is-warning m-2 btn btn-warning" value="{% translate 'send me an email' %}">
     </p>
 
 </form>
 
 {% endblock content %}
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html` & `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/request_resend_account_confirmation_email.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,29 @@
 {% extends base_template %}
 
+{% load i18n %}
 
 {% block content %}
 
 
-<h1 class="h2 subtitle">Request resend account confirmation email</h1>
+<h1 class="h2 subtitle">
+  {% translate "Request resend account confirmation email" %}
+</h1>
 
 <form method="post">
     {% csrf_token %}
     <p>
         {{ form.credential.label }} <br>
         {{ form.credential }} <br>
         {% for error in form.errors.credential %}
         <span style="color: red;">{{ error }}</span>
         {% endfor %}
 
     </p>
     <p>
-        <input type="submit" class="button is-warning m-2 btn btn-warning" value="send me an email">
+        <input type="submit" class="button is-warning m-2 btn btn-warning" value="{% translate 'send me an email' %}">
     </p>
 
 </form>
 
 
 {% endblock %}
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/reset_password.html` & `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/reset_password.html`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 {% extends base_template %}
-
+{% load i18n %}
 
 {% block content %}
 
-<h1 class="h2 subtitle">Reset Password</h1>
+<h1 class="h2 subtitle">{% translate "Reset Password" %}</h1>
 
-user: {{ user.username }} <br>
+{% translate "user" %}: {{ user.username }} <br>
 
 <form method="post">
     {% csrf_token %}
 
     <p>
         {{ form.password.label }} <br>
         {{ form.password }} <br>
@@ -29,15 +29,15 @@
           <li style="color: red;">{{ error }}</li>
           {% endfor %}
 
         </ul>
 
     </p>
     <p>
-        <input type="submit" class="button is-success m-2 btn btn-success"value="confirm">
+        <input type="submit" class="button is-success m-2 btn btn-success" value="{% translate 'confirm' %}">
     </p>
 
 </form>
 
 
 
 {% endblock content %}
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/templates/silly_auth/classic/signup.html` & `django-silly-auth-1.0.1/django_silly_auth/templates/silly_auth/classic/signup.html`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 {% extends base_template %}
 
-<h1 class="h2 subtitle">Sign up</h1>
+{% load i18n %}
+
+<h1 class="h2 subtitle">{% translate "Sign up" %}</h1>
 
 {% block content %}
 
 <form method="post">
     {% csrf_token %}
 
     <p>
@@ -31,14 +33,14 @@
     <p>
         {{ form.password2.label }} <br>
         {{ form.password2 }} <br>
         {% for error in form.errors.password2 %}
         <span style="color: red;">{{ error }}</span>
         {% endfor %}
     </p>
-        <input type="submit" class="button is-success m-2 btn btn-success" value="Sign In">
+        <input type="submit" class="button is-success m-2 btn btn-success" value="{% translate 'Sign Up' %}">
 
 
 </form>
 
 
 {% endblock content %}
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/urls.py` & `django-silly-auth-1.0.1/django_silly_auth/urls.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from django_silly_auth.config import SILLY_AUTH_SETTINGS as conf
 from django_silly_auth.views import (
     api_views,
     test_views,
     silly_views,
     classics)
 
-import django_silly_auth
 
 if conf["VERBOSE"]:
     print("=== DSA IMPORT django_silly_auth.urls")
     if conf["USE_DRF"]:
         print("=== DSA login_with_auth_token FROM django_silly_auth.views.api_custom_login")
 
 if conf["USE_DRF"]:
@@ -79,14 +78,19 @@
         path(f'{prefix}classic_change_email/', classics.change_email, name='classic_change_email'),
         path(f'{prefix}classic_confirm_email/<token>', classics.confirm_email, name='classic_confirm_email'),
         path(
             f'{prefix}classic_request_resend_confirmation_email/',
             classics.request_resend_account_confirmation_email,
             name='classic_request_resend_confirmation_email'
         ),
+        path(
+            f'{prefix}classic_reset_password/',
+            classics.reset_password,
+            name='classic_reset_password_authenticated'
+        ),
     ]
     if conf["USE_CLASSIC_INDEX"]:
         urlpatterns += [path('', classics.index, name='classic_index'), ]
     if conf["USE_CLASSIC_ACCOUNT"]:
         urlpatterns += [path(f'{prefix}classic_account/', classics.account, name='classic_account'), ]
 
 # Email Confirmation routes
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/utils.py` & `django-silly-auth-1.0.1/django_silly_auth/utils.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.0/django_silly_auth/views/api_custom_login.py` & `django-silly-auth-1.0.1/django_silly_auth/views/api_custom_login.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,19 +37,21 @@
             user = User.objects.filter(username=credential).first()
         password = serializer.validated_data['password']
         match = False
         if user:
             match = user.check_password(password)
         if match:
             if not user.is_confirmed and not user.is_superuser:
-                msg = _('Account not confirmed. Please check your email for a confirmation link.')
+                msg = _(
+                    'Your account has not been confirmed yet. '
+                    'Please check your inbox for a confirmation link.')
                 raise ValidationError(msg, code='authorization')
             token, created = Token.objects.get_or_create(user=user)
             return Response({'token': token.key})
-        msg = _('Unable to log in with the provided credentials.')
+        msg = _('Incorrect credentials.')
         raise ValidationError(msg, code='authorization')
 
 
 class LoginWithJWTToken(APIView):
     @transaction.atomic
     def post(self, request, *args, **kwargs):
         serializer = CredentialJWTokenSerializer(data=request.data)
@@ -61,13 +63,14 @@
                 user.new_email = None
                 user.save()
                 msg = _("Your account has been confirmed.")
             elif user.new_email:
                 user.email = user.new_email
                 user.new_email = None
                 user.save()
-                msg = _("Your new email has been activated")
+                msg = _("Your new email has been confirmed.")
             else:
-                msg = _("You've been logged in, please change your password if necessary.")
+                msg = _("You've been logged in via email confirmation, "
+                        "please change your password if necessary.")
             token, created = Token.objects.get_or_create(user=user)
             return Response({'token': token.key, 'message': msg})
         raise ValidationError(serializer.errors, code='authorization')
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/views/api_views_if_drf.py` & `django-silly-auth-1.0.1/django_silly_auth/views/api_views_if_drf.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,49 +40,49 @@
         raise ValidationError({"error": msg}, code='authorization')
     if "@" in credential:
         user = User.objects.filter(email=credential).first()
     else:
         user = User.objects.filter(username=credential).first()
     if user:
         if user.is_confirmed:
-            msg = _('account already confirmed')
+            msg = _("Your account is already confirmed.")
             raise ValidationError({"error": msg}, code='authorization')
             # return Response({'error': _('account already confirmed')})
         send_confirm_email(request, user)
-        return Response({'success': _('email sent for password reset')})
+        return Response({'success': _('Email sent for password reset')})
     msg = "Invalid credential"
     raise ValidationError({"error": msg}, code='authorization')
 
 
 @transaction.atomic
 @api_view(['GET'])
 @permission_classes([IsAuthenticated])
 def logout_api_view(request):
     """Destroys the auth token"""
     print("=== DSA LOGOUT API VIEW")
     request.user.auth_token.delete()
-    return Response({'success': _('logged out, token destroyed')})
+    return Response({'success': _('Logged out.')})
 
 
 @transaction.atomic
 @api_view(['POST'])
 @permission_classes([AllowAny])
 def request_password_reset(request):
     """Sends an email to the user with a link to reset their password"""
     credential = request.data.get('credential')
     if not credential:
-        msg = _("no credential provided")
+        msg = _("No credentials were provided")
         raise ValidationError({"error": msg}, code='authorization')
     if "@" in credential:
         user = User.objects.filter(email=credential).first()
     else:
         user = User.objects.filter(username=credential).first()
     if user:
         send_password_reset_email(request, user)
-        return Response({'success': _('email sent for password reset')})
+        return Response({'success': _("Email sent for password reset")})
     msg = _("Invalid credential")
     raise ValidationError({"error": msg}, code='authorization')
 
 
 class UserView(APIView):
     permission_classes = []
 
@@ -92,22 +92,22 @@
         serializer = CreateUserSerializer(data=request.data)
         if serializer.is_valid():
             user = serializer.save()
             user.set_password(request.data['password'])
             user.save()
             delete_unconfirmed(user)
             message = _(
-                    f"Please check your inbox '{user.email}' "
+                    f"Please check your inbox at '{user.email}' "
                     "to confirm your account. "
             )
             if conf["DELETE_UNCONFIRMED_TIME"] != 0:
-                message += _(
-                    "If your account is not confirmed in the next "
-                    f"{conf['DELETE_UNCONFIRMED_TIME']} hours, "
-                    "it will be deleted."
+                message += (
+                    _("If you do not confirm your account within the next "),
+                    _(f"{conf['DELETE_UNCONFIRMED_TIME']} hours, "),
+                    _("it will be deleted.")
                 )
             serializer = GetAllUsersSerializer(user)
             msg = {
                 "user": serializer.data,
             }
 
             send_confirm_email(request, user)
@@ -125,15 +125,15 @@
     """Changes the user's password"""
     serializer = PasswordsSerializer(data=request.data)
     if serializer.is_valid():
         user = request.user
         password = request.data.get('password')
         user.set_password(password)
         user.save()
-        return Response({'success': _('password changed')})
+        return Response({'success': _('Password successfully changed.')})
     msg = serializer.errors
     raise ValidationError({"error": msg}, code='authorization')
 
 
 @transaction.atomic
 @api_view(['POST'])
 @permission_classes([IsAuthenticated])
@@ -142,10 +142,11 @@
     serializer = EmailSerializer(data=request.data)
     if serializer.is_valid():
         new_email = request.data.get('email')
         user.new_email = new_email
         user.save()
         send_confirm_email(request, user, new_email=True)
 
-        return Response({'success': _('New email saved, check your inbox to activate it')})
+        return Response(
+            {'success': _(f"New email saved, check your inbox at '{new_email}' to activate it.")})
     msg = serializer.errors
     raise ValidationError({"error": msg}, code='authorization')
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/views/classics.py` & `django-silly-auth-1.0.1/django_silly_auth/views/classics.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,15 +51,15 @@
                     request, username=credential, password=password)
             if user is not None and user.is_confirmed:
                 login(request, user)
                 return redirect('classic_index')
             else:
                 messages.add_message(
                     request, messages.ERROR,
-                    message=_("Wrong credentials or unconfirmed account"),
+                    message=_("Incorrect credentials or unconfirmed account."),
                     extra_tags="warning"),
         else:
             context = {
                 "form": form,
                 "base_template": conf["BASE_TEMPLATE"],
                 "title": conf["TEMPLATES_TITLE"],
             }
@@ -98,23 +98,23 @@
             email = form.cleaned_data['email']
             password = form.cleaned_data['password']
             user = User(username=username, email=email, is_active=True)
             user.set_password(password)
             user.save()
             send_confirm_email(request, user)
             delete_unconfirmed(user)
-            message = _(
-                    f"Please check your email '{user.email}' "
-                    "to confirm your account. "
+            message = (
+                    _(f"Please check your inbox at '{user.email}' "),
+                    _("to confirm your account.")
             )
             if conf["DELETE_UNCONFIRMED_TIME"] != 0.0:
-                message += _(
-                    "If your account is not confirmed in the next "
-                    f"{conf['DELETE_UNCONFIRMED_TIME']} hours, "
-                    "it will be deleted."
+                message += (
+                    _("If you do not confirm your account within the next "),
+                    _(f"{conf['DELETE_UNCONFIRMED_TIME']} hours, "),
+                    _("it will be deleted.")
                 )
             messages.add_message(
                 request, messages.INFO,
                 message=message,
                 extra_tags="info"
             )
             return redirect('classic_login')
@@ -147,26 +147,27 @@
                 user = User.objects.get(username=credential)
             # user existence is checked by the form validation #
             if user.is_active:
                 messages.add_message(
                     request, messages.INFO,
                     message=(_(
                         "Please check your inbox "
-                        "to reset your password"
+                        "and follow the instructions "
+                        "to reset your password."
                         )),
                     extra_tags="info"
                 )
                 send_password_reset_email(request, user)
 
             else:
                 messages.add_message(
                     request, messages.INFO,
                     message=(_(
-                        "Your account is not active anymore, please contact the administrator, "
-                        "no email has been sent"
+                        "Your account is no longer active. Please contact the administrator. "
+                        "No email has been sent."
                         )),
                     extra_tags="info"
                 )
         else:
             context = {
                 "form": form,
                 "base_template": conf["BASE_TEMPLATE"],
@@ -185,56 +186,65 @@
         "base_template": conf["BASE_TEMPLATE"],
         "title": conf["TEMPLATES_TITLE"],
     }
     return render(request, conf["CLASSIC_REQUEST_PASSWORD_RESET"], context)
 
 
 @transaction.atomic
-def reset_password(request, token):
-    """Receive the token from the confirmation email and reset the password"""
-    user = User.verify_jwt_token(token)
+def reset_password(request, token=None):
+    """Receive the token from the confirmation email and reset the password
+    or already authenticated user.
+    """
+    if token:
+        user = User.verify_jwt_token(token)
+    elif request.user.is_authenticated:
+        user = request.user
+    else:
+        user = None
+
     if user is None:
         messages.add_message(
             request, messages.INFO,
             message=(_(
-                "Invalid or expired token"
+                "Token invalid or expired"
                 )),
             extra_tags="danger"
         )
         return redirect('classic_index')
 
     if request.method == 'POST':
         form = ResetPasswordForm(request.POST)
         if form.is_valid():
             user.set_password(form.cleaned_data['password'])
             user.save()
             if conf["USE_SILLY"]:
                 return redirect('silly_password_reset_done')
-
+            login(request, user)
             messages.add_message(
                 request, messages.SUCCESS,
-                message=_("Your password have been reset, please login"),
+                message=_("Your password has been successfully reset. Please log in."),
                 extra_tags="success"
             )
             return redirect('classic_index')
         else:
             context = {
                 'form': form,
                 "base_template": conf["BASE_TEMPLATE"],
                 "title": conf["TEMPLATES_TITLE"],
             }
             return render(request, conf["CLASSIC_RESET_PASSWORD"], context)
 
     form = ResetPasswordForm()
     login(request, user)
-    messages.add_message(
-        request, messages.SUCCESS,
-        message=_("Your have been logged in by email confirmation, please reset your password."),
-        extra_tags="warning"
-    )
+    if token:
+        messages.add_message(
+            request, messages.SUCCESS,
+            message=_("You have been logged in via email confirmation. Please reset your password."),
+            extra_tags="warning"
+        )
 
     context = {
         'form': form,
         "base_template": conf["BASE_TEMPLATE"],
         "title": conf["TEMPLATES_TITLE"],
     }
     return render(request, conf["CLASSIC_RESET_PASSWORD"], context)
@@ -248,15 +258,15 @@
         if form.is_valid():
             username = form.cleaned_data['username']
             user = request.user
             user.username = username
             user.save()
             messages.add_message(
                 request, messages.SUCCESS,
-                message=_(f"New username set: '{username}'"),
+                message=_(f"New username set: '{username}'."),
                 extra_tags="success"
             )
             return redirect("classic_account")
         else:
             context = {
                 'form': form,
                 "base_template": conf["BASE_TEMPLATE"],
@@ -287,18 +297,18 @@
             user = request.user
             user.new_email = email
             user.save()
             send_confirm_email(request, user)
 
             messages.add_message(
                 request, messages.INFO,
-                message=(_(
-                    "Please check your inbox to"
-                    f" confirm your new address '{email}'"
-                    )),
+                message=(
+                    _("Please check your inbox to"),
+                    _(f" confirm your new address at '{email}'")
+                    ),
                 extra_tags="info"
             )
             return redirect("classic_account")
         else:
             context = {
                 'form': form,
                 "base_template": conf["BASE_TEMPLATE"],
@@ -318,32 +328,32 @@
 @transaction.atomic
 def confirm_email(request, token):
     user = User.verify_jwt_token(token)
     if user is None:
         messages.add_message(
             request, messages.INFO,
             message=(_(
-                "Invalid or expired token"
+                "Token invalid or expired"
                 )),
             extra_tags="danger"
         )
         return redirect('classic_index')
     if user is not None and user.is_active:
         if not user.is_confirmed:
             user.is_confirmed = True
             user.new_email = None
-            msg = _("Your account have been confirmed")
+            msg = _("Your account has been confirmed.")
             user.save()
         elif user.new_email:
             user.email = user.new_email
             user.new_email = None
-            msg = _("Your new email have been confirmed")
+            msg = _("Your new email has been confirmed.")
             user.save()
         else:
-            msg = _("Your account is already confirmed")
+            msg = _("Your account is already confirmed.")
         messages.add_message(
             request, messages.SUCCESS,
             message=msg,
             extra_tags="success"
         )
 
         return redirect("classic_index")
@@ -362,28 +372,28 @@
 
             # user existence is checked by the form validation #
 
             if user.is_confirmed:
                 messages.add_message(
                     request, messages.INFO,
                     message=(_(
-                        "Your account is already confirmed, "
-                        "no email has been sent."
+                        "Your account is already confirmed. "
+                        "No email has been sent."
                         )),
                     extra_tags="info"
                 )
                 return redirect("classic_login")
 
             send_confirm_email(request, user)
 
             messages.add_message(
                 request, messages.INFO,
                 message=(_(
                     "Please check your inbox "
-                    "to confirm your account"
+                    "to confirm your account."
                     )),
                 extra_tags="info"
             )
         else:
             context = {
                 "form": form,
                 "base_template": conf["BASE_TEMPLATE"],
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/views/silly_views.py` & `django-silly-auth-1.0.1/django_silly_auth/views/silly_views.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,45 +13,45 @@
 User = get_user_model()
 
 
 @transaction.atomic
 def silly_confirm_email(request, token):
     user = User.verify_jwt_token(token)
     if user is None:
-        msg = _("Invalid or expired token"),
+        msg = _("Token invalid or expired"),
         tag = "danger"
     if user is not None and user.is_active:
         if not user.is_confirmed:
             user.is_confirmed = True
             user.new_email = None
-            msg = _("Your account have been confirmed")
+            msg = _("Your account has been confirmed")
             tag = "success"
             user.save()
         elif user.new_email:
             user.email = user.new_email
             user.new_email = None
-            msg = _("Your new email have been confirmed")
+            msg = _("Your new email has been confirmed")
             tag = "success"
             user.save()
         else:
-            msg = _("Your account is already confirmed")
+            msg = _("Your account has already been confirmed.")
             tag = "warning"
 
     context = {
         "base_template": conf["BASE_TEMPLATE"],
         "message": msg,
         "tag": tag,
         "link": conf["SILLY_LINK_TO_SPA"],
         "site_name": conf["SITE_NAME"],
     }
     return render(request, 'silly_auth/silly/silly_confirm_email.html', context)
 
 
 def silly_password_reset_done(request):
-    msg = _("Your password has been reset")
+    msg = _("Your password has been successfully reset.")
     context = {
         "base_template": conf["BASE_TEMPLATE"],
         "message": msg,
         "tag": "success",
         "link": conf["SILLY_LINK_TO_SPA"],
         "site_name": conf["SITE_NAME"],
     }
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth/views/test_views.py` & `django-silly-auth-1.0.1/django_silly_auth/views/test_views.py`

 * *Files identical despite different names*

### Comparing `django-silly-auth-1.0.0/django_silly_auth.egg-info/PKG-INFO` & `django-silly-auth-1.0.1/django_silly_auth.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-silly-auth
-Version: 1.0.0
+Version: 1.0.1
 Summary: Authentication package for Django and DRF
 Home-page: https://github.com/byoso/django_silly_auth
 Author: Vincent Fabre
 Author-email: peigne.plume@gmail.com
 License: MIT
 Keywords: django auth drf jwt
 Platform: UNKNOWN
@@ -37,7 +37,11 @@
 # [WIKI documentation](https://github.com/byoso/django_silly_auth/wiki)
 
 ## [Read this FIRST](https://github.com/byoso/django_silly_auth/wiki/Must-read-this-few-lines-!)
 
 ### :coffee: [If you find this package usefull, consider buying me a coffee](https://www.buymeacoffee.com/byoso)
 
 
+### Changelog
+- 1.0.1: i18n fr + en
+
+
```

### Comparing `django-silly-auth-1.0.0/django_silly_auth.egg-info/SOURCES.txt` & `django-silly-auth-1.0.1/django_silly_auth.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,18 @@
 django_silly_auth/urls.py
 django_silly_auth/utils.py
 django_silly_auth.egg-info/PKG-INFO
 django_silly_auth.egg-info/SOURCES.txt
 django_silly_auth.egg-info/dependency_links.txt
 django_silly_auth.egg-info/requires.txt
 django_silly_auth.egg-info/top_level.txt
+django_silly_auth/locale/django.pot
+django_silly_auth/locale/en/LC_MESSAGES/django.po
+django_silly_auth/locale/fr/LC_MESSAGES/django.mo
+django_silly_auth/locale/fr/LC_MESSAGES/django.po
 django_silly_auth/templates/__init__.py
 django_silly_auth/templates/silly_auth/__init__.py
 django_silly_auth/templates/silly_auth/_base.html
 django_silly_auth/templates/silly_auth/_test/__init__.py
 django_silly_auth/templates/silly_auth/_test/_base.html
 django_silly_auth/templates/silly_auth/_test/_test.html
 django_silly_auth/templates/silly_auth/_test/_users.html
```

### Comparing `django-silly-auth-1.0.0/setup.py` & `django-silly-auth-1.0.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -49,17 +49,22 @@
         "django_silly_auth.templates",
         "django_silly_auth.templates.silly_auth",
         "django_silly_auth.templates.silly_auth._test",
         "django_silly_auth.templates.silly_auth.classic",
         "django_silly_auth.templates.silly_auth.emails",
         "django_silly_auth.templates.silly_auth.silly",
         "django_silly_auth.views",
+        "django_silly_auth.locale",
+        "django_silly_auth.locale.fr",
+        "django_silly_auth.locale.fr.LC_MESSAGES",
+        "django_silly_auth.locale.en",
+        "django_silly_auth.locale.en.LC_MESSAGES",
         ],
     # include_package_data=True,
-    package_data={'': ['*.txt', '*.html']},
+    package_data={'': ['*.txt', '*.html', '*.po', '*.mo', '*.pot']},
     python_requires='>=3.7',
     install_requires=[
         "pyjwt >= 2.6.0",
     ],
     keywords='django auth drf jwt',
     # entry_points={
     #     "console_scripts": [
```

