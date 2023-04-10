# Comparing `tmp/npf-web-extension-0.2.2.tar.gz` & `tmp/npf-web-extension-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "npf-web-extension-0.2.2.tar", last modified: Mon Apr 10 18:02:49 2023, max compression
+gzip compressed data, was "npf-web-extension-0.2.3.tar", last modified: Mon Apr 10 21:46:18 2023, max compression
```

## Comparing `npf-web-extension-0.2.2.tar` & `npf-web-extension-0.2.3.tar`

### file list

```diff
@@ -1,50 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:02:49.035929 npf-web-extension-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/.env.example
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/.eslintrc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:02:49.023928 npf-web-extension-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:02:49.031928 npf-web-extension-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3083 2023-04-10 18:02:38.000000 npf-web-extension-0.2.2/.github/workflows/release_on_pr.yml
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/.prettierrc
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-10 18:02:49.035929 npf-web-extension-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/craco.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/gulpfile.js
--rw-r--r--   0 runner    (1001) docker     (123)   854145 2023-04-10 18:02:37.000000 npf-web-extension-0.2.2/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:02:49.031928 npf-web-extension-0.2.2/public/
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/public/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:02:49.027928 npf-web-extension-0.2.2/python_src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:02:49.031928 npf-web-extension-0.2.2/python_src/npf_web_extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/python_src/npf_web_extension/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/python_src/npf_web_extension/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:02:49.035929 npf-web-extension-0.2.2/python_src/npf_web_extension.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-10 18:02:48.000000 npf-web-extension-0.2.2/python_src/npf_web_extension.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-10 18:02:49.000000 npf-web-extension-0.2.2/python_src/npf_web_extension.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 18:02:48.000000 npf-web-extension-0.2.2/python_src/npf_web_extension.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-10 18:02:48.000000 npf-web-extension-0.2.2/python_src/npf_web_extension.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 18:02:48.000000 npf-web-extension-0.2.2/python_src/npf_web_extension.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-10 18:02:49.039929 npf-web-extension-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:02:49.035929 npf-web-extension-0.2.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/src/App.css
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/src/App.test.tsx
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/src/App.tsx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:02:49.035929 npf-web-extension-0.2.2/src/components/
--rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/src/components/ChartComponent.tsx
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/src/index.css
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/src/index.tsx
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/src/react-app-env.d.ts
--rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/src/reportWebVitals.ts
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/src/setupTests.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 18:02:49.035929 npf-web-extension-0.2.2/src/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/src/utils/chart.ts
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/src/utils/data.ts
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/src/utils/events.ts
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/tailwind.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/tsconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-10 18:01:36.000000 npf-web-extension-0.2.2/workspace.code-workspace
--rw-r--r--   0 runner    (1001) docker     (123)   483043 2023-04-10 18:02:05.000000 npf-web-extension-0.2.2/yarn.lock
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:46:18.978119 npf-web-extension-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/.env.example
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/.eslintrc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:46:18.970119 npf-web-extension-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:46:18.978119 npf-web-extension-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3704 2023-04-10 21:46:05.000000 npf-web-extension-0.2.3/.github/workflows/release_on_pr.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/.prettierrc
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-10 21:46:18.978119 npf-web-extension-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/craco.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/gulpfile.js
+-rw-r--r--   0 runner    (1001) docker     (123)   854145 2023-04-10 21:46:05.000000 npf-web-extension-0.2.3/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1542 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:46:18.978119 npf-web-extension-0.2.3/public/
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:46:18.974119 npf-web-extension-0.2.3/python_src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:46:18.978119 npf-web-extension-0.2.3/python_src/npf_web_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/python_src/npf_web_extension/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1470 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/python_src/npf_web_extension/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)   373013 2023-04-10 21:45:58.000000 npf-web-extension-0.2.3/python_src/npf_web_extension/template.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:46:18.978119 npf-web-extension-0.2.3/python_src/npf_web_extension.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-04-10 21:46:18.000000 npf-web-extension-0.2.3/python_src/npf_web_extension.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-04-10 21:46:18.000000 npf-web-extension-0.2.3/python_src/npf_web_extension.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 21:46:18.000000 npf-web-extension-0.2.3/python_src/npf_web_extension.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-10 21:46:18.000000 npf-web-extension-0.2.3/python_src/npf_web_extension.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-04-10 21:46:18.000000 npf-web-extension-0.2.3/python_src/npf_web_extension.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-10 21:46:18.982119 npf-web-extension-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:46:18.978119 npf-web-extension-0.2.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/src/App.css
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/src/App.test.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/src/App.tsx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:46:18.978119 npf-web-extension-0.2.3/src/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     3438 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/src/components/ChartComponent.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/src/index.tsx
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/src/react-app-env.d.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/src/reportWebVitals.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/src/setupTests.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 21:46:18.978119 npf-web-extension-0.2.3/src/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/src/utils/chart.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/src/utils/data.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/src/utils/events.ts
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/tailwind.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/tsconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-04-10 21:45:14.000000 npf-web-extension-0.2.3/workspace.code-workspace
+-rw-r--r--   0 runner    (1001) docker     (123)   483043 2023-04-10 21:45:34.000000 npf-web-extension-0.2.3/yarn.lock
```

### Comparing `npf-web-extension-0.2.2/.eslintrc` & `npf-web-extension-0.2.3/.eslintrc`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/.github/workflows/build.yml` & `npf-web-extension-0.2.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/.github/workflows/release_on_pr.yml` & `npf-web-extension-0.2.3/.github/workflows/release_on_pr.yml`

 * *Files 11% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 
 jobs:
   release:
     permissions: write-all
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
+        with:
+          token: ${{ secrets.PAT }}
 
       # Getting package version
       - name: get-npm-version
         id: package-version
         uses: martinbeentjes/npm-get-version-action@main
       
       # Node modules cache
@@ -46,14 +48,24 @@
         run: npm run deploy
 
       # Zipping build dir
       # - uses: montudor/action-zip@v1
       #   with:
       #     args: zip -qq -r release-${{ steps.package-version.outputs.current-version }}.zip build
 
+      # Uploading template.html to repo
+      - name: Upload template.html to repo
+        uses: EndBug/add-and-commit@v9
+        with:
+          add: 'python_src/npf_web_extension/template.html'
+          commit: --signoff
+          default_author: github_actions
+          fetch: false
+          pathspec_error_handling: exitImmediately
+
       # Releasing
       - name: Create Release
         id: create_release
         uses: ncipollo/release-action@v1.12.0
         with:
           tag: v${{ steps.package-version.outputs.current-version }}
           name: Release ${{ steps.package-version.outputs.current-version }}
@@ -63,36 +75,44 @@
           allowUpdates: true
           token: ${{ secrets.PAT }}
 
       # Uploading release
       - name: Upload Release Assets
         uses: actions/upload-artifact@v3
         with:
-          name: index.html
+          name: template.html
           path: build/index.html
           if-no-files-found: error
       
       # Checkout last version
       - uses: actions/checkout@v3
         with:
           ref: v${{ steps.package-version.outputs.current-version }}
       
       # Download release after checkout
-      - uses: actions/download-artifact@v3
-        with:
-          name: index.html
-          path: python_src/npf_web_extension/template.py
+      # - uses: actions/download-artifact@v3
+      #   with:
+      #     name: template.html
+      #     path: python_src/npf_web_extension/template.html
 
       # Building package for pypi
       - name: Building package
         run: python3 -m pip install --upgrade build && python3 -m build
       
       # Debug
       - name: Debug
         run: ls -la python_src/npf_web_extension/
+      
+      # Upload package artifact
+      - name: Upload PyPi Package artifact
+        uses: actions/upload-artifact@v3
+        with:
+          name: build
+          path: dist
+          if-no-files-found: error
 
       # Publishing to pypi
       # - name: Publish package
       #   uses: pypa/gh-action-pypi-publish@release/v1
       #   with:
       #     verbose: true
       #     verify-metadata: false # The twine check version used is not updated and still uses the legacy which doesn't handle gh markdown properly
```

### Comparing `npf-web-extension-0.2.2/LICENSE` & `npf-web-extension-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/PKG-INFO` & `npf-web-extension-0.2.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npf-web-extension
-Version: 0.2.2
+Version: 0.2.3
 Summary: NPF Web extension designed to export results to a single html web app
 Home-page: https://github.com/dpcodebiz/npf-web-extension
 Project-URL: Bug Tracker, https://github.com/dpcodebiz/npf-web-extension/issues
 Project-URL: Changelog, https://github.com/dpcodebiz/npf-web-extension/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
@@ -41,14 +41,17 @@
 ### `npm run eject` -- DO NOT USE
 
 **Note: this is a one-way operation. Once you `eject`, you can’t go back!**
 This will be removed in the near future
 
 ## Releases
 
+- V0.2.3
+  - Added automatic build and commit to repo of template to fix it not being included properly.
+  - Renamed template.py to template.html
 - V0.2.2
   - Fixed checkout reset when building with github actions
 - V0.2.1
   - Fixed html file not being included properly. Added prebuild script.
 - V0.2
   - Inlining all app source codes into a single html file instead of external scripts
 - V0.1.1
```

### Comparing `npf-web-extension-0.2.2/README.md` & `npf-web-extension-0.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -27,14 +27,17 @@
 ### `npm run eject` -- DO NOT USE
 
 **Note: this is a one-way operation. Once you `eject`, you can’t go back!**
 This will be removed in the near future
 
 ## Releases
 
+- V0.2.3
+  - Added automatic build and commit to repo of template to fix it not being included properly.
+  - Renamed template.py to template.html
 - V0.2.2
   - Fixed checkout reset when building with github actions
 - V0.2.1
   - Fixed html file not being included properly. Added prebuild script.
 - V0.2
   - Inlining all app source codes into a single html file instead of external scripts
 - V0.1.1
```

### Comparing `npf-web-extension-0.2.2/craco.config.js` & `npf-web-extension-0.2.3/craco.config.js`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/gulpfile.js` & `npf-web-extension-0.2.3/gulpfile.js`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/package-lock.json` & `npf-web-extension-0.2.3/package-lock.json`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/package.json` & `npf-web-extension-0.2.3/package.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9431818181818182%*

 * *Differences: {"'copyFiles'": "{0: {'to': 'python_src/npf_web_extension/template.html'}}", "'version'": "'0.2.3'"}*

```diff
@@ -10,15 +10,15 @@
             "not dead",
             "not op_mini all"
         ]
     },
     "copyFiles": [
         {
             "from": "build/index.html",
-            "to": "python_src/npf_web_extension/template.py"
+            "to": "python_src/npf_web_extension/template.html"
         }
     ],
     "copyFilesSettings": {
         "whenFileExists": "overwrite"
     },
     "dependencies": {
         "@testing-library/jest-dom": "^5.16.5",
@@ -57,9 +57,9 @@
     "scripts": {
         "build": "craco build",
         "deploy": "npm run build && npx gulp && npx copy-files-from-to",
         "eject": "react-scripts eject",
         "start": "react-scripts start",
         "test": "react-scripts test"
     },
-    "version": "0.2.2"
+    "version": "0.2.3"
 }
```

### Comparing `npf-web-extension-0.2.2/public/index.html` & `npf-web-extension-0.2.3/public/index.html`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/python_src/npf_web_extension/app.py` & `npf-web-extension-0.2.3/python_src/npf_web_extension/app.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from argparse import ArgumentParser
 from importlib.metadata import version
 import os
 import shutil
 
 # Getting package directory
 package_directory = os.path.dirname(os.path.abspath(__file__))
-template_path = os.path.join(package_directory, "template.py")
+template_path = os.path.join(package_directory, "template.html")
 
 def main():
     parser = ArgumentParser()
     parser.add_argument("-v", "--version", action="store_true")
 
     args = parser.parse_args()
```

### Comparing `npf-web-extension-0.2.2/python_src/npf_web_extension.egg-info/PKG-INFO` & `npf-web-extension-0.2.3/python_src/npf_web_extension.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: npf-web-extension
-Version: 0.2.2
+Version: 0.2.3
 Summary: NPF Web extension designed to export results to a single html web app
 Home-page: https://github.com/dpcodebiz/npf-web-extension
 Project-URL: Bug Tracker, https://github.com/dpcodebiz/npf-web-extension/issues
 Project-URL: Changelog, https://github.com/dpcodebiz/npf-web-extension/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
@@ -41,14 +41,17 @@
 ### `npm run eject` -- DO NOT USE
 
 **Note: this is a one-way operation. Once you `eject`, you can’t go back!**
 This will be removed in the near future
 
 ## Releases
 
+- V0.2.3
+  - Added automatic build and commit to repo of template to fix it not being included properly.
+  - Renamed template.py to template.html
 - V0.2.2
   - Fixed checkout reset when building with github actions
 - V0.2.1
   - Fixed html file not being included properly. Added prebuild script.
 - V0.2
   - Inlining all app source codes into a single html file instead of external scripts
 - V0.1.1
```

### Comparing `npf-web-extension-0.2.2/python_src/npf_web_extension.egg-info/SOURCES.txt` & `npf-web-extension-0.2.3/python_src/npf_web_extension.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 workspace.code-workspace
 yarn.lock
 .github/workflows/build.yml
 .github/workflows/release_on_pr.yml
 public/index.html
 python_src/npf_web_extension/__init__.py
 python_src/npf_web_extension/app.py
-python_src/npf_web_extension/template.py
+python_src/npf_web_extension/template.html
 python_src/npf_web_extension.egg-info/PKG-INFO
 python_src/npf_web_extension.egg-info/SOURCES.txt
 python_src/npf_web_extension.egg-info/dependency_links.txt
 python_src/npf_web_extension.egg-info/entry_points.txt
 python_src/npf_web_extension.egg-info/top_level.txt
 src/App.css
 src/App.test.tsx
```

### Comparing `npf-web-extension-0.2.2/readme.rst` & `npf-web-extension-0.2.3/readme.rst`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/setup.cfg` & `npf-web-extension-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/src/App.css` & `npf-web-extension-0.2.3/src/App.css`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/src/App.tsx` & `npf-web-extension-0.2.3/src/App.tsx`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/src/components/ChartComponent.tsx` & `npf-web-extension-0.2.3/src/components/ChartComponent.tsx`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/src/index.tsx` & `npf-web-extension-0.2.3/src/index.tsx`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/src/utils/chart.ts` & `npf-web-extension-0.2.3/src/utils/chart.ts`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/workspace.code-workspace` & `npf-web-extension-0.2.3/workspace.code-workspace`

 * *Files identical despite different names*

### Comparing `npf-web-extension-0.2.2/yarn.lock` & `npf-web-extension-0.2.3/yarn.lock`

 * *Files identical despite different names*

