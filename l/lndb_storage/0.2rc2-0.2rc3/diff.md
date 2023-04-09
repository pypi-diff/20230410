# Comparing `tmp/lndb_storage-0.2rc2.tar.gz` & `tmp/lndb_storage-0.2rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lndb_storage-0.2rc2.tar", last modified: Sun Mar 26 19:28:26 2023, max compression
+gzip compressed data, was "lndb_storage-0.2rc3.tar", last modified: Sun Apr  9 22:17:27 2023, max compression
```

## Comparing `lndb_storage-0.2rc2.tar` & `lndb_storage-0.2rc3.tar`

### file list

```diff
@@ -1,39 +1,34 @@
--rw-r--r--   0        0        0     3055 2023-03-14 18:15:14.149651 lndb_storage-0.2rc2/.github/workflows/build.yml
--rw-r--r--   0        0        0      135 2022-11-13 16:42:34.073467 lndb_storage-0.2rc2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      622 2022-11-13 16:42:34.079466 lndb_storage-0.2rc2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1307 2022-11-13 16:42:34.087464 lndb_storage-0.2rc2/.gitignore
--rw-r--r--   0        0        0     1822 2022-11-13 16:42:34.094465 lndb_storage-0.2rc2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11525 2022-11-13 16:42:34.107465 lndb_storage-0.2rc2/LICENSE
--rw-r--r--   0        0        0      255 2022-11-13 16:42:34.115466 lndb_storage-0.2rc2/README.md
--rw-r--r--   0        0        0       59 2022-11-13 16:42:34.121466 lndb_storage-0.2rc2/docs/api.md
--rw-r--r--   0        0        0     1289 2023-03-26 19:27:49.050952 lndb_storage-0.2rc2/docs/changelog.md
--rw-r--r--   0        0        0      851 2022-11-13 16:42:34.131464 lndb_storage-0.2rc2/docs/examples/YYYY-MM-DD-task-slug.ipynb
--rw-r--r--   0        0        0      218 2022-11-13 16:42:34.138496 lndb_storage-0.2rc2/docs/examples/index.md
--rw-r--r--   0        0        0     1207 2022-11-13 16:42:34.147461 lndb_storage-0.2rc2/docs/faq/curate-data.ipynb
--rw-r--r--   0        0        0      145 2022-11-13 16:42:34.154463 lndb_storage-0.2rc2/docs/faq/index.md
--rw-r--r--   0        0        0      369 2023-03-21 10:08:33.895033 lndb_storage-0.2rc2/docs/guide/index.md
--rw-r--r--   0        0        0      859 2023-03-13 18:04:48.669623 lndb_storage-0.2rc2/docs/guide/quickstart.ipynb
--rw-r--r--   0        0        0     6973 2023-03-17 18:45:05.466209 lndb_storage-0.2rc2/docs/guide/storage.ipynb
--rw-r--r--   0        0        0     9667 2023-03-26 13:15:18.774715 lndb_storage-0.2rc2/docs/guide/stream.ipynb
--rw-r--r--   0        0        0      651 2022-11-13 16:42:34.173489 lndb_storage-0.2rc2/docs/index.md
--rw-r--r--   0        0        0      848 2022-11-13 16:42:34.180461 lndb_storage-0.2rc2/docs/notes/YYYY-MM-DD-my-design-choice.ipynb
--rw-r--r--   0        0        0      236 2022-11-13 16:42:34.187461 lndb_storage-0.2rc2/docs/notes/index.md
--rw-r--r--   0        0        0      165 2022-11-13 16:42:34.193462 lndb_storage-0.2rc2/lamin-project.yaml
--rw-r--r--   0        0        0      554 2023-03-26 19:27:49.781055 lndb_storage-0.2rc2/lndb_storage/__init__.py
--rw-r--r--   0        0        0     3414 2023-03-26 13:15:18.790335 lndb_storage-0.2rc2/lndb_storage/_file.py
--rw-r--r--   0        0        0      515 2023-03-14 18:15:14.187412 lndb_storage-0.2rc2/lndb_storage/_filesystem.py
--rw-r--r--   0        0        0      517 2023-03-26 13:15:18.805964 lndb_storage-0.2rc2/lndb_storage/_h5ad.py
--rw-r--r--   0        0        0      212 2023-03-13 18:04:48.685214 lndb_storage-0.2rc2/lndb_storage/_images.py
--rw-r--r--   0        0        0     2374 2023-03-26 12:52:12.411859 lndb_storage-0.2rc2/lndb_storage/_subset.py
--rw-r--r--   0        0        0     2066 2023-03-13 18:04:48.700802 lndb_storage-0.2rc2/lndb_storage/_upath_ext.py
--rw-r--r--   0        0        0     2852 2023-03-13 18:04:48.700802 lndb_storage-0.2rc2/lndb_storage/_zarr.py
--rw-r--r--   0        0        0      332 2023-03-26 12:52:12.411859 lndb_storage-0.2rc2/lndb_storage/object/__init__.py
--rw-r--r--   0        0        0      978 2023-03-26 13:15:18.805964 lndb_storage-0.2rc2/lndb_storage/object/_anndata.py
--rw-r--r--   0        0        0      761 2023-03-13 18:04:48.716390 lndb_storage-0.2rc2/lndb_storage/object/_anndata_sizes.py
--rw-r--r--   0        0        0      931 2023-03-14 18:15:14.187412 lndb_storage-0.2rc2/lndb_storage/object/_core.py
--rw-r--r--   0        0        0     4274 2023-03-13 18:04:48.716390 lndb_storage-0.2rc2/lndb_storage/object/_lazy_field.py
--rw-r--r--   0        0        0     3584 2023-03-26 12:52:12.433964 lndb_storage-0.2rc2/lndb_storage/object/_subset_anndata.py
--rw-r--r--   0        0        0      939 2023-03-26 12:52:12.449603 lndb_storage-0.2rc2/noxfile.py
--rw-r--r--   0        0        0     1048 2023-03-26 19:18:45.031918 lndb_storage-0.2rc2/pyproject.toml
--rw-r--r--   0        0        0      506 2022-11-13 16:42:34.236464 lndb_storage-0.2rc2/tests/test_notebooks.py
--rw-r--r--   0        0        0     1141 1970-01-01 00:00:00.000000 lndb_storage-0.2rc2/PKG-INFO
+-rw-r--r--   0        0        0     2961 2023-03-29 20:45:21.388257 lndb_storage-0.2rc3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-03-29 20:45:21.388328 lndb_storage-0.2rc3/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-03-29 20:45:21.388401 lndb_storage-0.2rc3/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1199 2023-03-29 20:45:21.388463 lndb_storage-0.2rc3/.gitignore
+-rw-r--r--   0        0        0     1758 2023-03-29 20:45:21.388537 lndb_storage-0.2rc3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-03-29 20:45:21.388633 lndb_storage-0.2rc3/LICENSE
+-rw-r--r--   0        0        0      124 2023-03-29 20:45:21.388936 lndb_storage-0.2rc3/README.md
+-rw-r--r--   0        0        0     1884 2023-04-09 22:16:50.608709 lndb_storage-0.2rc3/docs/changelog.md
+-rw-r--r--   0        0        0     3283 2023-04-09 22:15:42.448966 lndb_storage-0.2rc3/docs/guide/add-replace-stage.ipynb
+-rw-r--r--   0        0        0       88 2023-04-09 22:14:23.875135 lndb_storage-0.2rc3/docs/guide/index.md
+-rw-r--r--   0        0        0     3976 2023-04-08 09:43:17.308905 lndb_storage-0.2rc3/docs/guide/iris.csv
+-rw-r--r--   0        0        0     4550 2023-04-08 09:43:17.309082 lndb_storage-0.2rc3/docs/guide/iris.data
+-rw-r--r--   0        0        0     4615 2023-04-09 22:14:23.875491 lndb_storage-0.2rc3/docs/guide/serialize-cache.ipynb
+-rw-r--r--   0        0        0     7035 2023-04-09 22:14:23.875871 lndb_storage-0.2rc3/docs/guide/stream.ipynb
+-rw-r--r--   0        0        0     7566 2023-04-09 22:14:23.876185 lndb_storage-0.2rc3/docs/guide/upload.ipynb
+-rw-r--r--   0        0        0      593 2023-04-09 20:42:44.949159 lndb_storage-0.2rc3/docs/index.md
+-rw-r--r--   0        0        0       60 2023-04-09 20:42:44.949390 lndb_storage-0.2rc3/docs/reference.md
+-rw-r--r--   0        0        0      160 2023-03-29 20:45:21.390164 lndb_storage-0.2rc3/lamin-project.yaml
+-rw-r--r--   0        0        0      580 2023-04-09 22:16:33.330050 lndb_storage-0.2rc3/lndb_storage/__init__.py
+-rw-r--r--   0        0        0     3300 2023-04-09 20:42:44.949890 lndb_storage-0.2rc3/lndb_storage/_file.py
+-rw-r--r--   0        0        0      497 2023-04-09 20:42:44.950134 lndb_storage-0.2rc3/lndb_storage/_h5ad.py
+-rw-r--r--   0        0        0      204 2023-03-29 20:45:21.390606 lndb_storage-0.2rc3/lndb_storage/_images.py
+-rw-r--r--   0        0        0     2307 2023-03-29 20:45:21.390671 lndb_storage-0.2rc3/lndb_storage/_subset.py
+-rw-r--r--   0        0        0     2764 2023-04-09 20:42:44.950408 lndb_storage-0.2rc3/lndb_storage/_zarr.py
+-rw-r--r--   0        0        0      317 2023-03-29 20:45:21.390956 lndb_storage-0.2rc3/lndb_storage/object/__init__.py
+-rw-r--r--   0        0        0      950 2023-03-29 20:45:21.391028 lndb_storage-0.2rc3/lndb_storage/object/_anndata.py
+-rw-r--r--   0        0        0      730 2023-03-29 20:45:21.391077 lndb_storage-0.2rc3/lndb_storage/object/_anndata_sizes.py
+-rw-r--r--   0        0        0      900 2023-03-29 20:45:21.391132 lndb_storage-0.2rc3/lndb_storage/object/_core.py
+-rw-r--r--   0        0        0     4116 2023-03-29 20:45:21.391201 lndb_storage-0.2rc3/lndb_storage/object/_lazy_field.py
+-rw-r--r--   0        0        0     3507 2023-04-09 20:42:44.950762 lndb_storage-0.2rc3/lndb_storage/object/_subset_anndata.py
+-rw-r--r--   0        0        0      913 2023-04-09 22:16:03.478614 lndb_storage-0.2rc3/noxfile.py
+-rw-r--r--   0        0        0     1044 2023-04-09 20:42:44.951084 lndb_storage-0.2rc3/pyproject.toml
+-rw-r--r--   0        0        0      490 2023-03-29 20:45:21.391918 lndb_storage-0.2rc3/tests/test_notebooks.py
+-rw-r--r--   0        0        0     1099 1970-01-01 00:00:00.000000 lndb_storage-0.2rc3/PKG-INFO
```

### Comparing `lndb_storage-0.2rc2/.pre-commit-config.yaml` & `lndb_storage-0.2rc3/.pre-commit-config.yaml`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,64 +1,64 @@
-repos:
-  - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v3.2.0
-    hooks:
-      - id: trailing-whitespace
-      - id: end-of-file-fixer
-        exclude: |
-          (?x)(
-              .github/workflows/latest-changes.jinja2
-          )
-      - id: check-yaml
-      - id: check-added-large-files
-  - repo: https://github.com/psf/black
-    rev: 22.6.0
-    hooks:
-      - id: black-jupyter
-  - repo: https://github.com/pycqa/flake8
-    rev: 4.0.1
-    hooks:
-      - id: flake8
-        additional_dependencies:
-          - flake8-black==0.3.3
-          - flake8-typing-imports==1.10.0
-        language_version: python3
-        args:
-          - --max-line-length=88
-          - --ignore=E203
-        exclude: |
-          (?x)(
-              __init__.py
-          )
-  - repo: https://github.com/pre-commit/mirrors-prettier
-    rev: v2.6.2
-    hooks:
-      - id: prettier
-  - repo: https://github.com/kynan/nbstripout
-    rev: 0.3.9
-    hooks:
-      - id: nbstripout
-        exclude: |
-          (?x)(
-              docs/examples/|
-              docs/notes/
-          )
-  - repo: https://github.com/Lucas-C/pre-commit-hooks
-    rev: v1.1.9
-    hooks:
-      - id: forbid-crlf
-      - id: remove-crlf
-  - repo: https://github.com/pre-commit/mirrors-isort
-    rev: v5.8.0
-    hooks:
-      - id: isort
-        args: ["--profile", "black"]
-  - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v0.940
-    hooks:
-      - id: mypy
-  - repo: https://github.com/pycqa/pydocstyle
-    rev: 6.1.1
-    hooks:
-      - id: pydocstyle
-        args: # google style + __init__, see http://www.pydocstyle.org/en/stable/error_codes.html
-          - --ignore=D100,D101,D102,D103,D106,D107,D203,D204,D213,D215,D400,D401,D403,D404,D406,D407,D408,D409,D412,D413
+repos:
+  - repo: https://github.com/pre-commit/pre-commit-hooks
+    rev: v3.2.0
+    hooks:
+      - id: trailing-whitespace
+      - id: end-of-file-fixer
+        exclude: |
+          (?x)(
+              .github/workflows/latest-changes.jinja2
+          )
+      - id: check-yaml
+      - id: check-added-large-files
+  - repo: https://github.com/psf/black
+    rev: 22.6.0
+    hooks:
+      - id: black-jupyter
+  - repo: https://github.com/pycqa/flake8
+    rev: 4.0.1
+    hooks:
+      - id: flake8
+        additional_dependencies:
+          - flake8-black==0.3.3
+          - flake8-typing-imports==1.10.0
+        language_version: python3
+        args:
+          - --max-line-length=88
+          - --ignore=E203
+        exclude: |
+          (?x)(
+              __init__.py
+          )
+  - repo: https://github.com/pre-commit/mirrors-prettier
+    rev: v2.6.2
+    hooks:
+      - id: prettier
+  - repo: https://github.com/kynan/nbstripout
+    rev: 0.3.9
+    hooks:
+      - id: nbstripout
+        exclude: |
+          (?x)(
+              docs/examples/|
+              docs/notes/
+          )
+  - repo: https://github.com/Lucas-C/pre-commit-hooks
+    rev: v1.1.9
+    hooks:
+      - id: forbid-crlf
+      - id: remove-crlf
+  - repo: https://github.com/pre-commit/mirrors-isort
+    rev: v5.8.0
+    hooks:
+      - id: isort
+        args: ["--profile", "black"]
+  - repo: https://github.com/pre-commit/mirrors-mypy
+    rev: v0.940
+    hooks:
+      - id: mypy
+  - repo: https://github.com/pycqa/pydocstyle
+    rev: 6.1.1
+    hooks:
+      - id: pydocstyle
+        args: # google style + __init__, see http://www.pydocstyle.org/en/stable/error_codes.html
+          - --ignore=D100,D101,D102,D103,D106,D107,D203,D204,D213,D215,D400,D401,D403,D404,D406,D407,D408,D409,D412,D413
```

### Comparing `lndb_storage-0.2rc2/LICENSE` & `lndb_storage-0.2rc3/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
```

### Comparing `lndb_storage-0.2rc2/docs/changelog.md` & `lndb_storage-0.2rc3/docs/changelog.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✅ Introduce separate upload guide | [14](https://github.com/laminlabs/lndb-storage/pull/14) | [falexwolf](https://github.com/falexwolf) | 2023-04-09 | 0.2rc3
+💚 Attempt fix CI | [12](https://github.com/laminlabs/lndb-storage/pull/12) | [falexwolf](https://github.com/falexwolf) | 2023-04-09 |
+🚚 Move `UPath` back to `lndb` | [11](https://github.com/laminlabs/lndb-storage/pull/11) | [falexwolf](https://github.com/falexwolf) | 2023-04-08 |
+✅ Add test for replace and stage | [10](https://github.com/laminlabs/lndb-storage/pull/10) | [Koncopd](https://github.com/Koncopd) | 2023-04-04 |
 ➕ Add upath to deps | [9](https://github.com/laminlabs/lndb-storage/pull/9) | [Koncopd](https://github.com/Koncopd) | 2023-03-26 | 0.2rc2
 ➖ Remove lndb as explicit dependency | [7](https://github.com/laminlabs/lndb-storage/pull/7) | [Koncopd](https://github.com/Koncopd) | 2023-03-26 | 0.2rc1
 🚚 Rename `DObject` to `File` | [8](https://github.com/laminlabs/lndb-storage/pull/8) | [falexwolf](https://github.com/falexwolf) | 2023-03-24 |
 ✅ Test streaming here | [6](https://github.com/laminlabs/lndb-storage/pull/6) | [Koncopd](https://github.com/Koncopd) | 2023-03-17 |
 ♻️ Move the rest of storage code here | [4](https://github.com/laminlabs/lndb-storage/pull/4) | [Koncopd](https://github.com/Koncopd) | 2023-03-14 |
 :construction_worker: Update with latest cookiecutter | [5](https://github.com/laminlabs/lndb-storage/pull/5) | [falexwolf](https://github.com/falexwolf) | 2023-03-14 |
 🔨 Update storage code | [3](https://github.com/laminlabs/lndb-storage/pull/3) | [Koncopd](https://github.com/Koncopd) | 2023-03-11 |
```

### Comparing `lndb_storage-0.2rc2/docs/index.md` & `lndb_storage-0.2rc3/docs/index.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,38 @@
 00000000: 6060 607b 696e 636c 7564 657d 202e 2e2f  ```{include} ../
-00000010: 5245 4144 4d45 2e6d 640d 0a3a 7374 6172  README.md..:star
-00000020: 742d 6c69 6e65 3a20 300d 0a3a 656e 642d  t-line: 0..:end-
-00000030: 6c69 6e65 3a20 310d 0a60 6060 0d0a 0d0a  line: 1..```....
-00000040: 6060 607b 6e6f 7465 7d0d 0a0d 0a49 6620  ```{note}....If 
-00000050: 796f 7520 6172 656e 2774 2074 6865 2070  you aren't the p
-00000060: 6572 736f 6e20 7768 6f20 7573 6564 2074  erson who used t
-00000070: 6865 2063 6f6f 6b69 6563 7574 7465 722c  he cookiecutter,
-00000080: 206d 616b 6520 7375 7265 2079 6f75 2069   make sure you i
-00000090: 6e69 7420 6070 7265 2d63 6f6d 6d69 7420  nit `pre-commit 
-000000a0: 696e 7374 616c 6c60 2061 6e64 2060 6769  install` and `gi
-000000b0: 746d 6f6a 6920 2d69 6020 6f6e 2074 6865  tmoji -i` on the
-000000c0: 2043 4c49 2062 6566 6f72 6520 7374 6172   CLI before star
-000000d0: 7469 6e67 2074 6f20 776f 726b 206f 6e20  ting to work on 
-000000e0: 7468 6973 2072 6570 6f73 6974 6f72 7921  this repository!
-000000f0: 0d0a 6060 600d 0a0d 0a59 6f75 276c 6c20  ..```....You'll 
-00000100: 7072 6f62 6162 6c79 206e 6f74 206e 6565  probably not nee
-00000110: 6420 616c 6c20 7468 6520 6469 6666 6572  d all the differ
-00000120: 656e 7420 7479 7065 7320 6f66 2064 6972  ent types of dir
-00000130: 6563 746f 7269 6573 2068 6572 652e 0d0a  ectories here...
-00000140: 0d0a 4a75 7374 206d 616b 6520 7375 7265  ..Just make sure
-00000150: 2077 6861 7420 6561 6368 206f 6620 7468   what each of th
-00000160: 656d 2069 7320 7375 7070 6f73 6564 2074  em is supposed t
-00000170: 6f20 7072 6f76 6964 652e 0d0a 0d0a 5468  o provide.....Th
-00000180: 6520 6f72 6761 6e69 7a61 7469 6f6e 2072  e organization r
-00000190: 6f75 6768 6c79 2066 6f6c 6c6f 7773 205b  oughly follows [
-000001a0: 6469 6174 6178 6973 5d28 6874 7470 733a  diataxis](https:
-000001b0: 2f2f 6469 6174 6178 6973 2e66 722f 292c  //diataxis.fr/),
-000001c0: 2063 616c 6c69 6e67 2077 6861 7420 6469   calling what di
-000001d0: 6174 6178 6973 2063 616c 6c73 2022 7475  ataxis calls "tu
-000001e0: 746f 7269 616c 7322 2067 7569 6465 2c20  torials" guide, 
-000001f0: 616e 6420 7768 6174 2064 6961 7461 7869  and what diataxi
-00000200: 7320 6361 6c6c 7320 2267 7569 6465 7322  s calls "guides"
-00000210: 2046 4151 2e0d 0a0d 0a60 6060 7b74 6f63   FAQ.....```{toc
-00000220: 7472 6565 7d0d 0a3a 6d61 7864 6570 7468  tree}..:maxdepth
-00000230: 3a20 310d 0a3a 6869 6464 656e 3a0d 0a0d  : 1..:hidden:...
-00000240: 0a67 7569 6465 2f69 6e64 6578 0d0a 6170  .guide/index..ap
-00000250: 690d 0a66 6171 2f69 6e64 6578 0d0a 6e6f  i..faq/index..no
-00000260: 7465 732f 696e 6465 780d 0a65 7861 6d70  tes/index..examp
-00000270: 6c65 732f 696e 6465 780d 0a63 6861 6e67  les/index..chang
-00000280: 656c 6f67 0d0a 6060 600d 0a              elog..```..
+00000010: 5245 4144 4d45 2e6d 640a 3a73 7461 7274  README.md.:start
+00000020: 2d6c 696e 653a 2030 0a3a 656e 642d 6c69  -line: 0.:end-li
+00000030: 6e65 3a20 310a 6060 600a 0a60 6060 7b6e  ne: 1.```..```{n
+00000040: 6f74 657d 0a0a 4966 2079 6f75 2061 7265  ote}..If you are
+00000050: 6e27 7420 7468 6520 7065 7273 6f6e 2077  n't the person w
+00000060: 686f 2075 7365 6420 7468 6520 636f 6f6b  ho used the cook
+00000070: 6965 6375 7474 6572 2c20 6d61 6b65 2073  iecutter, make s
+00000080: 7572 6520 796f 7520 696e 6974 2060 7072  ure you init `pr
+00000090: 652d 636f 6d6d 6974 2069 6e73 7461 6c6c  e-commit install
+000000a0: 6020 616e 6420 6067 6974 6d6f 6a69 202d  ` and `gitmoji -
+000000b0: 6960 206f 6e20 7468 6520 434c 4920 6265  i` on the CLI be
+000000c0: 666f 7265 2073 7461 7274 696e 6720 746f  fore starting to
+000000d0: 2077 6f72 6b20 6f6e 2074 6869 7320 7265   work on this re
+000000e0: 706f 7369 746f 7279 210a 6060 600a 0a59  pository!.```..Y
+000000f0: 6f75 276c 6c20 7072 6f62 6162 6c79 206e  ou'll probably n
+00000100: 6f74 206e 6565 6420 616c 6c20 7468 6520  ot need all the 
+00000110: 6469 6666 6572 656e 7420 7479 7065 7320  different types 
+00000120: 6f66 2064 6972 6563 746f 7269 6573 2068  of directories h
+00000130: 6572 652e 0a0a 4a75 7374 206d 616b 6520  ere...Just make 
+00000140: 7375 7265 2077 6861 7420 6561 6368 206f  sure what each o
+00000150: 6620 7468 656d 2069 7320 7375 7070 6f73  f them is suppos
+00000160: 6564 2074 6f20 7072 6f76 6964 652e 0a0a  ed to provide...
+00000170: 5468 6520 6f72 6761 6e69 7a61 7469 6f6e  The organization
+00000180: 2072 6f75 6768 6c79 2066 6f6c 6c6f 7773   roughly follows
+00000190: 205b 6469 6174 6178 6973 5d28 6874 7470   [diataxis](http
+000001a0: 733a 2f2f 6469 6174 6178 6973 2e66 722f  s://diataxis.fr/
+000001b0: 292c 2063 616c 6c69 6e67 2077 6861 7420  ), calling what 
+000001c0: 6469 6174 6178 6973 2063 616c 6c73 2022  diataxis calls "
+000001d0: 7475 746f 7269 616c 7322 2067 7569 6465  tutorials" guide
+000001e0: 2c20 616e 6420 7768 6174 2064 6961 7461  , and what diata
+000001f0: 7869 7320 6361 6c6c 7320 2267 7569 6465  xis calls "guide
+00000200: 7322 2046 4151 2e0a 0a60 6060 7b74 6f63  s" FAQ...```{toc
+00000210: 7472 6565 7d0a 3a6d 6178 6465 7074 683a  tree}.:maxdepth:
+00000220: 2031 0a3a 6869 6464 656e 3a0a 0a67 7569   1.:hidden:..gui
+00000230: 6465 2f69 6e64 6578 0a72 6566 6572 656e  de/index.referen
+00000240: 6365 0a63 6861 6e67 656c 6f67 0a60 6060  ce.changelog.```
+00000250: 0a                                       .
```

### Comparing `lndb_storage-0.2rc2/lndb_storage/_file.py` & `lndb_storage-0.2rc3/lndb_storage/_file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-import shutil
-from pathlib import Path
-from typing import Union
-
-import fsspec
-import nbproject
-import pandas as pd
-import readfcs
-
-from ._h5ad import read_adata_h5ad
-from ._upath_ext import UPath
-from ._zarr import read_adata_zarr
-
-READER_FUNCS = {
-    ".csv": pd.read_csv,
-    ".h5ad": read_adata_h5ad,
-    ".parquet": pd.read_parquet,
-    ".fcs": readfcs.read,
-    ".zarr": read_adata_zarr,
-}
-
-
-def print_hook(size, value, **kwargs):
-    progress = value / size
-    out = f"Uploading {kwargs['filepath']}: {min(progress, 1.):4.2f}"
-    if progress >= 1:
-        out += "\n"
-    if nbproject.meta.env != "test":
-        print(out, end="\r")
-
-
-class ProgressCallback(fsspec.callbacks.Callback):
-    def branch(self, path_1, path_2, kwargs):
-        kwargs["callback"] = fsspec.callbacks.Callback(
-            hooks=dict(print_hook=print_hook), filepath=path_1
-        )
-
-    def call(self, *args, **kwargs):
-        return None
-
-
-def store_object(localpath: Union[str, Path], storagekey: str) -> float:
-    """Store arbitrary file to configured storage location.
-
-    Returns size in bytes.
-    """
-    from lndb import settings
-
-    storagepath = settings.instance.storage.key_to_filepath(storagekey)
-    localpath = Path(localpath)
-
-    if localpath.is_file():
-        size = localpath.stat().st_size
-    else:
-        size = sum(f.stat().st_size for f in localpath.rglob("*") if f.is_file())
-
-    if isinstance(storagepath, UPath):
-        if localpath.suffix != ".zarr":
-            cb = ProgressCallback()
-        else:
-            # todo: make proper progress bar for zarr
-            cb = fsspec.callbacks.NoOpCallback()
-        storagepath.upload_from(localpath, recursive=True, callback=cb)
-    else:
-        if localpath.is_file():
-            try:
-                shutil.copyfile(localpath, storagepath)
-            except shutil.SameFileError:
-                pass
-        else:
-            if storagepath.exists():
-                shutil.rmtree(storagepath)
-            shutil.copytree(localpath, storagepath)
-    return float(size)  # because this is how we store in the db
-
-
-def delete_storage(storagekey: str):
-    """Delete arbitrary file."""
-    from lndb import settings
-
-    storagepath = settings.instance.storage.key_to_filepath(storagekey)
-    if storagepath.is_file():
-        storagepath.unlink()
-    elif storagepath.is_dir():
-        if isinstance(storagepath, UPath):
-            storagepath.rmdir()
-        else:
-            shutil.rmtree(storagepath)
-    else:
-        raise FileNotFoundError(f"{storagepath} is not an existing path!")
-
-
-def load_to_memory(filepath: Union[str, Path, UPath], stream: bool = False):
-    """Load a file into memory.
-
-    Returns the filepath if no in-memory form is found.
-    """
-    from lndb import settings
-
-    if isinstance(filepath, str):
-        filepath = Path(filepath)
-
-    if filepath.suffix == ".zarr":
-        stream = True
-    elif filepath.suffix != ".h5ad":
-        stream = False
-
-    if not stream:
-        # caching happens here if filename is a UPath
-        # todo: make it safe when filepath is just Path
-        filepath = settings.instance.storage.cloud_to_local(filepath)
-
-    reader = READER_FUNCS.get(filepath.suffix)
-    if reader is None:
-        return filepath
-    else:
-        return reader(filepath)
+import shutil
+from pathlib import Path
+from typing import Union
+
+import fsspec
+import nbproject
+import pandas as pd
+import readfcs
+from lndb.dev.upath import UPath
+
+from ._h5ad import read_adata_h5ad
+from ._zarr import read_adata_zarr
+
+READER_FUNCS = {
+    ".csv": pd.read_csv,
+    ".h5ad": read_adata_h5ad,
+    ".parquet": pd.read_parquet,
+    ".fcs": readfcs.read,
+    ".zarr": read_adata_zarr,
+}
+
+
+def print_hook(size, value, **kwargs):
+    progress = value / size
+    out = f"Uploading {kwargs['filepath']}: {min(progress, 1.):4.2f}"
+    if progress >= 1:
+        out += "\n"
+    if nbproject.meta.env != "test":
+        print(out, end="\r")
+
+
+class ProgressCallback(fsspec.callbacks.Callback):
+    def branch(self, path_1, path_2, kwargs):
+        kwargs["callback"] = fsspec.callbacks.Callback(
+            hooks=dict(print_hook=print_hook), filepath=path_1
+        )
+
+    def call(self, *args, **kwargs):
+        return None
+
+
+def store_object(localpath: Union[str, Path], storagekey: str) -> float:
+    """Store arbitrary file to configured storage location.
+
+    Returns size in bytes.
+    """
+    from lndb import settings
+
+    storagepath = settings.instance.storage.key_to_filepath(storagekey)
+    localpath = Path(localpath)
+
+    if localpath.is_file():
+        size = localpath.stat().st_size
+    else:
+        size = sum(f.stat().st_size for f in localpath.rglob("*") if f.is_file())
+
+    if isinstance(storagepath, UPath):
+        if localpath.suffix != ".zarr":
+            cb = ProgressCallback()
+        else:
+            # todo: make proper progress bar for zarr
+            cb = fsspec.callbacks.NoOpCallback()
+        storagepath.upload_from(localpath, recursive=True, callback=cb)
+    else:
+        if localpath.is_file():
+            try:
+                shutil.copyfile(localpath, storagepath)
+            except shutil.SameFileError:
+                pass
+        else:
+            if storagepath.exists():
+                shutil.rmtree(storagepath)
+            shutil.copytree(localpath, storagepath)
+    return float(size)  # because this is how we store in the db
+
+
+def delete_storage(storagekey: str):
+    """Delete arbitrary file."""
+    from lndb import settings
+
+    storagepath = settings.instance.storage.key_to_filepath(storagekey)
+    if storagepath.is_file():
+        storagepath.unlink()
+    elif storagepath.is_dir():
+        if isinstance(storagepath, UPath):
+            storagepath.rmdir()
+        else:
+            shutil.rmtree(storagepath)
+    else:
+        raise FileNotFoundError(f"{storagepath} is not an existing path!")
+
+
+def load_to_memory(filepath: Union[str, Path, UPath], stream: bool = False):
+    """Load a file into memory.
+
+    Returns the filepath if no in-memory form is found.
+    """
+    from lndb import settings
+
+    if isinstance(filepath, str):
+        filepath = Path(filepath)
+
+    if filepath.suffix == ".zarr":
+        stream = True
+    elif filepath.suffix != ".h5ad":
+        stream = False
+
+    if not stream:
+        # caching happens here if filename is a UPath
+        # todo: make it safe when filepath is just Path
+        filepath = settings.instance.storage.cloud_to_local(filepath)
+
+    reader = READER_FUNCS.get(filepath.suffix)
+    if reader is None:
+        return filepath
+    else:
+        return reader(filepath)
```

### Comparing `lndb_storage-0.2rc2/lndb_storage/_subset.py` & `lndb_storage-0.2rc3/lndb_storage/_subset.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,67 +1,67 @@
-from typing import List, Optional, Union
-
-from anndata import AnnData, concat
-from lamin_logger import logger
-from lnschema_core import File
-
-from .object import LazySelector, _subset_anndata_file
-
-SUFFIXES = (".h5ad", ".zarr")
-
-
-def subset(
-    files: Union[List[File], File],
-    query_obs: Optional[Union[List[str], str, LazySelector]] = None,
-    query_var: Optional[Union[List[str], str, LazySelector]] = None,
-    use_concat: bool = False,
-    concat_args: Optional[dict] = None,
-) -> Union[List[AnnData], AnnData, None]:
-    """Subset AnnData files and stream results into memory.
-
-    Args:
-        files: A `File` or a list of `Files` containing `AnnData` objects
-        to subset and load into memory.
-        query_obs: The pandas query string to evaluate on `.obs` of each
-        underlying `AnnData` object.
-        query_var: The pandas query string to evaluate on `.var` of each
-        underlying `AnnData` object.
-        use_concat: If `True`, applies `anndata.concat` on
-        the returned `AnnData` objects.
-        concat_args: Arguments for concatenation.
-    """
-    if isinstance(files, File):
-        files = [files]
-
-    n_files = len(files)
-    if isinstance(query_obs, list):
-        if len(query_obs) != n_files:
-            raise ValueError("query_obs list should be the same length as files.")
-    else:
-        query_obs = [query_obs] * n_files  # type: ignore
-    if isinstance(query_var, list):
-        if len(query_var) != n_files:
-            raise ValueError("query_var list should be the same length as files.")
-    else:
-        query_var = [query_var] * n_files  # type: ignore
-
-    adatas = []
-    # todo: implement parallel processing
-    for i, file in enumerate(files):
-        if file.suffix not in SUFFIXES:
-            logger.warning(f"File {file.id} is not an AnnData object, ignoring.")
-            continue
-        result = _subset_anndata_file(file, query_obs[i], query_var[i])
-        if result is not None:
-            adatas.append(result)
-
-    if not use_concat:
-        return adatas
-    # concat branch here
-    n_adatas = len(adatas)
-    if n_adatas == 0:
-        return None
-    elif n_adatas == 1:
-        return adatas[0]
-    else:
-        concat_args = {} if concat_args is None else concat_args
-        return concat(adatas, **concat_args)
+from typing import List, Optional, Union
+
+from anndata import AnnData, concat
+from lamin_logger import logger
+from lnschema_core import File
+
+from .object import LazySelector, _subset_anndata_file
+
+SUFFIXES = (".h5ad", ".zarr")
+
+
+def subset(
+    files: Union[List[File], File],
+    query_obs: Optional[Union[List[str], str, LazySelector]] = None,
+    query_var: Optional[Union[List[str], str, LazySelector]] = None,
+    use_concat: bool = False,
+    concat_args: Optional[dict] = None,
+) -> Union[List[AnnData], AnnData, None]:
+    """Subset AnnData files and stream results into memory.
+
+    Args:
+        files: A `File` or a list of `Files` containing `AnnData` objects
+        to subset and load into memory.
+        query_obs: The pandas query string to evaluate on `.obs` of each
+        underlying `AnnData` object.
+        query_var: The pandas query string to evaluate on `.var` of each
+        underlying `AnnData` object.
+        use_concat: If `True`, applies `anndata.concat` on
+        the returned `AnnData` objects.
+        concat_args: Arguments for concatenation.
+    """
+    if isinstance(files, File):
+        files = [files]
+
+    n_files = len(files)
+    if isinstance(query_obs, list):
+        if len(query_obs) != n_files:
+            raise ValueError("query_obs list should be the same length as files.")
+    else:
+        query_obs = [query_obs] * n_files  # type: ignore
+    if isinstance(query_var, list):
+        if len(query_var) != n_files:
+            raise ValueError("query_var list should be the same length as files.")
+    else:
+        query_var = [query_var] * n_files  # type: ignore
+
+    adatas = []
+    # todo: implement parallel processing
+    for i, file in enumerate(files):
+        if file.suffix not in SUFFIXES:
+            logger.warning(f"File {file.id} is not an AnnData object, ignoring.")
+            continue
+        result = _subset_anndata_file(file, query_obs[i], query_var[i])
+        if result is not None:
+            adatas.append(result)
+
+    if not use_concat:
+        return adatas
+    # concat branch here
+    n_adatas = len(adatas)
+    if n_adatas == 0:
+        return None
+    elif n_adatas == 1:
+        return adatas[0]
+    else:
+        concat_args = {} if concat_args is None else concat_args
+        return concat(adatas, **concat_args)
```

### Comparing `lndb_storage-0.2rc2/lndb_storage/_zarr.py` & `lndb_storage-0.2rc3/lndb_storage/_zarr.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-import warnings
-from typing import Optional
-
-import scipy.sparse as sparse
-import zarr
-from anndata import AnnData
-from anndata._io import read_zarr
-from anndata._io.specs import write_elem
-
-from ._filesystem import _infer_filesystem
-from .object._anndata_sizes import _size_elem, _size_raw, size_adata
-
-
-def read_adata_zarr(storepath) -> AnnData:
-    fs, storepath = _infer_filesystem(storepath)
-
-    store = fs.get_mapper(storepath, check=True)
-    adata = read_zarr(store)
-
-    return adata
-
-
-def write_adata_zarr(
-    adata: AnnData, storepath, callback=None, chunks=None, **dataset_kwargs
-):
-    fs, storepath = _infer_filesystem(storepath)
-
-    store = fs.get_mapper(storepath, create=True)
-    f = zarr.open(store, mode="w")
-
-    adata.strings_to_categoricals()
-    if adata.raw is not None:
-        adata.strings_to_categoricals(adata.raw.var)
-
-    f.attrs.setdefault("encoding-type", "anndata")
-    f.attrs.setdefault("encoding-version", "0.1.0")
-
-    adata_size = None
-    cumulative_val = 0
-
-    def _cb(key_write: Optional[str] = None):
-        nonlocal adata_size
-        nonlocal cumulative_val
-
-        if callback is None:
-            return None
-        if adata_size is None:
-            adata_size = size_adata(adata)
-        if key_write is None:
-            # begin or finish
-            if cumulative_val < adata_size:
-                callback(adata_size, adata_size if cumulative_val > 0 else 0)
-            return None
-
-        elem = getattr(adata, key_write, None)
-        if elem is None:
-            return None
-        elem_size = _size_raw(elem) if key_write == "raw" else _size_elem(elem)
-        if elem_size == 0:
-            return None
-
-        cumulative_val += elem_size
-        callback(adata_size, cumulative_val)
-
-    def _write_elem_cb(f, k, elem, dataset_kwargs):
-        write_elem(f, k, elem, dataset_kwargs=dataset_kwargs)
-        _cb(k)
-
-    _cb(None)
-    with warnings.catch_warnings():
-        warnings.filterwarnings("ignore", category=UserWarning, module="zarr")
-
-        if chunks is not None and not isinstance(adata.X, sparse.spmatrix):
-            _write_elem_cb(
-                f, "X", adata.X, dataset_kwargs=dict(chunks=chunks, **dataset_kwargs)
-            )
-        else:
-            _write_elem_cb(f, "X", adata.X, dataset_kwargs=dataset_kwargs)
-        for elem in ("obs", "var"):
-            _write_elem_cb(f, elem, getattr(adata, elem), dataset_kwargs=dataset_kwargs)
-        for elem in ("obsm", "varm", "obsp", "varp", "layers", "uns"):
-            _write_elem_cb(
-                f, elem, dict(getattr(adata, elem)), dataset_kwargs=dataset_kwargs
-            )
-        _write_elem_cb(f, "raw", adata.raw, dataset_kwargs=dataset_kwargs)
-    # todo: fix size less than total at the end
-    _cb(None)
+import warnings
+from typing import Optional
+
+import scipy.sparse as sparse
+import zarr
+from anndata import AnnData
+from anndata._io import read_zarr
+from anndata._io.specs import write_elem
+from lndb.dev.upath import infer_filesystem
+
+from .object._anndata_sizes import _size_elem, _size_raw, size_adata
+
+
+def read_adata_zarr(storepath) -> AnnData:
+    fs, storepath = infer_filesystem(storepath)
+
+    store = fs.get_mapper(storepath, check=True)
+    adata = read_zarr(store)
+
+    return adata
+
+
+def write_adata_zarr(
+    adata: AnnData, storepath, callback=None, chunks=None, **dataset_kwargs
+):
+    fs, storepath = infer_filesystem(storepath)
+
+    store = fs.get_mapper(storepath, create=True)
+    f = zarr.open(store, mode="w")
+
+    adata.strings_to_categoricals()
+    if adata.raw is not None:
+        adata.strings_to_categoricals(adata.raw.var)
+
+    f.attrs.setdefault("encoding-type", "anndata")
+    f.attrs.setdefault("encoding-version", "0.1.0")
+
+    adata_size = None
+    cumulative_val = 0
+
+    def _cb(key_write: Optional[str] = None):
+        nonlocal adata_size
+        nonlocal cumulative_val
+
+        if callback is None:
+            return None
+        if adata_size is None:
+            adata_size = size_adata(adata)
+        if key_write is None:
+            # begin or finish
+            if cumulative_val < adata_size:
+                callback(adata_size, adata_size if cumulative_val > 0 else 0)
+            return None
+
+        elem = getattr(adata, key_write, None)
+        if elem is None:
+            return None
+        elem_size = _size_raw(elem) if key_write == "raw" else _size_elem(elem)
+        if elem_size == 0:
+            return None
+
+        cumulative_val += elem_size
+        callback(adata_size, cumulative_val)
+
+    def _write_elem_cb(f, k, elem, dataset_kwargs):
+        write_elem(f, k, elem, dataset_kwargs=dataset_kwargs)
+        _cb(k)
+
+    _cb(None)
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore", category=UserWarning, module="zarr")
+
+        if chunks is not None and not isinstance(adata.X, sparse.spmatrix):
+            _write_elem_cb(
+                f, "X", adata.X, dataset_kwargs=dict(chunks=chunks, **dataset_kwargs)
+            )
+        else:
+            _write_elem_cb(f, "X", adata.X, dataset_kwargs=dataset_kwargs)
+        for elem in ("obs", "var"):
+            _write_elem_cb(f, elem, getattr(adata, elem), dataset_kwargs=dataset_kwargs)
+        for elem in ("obsm", "varm", "obsp", "varp", "layers", "uns"):
+            _write_elem_cb(
+                f, elem, dict(getattr(adata, elem)), dataset_kwargs=dataset_kwargs
+            )
+        _write_elem_cb(f, "raw", adata.raw, dataset_kwargs=dataset_kwargs)
+    # todo: fix size less than total at the end
+    _cb(None)
```

### Comparing `lndb_storage-0.2rc2/lndb_storage/object/_anndata.py` & `lndb_storage-0.2rc3/lndb_storage/object/_anndata.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-import os
-from pathlib import Path
-
-from anndata import AnnData
-from lamin_logger import logger
-from typeguard import typechecked
-
-
-@typechecked
-def anndata_to_h5ad(adata: AnnData, filekey: str) -> Path:
-    """AnnData → h5ad."""
-    from lndb import settings
-
-    path = settings.instance.storage.key_to_filepath(filekey)
-    if settings.instance.storage.is_cloud:
-        cache_file = settings.instance.storage.cloud_to_local_no_update(path)  # type: ignore  # noqa
-        cache_file.parent.mkdir(exist_ok=True)
-        logger.debug(f"Writing cache file: {cache_file}.")
-        adata.write(cache_file)
-        logger.debug("Uploading cache file.")
-        path.upload_from(cache_file)  # type: ignore
-        # to avoid download from the cloud within synchronization
-        mtime = path.modified.timestamp()
-        os.utime(cache_file, times=(mtime, mtime))
-    else:
-        adata.write(path)
-        cache_file = path
-    return cache_file
+import os
+from pathlib import Path
+
+from anndata import AnnData
+from lamin_logger import logger
+from typeguard import typechecked
+
+
+@typechecked
+def anndata_to_h5ad(adata: AnnData, filekey: str) -> Path:
+    """AnnData → h5ad."""
+    from lndb import settings
+
+    path = settings.instance.storage.key_to_filepath(filekey)
+    if settings.instance.storage.is_cloud:
+        cache_file = settings.instance.storage.cloud_to_local_no_update(path)  # type: ignore  # noqa
+        cache_file.parent.mkdir(exist_ok=True)
+        logger.debug(f"Writing cache file: {cache_file}.")
+        adata.write(cache_file)
+        logger.debug("Uploading cache file.")
+        path.upload_from(cache_file)  # type: ignore
+        # to avoid download from the cloud within synchronization
+        mtime = path.modified.timestamp()
+        os.utime(cache_file, times=(mtime, mtime))
+    else:
+        adata.write(path)
+        cache_file = path
+    return cache_file
```

### Comparing `lndb_storage-0.2rc2/PKG-INFO` & `lndb_storage-0.2rc3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: lndb_storage
-Version: 0.2rc2
+Version: 0.2rc3
 Summary: Storage → object.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core
+Requires-Dist: lamin_logger>=0.3.0
 Requires-Dist: nbproject
 Requires-Dist: readfcs
 Requires-Dist: python-dateutil
 Requires-Dist: anndata
 Requires-Dist: zarr
 Requires-Dist: boto3==1.24.59
 Requires-Dist: botocore==1.27.59
@@ -20,19 +21,16 @@
 Requires-Dist: pandas
 Requires-Dist: typeguard
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "test"
 Requires-Dist: pytest-cov ; extra == "test"
 Requires-Dist: scanpy ; extra == "test"
+Requires-Dist: lndb>=0.41rc1 ; extra == "test"
 Project-URL: Home, https://github.com/laminlabs/lndb-storage
 Provides-Extra: dev
 Provides-Extra: test
 
-# lndb-storage: Manage LaminDB storage interactions
+# lndb-storage: LaminDB storage
 
-This package is in private beta at this moment!
-
-Follow https://twitter.com/laminlabs to learn about a first public release.
-
-For beta users: Read the [docs](https://lamin.ai/docs/lndb-storage).
+Latest developer docs: [netlify](https://lndb-storage-soie.netlify.app/docs/lndb-storage/)
```

