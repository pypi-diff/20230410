# Comparing `tmp/thompcoutils-2.0.8.tar.gz` & `tmp/thompcoutils-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thompcoutils-2.0.8.tar", last modified: Sat Dec 11 17:23:05 2021, max compression
+gzip compressed data, was "thompcoutils-2.0.9.tar", last modified: Wed Feb 23 01:54:48 2022, max compression
```

## Comparing `thompcoutils-2.0.8.tar` & `thompcoutils-2.0.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0 jrt       (1000) jrt       (1000)        0 2021-12-11 17:23:05.355543 thompcoutils-2.0.8/
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     5357 2021-12-11 17:23:05.355543 thompcoutils-2.0.8/PKG-INFO
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     4095 2021-02-22 00:09:50.000000 thompcoutils-2.0.8/README.md
-drwxrwxrwx   0 jrt       (1000) jrt       (1000)        0 2021-12-11 17:23:03.604827 thompcoutils-2.0.8/Tests/
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)        0 2021-02-22 00:09:50.000000 thompcoutils-2.0.8/Tests/__init__.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)    11156 2021-11-03 05:17:02.000000 thompcoutils-2.0.8/Tests/test_config_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     6038 2021-02-22 00:09:50.000000 thompcoutils-2.0.8/Tests/test_pio.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     3924 2021-02-22 00:09:50.000000 thompcoutils-2.0.8/Tests/test_threadutils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     2245 2021-02-22 00:09:50.000000 thompcoutils-2.0.8/Tests/test_time_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)       38 2021-12-11 17:23:05.355543 thompcoutils-2.0.8/setup.cfg
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)      832 2021-10-19 14:48:47.000000 thompcoutils-2.0.8/setup.py
-drwxrwxrwx   0 jrt       (1000) jrt       (1000)        0 2021-12-11 17:23:05.284933 thompcoutils-2.0.8/thompcoutils/
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)        0 2021-02-22 00:09:50.000000 thompcoutils-2.0.8/thompcoutils/__init__.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     2887 2021-11-05 00:23:02.000000 thompcoutils-2.0.8/thompcoutils/cell_phone.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)    23894 2021-11-04 07:03:36.000000 thompcoutils-2.0.8/thompcoutils/config_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     4149 2021-02-22 00:09:50.000000 thompcoutils-2.0.8/thompcoutils/cron_time.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)    10605 2021-04-19 20:16:51.000000 thompcoutils-2.0.8/thompcoutils/db_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     8108 2021-11-06 01:52:49.000000 thompcoutils-2.0.8/thompcoutils/email_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     4479 2021-02-22 00:09:50.000000 thompcoutils-2.0.8/thompcoutils/file_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)    11104 2021-02-22 00:09:50.000000 thompcoutils-2.0.8/thompcoutils/html_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     5614 2021-11-01 21:54:47.000000 thompcoutils-2.0.8/thompcoutils/log_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     1080 2021-12-09 18:18:12.000000 thompcoutils-2.0.8/thompcoutils/math_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     4275 2021-06-12 22:21:28.000000 thompcoutils-2.0.8/thompcoutils/os_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)    35922 2021-12-11 17:22:21.000000 thompcoutils-2.0.8/thompcoutils/pio.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)       39 2021-02-22 00:09:50.000000 thompcoutils-2.0.8/thompcoutils/pio_exception.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     1719 2021-02-22 00:09:50.000000 thompcoutils-2.0.8/thompcoutils/security_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)        0 2021-02-22 00:09:50.000000 thompcoutils-2.0.8/thompcoutils/setup.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     2273 2021-12-08 21:09:53.000000 thompcoutils-2.0.8/thompcoutils/string_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     2774 2021-02-22 00:09:50.000000 thompcoutils-2.0.8/thompcoutils/test_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     4264 2021-11-30 04:22:07.000000 thompcoutils-2.0.8/thompcoutils/threading_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     3206 2021-12-10 18:14:18.000000 thompcoutils-2.0.8/thompcoutils/time_utils.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)      261 2021-02-22 00:09:50.000000 thompcoutils-2.0.8/thompcoutils/units.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)       18 2021-12-11 17:23:02.000000 thompcoutils-2.0.8/thompcoutils/version.py
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     5398 2021-12-08 21:09:53.000000 thompcoutils-2.0.8/thompcoutils/web_utils.py
-drwxrwxrwx   0 jrt       (1000) jrt       (1000)        0 2021-12-11 17:23:05.339918 thompcoutils-2.0.8/thompcoutils.egg-info/
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)     5357 2021-12-11 17:23:03.000000 thompcoutils-2.0.8/thompcoutils.egg-info/PKG-INFO
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)      893 2021-12-11 17:23:03.000000 thompcoutils-2.0.8/thompcoutils.egg-info/SOURCES.txt
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)        1 2021-12-11 17:23:03.000000 thompcoutils-2.0.8/thompcoutils.egg-info/dependency_links.txt
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)       33 2021-12-11 17:23:03.000000 thompcoutils-2.0.8/thompcoutils.egg-info/requires.txt
--rwxrwxrwx   0 jrt       (1000) jrt       (1000)       19 2021-12-11 17:23:03.000000 thompcoutils-2.0.8/thompcoutils.egg-info/top_level.txt
+drwxrwxrwx   0 jrt       (1000) jrt       (1000)        0 2022-02-23 01:54:48.982676 thompcoutils-2.0.9/
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     5357 2022-02-23 01:54:48.971346 thompcoutils-2.0.9/PKG-INFO
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     4095 2021-02-22 00:09:50.000000 thompcoutils-2.0.9/README.md
+drwxrwxrwx   0 jrt       (1000) jrt       (1000)        0 2022-02-23 01:54:48.647439 thompcoutils-2.0.9/Tests/
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)        0 2021-02-22 00:09:50.000000 thompcoutils-2.0.9/Tests/__init__.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)    11156 2021-11-03 05:17:02.000000 thompcoutils-2.0.9/Tests/test_config_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     6038 2021-02-22 00:09:50.000000 thompcoutils-2.0.9/Tests/test_pio.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     3924 2021-02-22 00:09:50.000000 thompcoutils-2.0.9/Tests/test_threadutils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     2245 2021-02-22 00:09:50.000000 thompcoutils-2.0.9/Tests/test_time_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)       38 2022-02-23 01:54:48.982676 thompcoutils-2.0.9/setup.cfg
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)      832 2021-10-19 14:48:47.000000 thompcoutils-2.0.9/setup.py
+drwxrwxrwx   0 jrt       (1000) jrt       (1000)        0 2022-02-23 01:54:48.913715 thompcoutils-2.0.9/thompcoutils/
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)        0 2021-02-22 00:09:50.000000 thompcoutils-2.0.9/thompcoutils/__init__.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     2887 2021-11-05 00:23:02.000000 thompcoutils-2.0.9/thompcoutils/cell_phone.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)    23894 2021-12-18 17:34:56.000000 thompcoutils-2.0.9/thompcoutils/config_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     4149 2021-02-22 00:09:50.000000 thompcoutils-2.0.9/thompcoutils/cron_time.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)    10605 2021-04-19 20:16:51.000000 thompcoutils-2.0.9/thompcoutils/db_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     8108 2021-11-06 01:52:49.000000 thompcoutils-2.0.9/thompcoutils/email_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     4479 2021-02-22 00:09:50.000000 thompcoutils-2.0.9/thompcoutils/file_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)    11104 2021-02-22 00:09:50.000000 thompcoutils-2.0.9/thompcoutils/html_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     5614 2021-11-01 21:54:47.000000 thompcoutils-2.0.9/thompcoutils/log_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     1080 2021-12-09 18:18:12.000000 thompcoutils-2.0.9/thompcoutils/math_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     4275 2021-06-12 22:21:28.000000 thompcoutils-2.0.9/thompcoutils/os_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)    35922 2021-12-11 17:22:21.000000 thompcoutils-2.0.9/thompcoutils/pio.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)       39 2021-02-22 00:09:50.000000 thompcoutils-2.0.9/thompcoutils/pio_exception.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     1719 2021-02-22 00:09:50.000000 thompcoutils-2.0.9/thompcoutils/security_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)        0 2021-02-22 00:09:50.000000 thompcoutils-2.0.9/thompcoutils/setup.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     2273 2021-12-08 21:09:53.000000 thompcoutils-2.0.9/thompcoutils/string_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     2774 2021-02-22 00:09:50.000000 thompcoutils-2.0.9/thompcoutils/test_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     4264 2021-11-30 04:22:07.000000 thompcoutils-2.0.9/thompcoutils/threading_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     3123 2022-02-23 01:53:04.000000 thompcoutils-2.0.9/thompcoutils/time_utils.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)      261 2021-02-22 00:09:50.000000 thompcoutils-2.0.9/thompcoutils/units.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)       18 2022-02-23 01:54:47.000000 thompcoutils-2.0.9/thompcoutils/version.py
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     5398 2021-12-08 21:09:53.000000 thompcoutils-2.0.9/thompcoutils/web_utils.py
+drwxrwxrwx   0 jrt       (1000) jrt       (1000)        0 2022-02-23 01:54:48.960475 thompcoutils-2.0.9/thompcoutils.egg-info/
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)     5357 2022-02-23 01:54:48.000000 thompcoutils-2.0.9/thompcoutils.egg-info/PKG-INFO
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)      893 2022-02-23 01:54:48.000000 thompcoutils-2.0.9/thompcoutils.egg-info/SOURCES.txt
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)        1 2022-02-23 01:54:48.000000 thompcoutils-2.0.9/thompcoutils.egg-info/dependency_links.txt
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)       33 2022-02-23 01:54:48.000000 thompcoutils-2.0.9/thompcoutils.egg-info/requires.txt
+-rwxrwxrwx   0 jrt       (1000) jrt       (1000)       19 2022-02-23 01:54:48.000000 thompcoutils-2.0.9/thompcoutils.egg-info/top_level.txt
```

### Comparing `thompcoutils-2.0.8/PKG-INFO` & `thompcoutils-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thompcoutils
-Version: 2.0.8
+Version: 2.0.9
 Summary: Another collection of utilities
 Home-page: https://github.com/pypa/sampleproject
 Author: Jordan Thompson
 Author-email: Jordan@ThompCo.com
 License: UNKNOWN
 Description: # logging_utils
         logging consists of the following classes and functions to help with the burden of logging
```

### Comparing `thompcoutils-2.0.8/README.md` & `thompcoutils-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/Tests/test_config_utils.py` & `thompcoutils-2.0.9/Tests/test_config_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/Tests/test_pio.py` & `thompcoutils-2.0.9/Tests/test_pio.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/Tests/test_threadutils.py` & `thompcoutils-2.0.9/Tests/test_threadutils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/Tests/test_time_utils.py` & `thompcoutils-2.0.9/Tests/test_time_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/setup.py` & `thompcoutils-2.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/cell_phone.py` & `thompcoutils-2.0.9/thompcoutils/cell_phone.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/config_utils.py` & `thompcoutils-2.0.9/thompcoutils/config_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/cron_time.py` & `thompcoutils-2.0.9/thompcoutils/cron_time.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/db_utils.py` & `thompcoutils-2.0.9/thompcoutils/db_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/email_utils.py` & `thompcoutils-2.0.9/thompcoutils/email_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/file_utils.py` & `thompcoutils-2.0.9/thompcoutils/file_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/html_utils.py` & `thompcoutils-2.0.9/thompcoutils/html_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/log_utils.py` & `thompcoutils-2.0.9/thompcoutils/log_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/math_utils.py` & `thompcoutils-2.0.9/thompcoutils/math_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/os_utils.py` & `thompcoutils-2.0.9/thompcoutils/os_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/pio.py` & `thompcoutils-2.0.9/thompcoutils/pio.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/security_utils.py` & `thompcoutils-2.0.9/thompcoutils/security_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/string_utils.py` & `thompcoutils-2.0.9/thompcoutils/string_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/test_utils.py` & `thompcoutils-2.0.9/thompcoutils/test_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/threading_utils.py` & `thompcoutils-2.0.9/thompcoutils/threading_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils/time_utils.py` & `thompcoutils-2.0.9/thompcoutils/time_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import datetime
 import calendar
+from typing import Optional
+
 from dateutil.relativedelta import relativedelta, TH, MO
 
 
 class Holiday(datetime.datetime):
     THANKSGIVING = "thanksgiving"
     CHRISTMAS = "christmas"
     NEW_YEARS = "newyears"
@@ -42,41 +44,45 @@
         return super().__new__(cls, year=year, month=month, day=day)
 
 
 def is_weekend(dt):
     return dt.weekday() >= 5
 
 
-def time_diff_to_str(diff, short=False, show_seconds=False):
+def time_diff_to_str(td: Optional['datetime.timedelta'], format):  # short=False, show_seconds=False):
     """
     Converts the difference to a string
-    :param diff: the time difference to convert
-    :param short: represent it as #d #h #m #s as opposed to # days # hours # minutes # seconds
-    :param show_seconds: show the string including seconds (note if diff < 1 minute, seconds will be diplayed
+    :param td: the time difference to convert
+    :param format: format to display
     :return: the time difference as a string
+
+%d	08	Day of the month as a zero-padded decimal number.
+%D	8	Day of the month as a decimal number.
+%H	07	Hour (24-hour clock) as a zero-padded decimal number.
+%h	07	Hour (24-hour clock) as a decimal number.
+%M	06	Minute as a zero-padded decimal number.
+%m	06	Minute as a decimal number.
+%S	05	Second as a zero-padded decimal number.
+%s	05	Second as a decimal number.
     """
     days, remainder = divmod(diff.total_seconds(), 86400)
     hours, remainder = divmod(remainder, 3600)
     minutes, seconds = divmod(remainder, 60)
     days = int(days)
     hours = int(hours)
     minutes = int(minutes)
     seconds = int(seconds)
-    rtn = ''
-
-    if days > 0:
-        rtn += '{}{}{} '.format(days, 'd' if short else ' day', 's' if days > 1 and not short else '')
-    if hours > 0:
-        rtn += '{}{}{} '.format(hours, 'h' if short else ' hour', 's' if minutes > 1 and not short else '')
-    if minutes > 0:
-        rtn += '{}{}{} '.format(minutes, 'm' if short else ' minute', 's' if minutes > 1 and not short else '')
-    if show_seconds or days == 0 and hours == 0 and minutes == 0 and seconds > 0:
-        rtn += '{}{}{} '.format(seconds, 's' if short else ' second', 's' if seconds > 1 and not short else '')
-    return rtn
+    return format.\
+        replace('%H', '{:02d}'.format(hours)). \
+        replace('%h', '{}'.format(hours)). \
+        replace('%M', '{:02d}'.format(minutes)). \
+        replace('%m', '{}'.format(minutes)). \
+        replace('%S', '{:02d}'.format(seconds)). \
+        replace('%s', '{}'.format(seconds)). \
+        replace('%d', '{:02d}'.format(days)). \
+        replace('%D', '{}'.format(days))
 
 
 if __name__ == "__main__":
-    diff = datetime.timedelta(seconds=1, minutes=2, hours=16, days=0)
-    print(time_diff_to_str(diff, short=True, show_seconds=True))
-    print(time_diff_to_str(diff, short=True, show_seconds=False))
-    print(time_diff_to_str(diff, short=False, show_seconds=True))
-    print(time_diff_to_str(diff, short=False, show_seconds=False))
+    diff = datetime.timedelta(seconds=1, minutes=2, hours=16, days=5)
+    print(time_diff_to_str(diff, '%d days %H:%M:%S'))
+    print(time_diff_to_str(diff, '%D days %h:%m:%s'))
```

### Comparing `thompcoutils-2.0.8/thompcoutils/web_utils.py` & `thompcoutils-2.0.9/thompcoutils/web_utils.py`

 * *Files identical despite different names*

### Comparing `thompcoutils-2.0.8/thompcoutils.egg-info/PKG-INFO` & `thompcoutils-2.0.9/thompcoutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thompcoutils
-Version: 2.0.8
+Version: 2.0.9
 Summary: Another collection of utilities
 Home-page: https://github.com/pypa/sampleproject
 Author: Jordan Thompson
 Author-email: Jordan@ThompCo.com
 License: UNKNOWN
 Description: # logging_utils
         logging consists of the following classes and functions to help with the burden of logging
```

### Comparing `thompcoutils-2.0.8/thompcoutils.egg-info/SOURCES.txt` & `thompcoutils-2.0.9/thompcoutils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

