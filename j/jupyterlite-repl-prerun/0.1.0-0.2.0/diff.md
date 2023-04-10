# Comparing `tmp/jupyterlite_repl_prerun-0.1.0.tar.gz` & `tmp/jupyterlite_repl_prerun-0.2.0.tar.gz`

## Comparing `jupyterlite_repl_prerun-0.1.0.tar` & `jupyterlite_repl_prerun-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,29 @@
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
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/.prettierignore
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/.readthedocs.yml
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/RELEASE.md
+-rw-r--r--   0        0        0      207 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/install.json
+-rw-r--r--   0        0        0     4970 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/package.json
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/setup.py
+-rw-r--r--   0        0        0      554 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/tsconfig.json
+-rw-r--r--   0        0        0   216144 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/yarn.lock
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/docs/conf.py
+-rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/docs/environment.yml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/docs/index.md
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/jupyterlite_repl_prerun/__init__.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/jupyterlite_repl_prerun/_version.py
+-rw-r--r--   0        0        0     5112 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/jupyterlite_repl_prerun/labextension/package.json
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/jupyterlite_repl_prerun/labextension/static/568.d794d3d66d23dc14a2f4.js
+-rw-r--r--   0        0        0     3522 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/jupyterlite_repl_prerun/labextension/static/747.a1a07690be9cf9e8e997.js
+-rw-r--r--   0        0        0     6386 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/jupyterlite_repl_prerun/labextension/static/remoteEntry.837d91241593cb213d2f.js
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/jupyterlite_repl_prerun/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/jupyterlite_repl_prerun/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0     1208 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/src/index.ts
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/style/base.css
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/style/index.css
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/style/index.js
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4667 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/README.md
+-rw-r--r--   0        0        0     2398 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     7585 2020-02-02 00:00:00.000000 jupyterlite_repl_prerun-0.2.0/PKG-INFO
```

### Comparing `jupyterlite_repl_prerun-0.1.0/RELEASE.md` & `jupyterlite_repl_prerun-0.2.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `jupyterlite_repl_prerun-0.1.0/package.json` & `jupyterlite_repl_prerun-0.2.0/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'version'": "'0.2.0'"}*

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
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlite_repl_prerun-0.1.0/tsconfig.json` & `jupyterlite_repl_prerun-0.2.0/tsconfig.json`

 * *Files identical despite different names*

### Comparing `jupyterlite_repl_prerun-0.1.0/yarn.lock` & `jupyterlite_repl_prerun-0.2.0/yarn.lock`

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
```

### Comparing `jupyterlite_repl_prerun-0.1.0/jupyterlite_repl_prerun/labextension/package.json` & `jupyterlite_repl_prerun-0.2.0/jupyterlite_repl_prerun/labextension/package.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9785879629629629%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.837d91241593cb213d2f.js'}}",*

 * * "'version'": "'0.2.0'"}*

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
+            "load": "static/remoteEntry.837d91241593cb213d2f.js",
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
+    "version": "0.2.0"
 }
```

### Comparing `jupyterlite_repl_prerun-0.1.0/src/index.ts` & `jupyterlite_repl_prerun-0.2.0/src/index.ts`

 * *Files 14% similar despite different names*

```diff
@@ -15,26 +15,32 @@
   activate: (app: JupyterFrontEnd, tracker: IConsoleTracker | null) => {
     if (!tracker) {
       return;
     }
     const search = window.location.search;
     const urlParams = new URLSearchParams(search);
     const prerun = urlParams.getAll('prerun');
+    const prerunCode = urlParams.getAll('prerun-code');
 
     tracker.widgetAdded.connect(async (_, widget) => {
       const { console } = widget;
 
       if (prerun[0]) {
         await console.sessionContext.ready;
         prerun.forEach(line =>
           console.sessionContext.session?.kernel?.requestExecute({
             code: line,
             silent: true,
             store_history: false
           })
         );
       }
+
+      if (prerunCode) {
+        await console.sessionContext.ready;
+        prerunCode.forEach(line => console.inject(line));
+      }
     });
   }
 };
 
 export default plugin;
```

### Comparing `jupyterlite_repl_prerun-0.1.0/.gitignore` & `jupyterlite_repl_prerun-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlite_repl_prerun-0.1.0/LICENSE` & `jupyterlite_repl_prerun-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyterlite_repl_prerun-0.1.0/pyproject.toml` & `jupyterlite_repl_prerun-0.2.0/pyproject.toml`

 * *Files identical despite different names*

