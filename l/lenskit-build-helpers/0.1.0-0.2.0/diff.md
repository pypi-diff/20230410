# Comparing `tmp/lenskit-build-helpers-0.1.0.tar.gz` & `tmp/lenskit-build-helpers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenskit-build-helpers-0.1.0.tar", last modified: Thu Jul 21 21:37:43 2022, max compression
+gzip compressed data, was "lenskit-build-helpers-0.2.0.tar", last modified: Mon Apr 10 20:52:02 2023, max compression
```

## Comparing `lenskit-build-helpers-0.1.0.tar` & `lenskit-build-helpers-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,29 @@
--rw-r--r--   0        0        0      245 2022-04-22 00:09:15.563746 lenskit-build-helpers-0.1.0/.editorconfig
--rw-r--r--   0        0        0      137 2022-07-15 21:42:25.528559 lenskit-build-helpers-0.1.0/.gitignore
--rw-r--r--   0        0        0     1092 2022-07-15 21:43:03.817514 lenskit-build-helpers-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     1116 2022-07-18 15:26:05.198485 lenskit-build-helpers-0.1.0/README.md
--rw-r--r--   0        0        0      270 2022-07-15 22:53:46.603660 lenskit-build-helpers-0.1.0/boot-env.yml
--rw-r--r--   0        0        0      377 2022-07-15 21:49:44.575868 lenskit-build-helpers-0.1.0/lkbuild/__init__.py
--rw-r--r--   0        0        0      132 2022-07-15 19:27:54.832386 lenskit-build-helpers-0.1.0/lkbuild/__main__.py
--rw-r--r--   0        0        0      895 2021-12-15 20:02:20.381827 lenskit-build-helpers-0.1.0/lkbuild/datasets.py
--rw-r--r--   0        0        0      563 2021-11-12 01:29:13.740630 lenskit-build-helpers-0.1.0/lkbuild/env.py
--rw-r--r--   0        0        0       86 2022-01-24 19:06:47.222770 lenskit-build-helpers-0.1.0/lkbuild/specs/mkl-spec.yml
--rw-r--r--   0        0        0       87 2021-11-12 01:29:13.741644 lenskit-build-helpers-0.1.0/lkbuild/specs/openblas-spec.yml
--rw-r--r--   0        0        0       80 2021-11-12 01:29:13.742638 lenskit-build-helpers-0.1.0/lkbuild/specs/python-3.10-spec.yml
--rw-r--r--   0        0        0       78 2021-11-12 01:29:13.742638 lenskit-build-helpers-0.1.0/lkbuild/specs/python-3.7-spec.yml
--rw-r--r--   0        0        0       78 2021-11-12 01:29:13.742638 lenskit-build-helpers-0.1.0/lkbuild/specs/python-3.8-spec.yml
--rw-r--r--   0        0        0       78 2021-11-12 01:29:13.743630 lenskit-build-helpers-0.1.0/lkbuild/specs/python-3.9-spec.yml
--rw-r--r--   0        0        0     4007 2022-07-18 18:30:53.295830 lenskit-build-helpers-0.1.0/lkbuild/tasks.py
--rw-r--r--   0        0        0      224 2022-04-22 00:08:15.738459 lenskit-build-helpers-0.1.0/lock-for-ci.sh
--rw-r--r--   0        0        0      481 2022-07-18 23:13:38.522431 lenskit-build-helpers-0.1.0/meta.yaml
--rw-r--r--   0        0        0      620 2022-07-18 18:09:53.238106 lenskit-build-helpers-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1456 1970-01-01 00:00:00.000000 lenskit-build-helpers-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      228 2022-07-16 00:06:38.137880 lenskit-build-helpers-0.2.0/.editorconfig
+-rw-r--r--   0        0        0      121 2022-07-16 00:06:38.138887 lenskit-build-helpers-0.2.0/.gitignore
+-rw-r--r--   0        0        0     2858 2022-12-07 00:26:56.364440 lenskit-build-helpers-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1083 2022-07-21 03:02:08.855947 lenskit-build-helpers-0.2.0/README.md
+-rw-r--r--   0        0        0      255 2022-12-07 00:26:56.405575 lenskit-build-helpers-0.2.0/boot-env.yml
+-rw-r--r--   0        0        0   156523 2022-12-07 00:29:13.161444 lenskit-build-helpers-0.2.0/conda-lock.yml
+-rw-r--r--   0        0        0      363 2023-04-10 20:51:40.606368 lenskit-build-helpers-0.2.0/lkbuild/__init__.py
+-rw-r--r--   0        0        0      125 2022-07-16 00:06:38.139756 lenskit-build-helpers-0.2.0/lkbuild/__main__.py
+-rw-r--r--   0        0        0      165 2022-12-07 00:26:56.425263 lenskit-build-helpers-0.2.0/lkbuild/data/__init__.py
+-rw-r--r--   0        0        0     8364 2022-12-07 00:26:56.426184 lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/README.txt
+-rw-r--r--   0        0        0   174246 2022-12-07 00:26:56.433179 lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/links.csv
+-rw-r--r--   0        0        0   449264 2022-12-07 00:26:56.439178 lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/movies.csv
+-rw-r--r--   0        0        0  2338261 2022-12-07 00:26:56.460260 lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/ratings.csv
+-rw-r--r--   0        0        0    40605 2022-12-07 00:26:56.465184 lenskit-build-helpers-0.2.0/lkbuild/data/ml-latest-small/tags.csv
+-rw-r--r--   0        0        0      958 2022-12-08 23:27:24.561754 lenskit-build-helpers-0.2.0/lkbuild/datasets.py
+-rw-r--r--   0        0        0      541 2022-07-16 00:06:38.140253 lenskit-build-helpers-0.2.0/lkbuild/env.py
+-rw-r--r--   0        0        0       82 2022-07-16 00:06:38.140612 lenskit-build-helpers-0.2.0/lkbuild/specs/mkl-spec.yml
+-rw-r--r--   0        0        0       84 2022-07-16 00:06:38.144272 lenskit-build-helpers-0.2.0/lkbuild/specs/openblas-spec.yml
+-rw-r--r--   0        0        0       77 2022-07-16 00:06:38.142000 lenskit-build-helpers-0.2.0/lkbuild/specs/python-3.10-spec.yml
+-rw-r--r--   0        0        0       77 2023-04-06 20:53:12.695024 lenskit-build-helpers-0.2.0/lkbuild/specs/python-3.11-spec.yml
+-rw-r--r--   0        0        0       75 2022-07-16 00:06:38.143743 lenskit-build-helpers-0.2.0/lkbuild/specs/python-3.7-spec.yml
+-rw-r--r--   0        0        0       75 2022-07-16 00:06:38.144272 lenskit-build-helpers-0.2.0/lkbuild/specs/python-3.8-spec.yml
+-rw-r--r--   0        0        0       75 2022-07-16 00:06:38.140612 lenskit-build-helpers-0.2.0/lkbuild/specs/python-3.9-spec.yml
+-rw-r--r--   0        0        0     4028 2022-12-07 00:42:45.886534 lenskit-build-helpers-0.2.0/lkbuild/tasks.py
+-rw-r--r--   0        0        0      224 2022-02-19 17:32:27.353316 lenskit-build-helpers-0.2.0/lock-for-ci.sh
+-rw-r--r--   0        0        0      453 2022-07-21 03:02:08.918887 lenskit-build-helpers-0.2.0/meta.yaml
+-rw-r--r--   0        0        0      705 2022-12-07 00:32:24.589580 lenskit-build-helpers-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      567 2022-12-07 00:26:56.486378 lenskit-build-helpers-0.2.0/tasks.py
+-rw-r--r--   0        0        0     1458 1970-01-01 00:00:00.000000 lenskit-build-helpers-0.2.0/PKG-INFO
```

### Comparing `lenskit-build-helpers-0.1.0/README.md` & `lenskit-build-helpers-0.2.0/README.md`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-# LensKit build support code
-
-This repository provides support code for use in LensKit builds and development.  If you are trying to
-use LensKit, you don't need it; it is only used for working on developing LensKit (and related packages).
-
-To set up a Conda environment that contains the utilities needed to bootstrap a LensKit
-development environment:
-
-    conda env create -n lkboot -f https://raw.githubusercontent.com/lenskit/lkbuild/main/boot-env.yml
-
-Then you can run the lkbuild utilities:
-
-    conda activate lkboot
-    lkbuild --help
-
-For example, you can create a lock file for developing LensKit:
-
-    lkbuild dev-lock -v 3.9 -b mkl
-
-Or you can download some testing data:
-
-    lkbuild fetch-data -d ml-20m
-
-You can also install into a Python environment with one of:
-
-    pip install lenskit-build-helpers
-    conda install -c lenskit lenskit-build-helpers
-
-## GitHub Actions
-
-This repository also provides some GitHub actions to support our CI workflow.
-
-- `actions/setup-env` — sets up an Anaconda environment based on locking the dependencies from `pyproject.toml`.
+# LensKit build support code
+
+This repository provides support code for use in LensKit builds and development.  If you are trying to
+use LensKit, you don't need it; it is only used for working on developing LensKit (and related packages).
+
+To set up a Conda environment that contains the utilities needed to bootstrap a LensKit
+development environment:
+
+    conda env create -n lkboot -f https://raw.githubusercontent.com/lenskit/lkbuild/main/boot-env.yml
+
+Then you can run the lkbuild utilities:
+
+    conda activate lkboot
+    lkbuild --help
+
+For example, you can create a lock file for developing LensKit:
+
+    lkbuild dev-lock -v 3.9 -b mkl
+
+Or you can download some testing data:
+
+    lkbuild fetch-data -d ml-20m
+
+You can also install into a Python environment with one of:
+
+    pip install lenskit-build-helpers
+    conda install -c lenskit lenskit-build-helpers
+
+## GitHub Actions
+
+This repository also provides some GitHub actions to support our CI workflow.
+
+- `actions/setup-env` — sets up an Anaconda environment based on locking the dependencies from `pyproject.toml`.
```

### Comparing `lenskit-build-helpers-0.1.0/lkbuild/env.py` & `lenskit-build-helpers-0.2.0/lkbuild/env.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import sysconfig
-import re
-
-
-def conda_platform():
-    plat = sysconfig.get_platform()
-    if re.match(r'^macosx-.*-x86_64', plat):
-        return 'osx-64'
-    if re.match(r'^macosx-.*-arm64', plat):
-        return 'osx-arm64'
-    if re.match(r'^[Ll]inux.*-x86_64', plat):
-        return 'linux-64'
-    if re.match(r'^[Ll]inux.*-aarch64', plat):
-        return 'linux-aarch64'
-    if plat == 'win-amd64':
-        return 'win-64'
-
-    raise ValueError('unrecognized platform ' + plat)
-
-
-if __name__ == '__main__':
-    print(conda_platform())
+import sysconfig
+import re
+
+
+def conda_platform():
+    plat = sysconfig.get_platform()
+    if re.match(r'^macosx-.*-x86_64', plat):
+        return 'osx-64'
+    if re.match(r'^macosx-.*-arm64', plat):
+        return 'osx-arm64'
+    if re.match(r'^[Ll]inux.*-x86_64', plat):
+        return 'linux-64'
+    if re.match(r'^[Ll]inux.*-aarch64', plat):
+        return 'linux-aarch64'
+    if plat == 'win-amd64':
+        return 'win-64'
+
+    raise ValueError('unrecognized platform ' + plat)
+
+
+if __name__ == '__main__':
+    print(conda_platform())
```

### Comparing `lenskit-build-helpers-0.1.0/lkbuild/tasks.py` & `lenskit-build-helpers-0.2.0/lkbuild/tasks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,147 +1,151 @@
-"""
-Support tasks shared across LensKit packages.
-"""
-
-from os import fspath
-import sys
-from pathlib import Path
-from invoke import task, Program, Collection
-from . import env
-import yaml
-import requests
-
-__ALL__ = [
-    'dev_lock',
-    'conda_platform'
-]
-
-DATA_DIR = Path('data')
-BIBTEX_URL = 'https://paperpile.com/eb/YdOlWmnlit'
-BIBTEX_FILE = Path('docs/lenskit.bib')
-
-
-@task(iterable=['extras', 'mixins'])
-def dev_lock(c, platform=None, extras=None, version=None, blas=None, mixins=None, env_file=False,
-             filter_extras=True, gh_set_output=False):
-    "Create a development lockfile"
-    plat = env.conda_platform()
-
-    if platform == 'all':
-        plat_opt = ''
-    elif platform:
-        plat_opt = f'-p {platform}'
-    else:
-        plat_opt = f'-p {plat}'
-
-    build_dir = Path('build')
-    build_dir.mkdir(exist_ok=True)
-
-    spec_dir = Path(__file__).parent / 'specs'
-    if not spec_dir.exists():
-        raise RuntimeError('spec dir not found, is lkbuild installed correctly?')
-
-    cmd = f'conda-lock lock --mamba {plat_opt} --dev-dependencies'
-    if env_file:
-        cmd += ' -k env'
-    else:
-        cmd += ' -k explicit'
-    cmd += ' -f pyproject.toml'
-
-    if version:
-        fn = f'python-{version}-spec.yml'
-        sf = spec_dir / fn
-        bf = build_dir / fn
-        bf.write_bytes(sf.read_bytes())
-        cmd += ' -f ' + fspath(bf)
-    if blas:
-        fn = f'{blas}-spec.yml'
-        sf = spec_dir / fn
-        bf = build_dir / fn
-        bf.write_bytes(sf.read_bytes())
-        cmd += ' -f ' + fspath(bf)
-    for m in mixins:
-        cmd += f' -f {m}'
-    for e in extras:
-        cmd += f' -e {e}'
-
-    if filter_extras:
-        cmd += ' --filter-extras'
-
-    print('running', cmd, file=sys.stderr)
-    c.run(cmd)
-
-    if gh_set_output:
-        print(f'::set-output name=platform::{plat}')
-        if env_file:
-            fn = f'conda-{plat}.lock.yml'
-        else:
-            fn = f'conda-{plat}.lock'
-        print(f'::set-output name=environment-file::{fn}')
-
-
-@task(iterable=['extras'])
-def env_file(c, platform=None, extras=None, version=None, blas=None, dev_deps=True,
-             output=None, name=None):
-    "Create an unresolved environment file"
-    from conda_lock.conda_lock import parse_source_files, aggregate_lock_specs
-
-    if not platform:
-        platform = env.conda_platform()
-
-    files = [Path('pyproject.toml')]
-
-    spec_dir = Path(__file__).parent / 'specs'
-    if not spec_dir.exists():
-        raise RuntimeError('spec dir not found, is lkbuild installed correctly?')
-
-    if version:
-        files.append(spec_dir / f'python-{version}-spec.yml')
-    if blas:
-        files.append(spec_dir / f'{blas}-spec.yml')
-
-    lock = parse_source_files(files, platform, dev_deps, extras)
-    lock = aggregate_lock_specs(lock)
-    env_spec = {
-        'channels': lock.channels,
-        'dependencies': lock.specs,
-    }
-    if name:
-        env_spec['name'] = name
-
-    if output:
-        print('writing environment to', output, file=sys.stderr)
-        out = Path(output)
-        with out.open('w') as f:
-            yaml.dump(env_spec, f)
-    else:
-        yaml.dump(env_spec, sys.stdout)
-
-
-@task
-def conda_platform(c, gh_output=False):
-    plat = env.conda_platform()
-    if gh_output:
-        print('::set-output name=conda-platform::' + plat)
-    else:
-        print(plat)
-
-
-@task
-def update_bibtex(c):
-    "Update the BibTeX file"
-    res = requests.get(BIBTEX_URL)
-    print('updating file', BIBTEX_FILE)
-    BIBTEX_FILE.write_text(res.text, encoding='utf-8')
-
-
-@task
-def fetch_data(c, data='ml-100k', data_dir=DATA_DIR):
-    "Fetch a data set."
-    from . import datasets
-
-    data_dir = Path(data_dir)
-    data_dir.mkdir(exist_ok=True, parents=True)
-    if data.startswith('ml-'):
-        datasets.fetch_ml(DATA_DIR, data)
-    else:
-        raise ValueError(f'unknown data set {data}')
+"""
+Support tasks shared across LensKit packages.
+"""
+
+from os import fspath, environ
+import sys
+from pathlib import Path
+from invoke import task, Program, Collection
+from . import env
+import yaml
+import requests
+
+__ALL__ = [
+    'dev_lock',
+    'conda_platform'
+]
+
+DATA_DIR = Path('data')
+BIBTEX_URL = 'https://paperpile.com/eb/YdOlWmnlit'
+BIBTEX_FILE = Path('docs/lenskit.bib')
+
+
+@task(iterable=['extras', 'mixins'])
+def dev_lock(c, platform=None, extras=None, version=None, blas=None, mixins=None, env_file=False,
+             filter_extras=True, combined_lock_file=False):
+    "Create a development lockfile"
+    plat = env.conda_platform()
+
+    build_dir = Path('build')
+    build_dir.mkdir(exist_ok=True)
+
+    spec_dir = Path(__file__).parent / 'specs'
+    if not spec_dir.exists():
+        raise RuntimeError('spec dir not found, is lkbuild installed correctly?')
+
+    cmd = f'conda-lock lock --mamba --dev-dependencies '
+    if platform and platform != 'all':
+        cmd += f'-p {platform}'
+    elif not combined_lock_file:
+        cmd += f'-p {plat}'
+
+    if env_file:
+        cmd += ' -k env'
+    elif not combined_lock_file:
+        cmd += ' -k explicit'
+
+    if version:
+        fn = f'python-{version}-spec.yml'
+        sf = spec_dir / fn
+        bf = build_dir / fn
+        bf.write_bytes(sf.read_bytes())
+        cmd += ' -f ' + fspath(bf)
+    if blas:
+        fn = f'{blas}-spec.yml'
+        sf = spec_dir / fn
+        bf = build_dir / fn
+        bf.write_bytes(sf.read_bytes())
+        cmd += ' -f ' + fspath(bf)
+
+    for m in mixins:
+        cmd += f' -f {m}'
+
+    cmd += ' -f pyproject.toml'
+
+    for e in extras:
+        cmd += f' -e {e}'
+
+    if filter_extras:
+        cmd += ' --filter-extras'
+
+    print('running', cmd, file=sys.stderr)
+    c.run(cmd)
+
+    gh_out = environ.get('GITHUB_OUTPUT', None)
+    if gh_out:
+        print('detected github actions, writing output file')
+        with open(gh_out, 'a') as ghof:
+            print(f'platform={plat}', file=ghof)
+            if env_file:
+                fn = f'conda-{plat}.lock.yml'
+            else:
+                fn = f'conda-{plat}.lock'
+            print(f'environment-file={fn}', file=ghof)
+
+
+@task(iterable=['extras'])
+def env_file(c, platform=None, extras=None, version=None, blas=None, dev_deps=True,
+             output=None, name=None):
+    "Create an unresolved environment file"
+    from conda_lock.conda_lock import parse_source_files, aggregate_lock_specs
+
+    if not platform:
+        platform = env.conda_platform()
+
+    files = [Path('pyproject.toml')]
+
+    spec_dir = Path(__file__).parent / 'specs'
+    if not spec_dir.exists():
+        raise RuntimeError('spec dir not found, is lkbuild installed correctly?')
+
+    if version:
+        files.append(spec_dir / f'python-{version}-spec.yml')
+    if blas:
+        files.append(spec_dir / f'{blas}-spec.yml')
+
+    lock = parse_source_files(files, platform, dev_deps, extras)
+    lock = aggregate_lock_specs(lock)
+    env_spec = {
+        'channels': lock.channels,
+        'dependencies': lock.specs,
+    }
+    if name:
+        env_spec['name'] = name
+
+    if output:
+        print('writing environment to', output, file=sys.stderr)
+        out = Path(output)
+        with out.open('w') as f:
+            yaml.dump(env_spec, f)
+    else:
+        yaml.dump(env_spec, sys.stdout)
+
+
+@task
+def conda_platform(c, gh_output=False):
+    plat = env.conda_platform()
+    if gh_output:
+        print('::set-output name=conda-platform::' + plat)
+    else:
+        print(plat)
+
+
+@task
+def update_bibtex(c):
+    "Update the BibTeX file"
+    res = requests.get(BIBTEX_URL)
+    print('updating file', BIBTEX_FILE)
+    BIBTEX_FILE.write_text(res.text, encoding='utf-8')
+
+
+@task
+def fetch_data(c, data='ml-100k', data_dir=DATA_DIR):
+    "Fetch a data set."
+    from . import datasets
+
+    data_dir = Path(data_dir)
+    data_dir.mkdir(exist_ok=True, parents=True)
+    if data.startswith('ml-'):
+        datasets.fetch_ml(DATA_DIR, data)
+    else:
+        raise ValueError(f'unknown data set {data}')
```

### Comparing `lenskit-build-helpers-0.1.0/PKG-INFO` & `lenskit-build-helpers-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: lenskit-build-helpers
-Version: 0.1.0
+Version: 0.2.0
 Summary: LensKit build support helpers.
 Author-email: Michael Ekstrand <michaelekstrand@boisestate.edu>
 Requires-Python: >= 3.7
 Description-Content-Type: text/markdown
 Requires-Dist: flit >=3.2,<4
 Requires-Dist: requests ==2.*
 Requires-Dist: invoke ==1.*
 Requires-Dist: pip
-Requires-Dist: conda-lock ==1.*
+Requires-Dist: conda-lock >=1.2.1
 
 # LensKit build support code
 
 This repository provides support code for use in LensKit builds and development.  If you are trying to
 use LensKit, you don't need it; it is only used for working on developing LensKit (and related packages).
 
 To set up a Conda environment that contains the utilities needed to bootstrap a LensKit
```

