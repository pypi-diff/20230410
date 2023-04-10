# Comparing `tmp/npf-web-extension-0.2.0.tar.gz` & `tmp/npf-web-extension-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npf-web-extension-0.2.0.tar", last modified: Mon Apr 10 16:29:03 2023, max compression
+gzip compressed data, was "npf-web-extension-0.2.1.tar", last modified: Mon Apr 10 17:28:41 2023, max compression
```

## Comparing `npf-web-extension-0.2.0.tar` & `npf-web-extension-0.2.1.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:03.742698 npf-web-extension-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/.env.example
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/.eslintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:03.726698 npf-web-extension-0.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:03.734698 npf-web-extension-0.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-04-10 16:28:55.000000 npf-web-extension-0.2.0/.github/workflows/release_on_pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-10 16:29:03.742698 npf-web-extension-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-10 16:28:55.000000 npf-web-extension-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/craco.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/gulpfile.js
--rw-r--r--   0 runner    (1001) docker     (123)   854639 2023-04-10 16:28:21.000000 npf-web-extension-0.2.0/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:03.738698 npf-web-extension-0.2.0/public/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:03.726698 npf-web-extension-0.2.0/python_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:03.738698 npf-web-extension-0.2.0/python_src/npf_web_extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/python_src/npf_web_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/python_src/npf_web_extension/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:03.738698 npf-web-extension-0.2.0/python_src/npf_web_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-10 16:29:03.000000 npf-web-extension-0.2.0/python_src/npf_web_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-04-10 16:29:03.000000 npf-web-extension-0.2.0/python_src/npf_web_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 16:29:03.000000 npf-web-extension-0.2.0/python_src/npf_web_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-10 16:29:03.000000 npf-web-extension-0.2.0/python_src/npf_web_extension.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 16:29:03.000000 npf-web-extension-0.2.0/python_src/npf_web_extension.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-10 16:29:03.742698 npf-web-extension-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:03.742698 npf-web-extension-0.2.0/src/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/src/App.css
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/src/App.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/src/App.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:03.742698 npf-web-extension-0.2.0/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/src/components/ChartComponent.tsx
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/src/index.tsx
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/src/react-app-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/src/reportWebVitals.ts
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/src/setupTests.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 16:29:03.742698 npf-web-extension-0.2.0/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/src/utils/chart.ts
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/src/utils/data.ts
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/src/utils/events.ts
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/tailwind.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-10 16:28:02.000000 npf-web-extension-0.2.0/workspace.code-workspace
--rw-r--r--   0 runner    (1001) docker     (123)   483043 2023-04-10 16:28:22.000000 npf-web-extension-0.2.0/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:28:41.750000 npf-web-extension-0.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/.env.example
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/.eslintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:28:41.741999 npf-web-extension-0.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:28:41.750000 npf-web-extension-0.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-04-10 17:28:33.000000 npf-web-extension-0.2.1/.github/workflows/release_on_pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-10 17:28:41.750000 npf-web-extension-0.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/craco.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/gulpfile.js
+-rw-r--r--   0 runner    (1001) docker     (123)   844730 2023-04-10 17:28:33.000000 npf-web-extension-0.2.1/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-10 17:28:33.000000 npf-web-extension-0.2.1/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-04-10 17:28:33.000000 npf-web-extension-0.2.1/pre_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:28:41.750000 npf-web-extension-0.2.1/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:28:41.746000 npf-web-extension-0.2.1/python_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:28:41.750000 npf-web-extension-0.2.1/python_src/npf_web_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/python_src/npf_web_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/python_src/npf_web_extension/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:28:41.750000 npf-web-extension-0.2.1/python_src/npf_web_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-04-10 17:28:41.000000 npf-web-extension-0.2.1/python_src/npf_web_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-04-10 17:28:41.000000 npf-web-extension-0.2.1/python_src/npf_web_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 17:28:41.000000 npf-web-extension-0.2.1/python_src/npf_web_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-10 17:28:41.000000 npf-web-extension-0.2.1/python_src/npf_web_extension.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 17:28:41.000000 npf-web-extension-0.2.1/python_src/npf_web_extension.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-10 17:28:41.750000 npf-web-extension-0.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:28:41.750000 npf-web-extension-0.2.1/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/src/App.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/src/App.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:28:41.750000 npf-web-extension-0.2.1/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/src/components/ChartComponent.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/src/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/src/react-app-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/src/reportWebVitals.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/src/setupTests.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 17:28:41.750000 npf-web-extension-0.2.1/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/src/utils/chart.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/src/utils/data.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/src/utils/events.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/tailwind.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-10 17:27:49.000000 npf-web-extension-0.2.1/workspace.code-workspace
+-rw-r--r--   0 runner    (1001) docker     (123)   478174 2023-04-10 17:28:33.000000 npf-web-extension-0.2.1/yarn.lock
```

### Comparing `npf-web-extension-0.2.0/.eslintrc` & `npf-web-extension-0.2.1/.eslintrc`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.0/.github/workflows/build.yml` & `npf-web-extension-0.2.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.0/.github/workflows/release_on_pr.yml` & `npf-web-extension-0.2.1/.github/workflows/release_on_pr.yml`

 * *Files 5% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 
       # Dependencies
       - name: Install Dependencies
         run: npm install
 
       # Building
       - name: Build
-        run: npm run build
+        run: npm run deploy
 
       # Zipping build dir
       - uses: montudor/action-zip@v1
         with:
           args: zip -qq -r release-${{ steps.package-version.outputs.current-version }}.zip build
 
       # Releasing
@@ -71,16 +71,22 @@
           if-no-files-found: error
       
       # Checkout last version
       - uses: actions/checkout@v3
         with:
           ref: v${{ steps.package-version.outputs.current-version }}
 
+      # Preparing package build for pypi
+      - name: Pre-build package
+        run: python3 pre_setup.py
+
       # Building package for pypi
       - name: Building package
         run: python3 -m pip install --upgrade build && python3 -m build
 
       # Publishing to pypi
       - name: Publish package
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
+          verbose: true
+          verify-metadata: false # The twine check version used is not updated and still uses the legacy which doesn't handle gh markdown properly 
           password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `npf-web-extension-0.2.0/LICENSE` & `npf-web-extension-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.0/README.md` & `npf-web-extension-0.2.1/readme.rst`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,58 @@
-# Network Performance Framework Web Extension
+Network Performance Framework Web Extension
+===========================================
 
-This repository is an extension to NPF (<https://github.com/tbarbette/npf>) and should therefore not be used as a standalone tool as the architecture has been built based on npf's internal architecture.
+This repository is an extension to NPF
+(https://github.com/tbarbette/npf) and should therefore not be used as a
+standalone tool as the architecture has been built based on npf's
+internal architecture.
 
-However for more advanced usage, it can be used as a standalone tool. In order to do so, the app has to be initialized by running the following javascript command:
+However for more advanced usage, it can be used as a standalone tool. In
+order to do so, the app has to be initialized by running the following
+javascript command:
 
-```js
-window.updateConfiguration(configuration);
-```
+.. code:: js
 
-where `configuration` follows the type specified inside `src/utils/data.ts`.
+   window.updateConfiguration(configuration);
 
-## Available Scripts
+where ``configuration`` follows the type specified inside
+``src/utils/data.ts``.
 
-### `npm start`
+Available Scripts
+-----------------
 
-Runs the app in development mode available at address `http://localhost:3000`
+``npm start``
+~~~~~~~~~~~~~
 
-### `npm test`
+Runs the app in development mode available at address
+``http://localhost:3000``
+
+``npm test``
+~~~~~~~~~~~~
 
 Will be updated later
 
-### `npm run build`
+``npm run build``
+~~~~~~~~~~~~~~~~~
 
 Builds the app for production and optimizes it.
 
-### `npm run eject` -- DO NOT USE
+``npm run eject`` -- DO NOT USE
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+**Note: this is a one-way operation. Once you ``eject``, you can’t go
+back!** This will be removed in the near future
+
+Releases
+--------
+
+-  V0.2
+
+   -  Inlining all app source codes into a single html file instead of external scripts
+
+-  V0.1.1
 
-**Note: this is a one-way operation. Once you `eject`, you can’t go back!**
-This will be removed in the near future
+   -  PyPi package creation and publishing
 
-## Releases
+-  V0.1
 
-- V0.1
-  - Github actions automatic releases
+   -  Github actions automatic releases
```

### Comparing `npf-web-extension-0.2.0/craco.config.js` & `npf-web-extension-0.2.1/craco.config.js`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.0/gulpfile.js` & `npf-web-extension-0.2.1/gulpfile.js`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.0/package-lock.json` & `npf-web-extension-0.2.1/package-lock.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8987907276380154%*

 * *Differences: {"'packages'": "{'': {'version': '0.2.1', 'devDependencies': {delete: ['copy-files-from-to']}}, "*

 * *               "delete: ['node_modules/axios', 'node_modules/axios/node_modules/form-data', "*

 * *               "'node_modules/charenc', 'node_modules/cjson', 'node_modules/copy-files-from-to', "*

 * *               "'node_modules/copy-files-from-to/node_modules/ansi-styles', "*

 * *               "'node_modules/copy-files-from-to/node_modules/chalk', "*

 * *               "'node_modules/copy-files-from-to/node_modules/cliui', " […]*

```diff
@@ -18,22 +18,21 @@
                 "react-dom": "^18.2.0",
                 "react-scripts": "5.0.1",
                 "typescript": "^4.9.5",
                 "web-vitals": "^2.1.4"
             },
             "devDependencies": {
                 "@craco/craco": "^7.1.0",
-                "copy-files-from-to": "^3.8.0",
                 "gulp": "^4.0.2",
                 "gulp-inline-source": "^4.0.0",
                 "gulp-replace": "^1.1.4",
                 "tailwindcss": "^3.2.6"
             },
             "name": "app",
-            "version": "0.2.0"
+            "version": "0.2.1"
         },
         "node_modules/@adobe/css-tools": {
             "integrity": "sha512-mMVJ/j/GbZ/De4ZHWbQAQO1J6iVnjtZLc9WEdkUQb8S/Bu2cAF2bETXUgMAdvMG3/ngtKmcNBe+Zms9bg6jnQQ==",
             "resolved": "https://registry.npmjs.org/@adobe/css-tools/-/css-tools-4.1.0.tgz",
             "version": "4.1.0"
         },
         "node_modules/@ampproject/remapping": {
@@ -5068,39 +5067,14 @@
             "engines": {
                 "node": ">=4"
             },
             "integrity": "sha512-/BQzOX780JhsxDnPpH4ZiyrJAzcd8AfzFPkv+89veFSr1rcMjuq2JDCwypKaPeB6ljHp9KjXhPpjgCvQlWYuqg==",
             "resolved": "https://registry.npmjs.org/axe-core/-/axe-core-4.6.3.tgz",
             "version": "4.6.3"
         },
-        "node_modules/axios": {
-            "dependencies": {
-                "follow-redirects": "^1.15.0",
-                "form-data": "^4.0.0",
-                "proxy-from-env": "^1.1.0"
-            },
-            "dev": true,
-            "integrity": "sha512-glL/PvG/E+xCWwV8S6nCHcrfg1exGx7vxyUIivIA1iL7BIh6bePylCfVHwp6k13ao7SATxB6imau2kqY+I67kw==",
-            "resolved": "https://registry.npmjs.org/axios/-/axios-1.3.5.tgz",
-            "version": "1.3.5"
-        },
-        "node_modules/axios/node_modules/form-data": {
-            "dependencies": {
-                "asynckit": "^0.4.0",
-                "combined-stream": "^1.0.8",
-                "mime-types": "^2.1.12"
-            },
-            "dev": true,
-            "engines": {
-                "node": ">= 6"
-            },
-            "integrity": "sha512-ETEklSGi5t0QMZuiXoA/Q6vcnxcLQP5vdugSpuAyi6SVGi2clPPp+xgEhuMaHC+zGgn31Kd235W35f7Hykkaww==",
-            "resolved": "https://registry.npmjs.org/form-data/-/form-data-4.0.0.tgz",
-            "version": "4.0.0"
-        },
         "node_modules/axobject-query": {
             "dependencies": {
                 "deep-equal": "^2.0.5"
             },
             "integrity": "sha512-goKlv8DZrK9hUh975fnHzhNIO4jUnFCfv/dszV5VwUGDFjI6vQ2VwoyjYjYNEbBE8AH87TduWP5uyDR1D+Iteg==",
             "resolved": "https://registry.npmjs.org/axobject-query/-/axobject-query-3.1.1.tgz",
             "version": "3.1.1"
@@ -5788,23 +5762,14 @@
             "engines": {
                 "node": ">=10"
             },
             "integrity": "sha512-kWWXztvZ5SBQV+eRgKFeh8q5sLuZY2+8WUIzlxWVTg+oGwY14qylx1KbKzHd8P6ZYkAg0xyIDU9JMHhyJMZ1jw==",
             "resolved": "https://registry.npmjs.org/char-regex/-/char-regex-1.0.2.tgz",
             "version": "1.0.2"
         },
-        "node_modules/charenc": {
-            "dev": true,
-            "engines": {
-                "node": "*"
-            },
-            "integrity": "sha512-yrLQ/yVUFXkzg7EDQsPieE/53+0RlaWTs+wBrvW36cyilJ2SaDWfl4Yj7MtLTXleV9uEKefbAGUPv2/iWSooRA==",
-            "resolved": "https://registry.npmjs.org/charenc/-/charenc-0.0.2.tgz",
-            "version": "0.0.2"
-        },
         "node_modules/chart.js": {
             "dependencies": {
                 "@kurkle/color": "^0.3.0"
             },
             "engines": {
                 "pnpm": "^7.0.0"
             },
@@ -5877,26 +5842,14 @@
             "version": "3.7.1"
         },
         "node_modules/cjs-module-lexer": {
             "integrity": "sha512-cOU9usZw8/dXIXKtwa8pM0OTJQuJkxMN6w30csNRUerHfeQ5R6U3kkU/FtJeIf3M202OHfY2U8ccInBG7/xogA==",
             "resolved": "https://registry.npmjs.org/cjs-module-lexer/-/cjs-module-lexer-1.2.2.tgz",
             "version": "1.2.2"
         },
-        "node_modules/cjson": {
-            "dependencies": {
-                "json-parse-helpfulerror": "^1.0.3"
-            },
-            "dev": true,
-            "engines": {
-                "node": ">= 0.3.0"
-            },
-            "integrity": "sha512-D3CKJU9YnZNyerUQ1IzNUvMnToP3MGC2XbIAPi/7yqunJJW3rBwCVapousoFtaR9IbejeEM0KIshxC1n4HQcXw==",
-            "resolved": "https://registry.npmjs.org/cjson/-/cjson-0.5.0.tgz",
-            "version": "0.5.0"
-        },
         "node_modules/class-utils": {
             "dependencies": {
                 "arr-union": "^3.1.0",
                 "define-property": "^0.2.5",
                 "isobject": "^3.0.0",
                 "static-extend": "^0.1.1"
             },
@@ -6418,166 +6371,14 @@
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-XgZ0pFcakEUlbwQEVNg3+QAis1FyTL3Qel9FYy8pSkQqoG3PNoT0bOCQtOXcOkur21r2Eq2kI+IE+gsmAEVlYw==",
             "resolved": "https://registry.npmjs.org/copy-descriptor/-/copy-descriptor-0.1.1.tgz",
             "version": "0.1.1"
         },
-        "node_modules/copy-files-from-to": {
-            "bin": {
-                "copy-files-from-to": "index.js"
-            },
-            "dependencies": {
-                "async": "^3.2.4",
-                "axios": "^1.2.4",
-                "chalk": "=4.1.2",
-                "cjson": "^0.5.0",
-                "fast-glob": "^3.2.12",
-                "glob-parent": "^6.0.2",
-                "is-glob": "^4.0.3",
-                "is-utf8": "^0.2.1",
-                "lodash": "^4.17.21",
-                "md5": "^2.3.0",
-                "mkdirp": "^2.1.3",
-                "note-down": "0.2.3",
-                "terser": "^5.16.1",
-                "unixify": "^1.0.0",
-                "yargs": "^17.6.2"
-            },
-            "dev": true,
-            "integrity": "sha512-jhAB2eOup138hl3iRmThap5R9ymiVDOUfvWbgEr3MDN4xneyru/XJC+qY/ROCljC4asmAd459pv7yIfHFutD+w==",
-            "resolved": "https://registry.npmjs.org/copy-files-from-to/-/copy-files-from-to-3.8.0.tgz",
-            "version": "3.8.0"
-        },
-        "node_modules/copy-files-from-to/node_modules/ansi-styles": {
-            "dependencies": {
-                "color-convert": "^2.0.1"
-            },
-            "dev": true,
-            "engines": {
-                "node": ">=8"
-            },
-            "funding": {
-                "url": "https://github.com/chalk/ansi-styles?sponsor=1"
-            },
-            "integrity": "sha512-zbB9rCJAT1rbjiVDb2hqKFHNYLxgtk8NURxZ3IZwD3F6NtxbXZQCnnSi1Lkx+IDohdPlFp222wVALIheZJQSEg==",
-            "resolved": "https://registry.npmjs.org/ansi-styles/-/ansi-styles-4.3.0.tgz",
-            "version": "4.3.0"
-        },
-        "node_modules/copy-files-from-to/node_modules/chalk": {
-            "dependencies": {
-                "ansi-styles": "^4.1.0",
-                "supports-color": "^7.1.0"
-            },
-            "dev": true,
-            "engines": {
-                "node": ">=10"
-            },
-            "funding": {
-                "url": "https://github.com/chalk/chalk?sponsor=1"
-            },
-            "integrity": "sha512-oKnbhFyRIXpUuez8iBMmyEa4nbj4IOQyuhc/wy9kY7/WVPcwIO9VA668Pu8RkO7+0G76SLROeyw9CpQ061i4mA==",
-            "resolved": "https://registry.npmjs.org/chalk/-/chalk-4.1.2.tgz",
-            "version": "4.1.2"
-        },
-        "node_modules/copy-files-from-to/node_modules/cliui": {
-            "dependencies": {
-                "string-width": "^4.2.0",
-                "strip-ansi": "^6.0.1",
-                "wrap-ansi": "^7.0.0"
-            },
-            "dev": true,
-            "engines": {
-                "node": ">=12"
-            },
-            "integrity": "sha512-BSeNnyus75C4//NQ9gQt1/csTXyo/8Sb+afLAkzAptFuMsod9HFokGNudZpi/oQV73hnVK+sR+5PVRMd+Dr7YQ==",
-            "resolved": "https://registry.npmjs.org/cliui/-/cliui-8.0.1.tgz",
-            "version": "8.0.1"
-        },
-        "node_modules/copy-files-from-to/node_modules/color-convert": {
-            "dependencies": {
-                "color-name": "~1.1.4"
-            },
-            "dev": true,
-            "engines": {
-                "node": ">=7.0.0"
-            },
-            "integrity": "sha512-RRECPsj7iu/xb5oKYcsFHSppFNnsj/52OVTRKb4zP5onXwVF3zVmmToNcOfGC+CRDpfK/U584fMg38ZHCaElKQ==",
-            "resolved": "https://registry.npmjs.org/color-convert/-/color-convert-2.0.1.tgz",
-            "version": "2.0.1"
-        },
-        "node_modules/copy-files-from-to/node_modules/color-name": {
-            "dev": true,
-            "integrity": "sha512-dOy+3AuW3a2wNbZHIuMZpTcgjGuLU/uBL/ubcZF9OXbDo8ff4O8yVp5Bf0efS8uEoYo5q4Fx7dY9OgQGXgAsQA==",
-            "resolved": "https://registry.npmjs.org/color-name/-/color-name-1.1.4.tgz",
-            "version": "1.1.4"
-        },
-        "node_modules/copy-files-from-to/node_modules/has-flag": {
-            "dev": true,
-            "engines": {
-                "node": ">=8"
-            },
-            "integrity": "sha512-EykJT/Q1KjTWctppgIAgfSO0tKVuZUjhgMr17kqTumMl6Afv3EISleU7qZUzoXDFTAHTDC4NOoG/ZxU3EvlMPQ==",
-            "resolved": "https://registry.npmjs.org/has-flag/-/has-flag-4.0.0.tgz",
-            "version": "4.0.0"
-        },
-        "node_modules/copy-files-from-to/node_modules/mkdirp": {
-            "bin": {
-                "mkdirp": "dist/cjs/src/bin.js"
-            },
-            "dev": true,
-            "engines": {
-                "node": ">=10"
-            },
-            "funding": {
-                "url": "https://github.com/sponsors/isaacs"
-            },
-            "integrity": "sha512-+hEnITedc8LAtIP9u3HJDFIdcLV2vXP33sqLLIzkv1Db1zO/1OxbvYf0Y1OC/S/Qo5dxHXepofhmxL02PsKe+A==",
-            "resolved": "https://registry.npmjs.org/mkdirp/-/mkdirp-2.1.6.tgz",
-            "version": "2.1.6"
-        },
-        "node_modules/copy-files-from-to/node_modules/supports-color": {
-            "dependencies": {
-                "has-flag": "^4.0.0"
-            },
-            "dev": true,
-            "engines": {
-                "node": ">=8"
-            },
-            "integrity": "sha512-qpCAvRl9stuOHveKsn7HncJRvv501qIacKzQlO/+Lwxc9+0q2wLyv4Dfvt80/DPn2pqOBsJdDiogXGR9+OvwRw==",
-            "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-7.2.0.tgz",
-            "version": "7.2.0"
-        },
-        "node_modules/copy-files-from-to/node_modules/yargs": {
-            "dependencies": {
-                "cliui": "^8.0.1",
-                "escalade": "^3.1.1",
-                "get-caller-file": "^2.0.5",
-                "require-directory": "^2.1.1",
-                "string-width": "^4.2.3",
-                "y18n": "^5.0.5",
-                "yargs-parser": "^21.1.1"
-            },
-            "dev": true,
-            "engines": {
-                "node": ">=12"
-            },
-            "integrity": "sha512-cwiTb08Xuv5fqF4AovYacTFNxk62th7LKJ6BL9IGUpTJrWoU7/7WdQGTP2SjKf1dUNBGzDd28p/Yfs/GI6JrLw==",
-            "resolved": "https://registry.npmjs.org/yargs/-/yargs-17.7.1.tgz",
-            "version": "17.7.1"
-        },
-        "node_modules/copy-files-from-to/node_modules/yargs-parser": {
-            "dev": true,
-            "engines": {
-                "node": ">=12"
-            },
-            "integrity": "sha512-tVpsJW7DdjecAiFpbIB1e3qxIQsE6NoPc5/eTdrbbIC4h0LVsWhnoa3g+m2HclBIujHzsxZ4VJVA+GUuc2/LBw==",
-            "resolved": "https://registry.npmjs.org/yargs-parser/-/yargs-parser-21.1.1.tgz",
-            "version": "21.1.1"
-        },
         "node_modules/copy-props": {
             "dependencies": {
                 "each-props": "^1.3.2",
                 "is-plain-object": "^5.0.0"
             },
             "dev": true,
             "integrity": "sha512-XBlx8HSqrT0ObQwmSzM7WE5k8FxTV75h1DX1Z3n6NhQ/UYYAvInWYmG06vFt7hQZArE2fuO62aihiWIVQwh1sw==",
@@ -6670,23 +6471,14 @@
             "engines": {
                 "node": ">= 8"
             },
             "integrity": "sha512-iRDPJKUPVEND7dHPO8rkbOnPpyDygcDFtWjpeWNCgy8WP2rXcxXL8TskReQl6OrB2G7+UJrags1q15Fudc7G6w==",
             "resolved": "https://registry.npmjs.org/cross-spawn/-/cross-spawn-7.0.3.tgz",
             "version": "7.0.3"
         },
-        "node_modules/crypt": {
-            "dev": true,
-            "engines": {
-                "node": "*"
-            },
-            "integrity": "sha512-mCxBlsHFYh9C+HVpiEacem8FEBnMXgU9gy4zmNC+SXAZNB/1idgp/aulFJ4FgCi7GPEVbfyng092GqL2k2rmow==",
-            "resolved": "https://registry.npmjs.org/crypt/-/crypt-0.0.2.tgz",
-            "version": "0.0.2"
-        },
         "node_modules/crypto-random-string": {
             "engines": {
                 "node": ">=8"
             },
             "integrity": "sha512-v1plID3y9r/lPhviJ1wrXpLeyUIGAZ2SHNYTEapm7/8A9nLPoyvVp3RK/EPFqn5kEznyWgYZNsRtYYIWbuG8KA==",
             "resolved": "https://registry.npmjs.org/crypto-random-string/-/crypto-random-string-2.0.0.tgz",
             "version": "2.0.0"
@@ -14118,20 +13910,14 @@
             "funding": {
                 "url": "https://github.com/chalk/supports-color?sponsor=1"
             },
             "integrity": "sha512-MpUEN2OodtUzxvKQl72cUF7RQ5EiHsGvSsVG0ia9c5RbWGL2CI4C7EpPS8UTBIplnlzZiNuV56w+FuNxy3ty2Q==",
             "resolved": "https://registry.npmjs.org/supports-color/-/supports-color-8.1.1.tgz",
             "version": "8.1.1"
         },
-        "node_modules/jju": {
-            "dev": true,
-            "integrity": "sha512-8wb9Yw966OSxApiCt0K3yNJL8pnNeIv+OEq2YMidz4FKP6nonSRoOXc80iXY4JaN2FC11B9qsNmDsm+ZOfMROA==",
-            "resolved": "https://registry.npmjs.org/jju/-/jju-1.4.0.tgz",
-            "version": "1.4.0"
-        },
         "node_modules/js-sdsl": {
             "funding": {
                 "type": "opencollective",
                 "url": "https://opencollective.com/js-sdsl"
             },
             "integrity": "sha512-mifzlm2+5nZ+lEcLJMoBK0/IH/bDg8XnJfd/Wq6IP+xoCjLZsTOnV2QpxlVbX9bMnkl5PdEjNtBJ9Cj1NjifhQ==",
             "resolved": "https://registry.npmjs.org/js-sdsl/-/js-sdsl-4.3.0.tgz",
@@ -14211,23 +13997,14 @@
             "version": "2.5.2"
         },
         "node_modules/json-parse-even-better-errors": {
             "integrity": "sha512-xyFwyhro/JEof6Ghe2iz2NcXoj2sloNsWr/XsERDK/oiPCfaNhl5ONfp+jQdAZRQQ0IJWNzH9zIZF7li91kh2w==",
             "resolved": "https://registry.npmjs.org/json-parse-even-better-errors/-/json-parse-even-better-errors-2.3.1.tgz",
             "version": "2.3.1"
         },
-        "node_modules/json-parse-helpfulerror": {
-            "dependencies": {
-                "jju": "^1.1.0"
-            },
-            "dev": true,
-            "integrity": "sha512-XgP0FGR77+QhUxjXkwOMkC94k3WtqEBfcnjWqhRd82qTat4SWKRE+9kUnynz/shm3I4ea2+qISvTIeGTNU7kJg==",
-            "resolved": "https://registry.npmjs.org/json-parse-helpfulerror/-/json-parse-helpfulerror-1.0.3.tgz",
-            "version": "1.0.3"
-        },
         "node_modules/json-schema": {
             "integrity": "sha512-es94M3nTIfsEPisRafak+HDLfHXnKBhV3vU5eqPcS3flIWqcxJWgXHXiey3YrpaNsanY5ei1VoYEbOzijuq9BA==",
             "resolved": "https://registry.npmjs.org/json-schema/-/json-schema-0.4.0.tgz",
             "version": "0.4.0"
         },
         "node_modules/json-schema-traverse": {
             "integrity": "sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==",
@@ -14858,25 +14635,14 @@
             "engines": {
                 "node": ">=0.10.0"
             },
             "integrity": "sha512-ZZWNfCjUokXXDGXFpZehJIkZqq91BcULFq/Pi7M5i4JnxXdhMKAK682z8bCW3o8Hj1wuuzoKcW3DfVzaP6VuNg==",
             "resolved": "https://registry.npmjs.org/to-regex-range/-/to-regex-range-2.1.1.tgz",
             "version": "2.1.1"
         },
-        "node_modules/md5": {
-            "dependencies": {
-                "charenc": "0.0.2",
-                "crypt": "0.0.2",
-                "is-buffer": "~1.1.6"
-            },
-            "dev": true,
-            "integrity": "sha512-T1GITYmFaKuO91vxyoQMFETst+O71VUPEU3ze5GNzDm0OWdP8v1ziTaAEPUr/3kLsY3Sftgz242A1SetQiDL7g==",
-            "resolved": "https://registry.npmjs.org/md5/-/md5-2.3.0.tgz",
-            "version": "2.3.0"
-        },
         "node_modules/mdn-data": {
             "integrity": "sha512-iV3XNKw06j5Q7mi6h+9vbx23Tv7JkjEVgKHW4pimwyDGWm0OIQntJJ+u1C6mg6mK1EaTv42XQ7w76yuzH7M2cA==",
             "resolved": "https://registry.npmjs.org/mdn-data/-/mdn-data-2.0.4.tgz",
             "version": "2.0.4"
         },
         "node_modules/media-typer": {
             "engines": {
@@ -15262,23 +15028,14 @@
             "funding": {
                 "url": "https://github.com/sponsors/sindresorhus"
             },
             "integrity": "sha512-DlL+XwOy3NxAQ8xuC0okPgK46iuVNAK01YN7RueYBqqFeGsBjV9XmCAzAdgt+667bCl5kPh9EqKKDwnaPG1I7A==",
             "resolved": "https://registry.npmjs.org/normalize-url/-/normalize-url-6.1.0.tgz",
             "version": "6.1.0"
         },
-        "node_modules/note-down": {
-            "dependencies": {
-                "chalk": "^2.4.2"
-            },
-            "dev": true,
-            "integrity": "sha512-ozp9z0FQyAmTS4NGTw/wmPxkJ8zKuhsiK70yQIfmGV7PMwJ84OEdr8cj+0WC874xxBhsFYx3jxX+mORsQaCs4w==",
-            "resolved": "https://registry.npmjs.org/note-down/-/note-down-0.2.3.tgz",
-            "version": "0.2.3"
-        },
         "node_modules/now-and-later": {
             "dependencies": {
                 "once": "^1.3.2"
             },
             "dev": true,
             "engines": {
                 "node": ">= 0.10"
@@ -17455,20 +17212,14 @@
             "engines": {
                 "node": ">= 0.10"
             },
             "integrity": "sha512-0KI/607xoxSToH7GjN1FfSbLoU0+btTicjsQSWQlh/hZykN8KpmMf7uYwPW3R+akZ6R/w18ZlXSHBYXiYUPO3g==",
             "resolved": "https://registry.npmjs.org/ipaddr.js/-/ipaddr.js-1.9.1.tgz",
             "version": "1.9.1"
         },
-        "node_modules/proxy-from-env": {
-            "dev": true,
-            "integrity": "sha512-D+zkORCbA9f1tdWRK0RaCR3GPv50cMxcrz4X8k5LTSUD1Dkw47mKJEZQNunItRTkWwgtaUSo1RVFRIG9ZXiFYg==",
-            "resolved": "https://registry.npmjs.org/proxy-from-env/-/proxy-from-env-1.1.0.tgz",
-            "version": "1.1.0"
-        },
         "node_modules/psl": {
             "integrity": "sha512-E/ZsdU4HLs/68gYzgGTkMicWTLPdAftJLfJFlLUAAKZGkStNU72sZjT66SnMDVOfOWY/YAoiD7Jxa9iHvngcag==",
             "resolved": "https://registry.npmjs.org/psl/-/psl-1.9.0.tgz",
             "version": "1.9.0"
         },
         "node_modules/pump": {
             "dependencies": {
@@ -20715,38 +20466,14 @@
             "engines": {
                 "node": ">= 10.0.0"
             },
             "integrity": "sha512-hAZsKq7Yy11Zu1DE0OzWjw7nnLZmJZYTDZZyEFHZdUhV8FkH5MCfoU1XMaxXovpyW5nq5scPqq0ZDP9Zyl04oQ==",
             "resolved": "https://registry.npmjs.org/universalify/-/universalify-2.0.0.tgz",
             "version": "2.0.0"
         },
-        "node_modules/unixify": {
-            "dependencies": {
-                "normalize-path": "^2.1.1"
-            },
-            "dev": true,
-            "engines": {
-                "node": ">=0.10.0"
-            },
-            "integrity": "sha512-6bc58dPYhCMHHuwxldQxO3RRNZ4eCogZ/st++0+fcC1nr0jiGUtAdBJ2qzmLQWSxbtz42pWt4QQMiZ9HvZf5cg==",
-            "resolved": "https://registry.npmjs.org/unixify/-/unixify-1.0.0.tgz",
-            "version": "1.0.0"
-        },
-        "node_modules/unixify/node_modules/normalize-path": {
-            "dependencies": {
-                "remove-trailing-separator": "^1.0.1"
-            },
-            "dev": true,
-            "engines": {
-                "node": ">=0.10.0"
-            },
-            "integrity": "sha512-3pKJwH184Xo/lnH6oyP1q2pMd7HcypqqmRs91/6/i2CGtWwIKGCkOOMTm/zXbgTEWHw1uNpNi/igc3ePOYHb6w==",
-            "resolved": "https://registry.npmjs.org/normalize-path/-/normalize-path-2.1.1.tgz",
-            "version": "2.1.1"
-        },
         "node_modules/unpipe": {
             "engines": {
                 "node": ">= 0.8"
             },
             "integrity": "sha512-pjy2bYhSsufwWlKwPc+l3cN7+wuJlK6uz0YdJEOlQDbl6jo/YlPi4mb8agUkVC8BF7V8NuzeyPNqRksA3hztKQ==",
             "resolved": "https://registry.npmjs.org/unpipe/-/unpipe-1.0.0.tgz",
             "version": "1.0.0"
@@ -22071,9 +21798,9 @@
             },
             "integrity": "sha512-rVksvsnNCdJ/ohGc6xgPwyN8eheCxsiLM8mxuE/t/mOVqJewPuO1miLpTHQiRgTKCLexL4MeAFVagts7HmNZ2Q==",
             "resolved": "https://registry.npmjs.org/yocto-queue/-/yocto-queue-0.1.0.tgz",
             "version": "0.1.0"
         }
     },
     "requires": true,
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `npf-web-extension-0.2.0/package.json` & `npf-web-extension-0.2.1/package.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7606060606060606%*

 * *Differences: {"'devDependencies'": "{delete: ['copy-files-from-to']}",*

 * * "'scripts'": "{'deploy': 'npm run build && npx gulp'}",*

 * * "'version'": "'0.2.1'",*

 * * 'delete': "['copyFiles', 'copyFilesSettings']"}*

```diff
@@ -7,23 +7,14 @@
         ],
         "production": [
             ">0.2%",
             "not dead",
             "not op_mini all"
         ]
     },
-    "copyFiles": [
-        {
-            "from": "build/index.html",
-            "to": "index.html"
-        }
-    ],
-    "copyFilesSettings": {
-        "whenFileExists": "overwrite"
-    },
     "dependencies": {
         "@testing-library/jest-dom": "^5.16.5",
         "@testing-library/react": "^13.4.0",
         "@testing-library/user-event": "^13.5.0",
         "@types/jest": "^27.5.2",
         "@types/node": "^16.18.12",
         "@types/react": "^18.0.27",
@@ -35,15 +26,14 @@
         "react-dom": "^18.2.0",
         "react-scripts": "5.0.1",
         "typescript": "^4.9.5",
         "web-vitals": "^2.1.4"
     },
     "devDependencies": {
         "@craco/craco": "^7.1.0",
-        "copy-files-from-to": "^3.8.0",
         "gulp": "^4.0.2",
         "gulp-inline-source": "^4.0.0",
         "gulp-replace": "^1.1.4",
         "tailwindcss": "^3.2.6"
     },
     "eslintConfig": {
         "extends": [
@@ -52,14 +42,14 @@
         ]
     },
     "homepage": ".",
     "name": "app",
     "private": true,
     "scripts": {
         "build": "craco build",
-        "deploy": "npm run build && npx gulp && npx copyfiles build/index.html index.html",
+        "deploy": "npm run build && npx gulp",
         "eject": "react-scripts eject",
         "start": "react-scripts start",
         "test": "react-scripts test"
     },
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `npf-web-extension-0.2.0/public/index.html` & `npf-web-extension-0.2.1/public/index.html`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.0/python_src/npf_web_extension/app.py` & `npf-web-extension-0.2.1/python_src/npf_web_extension/app.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
 import json
-import shutil
 import sys
 from argparse import ArgumentParser
 from importlib.metadata import version
+import os
+import shutil
 
+# Getting package directory
+package_directory = os.path.dirname(os.path.abspath(__file__))
+template_path = os.path.join(package_directory, "template.py")
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("-v", "--version", action="store_true")
 
     args = parser.parse_args()
 
@@ -15,34 +19,34 @@
         print(version("npf-web-extension"))
         sys.exit()
 
 
 def _prepare(outdir):
 
     # Configuration
-    file_path = "index.html"
+    output_path = f"{outdir}/index.html"
 
     # Copying app to outdir
-    shutil.copy(file_path, f"{outdir}/{file_path}")
+    shutil.copy(template_path, output_path)
 
     
 def _hydrate(configuration, outdir):
 
     # Configuration
     file_path = f"{outdir}/index.html"
     insertion_point = "<!-- NPF_CONFIG_INSERTION -->"
     js_snippet = f'\t<script type="text/javascript">setTimeout(() => window.updateConfiguration({json.dumps(configuration)}), 2500)</script>'
 
     # Replacing the insertion point with the js_snippet
-    with open(file_path, 'r') as file:
+    with open(file_path, 'r', encoding='utf-8') as file:
         file_contents = file.read()
 
     new_contents = file_contents.replace(insertion_point, js_snippet)
 
-    with open(file_path, 'w') as file:
+    with open(file_path, 'w', encoding='utf-8') as file:
         # Write the modified contents to the file
         file.write(new_contents)
 
 
 def export(configuration, outdir):
     
     _prepare(outdir)
```

### Comparing `npf-web-extension-0.2.0/python_src/npf_web_extension.egg-info/SOURCES.txt` & `npf-web-extension-0.2.1/python_src/npf_web_extension.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 .env.example
 .eslintrc
 .gitignore
 .prettierrc
 LICENSE
-MANIFEST.in
 README.md
 craco.config.js
 gulpfile.js
 package-lock.json
 package.json
+pre_setup.py
 pyproject.toml
+readme.rst
 setup.cfg
 tailwind.config.js
 tsconfig.json
 workspace.code-workspace
 yarn.lock
 .github/workflows/build.yml
 .github/workflows/release_on_pr.yml
```

### Comparing `npf-web-extension-0.2.0/setup.cfg` & `npf-web-extension-0.2.1/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 [metadata]
 name = npf-web-extension
 description = NPF Web extension designed to export results to a single html web app
-long_description_content_type = file: README.md
+long_description = file: README.md
+long_description_content_type = text/markdown
 url = https://github.com/dpcodebiz/npf-web-extension
 project_urls = 
 	Bug Tracker = https://github.com/dpcodebiz/npf-web-extension/issues
 	Changelog = https://github.com/dpcodebiz/npf-web-extension/releases
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: BSD License
```

### Comparing `npf-web-extension-0.2.0/src/App.css` & `npf-web-extension-0.2.1/src/App.css`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.0/src/App.tsx` & `npf-web-extension-0.2.1/src/App.tsx`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.0/src/components/ChartComponent.tsx` & `npf-web-extension-0.2.1/src/components/ChartComponent.tsx`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.0/src/index.tsx` & `npf-web-extension-0.2.1/src/index.tsx`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.0/src/utils/chart.ts` & `npf-web-extension-0.2.1/src/utils/chart.ts`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.0/workspace.code-workspace` & `npf-web-extension-0.2.1/workspace.code-workspace`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.0/yarn.lock` & `npf-web-extension-0.2.1/yarn.lock`

 * *Files 0% similar despite different names*

```diff
@@ -2832,15 +2832,15 @@
 async-settle@^1.0.0:
   version "1.0.0"
   resolved "https://registry.npmjs.org/async-settle/-/async-settle-1.0.0.tgz"
   integrity sha512-VPXfB4Vk49z1LHHodrEQ6Xf7W4gg1w0dAPROHngx7qgDjqmIQ+fXmwgGXTW/ITLai0YLSvWepJOP9EVpMnEAcw==
   dependencies:
     async-done "^1.2.2"
 
-async@^3.2.3, async@^3.2.4:
+async@^3.2.3:
   version "3.2.4"
   resolved "https://registry.npmjs.org/async/-/async-3.2.4.tgz"
   integrity sha512-iAB+JbDEGXhyIUavoDl9WP/Jj106Kz9DEn1DPgYw5ruDn0e3Wgi3sKFm55sASdGBNOQB8F59d9qQ7deqrHA8wQ==
 
 asynckit@^0.4.0:
   version "0.4.0"
   resolved "https://registry.npmjs.org/asynckit/-/asynckit-0.4.0.tgz"
@@ -2874,23 +2874,14 @@
   integrity sha512-DMD0KiN46eipeziST1LPP/STfDU0sufISXmjSgvVsoU2tqxctQeASejWcfNtxYKqETM1UxQ8sp2OrSBWpHY6sw==
 
 axe-core@^4.6.2:
   version "4.6.3"
   resolved "https://registry.npmjs.org/axe-core/-/axe-core-4.6.3.tgz"
   integrity sha512-/BQzOX780JhsxDnPpH4ZiyrJAzcd8AfzFPkv+89veFSr1rcMjuq2JDCwypKaPeB6ljHp9KjXhPpjgCvQlWYuqg==
 
-axios@^1.2.4:
-  version "1.3.5"
-  resolved "https://registry.npmjs.org/axios/-/axios-1.3.5.tgz"
-  integrity sha512-glL/PvG/E+xCWwV8S6nCHcrfg1exGx7vxyUIivIA1iL7BIh6bePylCfVHwp6k13ao7SATxB6imau2kqY+I67kw==
-  dependencies:
-    follow-redirects "^1.15.0"
-    form-data "^4.0.0"
-    proxy-from-env "^1.1.0"
-
 axobject-query@^3.1.1:
   version "3.1.1"
   resolved "https://registry.npmjs.org/axobject-query/-/axobject-query-3.1.1.tgz"
   integrity sha512-goKlv8DZrK9hUh975fnHzhNIO4jUnFCfv/dszV5VwUGDFjI6vQ2VwoyjYjYNEbBE8AH87TduWP5uyDR1D+Iteg==
   dependencies:
     deep-equal "^2.0.5"
 
@@ -3293,15 +3284,15 @@
   integrity sha512-XY7UbUpGRatZzoRft//5xOa69/1iGJRBlrieH6QYrkKLIFn3m7OVEJ81dSrKoy2BnKsdbX5cLrOispZNYo9v2w==
 
 case-sensitive-paths-webpack-plugin@^2.4.0:
   version "2.4.0"
   resolved "https://registry.npmjs.org/case-sensitive-paths-webpack-plugin/-/case-sensitive-paths-webpack-plugin-2.4.0.tgz"
   integrity sha512-roIFONhcxog0JSSWbvVAh3OocukmSgpqOH6YpMkCvav/ySIV3JKg4Dc8vYtQjYi/UxpNE36r/9v+VqTQqgkYmw==
 
-chalk@^2.0.0, chalk@^2.4.1, chalk@^2.4.2:
+chalk@^2.0.0, chalk@^2.4.1:
   version "2.4.2"
   resolved "https://registry.npmjs.org/chalk/-/chalk-2.4.2.tgz"
   integrity sha512-Mti+f9lpJNcwF4tWV8/OrTTtF1gZi+f8FqlyAdouralcFWFQWF2+NgCHShjkCb+IFBLq9buZwE1xckQU4peSuQ==
   dependencies:
     ansi-styles "^3.2.1"
     escape-string-regexp "^1.0.5"
     supports-color "^5.3.0"
@@ -3342,37 +3333,24 @@
   version "4.1.2"
   resolved "https://registry.npmjs.org/chalk/-/chalk-4.1.2.tgz"
   integrity sha512-oKnbhFyRIXpUuez8iBMmyEa4nbj4IOQyuhc/wy9kY7/WVPcwIO9VA668Pu8RkO7+0G76SLROeyw9CpQ061i4mA==
   dependencies:
     ansi-styles "^4.1.0"
     supports-color "^7.1.0"
 
-chalk@=4.1.2:
-  version "4.1.2"
-  resolved "https://registry.npmjs.org/chalk/-/chalk-4.1.2.tgz"
-  integrity sha512-oKnbhFyRIXpUuez8iBMmyEa4nbj4IOQyuhc/wy9kY7/WVPcwIO9VA668Pu8RkO7+0G76SLROeyw9CpQ061i4mA==
-  dependencies:
-    ansi-styles "^4.1.0"
-    supports-color "^7.1.0"
-
 char-regex@^1.0.2:
   version "1.0.2"
   resolved "https://registry.npmjs.org/char-regex/-/char-regex-1.0.2.tgz"
   integrity sha512-kWWXztvZ5SBQV+eRgKFeh8q5sLuZY2+8WUIzlxWVTg+oGwY14qylx1KbKzHd8P6ZYkAg0xyIDU9JMHhyJMZ1jw==
 
 char-regex@^2.0.0:
   version "2.0.1"
   resolved "https://registry.npmjs.org/char-regex/-/char-regex-2.0.1.tgz"
   integrity sha512-oSvEeo6ZUD7NepqAat3RqoucZ5SeqLJgOvVIwkafu6IP3V0pO38s/ypdVUmDDK6qIIHNlYHJAKX9E7R7HoKElw==
 
-charenc@0.0.2:
-  version "0.0.2"
-  resolved "https://registry.npmjs.org/charenc/-/charenc-0.0.2.tgz"
-  integrity sha512-yrLQ/yVUFXkzg7EDQsPieE/53+0RlaWTs+wBrvW36cyilJ2SaDWfl4Yj7MtLTXleV9uEKefbAGUPv2/iWSooRA==
-
 chart.js@^4.1.1, chart.js@^4.2.1:
   version "4.2.1"
   resolved "https://registry.npmjs.org/chart.js/-/chart.js-4.2.1.tgz"
   integrity sha512-6YbpQ0nt3NovAgOzbkSSeeAQu/3za1319dPUQTXn9WcOpywM8rGKxJHrhS8V8xEkAlk8YhEfjbuAPfUyp6jIsw==
   dependencies:
     "@kurkle/color" "^0.3.0"
 
@@ -3426,21 +3404,14 @@
   integrity sha512-4jYS4MOAaCIStSRwiuxc4B8MYhIe676yO1sYGzARnjXkWpmzZMMYxY6zu8WYWDhSuth5zhrQ1rhNSibyyvv4/w==
 
 cjs-module-lexer@^1.0.0:
   version "1.2.2"
   resolved "https://registry.npmjs.org/cjs-module-lexer/-/cjs-module-lexer-1.2.2.tgz"
   integrity sha512-cOU9usZw8/dXIXKtwa8pM0OTJQuJkxMN6w30csNRUerHfeQ5R6U3kkU/FtJeIf3M202OHfY2U8ccInBG7/xogA==
 
-cjson@^0.5.0:
-  version "0.5.0"
-  resolved "https://registry.npmjs.org/cjson/-/cjson-0.5.0.tgz"
-  integrity sha512-D3CKJU9YnZNyerUQ1IzNUvMnToP3MGC2XbIAPi/7yqunJJW3rBwCVapousoFtaR9IbejeEM0KIshxC1n4HQcXw==
-  dependencies:
-    json-parse-helpfulerror "^1.0.3"
-
 class-utils@^0.3.5:
   version "0.3.6"
   resolved "https://registry.npmjs.org/class-utils/-/class-utils-0.3.6.tgz"
   integrity sha512-qOhPa/Fj7s6TY8H8esGu5QNpMMQxz79h+urzrNYN6mn+9BnxlDGf5QZ+XeCDsxSjPqsSR56XOZOJmpeurnLMeg==
   dependencies:
     arr-union "^3.1.0"
     define-property "^0.2.5"
@@ -3468,23 +3439,14 @@
   resolved "https://registry.npmjs.org/cliui/-/cliui-7.0.4.tgz"
   integrity sha512-OcRE68cOsVMXp1Yvonl/fzkQOyjLSu/8bhPDfQt0e0/Eb283TKP20Fs2MqoPsr9SwA595rRCA+QMzYc9nBP+JQ==
   dependencies:
     string-width "^4.2.0"
     strip-ansi "^6.0.0"
     wrap-ansi "^7.0.0"
 
-cliui@^8.0.1:
-  version "8.0.1"
-  resolved "https://registry.npmjs.org/cliui/-/cliui-8.0.1.tgz"
-  integrity sha512-BSeNnyus75C4//NQ9gQt1/csTXyo/8Sb+afLAkzAptFuMsod9HFokGNudZpi/oQV73hnVK+sR+5PVRMd+Dr7YQ==
-  dependencies:
-    string-width "^4.2.0"
-    strip-ansi "^6.0.1"
-    wrap-ansi "^7.0.0"
-
 clone-buffer@^1.0.0:
   version "1.0.0"
   resolved "https://registry.npmjs.org/clone-buffer/-/clone-buffer-1.0.0.tgz"
   integrity sha512-KLLTJWrvwIP+OPfMn0x2PheDEP20RPUcGXj/ERegTgdmPEZylALQldygiqrPPu8P45uNuPs7ckmReLY6v/iA5g==
 
 clone-deep@^4.0.1:
   version "4.0.1"
@@ -3724,35 +3686,14 @@
   integrity sha512-LDx6oHrK+PhzLKJU9j5S7/Y3jM/mUHvD/DeI1WQmJn652iPC5Y4TBzC9l+5OMOXlyTTA+SmVUPm0HQUwpD5Jqw==
 
 copy-descriptor@^0.1.0:
   version "0.1.1"
   resolved "https://registry.npmjs.org/copy-descriptor/-/copy-descriptor-0.1.1.tgz"
   integrity sha512-XgZ0pFcakEUlbwQEVNg3+QAis1FyTL3Qel9FYy8pSkQqoG3PNoT0bOCQtOXcOkur21r2Eq2kI+IE+gsmAEVlYw==
 
-copy-files-from-to@^3.8.0:
-  version "3.8.0"
-  resolved "https://registry.npmjs.org/copy-files-from-to/-/copy-files-from-to-3.8.0.tgz"
-  integrity sha512-jhAB2eOup138hl3iRmThap5R9ymiVDOUfvWbgEr3MDN4xneyru/XJC+qY/ROCljC4asmAd459pv7yIfHFutD+w==
-  dependencies:
-    async "^3.2.4"
-    axios "^1.2.4"
-    chalk "=4.1.2"
-    cjson "^0.5.0"
-    fast-glob "^3.2.12"
-    glob-parent "^6.0.2"
-    is-glob "^4.0.3"
-    is-utf8 "^0.2.1"
-    lodash "^4.17.21"
-    md5 "^2.3.0"
-    mkdirp "^2.1.3"
-    note-down "0.2.3"
-    terser "^5.16.1"
-    unixify "^1.0.0"
-    yargs "^17.6.2"
-
 copy-props@^2.0.1:
   version "2.0.5"
   resolved "https://registry.npmjs.org/copy-props/-/copy-props-2.0.5.tgz"
   integrity sha512-XBlx8HSqrT0ObQwmSzM7WE5k8FxTV75h1DX1Z3n6NhQ/UYYAvInWYmG06vFt7hQZArE2fuO62aihiWIVQwh1sw==
   dependencies:
     each-props "^1.3.2"
     is-plain-object "^5.0.0"
@@ -3819,19 +3760,14 @@
   resolved "https://registry.npmjs.org/cross-spawn/-/cross-spawn-7.0.3.tgz"
   integrity sha512-iRDPJKUPVEND7dHPO8rkbOnPpyDygcDFtWjpeWNCgy8WP2rXcxXL8TskReQl6OrB2G7+UJrags1q15Fudc7G6w==
   dependencies:
     path-key "^3.1.0"
     shebang-command "^2.0.0"
     which "^2.0.1"
 
-crypt@0.0.2:
-  version "0.0.2"
-  resolved "https://registry.npmjs.org/crypt/-/crypt-0.0.2.tgz"
-  integrity sha512-mCxBlsHFYh9C+HVpiEacem8FEBnMXgU9gy4zmNC+SXAZNB/1idgp/aulFJ4FgCi7GPEVbfyng092GqL2k2rmow==
-
 crypto-random-string@^2.0.0:
   version "2.0.0"
   resolved "https://registry.npmjs.org/crypto-random-string/-/crypto-random-string-2.0.0.tgz"
   integrity sha512-v1plID3y9r/lPhviJ1wrXpLeyUIGAZ2SHNYTEapm7/8A9nLPoyvVp3RK/EPFqn5kEznyWgYZNsRtYYIWbuG8KA==
 
 css-blank-pseudo@^3.0.3:
   version "3.0.3"
@@ -5361,15 +5297,15 @@
   version "1.1.1"
   resolved "https://registry.npmjs.org/flush-write-stream/-/flush-write-stream-1.1.1.tgz"
   integrity sha512-3Z4XhFZ3992uIq0XOqb9AreonueSYphE6oYbpt5+3u06JWklbsPkNv3ZKkP9Bz/r+1MWCaMoSQ28P85+1Yc77w==
   dependencies:
     inherits "^2.0.3"
     readable-stream "^2.3.6"
 
-follow-redirects@^1.0.0, follow-redirects@^1.15.0:
+follow-redirects@^1.0.0:
   version "1.15.2"
   resolved "https://registry.npmjs.org/follow-redirects/-/follow-redirects-1.15.2.tgz"
   integrity sha512-VQLG33o04KaQ8uYi2tVNbdrWp1QWxNNea+nmIB4EVM28v0hmP17z7aG1+wAkNzVq4KeXTq3221ye5qTJP91JwA==
 
 for-each@^0.3.3:
   version "0.3.3"
   resolved "https://registry.npmjs.org/for-each/-/for-each-0.3.3.tgz"
@@ -5422,23 +5358,14 @@
   resolved "https://registry.npmjs.org/form-data/-/form-data-3.0.1.tgz"
   integrity sha512-RHkBKtLWUVwd7SqRIvCZMEvAMoGUp0XU+seQiZejj0COz3RI3hWP4sCv3gZWWLjJTd7rGwcsF5eKZGii0r/hbg==
   dependencies:
     asynckit "^0.4.0"
     combined-stream "^1.0.8"
     mime-types "^2.1.12"
 
-form-data@^4.0.0:
-  version "4.0.0"
-  resolved "https://registry.npmjs.org/form-data/-/form-data-4.0.0.tgz"
-  integrity sha512-ETEklSGi5t0QMZuiXoA/Q6vcnxcLQP5vdugSpuAyi6SVGi2clPPp+xgEhuMaHC+zGgn31Kd235W35f7Hykkaww==
-  dependencies:
-    asynckit "^0.4.0"
-    combined-stream "^1.0.8"
-    mime-types "^2.1.12"
-
 formidable@^1.2.1:
   version "1.2.6"
   resolved "https://registry.npmjs.org/formidable/-/formidable-1.2.6.tgz"
   integrity sha512-KcpbcpuLNOwrEjnbpMC0gS+X8ciDoZE1kkqzat4a8vrprf+s9pKNQ/QIwWfbfs4ltgmFl3MD177SNTkve3BwGQ==
 
 forwarded@0.2.0:
   version "0.2.0"
@@ -6269,15 +6196,15 @@
   version "1.1.2"
   resolved "https://registry.npmjs.org/is-boolean-object/-/is-boolean-object-1.1.2.tgz"
   integrity sha512-gDYaKHJmnj4aWxyj6YHyXVpdQawtVLHU5cb+eztPGczf6cjuTdwve5ZIEfgXqH4e57An1D1AKf8CZ3kYrQRqYA==
   dependencies:
     call-bind "^1.0.2"
     has-tostringtag "^1.0.0"
 
-is-buffer@^1.1.5, is-buffer@~1.1.6:
+is-buffer@^1.1.5:
   version "1.1.6"
   resolved "https://registry.npmjs.org/is-buffer/-/is-buffer-1.1.6.tgz"
   integrity sha512-NcdALwpXkTm5Zvvbk7owOUSvVvBKDgKP5/ewfXEznmQFfs4ZRmanOeKBTjRVjka3QFoN6XJ+9F3USqfHqTaU5w==
 
 is-callable@^1.1.3, is-callable@^1.1.4, is-callable@^1.2.7:
   version "1.2.7"
   resolved "https://registry.npmjs.org/is-callable/-/is-callable-1.2.7.tgz"
@@ -7168,19 +7095,14 @@
   resolved "https://registry.npmjs.org/jest/-/jest-27.5.1.tgz"
   integrity sha512-Yn0mADZB89zTtjkPJEXwrac3LHudkQMR+Paqa8uxJHCBr9agxztUifWCyiYrjhMPBoUVBjyny0I7XH6ozDr7QQ==
   dependencies:
     "@jest/core" "^27.5.1"
     import-local "^3.0.2"
     jest-cli "^27.5.1"
 
-jju@^1.1.0:
-  version "1.4.0"
-  resolved "https://registry.npmjs.org/jju/-/jju-1.4.0.tgz"
-  integrity sha512-8wb9Yw966OSxApiCt0K3yNJL8pnNeIv+OEq2YMidz4FKP6nonSRoOXc80iXY4JaN2FC11B9qsNmDsm+ZOfMROA==
-
 js-sdsl@^4.1.4:
   version "4.3.0"
   resolved "https://registry.npmjs.org/js-sdsl/-/js-sdsl-4.3.0.tgz"
   integrity sha512-mifzlm2+5nZ+lEcLJMoBK0/IH/bDg8XnJfd/Wq6IP+xoCjLZsTOnV2QpxlVbX9bMnkl5PdEjNtBJ9Cj1NjifhQ==
 
 "js-tokens@^3.0.0 || ^4.0.0", js-tokens@^4.0.0:
   version "4.0.0"
@@ -7246,21 +7168,14 @@
   integrity sha512-uZz5UnB7u4T9LvwmFqXii7pZSouaRPorGs5who1Ip7VO0wxanFvBL7GkM6dTHlgX+jhBApRetaWpnDabOeTcnA==
 
 json-parse-even-better-errors@^2.3.0, json-parse-even-better-errors@^2.3.1:
   version "2.3.1"
   resolved "https://registry.npmjs.org/json-parse-even-better-errors/-/json-parse-even-better-errors-2.3.1.tgz"
   integrity sha512-xyFwyhro/JEof6Ghe2iz2NcXoj2sloNsWr/XsERDK/oiPCfaNhl5ONfp+jQdAZRQQ0IJWNzH9zIZF7li91kh2w==
 
-json-parse-helpfulerror@^1.0.3:
-  version "1.0.3"
-  resolved "https://registry.npmjs.org/json-parse-helpfulerror/-/json-parse-helpfulerror-1.0.3.tgz"
-  integrity sha512-XgP0FGR77+QhUxjXkwOMkC94k3WtqEBfcnjWqhRd82qTat4SWKRE+9kUnynz/shm3I4ea2+qISvTIeGTNU7kJg==
-  dependencies:
-    jju "^1.1.0"
-
 json-schema-traverse@^0.4.1:
   version "0.4.1"
   resolved "https://registry.npmjs.org/json-schema-traverse/-/json-schema-traverse-0.4.1.tgz"
   integrity sha512-xbbCH5dCYU5T8LcEhhuh7HJ88HXuW3qsI3Y0zOZFKfZEHcpWiHU/Jxzk629Brsab/mMiHQti9wMP+845RPe3Vg==
 
 json-schema-traverse@^1.0.0:
   version "1.0.0"
@@ -7614,23 +7529,14 @@
   integrity sha512-LFgVbaHIHMqCRuCZyfCtUOq9/Lnzhi7Z0KFUE2fhD54+JN2jLh3hC02RLkqauJ3U4soU6H1J3tfj/Byk7GoEjA==
   dependencies:
     findup-sync "^2.0.0"
     micromatch "^3.0.4"
     resolve "^1.4.0"
     stack-trace "0.0.10"
 
-md5@^2.3.0:
-  version "2.3.0"
-  resolved "https://registry.npmjs.org/md5/-/md5-2.3.0.tgz"
-  integrity sha512-T1GITYmFaKuO91vxyoQMFETst+O71VUPEU3ze5GNzDm0OWdP8v1ziTaAEPUr/3kLsY3Sftgz242A1SetQiDL7g==
-  dependencies:
-    charenc "0.0.2"
-    crypt "0.0.2"
-    is-buffer "~1.1.6"
-
 mdn-data@~1.1.0:
   version "1.1.4"
   resolved "https://registry.npmjs.org/mdn-data/-/mdn-data-1.1.4.tgz"
   integrity sha512-FSYbp3lyKjyj3E7fMl6rYvUdX0FBXaluGqlFoYESWQlyUTq8R+wp0rkFxoYFqZlHCvsUXGjyJmLQSnXToYhOSA==
 
 mdn-data@2.0.14:
   version "2.0.14"
@@ -7787,19 +7693,14 @@
   version "1.3.2"
   resolved "https://registry.npmjs.org/mixin-deep/-/mixin-deep-1.3.2.tgz"
   integrity sha512-WRoDn//mXBiJ1H40rqa3vH0toePwSsGb45iInWlTySa+Uu4k3tYUSxa2v1KqAiLtvlrSzaExqS1gtk96A9zvEA==
   dependencies:
     for-in "^1.0.2"
     is-extendable "^1.0.1"
 
-mkdirp@^2.1.3:
-  version "2.1.6"
-  resolved "https://registry.npmjs.org/mkdirp/-/mkdirp-2.1.6.tgz"
-  integrity sha512-+hEnITedc8LAtIP9u3HJDFIdcLV2vXP33sqLLIzkv1Db1zO/1OxbvYf0Y1OC/S/Qo5dxHXepofhmxL02PsKe+A==
-
 mkdirp@~0.5.1:
   version "0.5.6"
   resolved "https://registry.npmjs.org/mkdirp/-/mkdirp-0.5.6.tgz"
   integrity sha512-FP+p8RB8OWpF3YZBCrP5gtADmtXApB5AMLn+vdyA+PyxCjrCs00mjyUozssO33cwDeT3wNGdLxJ5M//YqtHAJw==
   dependencies:
     minimist "^1.2.6"
 
@@ -7929,21 +7830,14 @@
   integrity sha512-bdok/XvKII3nUpklnV6P2hxtMNrCboOjAcyBuQnWEhO665FwrSNRxU+AqpsyvO6LgGYPspN+lu5CLtw4jPRKNA==
 
 normalize-url@^6.0.1:
   version "6.1.0"
   resolved "https://registry.npmjs.org/normalize-url/-/normalize-url-6.1.0.tgz"
   integrity sha512-DlL+XwOy3NxAQ8xuC0okPgK46iuVNAK01YN7RueYBqqFeGsBjV9XmCAzAdgt+667bCl5kPh9EqKKDwnaPG1I7A==
 
-note-down@0.2.3:
-  version "0.2.3"
-  resolved "https://registry.npmjs.org/note-down/-/note-down-0.2.3.tgz"
-  integrity sha512-ozp9z0FQyAmTS4NGTw/wmPxkJ8zKuhsiK70yQIfmGV7PMwJ84OEdr8cj+0WC874xxBhsFYx3jxX+mORsQaCs4w==
-  dependencies:
-    chalk "^2.4.2"
-
 now-and-later@^2.0.0:
   version "2.0.1"
   resolved "https://registry.npmjs.org/now-and-later/-/now-and-later-2.0.1.tgz"
   integrity sha512-KGvQ0cB70AQfg107Xvs/Fbu+dGmZoTRJp2TaPwcwQm3/7PteUyN2BCgk8KBMPGBUXZdVwyWS8fDCGFygBm19UQ==
   dependencies:
     once "^1.3.2"
 
@@ -9088,19 +8982,14 @@
   version "2.0.7"
   resolved "https://registry.npmjs.org/proxy-addr/-/proxy-addr-2.0.7.tgz"
   integrity sha512-llQsMLSUDUPT44jdrU/O37qlnifitDP+ZwrmmZcoSKyLKvtZxpyV0n2/bD/N4tBAAZ/gJEdZU7KMraoK1+XYAg==
   dependencies:
     forwarded "0.2.0"
     ipaddr.js "1.9.1"
 
-proxy-from-env@^1.1.0:
-  version "1.1.0"
-  resolved "https://registry.npmjs.org/proxy-from-env/-/proxy-from-env-1.1.0.tgz"
-  integrity sha512-D+zkORCbA9f1tdWRK0RaCR3GPv50cMxcrz4X8k5LTSUD1Dkw47mKJEZQNunItRTkWwgtaUSo1RVFRIG9ZXiFYg==
-
 psl@^1.1.33:
   version "1.9.0"
   resolved "https://registry.npmjs.org/psl/-/psl-1.9.0.tgz"
   integrity sha512-E/ZsdU4HLs/68gYzgGTkMicWTLPdAftJLfJFlLUAAKZGkStNU72sZjT66SnMDVOfOWY/YAoiD7Jxa9iHvngcag==
 
 pump@^2.0.0:
   version "2.0.1"
@@ -10383,15 +10272,15 @@
   resolved "https://registry.npmjs.org/string-width/-/string-width-1.0.2.tgz"
   integrity sha512-0XsVpQLnVCXHJfyEs8tC0zpTVIr5PKKsQtkT29IwupnPTjtPmQ3xT/4yCREF9hYkV/3M3kzcUTSAZT6a6h81tw==
   dependencies:
     code-point-at "^1.0.0"
     is-fullwidth-code-point "^1.0.0"
     strip-ansi "^3.0.0"
 
-string-width@^4.1.0, string-width@^4.2.0, string-width@^4.2.3:
+string-width@^4.1.0, string-width@^4.2.0:
   version "4.2.3"
   resolved "https://registry.npmjs.org/string-width/-/string-width-4.2.3.tgz"
   integrity sha512-wKyQRQpjJ0sIp62ErSZdGsjMJWsap5oRNihHhu6G7JVO/9jIB6UyevL+tXuOqrng8j/cxKTWyWUwvSTriiZz/g==
   dependencies:
     emoji-regex "^8.0.0"
     is-fullwidth-code-point "^3.0.0"
     strip-ansi "^6.0.1"
@@ -10707,15 +10596,15 @@
   dependencies:
     "@jridgewell/trace-mapping" "^0.3.14"
     jest-worker "^27.4.5"
     schema-utils "^3.1.1"
     serialize-javascript "^6.0.0"
     terser "^5.14.1"
 
-terser@^5.0.0, terser@^5.10.0, terser@^5.14.1, terser@^5.16.1:
+terser@^5.0.0, terser@^5.10.0, terser@^5.14.1:
   version "5.16.3"
   resolved "https://registry.npmjs.org/terser/-/terser-5.16.3.tgz"
   integrity sha512-v8wWLaS/xt3nE9dgKEWhNUFP6q4kngO5B8eYFUuebsu7Dw/UNAnpUod6UHo04jSSkv8TzKHjZDSd7EXdDQAl8Q==
   dependencies:
     "@jridgewell/source-map" "^0.3.2"
     acorn "^8.5.0"
     commander "^2.20.0"
@@ -11085,21 +10974,14 @@
   integrity sha512-CJ1QgKmNg3CwvAv/kOFmtnEN05f0D/cn9QntgNOQlQF9dgvVTHj3t+8JPdjqawCHk7V/KA+fbUqzZ9XWhcqPUg==
 
 universalify@^2.0.0:
   version "2.0.0"
   resolved "https://registry.npmjs.org/universalify/-/universalify-2.0.0.tgz"
   integrity sha512-hAZsKq7Yy11Zu1DE0OzWjw7nnLZmJZYTDZZyEFHZdUhV8FkH5MCfoU1XMaxXovpyW5nq5scPqq0ZDP9Zyl04oQ==
 
-unixify@^1.0.0:
-  version "1.0.0"
-  resolved "https://registry.npmjs.org/unixify/-/unixify-1.0.0.tgz"
-  integrity sha512-6bc58dPYhCMHHuwxldQxO3RRNZ4eCogZ/st++0+fcC1nr0jiGUtAdBJ2qzmLQWSxbtz42pWt4QQMiZ9HvZf5cg==
-  dependencies:
-    normalize-path "^2.1.1"
-
 unpipe@~1.0.0, unpipe@1.0.0:
   version "1.0.0"
   resolved "https://registry.npmjs.org/unpipe/-/unpipe-1.0.0.tgz"
   integrity sha512-pjy2bYhSsufwWlKwPc+l3cN7+wuJlK6uz0YdJEOlQDbl6jo/YlPi4mb8agUkVC8BF7V8NuzeyPNqRksA3hztKQ==
 
 unquote@~1.1.1:
   version "1.1.1"
@@ -11808,19 +11690,14 @@
   integrity sha512-r3vXyErRCYJ7wg28yvBY5VSoAF8ZvlcW9/BwUzEtUsjvX/DKs24dIkuwjtuprwJJHsbyUbLApepYTR1BN4uHrg==
 
 yargs-parser@^20.2.2, yargs-parser@>=5.0.0-security.0:
   version "20.2.9"
   resolved "https://registry.npmjs.org/yargs-parser/-/yargs-parser-20.2.9.tgz"
   integrity sha512-y11nGElTIV+CT3Zv9t7VKl+Q3hTQoT9a1Qzezhhl6Rp21gJ/IVTW7Z3y9EWXhuUBC2Shnf+DX0antecpAwSP8w==
 
-yargs-parser@^21.1.1:
-  version "21.1.1"
-  resolved "https://registry.npmjs.org/yargs-parser/-/yargs-parser-21.1.1.tgz"
-  integrity sha512-tVpsJW7DdjecAiFpbIB1e3qxIQsE6NoPc5/eTdrbbIC4h0LVsWhnoa3g+m2HclBIujHzsxZ4VJVA+GUuc2/LBw==
-
 yargs-parser@^5.0.1:
   version "5.0.1"
   resolved "https://registry.npmjs.org/yargs-parser/-/yargs-parser-5.0.1.tgz"
   integrity sha512-wpav5XYiddjXxirPoCTUPbqM0PXvJ9hiBMvuJgInvo4/lAOTZzUprArw17q2O1P2+GHhbBr18/iQwjL5Z9BqfA==
   dependencies:
     camelcase "^3.0.0"
     object.assign "^4.1.0"
@@ -11834,27 +11711,14 @@
     escalade "^3.1.1"
     get-caller-file "^2.0.5"
     require-directory "^2.1.1"
     string-width "^4.2.0"
     y18n "^5.0.5"
     yargs-parser "^20.2.2"
 
-yargs@^17.6.2:
-  version "17.7.1"
-  resolved "https://registry.npmjs.org/yargs/-/yargs-17.7.1.tgz"
-  integrity sha512-cwiTb08Xuv5fqF4AovYacTFNxk62th7LKJ6BL9IGUpTJrWoU7/7WdQGTP2SjKf1dUNBGzDd28p/Yfs/GI6JrLw==
-  dependencies:
-    cliui "^8.0.1"
-    escalade "^3.1.1"
-    get-caller-file "^2.0.5"
-    require-directory "^2.1.1"
-    string-width "^4.2.3"
-    y18n "^5.0.5"
-    yargs-parser "^21.1.1"
-
 yargs@^7.1.0:
   version "7.1.2"
   resolved "https://registry.npmjs.org/yargs/-/yargs-7.1.2.tgz"
   integrity sha512-ZEjj/dQYQy0Zx0lgLMLR8QuaqTihnxirir7EwUHp1Axq4e3+k8jXU5K0VLbNvedv1f4EWtBonDIZm0NUr+jCcA==
   dependencies:
     camelcase "^3.0.0"
     cliui "^3.2.0"
```

