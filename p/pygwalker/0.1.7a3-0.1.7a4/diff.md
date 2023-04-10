# Comparing `tmp/pygwalker-0.1.7a3.tar.gz` & `tmp/pygwalker-0.1.7a4.tar.gz`

## Comparing `pygwalker-0.1.7a3.tar` & `pygwalker-0.1.7a4.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/.gitignore
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/index.html
--rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/package.json
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/tsconfig.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/vite.config.ts
--rw-r--r--   0        0        0   124304 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/yarn.lock
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/src/index.tsx
--rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/src/components/options.tsx
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/app/src/interfaces/index.ts
--rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/__init__.py
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/__main__.py
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/__version__.py
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/base.py
--rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/gwalker.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/templates/.gitignore
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/templates/index.html
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/templates/walk.js
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/templates/dist/index.d.ts
--rw-r--r--   0        0        0  1765339 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/templates/dist/pygwalker-app.iife.js
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/templates/dist/components/options.d.ts
--rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/templates/dist/interfaces/index.d.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/utils/__init__.py
--rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/utils/check_update.py
--rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/utils/config.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/utils/defaults.json
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/utils/fname_encodings.py
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/utils/gwalker_props.py
--rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pygwalker/utils/render.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/scripts/__init__.py
--rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/scripts/compile.sh
--rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/scripts/develop.sh
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/scripts/test-init.py
--rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/scripts/test-init.sh
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/.gitignore
--rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/LICENSE
--rw-r--r--   0        0        0    12861 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/README.md
--rw-r--r--   0        0        0     2366 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/pyproject.toml
--rw-r--r--   0        0        0    26975 2020-02-02 00:00:00.000000 pygwalker-0.1.7a3/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/.gitignore
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/index.html
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/package.json
+-rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/tsconfig.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/vite.config.ts
+-rw-r--r--   0        0        0   124304 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/yarn.lock
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/src/index.tsx
+-rw-r--r--   0        0        0     8289 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/src/components/options.tsx
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/app/src/interfaces/index.ts
+-rw-r--r--   0        0        0      975 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/__init__.py
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/__main__.py
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/__version__.py
+-rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/base.py
+-rw-r--r--   0        0        0     5600 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/gwalker.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/templates/.gitignore
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/templates/index.html
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/templates/walk.js
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/templates/dist/index.d.ts
+-rw-r--r--   0        0        0  1765339 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/templates/dist/pygwalker-app.iife.js
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/templates/dist/components/options.d.ts
+-rw-r--r--   0        0        0      236 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/templates/dist/interfaces/index.d.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/utils/__init__.py
+-rw-r--r--   0        0        0     1293 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/utils/check_update.py
+-rw-r--r--   0        0        0     4242 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/utils/config.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/utils/defaults.json
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/utils/fname_encodings.py
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/utils/gwalker_props.py
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pygwalker/utils/render.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/scripts/__init__.py
+-rwxr-xr-x   0        0        0      293 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/scripts/compile.sh
+-rwxr-xr-x   0        0        0      458 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/scripts/develop.sh
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/scripts/test-init.py
+-rwxr-xr-x   0        0        0      540 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/scripts/test-init.sh
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/.gitignore
+-rw-r--r--   0        0        0    11353 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/LICENSE
+-rw-r--r--   0        0        0    12861 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/README.md
+-rw-r--r--   0        0        0     2375 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/pyproject.toml
+-rw-r--r--   0        0        0    14004 2020-02-02 00:00:00.000000 pygwalker-0.1.7a4/PKG-INFO
```

### Comparing `pygwalker-0.1.7a3/app/package.json` & `pygwalker-0.1.7a4/app/package.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/app/tsconfig.json` & `pygwalker-0.1.7a4/app/tsconfig.json`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/app/vite.config.ts` & `pygwalker-0.1.7a4/app/vite.config.ts`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/app/yarn.lock` & `pygwalker-0.1.7a4/app/yarn.lock`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/app/src/index.tsx` & `pygwalker-0.1.7a4/app/src/index.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/app/src/components/options.tsx` & `pygwalker-0.1.7a4/app/src/components/options.tsx`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/pygwalker/__init__.py` & `pygwalker-0.1.7a4/pygwalker/__init__.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/pygwalker/__main__.py` & `pygwalker-0.1.7a4/pygwalker/__main__.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/pygwalker/base.py` & `pygwalker-0.1.7a4/pygwalker/base.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/pygwalker/gwalker.py` & `pygwalker-0.1.7a4/pygwalker/gwalker.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/pygwalker/templates/walk.js` & `pygwalker-0.1.7a4/pygwalker/templates/walk.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/pygwalker/templates/dist/pygwalker-app.iife.js` & `pygwalker-0.1.7a4/pygwalker/templates/dist/pygwalker-app.iife.js`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/pygwalker/utils/check_update.py` & `pygwalker-0.1.7a4/pygwalker/utils/check_update.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/pygwalker/utils/config.py` & `pygwalker-0.1.7a4/pygwalker/utils/config.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/pygwalker/utils/gwalker_props.py` & `pygwalker-0.1.7a4/pygwalker/utils/gwalker_props.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/pygwalker/utils/render.py` & `pygwalker-0.1.7a4/pygwalker/utils/render.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/scripts/test-init.py` & `pygwalker-0.1.7a4/scripts/test-init.py`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/scripts/test-init.sh` & `pygwalker-0.1.7a4/scripts/test-init.sh`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/.gitignore` & `pygwalker-0.1.7a4/.gitignore`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/LICENSE` & `pygwalker-0.1.7a4/LICENSE`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/README.md` & `pygwalker-0.1.7a4/README.md`

 * *Files identical despite different names*

### Comparing `pygwalker-0.1.7a3/pyproject.toml` & `pygwalker-0.1.7a4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [project]
 name = "pygwalker"
 dynamic = ["version"]
 requires-python = ">=3.6"
 description = "pygwalker: Combining Jupyter Notebook with a Tableau-like UI"
 authors = [ { name = "Asm.Def", email = "woojson@zju.edu.cn" } ]
-license = { file = "LICENSE" }
+license-files = { paths = ["LICENSE"] }
 readme = "README.md"
 keywords = [ 'visualization', 'pandas', 'data-analysis', 'tableau', 'data-exploration', 'dataframe', 'tableau-alternative', 'jupyter' ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
 ]
 dependencies = [
```

