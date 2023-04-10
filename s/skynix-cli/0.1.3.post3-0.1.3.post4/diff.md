# Comparing `tmp/skynix-cli-0.1.3.post3.tar.gz` & `tmp/skynix-cli-0.1.3.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skynix-cli-0.1.3.post3.tar", max compression
+gzip compressed data, was "skynix-cli-0.1.3.post4.tar", max compression
```

## Comparing `skynix-cli-0.1.3.post3.tar` & `skynix-cli-0.1.3.post4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2022-09-17 09:56:47.029959 skynix-cli-0.1.3.post3/LICENSE
--rw-r--r--   0        0        0        0 2022-09-16 10:29:14.550632 skynix-cli-0.1.3.post3/README.md
--rw-r--r--   0        0        0      397 2022-09-17 21:48:06.406294 skynix-cli-0.1.3.post3/pyproject.toml
--rw-r--r--   0        0        0        0 2022-09-16 10:29:14.550632 skynix-cli-0.1.3.post3/skynix_cli/__init__.py
--rw-r--r--   0        0        0     1844 2022-09-17 21:47:47.975477 skynix-cli-0.1.3.post3/skynix_cli/skynixcli.py
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 skynix-cli-0.1.3.post3/setup.py
--rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 skynix-cli-0.1.3.post3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-09-17 09:56:47.029959 skynix-cli-0.1.3.post4/LICENSE
+-rw-r--r--   0        0        0        0 2022-09-16 10:29:14.550632 skynix-cli-0.1.3.post4/README.md
+-rw-r--r--   0        0        0      397 2023-04-10 12:56:57.529625 skynix-cli-0.1.3.post4/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-09-16 10:29:14.550632 skynix-cli-0.1.3.post4/skynix_cli/__init__.py
+-rw-r--r--   0        0        0     1696 2023-04-10 12:23:02.756509 skynix-cli-0.1.3.post4/skynix_cli/skynixcli.py
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 skynix-cli-0.1.3.post4/setup.py
+-rw-r--r--   0        0        0      340 1970-01-01 00:00:00.000000 skynix-cli-0.1.3.post4/PKG-INFO
```

### Comparing `skynix-cli-0.1.3.post3/LICENSE` & `skynix-cli-0.1.3.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `skynix-cli-0.1.3.post3/skynix_cli/skynixcli.py` & `skynix-cli-0.1.3.post4/skynix_cli/skynixcli.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,18 +24,15 @@
     with open(f"{path}/skynix/venv.txt", "r") as f:
         venv = f.read()
     
     if config != None:
         config["python"] = f"{venv.strip()}/bin/python"
     else:
         config = {"python": f"{venv.strip()}/bin/python",
-                  "nlpcloud_tokens": ["","","",""],
-                  "forefront_token": "",
-                  "forefront_gptj_url": "",
-                  "forefront_codegen_url": "",
+                  "poe_token": "",
                   "openweathermap_token": ""}
         
     with open(f"{path}/skynix/config.json", "w", encoding="utf-8") as f:
         json.dump(config, f, indent=4)
         
     typer.echo("Done installing requirements")
     typer.echo("#############################################")
@@ -50,8 +47,8 @@
     os.system(f"xfce4-terminal --drop-down -e '{python} -u '/home/{user}/skynix/main.py''")
 
 @cli.command()
 def config():
     os.system(f"nano /home/{os.getlogin()}/skynix/config.json")
 
 if __name__ == "__main__":
-    cli()
+    cli()
```

### Comparing `skynix-cli-0.1.3.post3/setup.py` & `skynix-cli-0.1.3.post4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['typer>=0.6.1,<0.7.0']
 
 entry_points = \
 {'console_scripts': ['skynix-cli = skynix_cli.skynixcli:cli']}
 
 setup_kwargs = {
     'name': 'skynix-cli',
-    'version': '0.1.3.post3',
+    'version': '0.1.3.post4',
     'description': '',
     'long_description': '',
     'author': 'AbdelrhmanNile',
     'author_email': 'abdelrhmannile@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

