# Comparing `tmp/Data_Cdvst-1.3.tar.gz` & `tmp/Data_Cdvst-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Data_Cdvst-1.3.tar", last modified: Sun Apr  9 19:10:57 2023, max compression
+gzip compressed data, was "Data_Cdvst-1.4.tar", last modified: Mon Apr 10 04:26:07 2023, max compression
```

## Comparing `Data_Cdvst-1.3.tar` & `Data_Cdvst-1.4.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-04-09 19:10:57.234100 Data_Cdvst-1.3/
-drwxrwxrwx   0        0        0        0 2023-04-09 19:10:57.217431 Data_Cdvst-1.3/Data_Cdvst/
--rw-rw-rw-   0        0        0        0 2023-04-08 11:10:24.000000 Data_Cdvst-1.3/Data_Cdvst/Files_Cdvst.py
--rw-rw-rw-   0        0        0     9531 2023-04-09 19:05:22.000000 Data_Cdvst-1.3/Data_Cdvst/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-09 19:10:57.234100 Data_Cdvst-1.3/Data_Cdvst.egg-info/
--rw-rw-rw-   0        0        0     1385 2023-04-09 19:10:56.000000 Data_Cdvst-1.3/Data_Cdvst.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      203 2023-04-09 19:10:57.000000 Data_Cdvst-1.3/Data_Cdvst.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-09 19:10:56.000000 Data_Cdvst-1.3/Data_Cdvst.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-04-09 19:10:56.000000 Data_Cdvst-1.3/Data_Cdvst.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1385 2023-04-09 19:10:57.234100 Data_Cdvst-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3791 2023-04-03 01:28:00.000000 Data_Cdvst-1.3/README.md
--rw-rw-rw-   0        0        0       42 2023-04-09 19:10:57.234100 Data_Cdvst-1.3/setup.cfg
--rw-rw-rw-   0        0        0     1606 2023-04-09 19:10:35.000000 Data_Cdvst-1.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:26:07.430729 Data_Cdvst-1.4/
+drwxrwxrwx   0        0        0        0 2023-04-10 04:26:07.405637 Data_Cdvst-1.4/Data_Cdvst/
+-rw-rw-rw-   0        0        0        0 2023-04-08 11:10:24.000000 Data_Cdvst-1.4/Data_Cdvst/Files_Cdvst.py
+-rw-rw-rw-   0        0        0     8601 2023-04-10 04:23:36.000000 Data_Cdvst-1.4/Data_Cdvst/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 04:26:07.430729 Data_Cdvst-1.4/Data_Cdvst.egg-info/
+-rw-rw-rw-   0        0        0     1385 2023-04-10 04:26:07.000000 Data_Cdvst-1.4/Data_Cdvst.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      203 2023-04-10 04:26:07.000000 Data_Cdvst-1.4/Data_Cdvst.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 04:26:07.000000 Data_Cdvst-1.4/Data_Cdvst.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-04-10 04:26:07.000000 Data_Cdvst-1.4/Data_Cdvst.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1385 2023-04-10 04:26:07.430729 Data_Cdvst-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3791 2023-04-03 01:28:00.000000 Data_Cdvst-1.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-04-10 04:26:07.430729 Data_Cdvst-1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1606 2023-04-10 04:24:17.000000 Data_Cdvst-1.4/setup.py
```

### Comparing `Data_Cdvst-1.3/Data_Cdvst/__init__.py` & `Data_Cdvst-1.4/Data_Cdvst/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,21 @@
+SQLite may not provide the expected performance benefits.
+
+```python
 import sqlite3
 from contextlib import contextmanager
 from sqlite3 import Error
 import time
-from Files_Cdvst import *
+import json
+import os
+import logging
+import asyncio
+
+logging.basicConfig(level=logging.DEBUG, format='%(asctime)s - %(levelname)s - %(message)s')
+
 
 class Database:
     """
     Eine Singleton-Klasse zum Verwalten von SQLite-Datenbanken.
 
     Beispiel:
 
@@ -22,54 +31,52 @@
 
     _instance = None
 
     def __new__(cls, db_path):
         """
         Erstellt eine neue Instanz der Klasse oder gibt eine vorhandene Instanz zurück.
 
-        Args:
+Args:
             db_path (str): Der Pfad zur Datenbankdatei.
 
         Returns:
             Eine Instanz der Klasse Database.
 
         """
         if cls._instance is None:
             cls._instance = super().__new__(cls)
             cls._instance.db_path = db_path
             cls._instance.conn = None
             cls._instance.cursor = None
         return cls._instance
 
-    def create_table(self):
-
+    async def create_table(self):
         """
         Erstellt eine Tabelle in der Datenbank, wenn sie nicht bereits existiert.
 
         """
-        with self.connect() as cursor:
+        async with self.connect() as cursor:
             try:
-                cursor.execute('CREATE TABLE IF NOT EXISTS entries (id INTEGER PRIMARY KEY, name TEXT, description TEXT, version TEXT, dirpath TEXT, timestamp INTEGER)')
-                self.conn.commit()
+                await cursor.execute('CREATE TABLE IF NOT EXISTS entries (id INTEGER PRIMARY KEY, name TEXT, description TEXT, version TEXT, dirpath TEXT, timestamp INTEGER)')
+                await self.conn.commit()
             except Error as e:
-                print(f"Fehler beim Erstellen der Tabelle: {e}")
+                logging.error(f"Fehler beim Erstellen der Tabelle: {e}")
 
     @contextmanager
-    def connect(self):
-
+    async def connect(self):
         """
         Stellt eine Verbindung zur Datenbank her und gibt den Cursor zurück.
 
         """
         try:
             self.conn = sqlite3.connect(self.db_path)
             self.cursor = self.conn.cursor()
             yield self.cursor
         except Error as e:
-            print(f"Fehler bei der Verbindung zur Datenbank: {e}")
+            logging.error(f"Fehler bei der Verbindung zur Datenbank: {e}")
             raise
         finally:
             if self.cursor:
                 self.cursor.close()
             if self.conn:
                 self.conn.close()
 
@@ -80,74 +87,74 @@
         Args:
             name (str): Der Name des Moduls.
             description (str): Die Beschreibung des Moduls.
             version (str): Die Versionsnummer des Moduls.
             dirpath (str): Der Dateipfad zum Modul.
 
         Returns:
-            True, wenn die Daten gültig sind, False sonst.
+            True, wenndie Daten gültig sind, False sonst.
 
         """
         if not name or not description or not version or not dirpath:
-            print("Ungültige Eingabe: Alle Felder müssen ausgefüllt sein.")
+            logging.warning("Ungültige Eingabe: Alle Felder müssen ausgefüllt sein.")
             return False
 
         # Weitere Validierungen können hier hinzugefügt werden.
 
         return True
 
-    def add_entry(self, name, description, version, dirpath):
+    async def add_entry(self, name, description, version, dirpath):
         """
         Fügt einen neuen Eintrag zur Datenbank hinzu.
 
         Args:
             name (str): Der Name des Moduls.
             description (str): Die Beschreibung des Moduls.
             version (str): Die Versionsnummer des Moduls.
             dirpath (str): Der Dateipfad zum Modul.
 
         """
         if not self.validate_entry(name, description, version, dirpath):
             return
 
-        with self.connect() as cursor:
+        async with self.connect() as cursor:
             try:
-                cursor.execute('INSERT INTO entries (name, description, version, dirpath, timestamp) VALUES (?, ?, ?, ?, ?)', (name, description, version, dirpath, int(time.time())))
-                self.conn.commit()
+                await cursor.execute('INSERT INTO entries (name, description, version, dirpath, timestamp) VALUES (?, ?, ?, ?, ?)', (name, description, version, dirpath, int(time.time())))
+                await self.conn.commit()
             except Error as e:
-                print(f"Fehler beim Erstellen des Eintrags: {e}")
+                logging.error(f"Fehler beim Erstellen des Eintrags: {e}")
 
-    def get_entry(self, *args, **kwargs):
+    async def get_entry(self, *args, **kwargs):
         """
         Ruft einen Eintrag aus der Datenbank ab.
 
         Args:
             kwargs: Die Bedingungen für die Abfrage als Schlüsselwertpaare.
 
         Returns:
             Eine Liste mit den abgerufenen Einträgen.
 
         """
-        with self.connect() as cursor:
+        async with self.connect() as cursor:
             try:
-                # create a# Liste von Bedingungen für die Abfrage
+                # Erstelle eine Liste von Bedingungen für die Abfrage
                 conditions = []
                 for key, value in kwargs.items():
                     conditions.append(f"{key}='{value}'")
 
                 # Erstelle die Abfrage-Zeichenfolge
                 query_string = 'SELECT * FROM entries'
                 if conditions:
                     query_string += f' WHERE {" AND ".join(conditions)}'
 
                 # Führe die Abfrage aus
-                cursor.execute(query_string)
+                await cursor.execute(query_string)
                 return cursor.fetchall()
             except Error as e:
-                print(f"Fehler beim Abrufen der Einträge: {e}")
+                logging.error(f"Fehler beim Abrufen der Einträge: {e}")
                 return []
 
     class EntryEditor:
         """
         Eine Unterklasse zum Bearbeiten von Einträgen in der Datenbank.
 
         Beispiel:
@@ -164,139 +171,94 @@
 
         def __getattr__(self, attr):
             def wrapper(value):
                 self.updates[attr] = value
                 return self
             return wrapper
 
-        def update(self):
+        async def update(self):
             """
             Aktualisiert den Eintrag in der Datenbank mit den neuen Werten.
 
             """
             if not self.updates:
                 return
-            with self.db.connect() as cursor:
+            async with self.db.connect() as cursor:
                 try:
-                    # create a list of update statements for the query
+                    # Erstelle eine Liste von Update-Anweisungen für die Abfrage
                     updates = []
                     for key, value in self.updates.items():
                         updates.append(f"{key}='{value}'")
 
-                    # create the query string
+                    # Erstelle die Abfrage-Zeichenfolge
                     query_string = f"UPDATE entries SET {', '.join(updates)} WHERE id={self.entry_id}"
-                    # execute the query
-                    cursor.execute(query_string)
-                    self.db.conn.commit()
+                    # Führe die Abfrage aus
+                    await cursor.execute(query_string)
+                    await self.db.conn.commit()
                 except Error as e:
-                    print(f"Fehler beim Aktualisieren des Eintrags: {e}")
+                    logging.error(f"Fehler beim Aktualisieren des Eintrags: {e}")
 
-    def edit_entry(self, *args, **kwargs):
+    async def edit_entry(self, *args, **kwargs):
         """
         Öffnet den Eintrag in der Datenbank zum Bearbeiten.
 
         Args:
             kwargs: Die Bedingungen zum Öffnen des Eintrags als Schlüsselwertpaare.
 
         Returns:
             Eine Instanz der Klasse EntryEditor zum Bearbeiten des Eintrags.
 
         """
         if 'ID' not in kwargs:
-            print("Ungültige Eingabe: Es muss eine ID angegeben werden.")
+            logging.warning("Ungültige Eingabe: Es muss eine ID angegeben werden.")
             return
 
         entry_id = kwargs.pop('ID')
 
         if not kwargs:
             return
 
-
         editor = Database.EntryEditor(self, entry_id)
         for key, value in kwargs.items():
             setattr(editor, key, value)
         return editor
 
-    def delete_entry(self, entry_id):
+    async def delete_entry(self, entry_id):
         """
         Löscht einen Eintrag aus der Datenbank.
+
         Args:
             entry_id (int): Die ID des zu löschenden Eintrags.
 
         """
-        with self.connect() as cursor:
+        async with self.connect() as cursor:
             try:
-                cursor.execute('DELETE FROM entries WHERE id=?', (entry_id,))
-                self.conn.commit()
+                await cursor.execute('DELETE FROM entries WHERE id=?', (entry_id,))
+                await self.conn.commit()
             except Error as e:
-                print(f"Fehler beim Löschen des Eintrags: {e}")
-        print("Hello")
-    def close(self):
+                logging.error(f"Fehler beim Löschen des Eintrags: {e}")
+
+    async def close(self):
         """
         Schließt die Verbindung zur Datenbank.
 
         """
         if self.conn:
             self.conn.close()
 
 
-
-class ConfigManager:
-    import json
-    import os
-    CONFIG_FILE_PATH = os.path.join(os.path.dirname(__file__), "config.json")
-    DEFAULT_API_KEY = "INSERT_YOUR_API_KEY_HERE"
-
-    @classmethod
-    def load_config(cls):
-        if not os.path.isfile(cls.CONFIG_FILE_PATH):
-            cls.save_config(cls.DEFAULT_API_KEY)
-        with open(cls.CONFIG_FILE_PATH, "r") as f:
-            config = json.load(f)
-        return config
-
-    @classmethod
-    def save_config(cls, api_key):
-        config = {"api_key": api_key}
-        with open(cls.CONFIG_FILE_PATH, "w") as f:
-            json.dump(config, f)
-
-class FavoritesManager:
-    import json
-    import os
-    FAVORITES_FILE_PATH = os.path.join(os.path.dirname(__file__), "favorites.json")
-    DEFAULT_CATEGORIES = {
-        "Category 1": [
-            "Prompt 1",
-            "Prompt 2"
-        ],
-        "Category 2": [
-            "Prompt 3",
-            "Prompt 4"
-        ]
-    }
-
-    @classmethod
-    def load_favorites(cls):
-        if not os.path.isfile(cls.FAVORITES_FILE_PATH):
-            cls.save_favorites(cls.DEFAULT_CATEGORIES)
-        with open(cls.FAVORITES_FILE_PATH, "r") as f:
-            favorites = json.load(f)
-        return favorites
-
-    @classmethod
-    def save_favorites(cls, favorites):
-        with open(cls.FAVORITES_FILE_PATH, "w") as f:
-            json.dump(favorites, f)
-
-if __name__ == "__main__":
+async def main():
     # Beispiel:
     db_path = "example.db"
     db = Database(db_path)
-    db.create_table()
-    db.add_entry(name="Module Name", description="Description", version="0.1", dirpath=r"F:\users\cdvst\OneDrive\Desktop\Pypi Module\ModuleName")
-    entry = db.get_entry(ID=1)
+    await db.create_table()
+    await db.add_entry(name="Module Name", description="Description", version="0.1", dirpath=r"F:\users\cdvst\OneDrive\Desktop\Pypi Module\ModuleName")
+    entry = await db.get_entry(ID=1)
     print(entry)
-    editor = db.edit_entry(ID=1).name("New Name")
-    editor.update()
-    db.delete_entry(1)
-    db.close()
+    editor = await db.edit_entry(ID=1).name("New Name")
+    await editor.update()
+    await db.delete_entry(1)
+    await db.close()
+
+
+if __name__ == "__main__":
+    asyncio.run(main())
```

### Comparing `Data_Cdvst-1.3/Data_Cdvst.egg-info/PKG-INFO` & `Data_Cdvst-1.4/Data_Cdvst.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Data-Cdvst
-Version: 1.3
+Version: 1.4
 Summary: Eine Python-Bibliothek zur einfachen Daten mangagment datenbanken undmehr und -aufnahme.
 Home-page: https://now4free.de/python/module/Data_Cdvst
 Author: Philipp Juen
 Author-email: support@now4free.de
 License: MIT
 Project-URL: Source, https://github.com/philippjuen/Audio_Cdvst
 Keywords: data,db,database,data handling,data saving,data sorting
```

### Comparing `Data_Cdvst-1.3/PKG-INFO` & `Data_Cdvst-1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Data_Cdvst
-Version: 1.3
+Version: 1.4
 Summary: Eine Python-Bibliothek zur einfachen Daten mangagment datenbanken undmehr und -aufnahme.
 Home-page: https://now4free.de/python/module/Data_Cdvst
 Author: Philipp Juen
 Author-email: support@now4free.de
 License: MIT
 Project-URL: Source, https://github.com/philippjuen/Audio_Cdvst
 Keywords: data,db,database,data handling,data saving,data sorting
```

### Comparing `Data_Cdvst-1.3/README.md` & `Data_Cdvst-1.4/README.md`

 * *Files identical despite different names*

### Comparing `Data_Cdvst-1.3/setup.py` & `Data_Cdvst-1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='Data_Cdvst',
-    version='1.3',
+    version='1.4',
     description='Eine Python-Bibliothek zur einfachen Daten mangagment datenbanken undmehr und -aufnahme.',
     long_description="""Data_Cdvst ist eine Python-Bibliothek zur einfachen nutzung von Datenbanken undeinfachen umgang mit datenverarbeitugn und -aufnahme. Die Bibliothek bietet Funktionen zum Abspielen von WAV- und MP3-Dateien sowie zur Aufnahme von Audio in einer WAV-Datei. Die Bibliothek umfasst auch eine automatische Spracherkennungsfunktion.
 
 Funktionen:
 - Einfache Datenbank erstellung
 - Einfache Datenbanken Einträge erzeugen
 - Einfahce Datenbanken auslesen
```

