# Comparing `tmp/pyvosklivesubtitle-0.1.0.tar.gz` & `tmp/pyvosklivesubtitle-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvosklivesubtitle-0.1.0.tar", last modified: Sun Apr  9 20:39:17 2023, max compression
+gzip compressed data, was "pyvosklivesubtitle-0.1.1.tar", last modified: Mon Apr 10 01:10:39 2023, max compression
```

## Comparing `pyvosklivesubtitle-0.1.0.tar` & `pyvosklivesubtitle-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 20:39:17.800402 pyvosklivesubtitle-0.1.0/
--rw-rw-rw-   0        0        0     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1617 2023-04-09 20:39:17.800402 pyvosklivesubtitle-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     4177 2022-11-06 07:43:14.000000 pyvosklivesubtitle-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-09 20:39:17.769683 pyvosklivesubtitle-0.1.0/pyvosklivesubtitle/
--rw-rw-rw-   0        0        0    90084 2023-04-09 20:22:54.000000 pyvosklivesubtitle-0.1.0/pyvosklivesubtitle/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 20:39:17.797406 pyvosklivesubtitle-0.1.0/pyvosklivesubtitle.egg-info/
--rw-rw-rw-   0        0        0     1617 2023-04-09 20:39:17.000000 pyvosklivesubtitle-0.1.0/pyvosklivesubtitle.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-04-09 20:39:17.000000 pyvosklivesubtitle-0.1.0/pyvosklivesubtitle.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 20:39:17.000000 pyvosklivesubtitle-0.1.0/pyvosklivesubtitle.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       63 2023-04-09 20:39:17.000000 pyvosklivesubtitle-0.1.0/pyvosklivesubtitle.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      109 2023-04-09 20:39:17.000000 pyvosklivesubtitle-0.1.0/pyvosklivesubtitle.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-09 20:39:17.000000 pyvosklivesubtitle-0.1.0/pyvosklivesubtitle.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-04-09 20:39:17.803398 pyvosklivesubtitle-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1556 2023-04-04 14:45:01.000000 pyvosklivesubtitle-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:10:38.985176 pyvosklivesubtitle-0.1.1/
+-rw-rw-rw-   0        0        0     1088 2022-11-03 03:32:17.000000 pyvosklivesubtitle-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0       34 2022-06-05 08:17:08.000000 pyvosklivesubtitle-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1617 2023-04-10 01:10:38.985925 pyvosklivesubtitle-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4177 2022-11-06 07:43:14.000000 pyvosklivesubtitle-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 01:10:38.966446 pyvosklivesubtitle-0.1.1/pyvosklivesubtitle/
+-rw-rw-rw-   0        0        0    90085 2023-04-10 00:42:57.000000 pyvosklivesubtitle-0.1.1/pyvosklivesubtitle/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 01:10:38.982926 pyvosklivesubtitle-0.1.1/pyvosklivesubtitle.egg-info/
+-rw-rw-rw-   0        0        0     1617 2023-04-10 01:10:38.000000 pyvosklivesubtitle-0.1.1/pyvosklivesubtitle.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      333 2023-04-10 01:10:38.000000 pyvosklivesubtitle-0.1.1/pyvosklivesubtitle.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 01:10:38.000000 pyvosklivesubtitle-0.1.1/pyvosklivesubtitle.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       63 2023-04-10 01:10:38.000000 pyvosklivesubtitle-0.1.1/pyvosklivesubtitle.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      109 2023-04-10 01:10:38.000000 pyvosklivesubtitle-0.1.1/pyvosklivesubtitle.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-04-10 01:10:38.000000 pyvosklivesubtitle-0.1.1/pyvosklivesubtitle.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-04-10 01:10:38.988171 pyvosklivesubtitle-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1556 2023-04-10 01:03:12.000000 pyvosklivesubtitle-0.1.1/setup.py
```

### Comparing `pyvosklivesubtitle-0.1.0/LICENSE` & `pyvosklivesubtitle-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.1.0/PKG-INFO` & `pyvosklivesubtitle-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvosklivesubtitle
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
 Home-page: https://github.com/botbahlul/pyvosklivesubtitle
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 Bot Bahlul
```

### Comparing `pyvosklivesubtitle-0.1.0/README.md` & `pyvosklivesubtitle-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pyvosklivesubtitle-0.1.0/pyvosklivesubtitle/__init__.py` & `pyvosklivesubtitle-0.1.1/pyvosklivesubtitle/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1366,15 +1366,15 @@
     multiline_height = int(0.0125*main_window_height)
     FONT_TYPE = "Helvetica"
     FONT_SIZE = 9
     sg.set_options(font=(FONT_TYPE, FONT_SIZE))
 
     layout = [[sg.Frame('Hints',[
                                 [sg.Text('Click \"Start\" button to start listening and printing subtitles on screen.', expand_x=True, expand_y=True)],
-                                [sg.Text('Check the \"Record Streaming\" checkbox and paste the streaming URL into URL inputbox to record the streaming.', expand_x=True, expand_y=True)],
+                                [sg.Text('Paste the streaming URL into URL inputbox then check the \"Record Streaming\" checkbox to record the streaming.', expand_x=True, expand_y=True)],
                                 [sg.Text('If you record the streaming, when you save transcriptions, all timestamps will be relative to the \"Start\" button clicked time.', expand_x=True, expand_y=True)],
                                 [sg.Text('If you don\'t record the streaming, all timestamps will be based on your system clock.', expand_x=True, expand_y=True)],
                                 [sg.Text('If you need accurate subtitles sync for the video, please use PyAutoSRT (https://github.com/botbahlul/PyAutoSRT) ', expand_x=True, expand_y=True, enable_events=True)],
                                 ], border_width=2, expand_x=True, expand_y=True)],
               [sg.Text('URL'), sg.Input(size=(12, 1), expand_x=True, expand_y=True, key='-URL-'),
                sg.Checkbox("Record Streaming", key='-RECORD-STREAMING-', enable_events=True)],
               [sg.Text('', size=(3, 1)),
@@ -1497,15 +1497,15 @@
         parser.exit(0)
 
     parser = argparse.ArgumentParser(description=__doc__, formatter_class=argparse.RawDescriptionHelpFormatter, parents=[parser])
 
     parser.add_argument("-af", "--audio-filename", type=str, metavar="AUDIO_FILENAME", help="audio file to store recording to")
     parser.add_argument("-d", "--device", type=int_or_str, help="input device (numeric ID or substring)")
     parser.add_argument("-r", "--samplerate", type=int, help="sampling rate in Hertz for example 8000, 16000, 44100, or 48000")
-    parser.add_argument('-v', '--version', action='version', version='0.1.0')
+    parser.add_argument('-v', '--version', action='version', version='0.1.1')
 
     parser.add_argument("-u", "--url", type=str, metavar="URL", help="URL of live streaming if you want to record the streaming")
     parser.add_argument("-vf", "--video-filename", type=str, metavar="VIDEO_FILENAME", help="video file to store recording to", default=None)
 
     args = parser.parse_args(remaining)
     args = parser.parse_args()
```

### Comparing `pyvosklivesubtitle-0.1.0/pyvosklivesubtitle.egg-info/PKG-INFO` & `pyvosklivesubtitle-0.1.1/pyvosklivesubtitle.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvosklivesubtitle
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES
 Home-page: https://github.com/botbahlul/pyvosklivesubtitle
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 Bot Bahlul
```

### Comparing `pyvosklivesubtitle-0.1.0/setup.py` & `pyvosklivesubtitle-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     'pyvosklivesubtitle is a python based desktop aplication which can recognize any live streaming'
     'in 21 languages that supported by VOSK then translate and display it as LIVE SUBTITLES'
     )
 
 setup(
     name="pyvosklivesubtitle",
     description="A Python based desktop aplication that can RECOGNIZE any live streaming in 21 languages that supported by VOSK then TRANSLATE and display it as LIVE SUBTITLES",
-    version="0.1.0",
+    version="0.1.1",
     include_package_data=True,
     author='Bot Bahlul',
     author_email='bot.bahlul@gmail.com',
     url='https://github.com/botbahlul/pyvosklivesubtitle',
     packages=[str('pyvosklivesubtitle')],
     entry_points={
         'console_scripts': [
```

