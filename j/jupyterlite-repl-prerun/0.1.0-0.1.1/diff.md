# Comparing `tmp/jupyterlite_repl_prerun-0.1.0.tar.gz` & `tmp/jupyterlite_repl_prerun-0.1.1.tar.gz`

## Comparing `jupyterlite_repl_prerun-0.1.0.tar` & `jupyterlite_repl_prerun-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,25 @@
--rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/.prettierignore
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/RELEASE.md
--rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/install.json
--rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/package.json
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/setup.py
--rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/tsconfig.json
--rw-r--r--   0        0        0   217285 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/yarn.lock
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/__init__.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/_version.py
--rw-r--r--   0        0        0    21420 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/labextension/build_log.json
--rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/labextension/package.json
--rw-r--r--   0        0        0     2064 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/labextension/static/lib_index_js.a8814b117236b47425c0.js
--rw-r--r--   0        0        0     2058 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/labextension/static/lib_index_js.a8814b117236b47425c0.js.map
--rw-r--r--   0        0        0    27626 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/labextension/static/remoteEntry.6b5d514970461f2ad6f8.js
--rw-r--r--   0        0        0    26520 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/labextension/static/remoteEntry.6b5d514970461f2ad6f8.js.map
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/labextension/static/style.js
--rw-r--r--   0        0        0     4618 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/labextension/static/style_index_js.f826786275745c1de575.js
--rw-r--r--   0        0        0     1814 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/labextension/static/style_index_js.f826786275745c1de575.js.map
--rw-r--r--   0        0        0    12076 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.5cf5d1a5272ae9a9bfc0.js
--rw-r--r--   0        0        0    13817 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.5cf5d1a5272ae9a9bfc0.js.map
--rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/src/index.ts
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/style/base.css
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/style/index.css
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/style/index.js
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/.gitignore
--rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/LICENSE
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/README.md
--rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       91 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/.prettierignore
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/RELEASE.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/install.json
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/tsconfig.json
+-rw-r--r--   0        0        0   216144 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/yarn.lock
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/jupyterlite_repl_prerun/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/jupyterlite_repl_prerun/_version.py
+-rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/jupyterlite_repl_prerun/labextension/package.json
+-rw-r--r--   0        0        0      635 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/jupyterlite_repl_prerun/labextension/static/568.82478801a88ad06390f2.js
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/jupyterlite_repl_prerun/labextension/static/747.a1a07690be9cf9e8e997.js
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/jupyterlite_repl_prerun/labextension/static/remoteEntry.fca6937b2f1032f423f9.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/jupyterlite_repl_prerun/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/jupyterlite_repl_prerun/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1017 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/style/index.js
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/README.md
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     5386 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.1.1/PKG-INFO
```

### Comparing `jupyterlite_repl_prerun-0.1.0/RELEASE.md` & `jupyterlite_repl_prerun-0.1.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlite_repl_prerun-0.1.0/package.json` & `jupyterlite_repl_prerun-0.1.1/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.1.1'"}*

```diff
@@ -159,9 +159,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `jupyterlite_repl_prerun-0.1.0/tsconfig.json` & `jupyterlite_repl_prerun-0.1.1/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlite_repl_prerun-0.1.0/yarn.lock` & `jupyterlite_repl_prerun-0.1.1/yarn.lock`

 * *Files 1% similar despite different names*

```diff
@@ -502,44 +502,14 @@
 "@jupyterlab/nbformat@^3.0.0 || ^4.0.0-alpha.15", "@jupyterlab/nbformat@^3.6.3":
   version "3.6.3"
   resolved "https://registry.yarnpkg.com/@jupyterlab/nbformat/-/nbformat-3.6.3.tgz#8520338e3679cbe8ce2ea8eb5a9b816f8b774ad3"
   integrity sha512-0qJLa4dtOmu9EmHFeM7gaZi4qheovIPc9ZrgGGRuG0obajs4YYlvh4MQvCSgpVhme4AuBfGlcfzhlx+Gbzr5Xw==
   dependencies:
     "@lumino/coreutils" "^1.11.0"
 
-"@jupyterlab/notebook@^3.6.3":
-  version "3.6.3"
-  resolved "https://registry.yarnpkg.com/@jupyterlab/notebook/-/notebook-3.6.3.tgz#1584be72184d67d59291e2b22f55bc257afde436"
-  integrity sha512-id1KD5/9IDPr/IZFCl/YX4Vc+Q198LZshhFNEcVJZcRdjD7Vh+LGvWcLOh80OAv86J4XSTTAsp3gHPr4iSwPDg==
-  dependencies:
-    "@jupyter/ydoc" "~0.2.3"
-    "@jupyterlab/apputils" "^3.6.3"
-    "@jupyterlab/cells" "^3.6.3"
-    "@jupyterlab/codeeditor" "^3.6.3"
-    "@jupyterlab/coreutils" "^5.6.3"
-    "@jupyterlab/docregistry" "^3.6.3"
-    "@jupyterlab/nbformat" "^3.6.3"
-    "@jupyterlab/observables" "^4.6.3"
-    "@jupyterlab/rendermime" "^3.6.3"
-    "@jupyterlab/services" "^6.6.3"
-    "@jupyterlab/settingregistry" "^3.6.3"
-    "@jupyterlab/statusbar" "^3.6.3"
-    "@jupyterlab/translation" "^3.6.3"
-    "@jupyterlab/ui-components" "^3.6.3"
-    "@lumino/algorithm" "^1.9.0"
-    "@lumino/coreutils" "^1.11.0"
-    "@lumino/domutils" "^1.8.0"
-    "@lumino/dragdrop" "^1.13.0"
-    "@lumino/messaging" "^1.10.0"
-    "@lumino/properties" "^1.8.0"
-    "@lumino/signaling" "^1.10.0"
-    "@lumino/virtualdom" "^1.14.0"
-    "@lumino/widgets" "^1.37.2"
-    react "^17.0.1"
-
 "@jupyterlab/observables@^4.6.3":
   version "4.6.3"
   resolved "https://registry.yarnpkg.com/@jupyterlab/observables/-/observables-4.6.3.tgz#49a9ca49fbda7428abbd1bfb8a4006ecd406c18d"
   integrity sha512-CvQoL+9WHXOy/CXp/PQLi4c5iZVJ4psz11+GrycDDinX1AdVQ8a43OLTC0gxWl3Tk2C8ZvAi1sgn4FS68E1ACQ==
   dependencies:
     "@lumino/algorithm" "^1.9.0"
     "@lumino/coreutils" "^1.11.0"
@@ -1448,17 +1418,17 @@
 
 camelcase@^5.3.1:
   version "5.3.1"
   resolved "https://registry.yarnpkg.com/camelcase/-/camelcase-5.3.1.tgz#e3c9b31569e106811df242f715725a1f4c494320"
   integrity sha512-L28STB170nwWS63UjtlEOE3dldQApaJXZkOI1uMFfzf3rRuPegHaHesyee+YxQ+W6SvRDQV6UrdOdRiR153wJg==
 
 caniuse-lite@^1.0.30001449:
-  version "1.0.30001476"
-  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001476.tgz#759906c53eae17133217d75b482f9dc5c02f7898"
-  integrity sha512-JmpktFppVSvyUN4gsLS0bShY2L9ZUslHLE72vgemBkS43JD2fOvKTKs+GtRwuxrtRGnwJFW0ye7kWRRlLJS9vQ==
+  version "1.0.30001477"
+  resolved "https://registry.yarnpkg.com/caniuse-lite/-/caniuse-lite-1.0.30001477.tgz#a2ffb2276258233034bbb869d4558b02658a511e"
+  integrity sha512-lZim4iUHhGcy5p+Ri/G7m84hJwncj+Kz7S5aD4hoQfslKZJgt0tHc/hafVbqHC5bbhHb+mrW2JOUHkI5KH7toQ==
 
 chalk@^2.0.0, chalk@^2.3.0, chalk@^2.4.1:
   version "2.4.2"
   resolved "https://registry.yarnpkg.com/chalk/-/chalk-2.4.2.tgz#cd42541677a54333cf541a49108c1432b44c9424"
   integrity sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==
   dependencies:
     ansi-styles "^3.2.1"
@@ -3147,17 +3117,17 @@
   version "3.3.6"
   resolved "https://registry.yarnpkg.com/minipass/-/minipass-3.3.6.tgz#7bba384db3a1520d18c9c0e5251c3444e95dd94a"
   integrity sha512-DxiNidxSEK+tHG6zOIklvNOwm3hvCrbUrdtzY74U6HKTJxvIDfOUL5W5P2Ghd3DTkhhKPYGqeNUIh5qcM4YBfw==
   dependencies:
     yallist "^4.0.0"
 
 minipass@^4.0.0:
-  version "4.2.5"
-  resolved "https://registry.yarnpkg.com/minipass/-/minipass-4.2.5.tgz#9e0e5256f1e3513f8c34691dd68549e85b2c8ceb"
-  integrity sha512-+yQl7SX3bIT83Lhb4BVorMAHVuqsskxRdlmO9kTpyukp8vsm2Sn/fUOV9xlnG8/a5JsypJzap21lz/y3FBMJ8Q==
+  version "4.2.7"
+  resolved "https://registry.yarnpkg.com/minipass/-/minipass-4.2.7.tgz#14c6fc0dcab54d9c4dd64b2b7032fef04efec218"
+  integrity sha512-ScVIgqHcXRMyfflqHmEW0bm8z8rb5McHyOY3ewX9JBgZaR77G7nxq9L/mtV96/QbAAwtbCAHVVLzD1kkyfFQEw==
 
 minizlib@^2.1.1:
   version "2.1.2"
   resolved "https://registry.yarnpkg.com/minizlib/-/minizlib-2.1.2.tgz#e90d3466ba209b932451508a11ce3d3632145931"
   integrity sha512-bAxsR8BVfj60DWXHE3u30oHzfl4G7khkSuPW+qvpd7jFRHm7dLxOjUk1EHACJ/hxLY8phGJ0YhYHZo7jil7Qdg==
   dependencies:
     minipass "^3.0.0"
```

### Comparing `jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/labextension/package.json` & `jupyterlite_repl_prerun-0.1.1/jupyterlite_repl_prerun/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785879629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.fca6937b2f1032f423f9.js'}}",*

 * * "'version'": "'0.1.1'"}*

```diff
@@ -92,15 +92,15 @@
         "lib/**/*.{d.ts,eot,gif,html,jpg,js,js.map,json,png,svg,woff2,ttf}",
         "style/**/*.{css,js,eot,gif,html,jpg,json,png,svg,woff2,ttf}"
     ],
     "homepage": "https://github.com/jobovy/jupyterlite-repl-prerun",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.6b5d514970461f2ad6f8.js",
+            "load": "static/remoteEntry.fca6937b2f1032f423f9.js",
             "style": "./style"
         },
         "extension": true,
         "outputDir": "jupyterlite_repl_prerun/labextension"
     },
     "keywords": [
         "jupyter",
@@ -164,9 +164,9 @@
         "rules": {
             "property-no-vendor-prefix": null,
             "selector-no-vendor-prefix": null,
             "value-no-vendor-prefix": null
         }
     },
     "types": "lib/index.d.ts",
-    "version": "0.1.0"
+    "version": "0.1.1"
 }
```

### Comparing `jupyterlite_repl_prerun-0.1.0/src/index.ts` & `jupyterlite_repl_prerun-0.1.1/src/index.ts`

 * *Files identical despite different names*

### Comparing `jupyterlite_repl_prerun-0.1.0/.gitignore` & `jupyterlite_repl_prerun-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlite_repl_prerun-0.1.0/LICENSE` & `jupyterlite_repl_prerun-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlite_repl_prerun-0.1.0/README.md` & `jupyterlite_repl_prerun-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `jupyterlite_repl_prerun-0.1.0/pyproject.toml` & `jupyterlite_repl_prerun-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlite_repl_prerun-0.1.0/PKG-INFO` & `jupyterlite_repl_prerun-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlite_repl_prerun
-Version: 0.1.0
+Version: 0.1.1
 Summary: Jupyterlite extension to allow code to be pre-run in the repl app
 Project-URL: Homepage, https://github.com/jobovy/jupyterlite-repl-prerun
 Project-URL: Bug Tracker, https://github.com/jobovy/jupyterlite-repl-prerun/issues
 Project-URL: Repository, https://github.com/jobovy/jupyterlite-repl-prerun.git
 Author-email: Jo Bovy <bovy@astro.utoronto.ca>
 License: BSD 3-Clause License
```

