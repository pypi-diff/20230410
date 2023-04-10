# Comparing `tmp/XBXBOT-1.0.3-py3-none-any.whl.zip` & `tmp/XBXBOT-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 14013 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    67859 b- defN 23-Apr-02 20:16 XBXBOT/__init__.py
--rw-rw-rw-  2.0 fat      849 b- defN 23-Apr-02 20:18 XBXBOT-1.0.3.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-02 20:18 XBXBOT-1.0.3.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-02 20:18 XBXBOT-1.0.3.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      368 b- defN 23-Apr-02 20:18 XBXBOT-1.0.3.dist-info/RECORD
-5 files, 69175 bytes uncompressed, 13327 bytes compressed:  80.7%
+Zip file size: 14045 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    67988 b- defN 23-Apr-10 12:34 XBXBOT/__init__.py
+-rw-rw-rw-  2.0 fat      849 b- defN 23-Apr-10 12:37 XBXBOT-1.0.4.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-10 12:37 XBXBOT-1.0.4.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-10 12:37 XBXBOT-1.0.4.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      368 b- defN 23-Apr-10 12:37 XBXBOT-1.0.4.dist-info/RECORD
+5 files, 69304 bytes uncompressed, 13359 bytes compressed:  80.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: XBXBOT/__init__.py
 Comment: 
 
-Filename: XBXBOT-1.0.3.dist-info/METADATA
+Filename: XBXBOT-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: XBXBOT-1.0.3.dist-info/WHEEL
+Filename: XBXBOT-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: XBXBOT-1.0.3.dist-info/top_level.txt
+Filename: XBXBOT-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: XBXBOT-1.0.3.dist-info/RECORD
+Filename: XBXBOT-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## XBXBOT/__init__.py

```diff
@@ -16,31 +16,35 @@
 
     # Third party imports.
     from fortnitepy.ext import commands
     from colorama import Fore, Back, Style, init
     init(autoreset=True)
     from functools import partial
 
+    #time import 
     from datetime import timedelta
+
+    os.system("pip uninstall fortnitepy --y")
     os.system("pip install git+https://github.com/juanfnde/fortnitepyfix")
+
     import crayons
     try:
         import PirxcyPinger
     except:
         pass
     import fortnitepy
     import FortniteAPIAsync
     import sanic
     import aiohttp
     import uvloop
     import requests
 
 except ModuleNotFoundError as e:
     print(f'Error: {e}\nAttempting to install packages now.')
-
+    #'fortnitepy==3.6.8',
     for module in (
         'crayons',
         'PirxcyPinger',
         'FortniteAPIAsync',
         'sanic==21.6.2',
         'aiohttp',
         'requests'
@@ -50,29 +54,29 @@
     os.system('clear')
 
     print('Installed packages, restarting script.')
 
     python = sys.executable
     os.execl(python, python, *sys.argv)
 
-
+os.system('clear')
 print(crayons.blue(f'Mathyslolbots by Mathyslol, Cousin & helped by Pirxcy.'))
 print(crayons.magenta(f'Discord server: https://discord.gg/EFZj6SdYzk - For support, questions, etc.'))
 
 
 sanic_app = sanic.Sanic(__name__)
 server = None
 
 cid = ""
 name = ""
 friendlist = ""
 
 password = "9678"
 copied_player = ""
-__version__ = "1.5"
+__version__ = "3.0"
 adminsss = 'MathyslolFN'
 owner = '097271eaeea9430a9e8e1ebe92a65b6b'
 errordiff = 'errors.com.epicgames.common.throttled', 'errors.com.epicgames.friends.inviter_friendships_limit_exceeded'
 
 shit_partys_errrors = 'errors.com.epicgames.social.party.invite_already_exists', 'errors.com.epicgames.social.party.party_not_found', 'errors.com.epicgames.social.party.stale_revision', 'errors.com.epicgames.social.party.party_change_forbidden', 'errors.com.epicgames.social.party.invite_forbidden'#HTTPexception (soon...)fix error like party invalid etc
 
 
@@ -637,16 +641,16 @@
 
           
           if not self.remove_bots_check == self.remove_bots:
               self.remove_bots = self.remove_bots_check
                       
           if not self.status_verif == self.status:
               self.status = self.status_verif
-
-              await self.set_presence(self.status)
+               
+              #await self.set_presence(self.status)
               try:
                 await self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC)
               except:
                 pass
 
           if not self.adminsss == adminsss:
               adminsss = self.adminsss
```

### html2text {}

```diff
@@ -1,26 +1,27 @@
 try: # System imports. from typing import Tuple, Any, Union, Optional import
 asyncio import sys import datetime import json import functools import os
 import random as py_random import logging import uuid import json import
 subprocess # Third party imports. from fortnitepy.ext import commands from
 colorama import Fore, Back, Style, init init(autoreset=True) from functools
-import partial from datetime import timedelta os.system("pip install git+https:
-//github.com/juanfnde/fortnitepyfix") import crayons try: import PirxcyPinger
-except: pass import fortnitepy import FortniteAPIAsync import sanic import
-aiohttp import uvloop import requests except ModuleNotFoundError as e: print
-(f'Error: {e}\nAttempting to install packages now.') for module in ( 'crayons',
-'PirxcyPinger', 'FortniteAPIAsync', 'sanic==21.6.2', 'aiohttp', 'requests' ):
-subprocess.check_call([sys.executable, "-m", "pip", "install", module])
-os.system('clear') print('Installed packages, restarting script.') python =
-sys.executable os.execl(python, python, *sys.argv) print(crayons.blue
-(f'Mathyslolbots by Mathyslol, Cousin & helped by Pirxcy.')) print
-(crayons.magenta(f'Discord server: https://discord.gg/EFZj6SdYzk - For support,
-questions, etc.')) sanic_app = sanic.Sanic(__name__) server = None cid = ""
-name = "" friendlist = "" password = "9678" copied_player = "" __version__ =
-"1.5" adminsss = 'MathyslolFN' owner = '097271eaeea9430a9e8e1ebe92a65b6b'
+import partial #time import from datetime import timedelta os.system("pip
+uninstall fortnitepy --y") os.system("pip install git+https://github.com/
+juanfnde/fortnitepyfix") import crayons try: import PirxcyPinger except: pass
+import fortnitepy import FortniteAPIAsync import sanic import aiohttp import
+uvloop import requests except ModuleNotFoundError as e: print(f'Error:
+{e}\nAttempting to install packages now.') #'fortnitepy==3.6.8', for module in
+( 'crayons', 'PirxcyPinger', 'FortniteAPIAsync', 'sanic==21.6.2', 'aiohttp',
+'requests' ): subprocess.check_call([sys.executable, "-m", "pip", "install",
+module]) os.system('clear') print('Installed packages, restarting script.')
+python = sys.executable os.execl(python, python, *sys.argv) os.system('clear')
+print(crayons.blue(f'Mathyslolbots by Mathyslol, Cousin & helped by Pirxcy.'))
+print(crayons.magenta(f'Discord server: https://discord.gg/EFZj6SdYzk - For
+support, questions, etc.')) sanic_app = sanic.Sanic(__name__) server = None cid
+= "" name = "" friendlist = "" password = "9678" copied_player = "" __version__
+= "3.0" adminsss = 'MathyslolFN' owner = '097271eaeea9430a9e8e1ebe92a65b6b'
 errordiff = 'errors.com.epicgames.common.throttled',
 'errors.com.epicgames.friends.inviter_friendships_limit_exceeded'
 shit_partys_errrors =
 'errors.com.epicgames.social.party.invite_already_exists',
 'errors.com.epicgames.social.party.party_not_found',
 'errors.com.epicgames.social.party.stale_revision',
 'errors.com.epicgames.social.party.party_change_forbidden',
@@ -202,15 +203,15 @@
 ['inv_all'] self.join_msg_check = z['join_msg'] self.vips_check = z['admin']
 self.versiongame = z['version_web'] self.inv_bl = z['bl_inv'] self.inv_on_check
 = z['inv_on'] self.number_check = z['style'] self.adminsss = z['admin']
 self.status_verif = z['status'] self.uptimerobot_key_check = z
 ['uptimerobot_apikey'] self.remove_bots_check = z['remove_bots'] if not
 self.remove_bots_check == self.remove_bots: self.remove_bots =
 self.remove_bots_check if not self.status_verif == self.status: self.status =
-self.status_verif await self.set_presence(self.status) try: await
+self.status_verif #await self.set_presence(self.status) try: await
 self.party.set_privacy(fortnitepy.PartyPrivacy.PUBLIC) except: pass if not
 self.adminsss == adminsss: adminsss = self.adminsss if not
 self.uptimerobot_key_check == self.uptimerobot_key: self.uptimerobot_key =
 self.uptimerobot_key_check if not self.number_check == self.number: self.number
 = self.number_check try: await self.party.me.set_outfit
 (asset=self.skin,variants=self.party.me.create_variants
 (material=self.number,clothing_color=self.number,parts=self.number,progressive=self.number))
```

## Comparing `XBXBOT-1.0.3.dist-info/METADATA` & `XBXBOT-1.0.4.dist-info/METADATA`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: XBXBOT
-Version: 1.0.3
+Version: 1.0.4
 Summary: The Best Fortnite LOBBYBOT with the latest features
 Home-page: https://www.youtube.com/
 Author: Mathyslol
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

