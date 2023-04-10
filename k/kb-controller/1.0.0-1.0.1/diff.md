# Comparing `tmp/kb_controller-1.0.0.tar.gz` & `tmp/kb_controller-1.0.1.tar.gz`

## Comparing `kb_controller-1.0.0.tar` & `kb_controller-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kb_controller-1.0.0/setup.py
--rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 kb_controller-1.0.0/start.sh
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 kb_controller-1.0.0/.vscode/launch.json
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 kb_controller-1.0.0/src/kb_controller/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kb_controller-1.0.0/src/kb_controller/__init__.py
--rw-r--r--   0        0        0     8823 2020-02-02 00:00:00.000000 kb_controller-1.0.0/src/kb_controller/controller.py
--rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 kb_controller-1.0.0/src/kb_controller/ubitemulator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kb_controller-1.0.0/src/kb_controller/helpers/__init__.py
--rw-r--r--   0        0        0     1453 2020-02-02 00:00:00.000000 kb_controller-1.0.0/src/kb_controller/helpers/event_poller.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 kb_controller-1.0.0/src/kb_controller/helpers/helper.py
--rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 kb_controller-1.0.0/src/kb_controller/helpers/kb_central.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 kb_controller-1.0.0/src/kb_controller/helpers/kb_config.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 kb_controller-1.0.0/src/kb_controller/helpers/kbc-default-config.ini
--rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 kb_controller-1.0.0/src/kb_controller/helpers/microbit.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 kb_controller-1.0.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 kb_controller-1.0.0/LICENSE
--rw-r--r--   0        0        0    15035 2020-02-02 00:00:00.000000 kb_controller-1.0.0/README.md
--rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 kb_controller-1.0.0/pyproject.toml
--rw-r--r--   0        0        0    15662 2020-02-02 00:00:00.000000 kb_controller-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 kb_controller-1.0.1/setup.py
+-rwxr-xr-x   0        0        0       33 2020-02-02 00:00:00.000000 kb_controller-1.0.1/start.sh
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 kb_controller-1.0.1/.vscode/launch.json
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 kb_controller-1.0.1/src/kb_controller/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kb_controller-1.0.1/src/kb_controller/__init__.py
+-rw-r--r--   0        0        0     8957 2020-02-02 00:00:00.000000 kb_controller-1.0.1/src/kb_controller/controller.py
+-rw-r--r--   0        0        0     4072 2020-02-02 00:00:00.000000 kb_controller-1.0.1/src/kb_controller/ubitemulator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 kb_controller-1.0.1/src/kb_controller/helpers/__init__.py
+-rw-r--r--   0        0        0     1452 2020-02-02 00:00:00.000000 kb_controller-1.0.1/src/kb_controller/helpers/event_poller.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 kb_controller-1.0.1/src/kb_controller/helpers/helper.py
+-rw-r--r--   0        0        0     4697 2020-02-02 00:00:00.000000 kb_controller-1.0.1/src/kb_controller/helpers/kb_central.py
+-rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 kb_controller-1.0.1/src/kb_controller/helpers/kb_config.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 kb_controller-1.0.1/src/kb_controller/helpers/kbc-default-config.ini
+-rw-r--r--   0        0        0     1532 2020-02-02 00:00:00.000000 kb_controller-1.0.1/src/kb_controller/helpers/microbit.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 kb_controller-1.0.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 kb_controller-1.0.1/LICENSE
+-rw-r--r--   0        0        0    15230 2020-02-02 00:00:00.000000 kb_controller-1.0.1/README.md
+-rw-r--r--   0        0        0      670 2020-02-02 00:00:00.000000 kb_controller-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0    15857 2020-02-02 00:00:00.000000 kb_controller-1.0.1/PKG-INFO
```

### Comparing `kb_controller-1.0.0/src/kb_controller/.DS_Store` & `kb_controller-1.0.1/src/kb_controller/.DS_Store`

 * *Files identical despite different names*

### Comparing `kb_controller-1.0.0/src/kb_controller/controller.py` & `kb_controller-1.0.1/src/kb_controller/controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
-import serial
-import os
 import getpass
-from kb_controller.helpers import kb_config, kb_central, microbit, event_poller, helper
+import os
+
+import serial
+
+from kb_controller.helpers import helper, kb_central, kb_config, microbit
 
 current_track_id = 0
 department_id = 0
 tracks_per_department = {}
 
 def start():
     clear_console()
@@ -27,16 +29,18 @@
     department_id = kb_central.get_department_id_from_token()
     tracks_per_department = kb_central.get_tracks()
 
     show_console_info()
 
     while True:
 
-        if current_track_id > 0 and event_poller.thread is None:
-            event_poller.start_thread(current_track_id)
+        # Do not make poll events automatically for now
+        # We let the micro:bit do that...
+        #if current_track_id > 0 and event_poller.thread is None:
+        #    event_poller.start_thread(current_track_id)
 
         try:
             byte_text = microbit.read_line()
             response = ''
             text = str(byte_text, 'utf-8').strip()
 
             if text != '':
@@ -46,15 +50,15 @@
                     microbit.send_message('OK:QUIT')
                     break
 
                 if text.startswith('init:'):
                     track = text[5:]
                     if track == '0':
                         print()
-                        print("FEJL! Micro:bit'en er sat rigtig op - den står til bane ID = 0")
+                        print("FEJL! Micro:bit'en er ikke sat rigtig op - den står til bane ID = 0")
                         print()
                         response = 'ERROR:INIT:INVALID-TRACK:' + track
                     elif not track in tracks_per_department[department_id]['tracks']:
                         print()
                         print(f'FEJL! Bane ID {track} findes ikke for afdeling {department_id}')
                         print()
                         response = 'ERROR:INIT:INVALID-TRACK:' + track
@@ -73,14 +77,15 @@
                     response = 'ERROR:NOT-INITIALIZED'
 
                 elif (text == 'events'):
                     print()
                     print('Henter events for kuglebanen')
                     print('-----------------------------')
                     count = kb_central.get_number_of_events_for_track(current_track_id)
+                    print(f'Antal beskeder modtaget til bane-ID: {current_track_id} = {count}')
                     response = f'OK:EVENTS-TRACK:{current_track_id}:{count}'
 
                 elif text.startswith('send:'):
                     to_track = text[5:]
                     to_track_exists = False
                     for dep_id in tracks_per_department:
                         to_track_exists = to_track in tracks_per_department[dep_id]['tracks']
@@ -145,16 +150,14 @@
 
 
 def pop_event(events):
     # first event is always the oldest
     event_id_to_pop = list(events['events'])[0]
     event = events['events'][event_id_to_pop]
 
-    kb_central.print_kb_event(event_id_to_pop, event)
-
     command_id = event['command_id']
     from_department_id = event['from_department_id']
     from_track_id = event['from_track_id']
 
     kb_central.delete_event(event_id_to_pop)
     return f'OK:POP:{from_department_id}:{from_track_id}:{command_id}'
```

### Comparing `kb_controller-1.0.0/src/kb_controller/ubitemulator.py` & `kb_controller-1.0.1/src/kb_controller/ubitemulator.py`

 * *Files identical despite different names*

### Comparing `kb_controller-1.0.0/src/kb_controller/helpers/event_poller.py` & `kb_controller-1.0.1/src/kb_controller/helpers/event_poller.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 thread = None
 
 def kb_central_poller(current_track_id):
     sleep(1) # Give controller time to initialize
     while True:
         print()
         print('- - - - - - - - - - - - - - - - - - - - -')
-        print('Henter events fra kukglebane centralen...')
+        print('Henter events fra kuglebane centralen...')
         print()
 
         count = kb_central.get_number_of_events_for_track(current_track_id)
         print()
         print(f'Antal events modtaget i alt: {count}')
         print()
```

### Comparing `kb_controller-1.0.0/src/kb_controller/helpers/kb_central.py` & `kb_controller-1.0.1/src/kb_controller/helpers/kb_central.py`

 * *Files identical despite different names*

### Comparing `kb_controller-1.0.0/src/kb_controller/helpers/kb_config.py` & `kb_controller-1.0.1/src/kb_controller/helpers/kb_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,18 @@
 def set_api_user(user, p):
     global api_user, pwd
     api_user = user
     pwd = p
 
 is_production = config['GENERAL'].getboolean('is_production')
 is_emulator = config['GENERAL'].getboolean('is_emulator')
-poll_interval_in_seconds = config['GENERAL'].getint('polling_interval')
+
+# Currently not used!!
+#poll_interval_in_seconds = config['GENERAL'].getint('polling_interval')
+
 EMULATOR = config['EMULATOR']
 MICROBIT = config['MICROBIT']
 LOCALHOST = config['LOCALHOST']
 PRODUCTION = config['PRODUCTION']
 
 def get_tty_value(key):
     return EMULATOR[key] if is_emulator else MICROBIT[key]
@@ -63,8 +66,8 @@
 
 print(f'  is_production        = {is_production}')
 print(f'  is_emulator          = {is_emulator}')
 print(f'  tty_name             = {tty_name}')
 print(f'  tty_rate             = {tty_rate}')
 print(f'  tty_timeout          = {tty_timeout}')
 print(f'  kbc_host             = {kbc_host}')
-print(f'  polling_interval (s) = {poll_interval_in_seconds}')
+#print(f'  polling_interval (s) = {poll_interval_in_seconds}')
```

### Comparing `kb_controller-1.0.0/src/kb_controller/helpers/microbit.py` & `kb_controller-1.0.1/src/kb_controller/helpers/microbit.py`

 * *Files identical despite different names*

### Comparing `kb_controller-1.0.0/LICENSE` & `kb_controller-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kb_controller-1.0.0/README.md` & `kb_controller-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,19 @@
 Når den serielle port er forbundet, skal api-bruger og adgangskode angives. API brugeren, er den bruger der har adgang til at lave forespørgsler til _kuglebane centralen_ (se evt. også https://kuglebane.pythonanywhere.com)
 
 
 ### Controller initialiseres ved opstart
 
 Når controlleren er startet op skriver den ud i konsollen hvilken afdeling den hører til og hvilke kommandoer man kan sende til den.
 
-Herefter venter den på at der sende en `init` kommando fra microbit'en, der fortæller hvilken kuglebane den tilhører. Dette gøres ved at få micro:bit'en til at sende en `init:<<ID>>` kommando, hvor `ID` er kuglebanens ID (en oversigt over kuglebane-ID'er kan ses på _kuglebane centralen_ - https://kuglebane.pythonanywhere.com/tracks/)
+Herefter venter den på at der sendes en `init` kommando fra microbit'en, der fortæller hvilken kuglebane den tilhører. 
+
+Dette gøres ved at få micro:bit'en til at sende en `init:<<ID>>` kommando, hvor `ID` er kuglebanens ID (en oversigt over kuglebane-ID'er kan ses på _kuglebane centralen_ - https://kuglebane.pythonanywhere.com/tracks/).
+
+I eksempelkoden til micro:bit'en prøver den at sende en `init` kommando når dnstarter - og ellers når man ryster micro:bit'en.
 
 Se desuden afsnittet _Kommandoer der kan sendes til controlleren_ herunder.
 
 Når controlleren har fået at vide hilken kuglebane den tilhører skrives listen af kuglebaner per afdeling ud i konsollen, f.eks.:
 
 ```text
   ============================================================
@@ -184,43 +188,43 @@
   [2023-03-19 22:56:16] m:b >>> OK:INIT:1
 ```
 
 Controlleren herover er placeret i afdeling _CPV_ og tilsluttet kuglebane _Smølfine_ med ID = 2.
 
 ### Hentning af beskeder til kuglebanen i baggrunden
 
-Når controlleren er startet op og initialiseret, startes en tråd, der står og poller _kuglebane centralen_ om der er kommet events til den kuglebane, controllere er tilsluttet. 
+I eksempelkoden til micro:bit'en sendes der en `events` kommando til controlleren hvert minut.
 
-Dette gøres i det interval (i sekunder) der er sat i `polling_interval` i _kbc-config.ini_ filen (se tidligere afsnit).
+Hvis der er en eller flere events, skrives dette ud i konsollen. 
 
-Hvis der er en eller flere events, skrives dette ud i konsollen, f.eks.:
+Hvis der f.eks. er modtaget én besked fra bane-ID 1 (i CPV) til bane-ID 5 (i CPS):
 
 ```text
-  - - - - - - - - - - - - - - - - - - - - -
-  Henter events fra kukglebane centralen...
-
-  [2023-03-19 23:09:18] KB-CENTRAL >>> https://kuglebane.pythonanywhere.com/api/events/1  [GET]
-  [2023-03-19 23:09:18] KB-CENTRAL <<< Response status OK!
+[2023-04-10 18:14:58] m:b <<< events
 
+Henter events for kuglebanen
+-----------------------------
+[2023-04-10 18:14:58] KB-CENTRAL >>> http://kuglebane.pythonanywhere.com/api/events/5  [GET]
+[2023-04-10 18:14:59] KB-CENTRAL <<< Response status OK!
 
-  Event id: 1 - kommando: START
-    - afsendt: 19-03-2023 23:08:41.787930
-    - fra CPB, bane 3 (Gammelsmølf)
 
+ Event id: 9 - kommando: START
+   - afsendt: 10-04-2023 16:12:07.974412
+   - fra CPV, bane 1 (Gammelsmølf)
 
-  Antal events modtaget i alt: 1
 
-  Kontakter kuglebane-centralen igen om 60 sekunder...
-  - - - - - - - - - - - - - - - - - - - - -
+Antal beskeder modtaget til bane-ID: 5 = 1
+[2023-04-10 18:14:59] m:b >>> OK:EVENTS-TRACK:1:1
 ```
 
+BEMÆRK: Dette fortæller kun OM der er beskeder. Det er efterfølgende op til micro:bit'en at hente en besked.
 
-Det er så op til micro:bit'en at hente en event.
+Man henter en besked ved at sende `pop` kommandoen til controlleren. Dette vil hente den ældste besked, der er sendt (altså den første besked), hvorefter denne slettes fra _kuglebane centralen_. 
 
-Nu og her, gøres dette ved at bruge `pop` kommandoen - så man henter den ælste event, der er sendt, hvorefter denne slettes fra _kuglebane centralen_.
+Når beskeden er "poppet" uden fejl, kan micro:bit'en gøre noget med den - hvilket typisk vil være at starte kuglen. :-)
 
 ### Logning af kommunikation i konsollen
 
 Generelt skrives al kommunikation ud i konsollen. Ud over tidsstemplet, benyttes der disse præfiks:
 
 - `m:b >>>` besked sendt TIL micro:bit
 - `m:b <<<` besked modtaget FRA micro:bit
```

### Comparing `kb_controller-1.0.0/pyproject.toml` & `kb_controller-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "kb_controller"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="esgem", email="esge@kodepirat.dk" },
 ]
 description = "CPVB Kuglebane Controller - forår 2023"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `kb_controller-1.0.0/PKG-INFO` & `kb_controller-1.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kb_controller
-Version: 1.0.0
+Version: 1.0.1
 Summary: CPVB Kuglebane Controller - forår 2023
 Project-URL: Homepage, https://github.com/Coding-Pirates-Viborg/kuglebane-controller
 Project-URL: Bug Tracker, https://github.com/Coding-Pirates-Viborg/kuglebane-controller/issues
 Author-email: esgem <esge@kodepirat.dk>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -160,15 +160,19 @@
 Når den serielle port er forbundet, skal api-bruger og adgangskode angives. API brugeren, er den bruger der har adgang til at lave forespørgsler til _kuglebane centralen_ (se evt. også https://kuglebane.pythonanywhere.com)
 
 
 ### Controller initialiseres ved opstart
 
 Når controlleren er startet op skriver den ud i konsollen hvilken afdeling den hører til og hvilke kommandoer man kan sende til den.
 
-Herefter venter den på at der sende en `init` kommando fra microbit'en, der fortæller hvilken kuglebane den tilhører. Dette gøres ved at få micro:bit'en til at sende en `init:<<ID>>` kommando, hvor `ID` er kuglebanens ID (en oversigt over kuglebane-ID'er kan ses på _kuglebane centralen_ - https://kuglebane.pythonanywhere.com/tracks/)
+Herefter venter den på at der sendes en `init` kommando fra microbit'en, der fortæller hvilken kuglebane den tilhører. 
+
+Dette gøres ved at få micro:bit'en til at sende en `init:<<ID>>` kommando, hvor `ID` er kuglebanens ID (en oversigt over kuglebane-ID'er kan ses på _kuglebane centralen_ - https://kuglebane.pythonanywhere.com/tracks/).
+
+I eksempelkoden til micro:bit'en prøver den at sende en `init` kommando når dnstarter - og ellers når man ryster micro:bit'en.
 
 Se desuden afsnittet _Kommandoer der kan sendes til controlleren_ herunder.
 
 Når controlleren har fået at vide hilken kuglebane den tilhører skrives listen af kuglebaner per afdeling ud i konsollen, f.eks.:
 
 ```text
   ============================================================
@@ -201,43 +205,43 @@
   [2023-03-19 22:56:16] m:b >>> OK:INIT:1
 ```
 
 Controlleren herover er placeret i afdeling _CPV_ og tilsluttet kuglebane _Smølfine_ med ID = 2.
 
 ### Hentning af beskeder til kuglebanen i baggrunden
 
-Når controlleren er startet op og initialiseret, startes en tråd, der står og poller _kuglebane centralen_ om der er kommet events til den kuglebane, controllere er tilsluttet. 
+I eksempelkoden til micro:bit'en sendes der en `events` kommando til controlleren hvert minut.
 
-Dette gøres i det interval (i sekunder) der er sat i `polling_interval` i _kbc-config.ini_ filen (se tidligere afsnit).
+Hvis der er en eller flere events, skrives dette ud i konsollen. 
 
-Hvis der er en eller flere events, skrives dette ud i konsollen, f.eks.:
+Hvis der f.eks. er modtaget én besked fra bane-ID 1 (i CPV) til bane-ID 5 (i CPS):
 
 ```text
-  - - - - - - - - - - - - - - - - - - - - -
-  Henter events fra kukglebane centralen...
-
-  [2023-03-19 23:09:18] KB-CENTRAL >>> https://kuglebane.pythonanywhere.com/api/events/1  [GET]
-  [2023-03-19 23:09:18] KB-CENTRAL <<< Response status OK!
+[2023-04-10 18:14:58] m:b <<< events
 
+Henter events for kuglebanen
+-----------------------------
+[2023-04-10 18:14:58] KB-CENTRAL >>> http://kuglebane.pythonanywhere.com/api/events/5  [GET]
+[2023-04-10 18:14:59] KB-CENTRAL <<< Response status OK!
 
-  Event id: 1 - kommando: START
-    - afsendt: 19-03-2023 23:08:41.787930
-    - fra CPB, bane 3 (Gammelsmølf)
 
+ Event id: 9 - kommando: START
+   - afsendt: 10-04-2023 16:12:07.974412
+   - fra CPV, bane 1 (Gammelsmølf)
 
-  Antal events modtaget i alt: 1
 
-  Kontakter kuglebane-centralen igen om 60 sekunder...
-  - - - - - - - - - - - - - - - - - - - - -
+Antal beskeder modtaget til bane-ID: 5 = 1
+[2023-04-10 18:14:59] m:b >>> OK:EVENTS-TRACK:1:1
 ```
 
+BEMÆRK: Dette fortæller kun OM der er beskeder. Det er efterfølgende op til micro:bit'en at hente en besked.
 
-Det er så op til micro:bit'en at hente en event.
+Man henter en besked ved at sende `pop` kommandoen til controlleren. Dette vil hente den ældste besked, der er sendt (altså den første besked), hvorefter denne slettes fra _kuglebane centralen_. 
 
-Nu og her, gøres dette ved at bruge `pop` kommandoen - så man henter den ælste event, der er sendt, hvorefter denne slettes fra _kuglebane centralen_.
+Når beskeden er "poppet" uden fejl, kan micro:bit'en gøre noget med den - hvilket typisk vil være at starte kuglen. :-)
 
 ### Logning af kommunikation i konsollen
 
 Generelt skrives al kommunikation ud i konsollen. Ud over tidsstemplet, benyttes der disse præfiks:
 
 - `m:b >>>` besked sendt TIL micro:bit
 - `m:b <<<` besked modtaget FRA micro:bit
```

