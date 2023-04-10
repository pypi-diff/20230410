# Comparing `tmp/pdm-bump-0.6.9.tar.gz` & `tmp/pdm-bump-0.7.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-bump-0.6.9.tar", last modified: Sat Nov 12 16:05:23 2022, max compression
+gzip compressed data, was "pdm-bump-0.7.0a1.tar", last modified: Mon Apr 10 20:10:45 2023, max compression
```

## Comparing `pdm-bump-0.6.9.tar` & `pdm-bump-0.7.0a1.tar`

### file list

```diff
@@ -1,23 +1,28 @@
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-11-12 16:04:59.381260 pdm-bump-0.6.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     2425 2022-11-12 16:04:59.381260 pdm-bump-0.6.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2919 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16558 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/action.py
--rw-r--r--   0 runner    (1001) docker     (121)     1816 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/auto.py
--rw-r--r--   0 runner    (1001) docker     (121)      837 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3005 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     5074 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/dynamic.py
--rw-r--r--   0 runner    (1001) docker     (121)     5710 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     8351 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/plugin.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)     1482 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/source.py
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/vcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6811 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/vcs/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/vcs/git.py
--rw-r--r--   0 runner    (1001) docker     (121)     6796 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/vcs/gitcli.py
--rw-r--r--   0 runner    (1001) docker     (121)     3966 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/vcs/mixins.py
--rw-r--r--   0 runner    (1001) docker     (121)     6929 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/src/pdm_bump/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    19323 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/tests/action_test.py
--rw-r--r--   0 runner    (1001) docker     (121)     4044 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/tests/plugin_test.py
--rw-r--r--   0 runner    (1001) docker     (121)    23999 2022-11-12 16:04:59.385260 pdm-bump-0.6.9/tests/version_test.py
--rw-------   0 runner    (1001) docker     (121)     2759 2022-11-12 16:05:23.581727 pdm-bump-0.6.9/PKG-INFO
+-rw-r--r--   0        0        0     1092 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/LICENSE
+-rw-r--r--   0        0        0     2397 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/README.md
+-rw-r--r--   0        0        0     3890 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/pyproject.toml
+-rw-r--r--   0        0        0      770 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/__init__.py
+-rw-r--r--   0        0        0      541 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/__init__.py
+-rw-r--r--   0        0        0     5964 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/base.py
+-rw-r--r--   0        0        0     1784 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/explicit.py
+-rw-r--r--   0        0        0     9068 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/increment.py
+-rw-r--r--   0        0        0     8128 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/preview.py
+-rw-r--r--   0        0        0     1193 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/actions/vcs.py
+-rw-r--r--   0        0        0      864 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/cli.py
+-rw-r--r--   0        0        0      251 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/core/__init__.py
+-rw-r--r--   0        0        0     7530 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/core/config.py
+-rw-r--r--   0        0        0     5755 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/core/logging.py
+-rw-r--r--   0        0        0     6908 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/core/version.py
+-rw-r--r--   0        0        0     4999 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/dynamic.py
+-rw-r--r--   0        0        0     5347 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/plugin.py
+-rw-r--r--   0        0        0        0 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/py.typed
+-rw-r--r--   0        0        0     2032 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/source.py
+-rw-r--r--   0        0        0      699 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/__init__.py
+-rw-r--r--   0        0        0     7057 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/core.py
+-rw-r--r--   0        0        0      948 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/git.py
+-rw-r--r--   0        0        0     6826 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/gitcli.py
+-rw-r--r--   0        0        0     3997 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/src/pdm_bump/vcs/mixins.py
+-rw-r--r--   0        0        0    28261 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/tests/action_test.py
+-rw-r--r--   0        0        0     4317 2023-04-10 20:10:12.664937 pdm-bump-0.7.0a1/tests/plugin_test.py
+-rw-r--r--   0        0        0    27307 2023-04-10 20:10:12.668938 pdm-bump-0.7.0a1/tests/version_test.py
+-rw-r--r--   0        0        0     2733 1970-01-01 00:00:00.000000 pdm-bump-0.7.0a1/PKG-INFO
```

### Comparing `pdm-bump-0.6.9/LICENSE` & `pdm-bump-0.7.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-bump-0.6.9/README.md` & `pdm-bump-0.7.0a1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # pdm-bump
 
 ![PyPI](https://img.shields.io/pypi/v/pdm-bump?logo=python&logoColor=%23cccccc)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
-A small PEP440 compliant bump utility for the [Python development master](https://pdm.fming.dev/)
+A small PEP440 compliant bump utility for PDM, the [Python Development Master](https://pdm.fming.dev/).
 
-## Why ?
+## Why?
 
-As of PEP621, the pyproject.toml supports project metadata including a project version. If you are using the PDM build backend (according to PEP517), you can also use a file provider that contains your version, which is often referred to as `dynamic` versions.
+As of PEP621, the pyproject.toml supports project metadata including a project version. If you are using the PDM build backend (according to PEP517), you can also use a file provider that contains your version, which is often referred to as a `dynamic` version.
 
 The project version itself must comply to PEP440, which tells us, that it must consist of
 
 * an optional epoch
 * a mandatory major version part
 * a mandatory minor version part
 * a mandatory micro version part
 * an optional pre-release part supporting alpha, beta or release-candidate part.
 
-Tools like bumpversion or bump2version use their own configuration an their own configuration and might not consider the PEP440 specifications.
+Tools like `bumpversion` or `bump2version` use their own configuration and might not conform to the PEP440 specification.
 
 ## Installation
 
-You can install it using either pip (`pip install [--user] pdm-bump`) or using the pdm cli (`pdm plugin add [--pip-args=--user] pdm-bump`).
+You can install it using either pip (`pip install [--user] pdm-bump`) or using the PDM CLI (`pdm self add [--pip-args=--user] pdm-bump`).
 
 ## Usage
 
 You can use it the following way:
 
 ```shell
 $ grep version= pyproject.toml
@@ -42,23 +42,23 @@
 ## VCS based actions
 
 **NOTE**: Currently, only `git` is supported as VCS provider.
 
 You can create tags based on your `pyproject.toml` version (or dynamic version) using the following command.
 
 ```shell
-$ pdm bump tag # Creates a git tag with a leading v
+$ pdm bump tag # creates a git tag with a leading v
 ```
 
 ## Contributing
 
 Feel free to submit issues and pull requests. Contributions are welcome.
 
 ## Pre-checks
 
 1. Tests: To run the tests for your current checks, run `pdm run pytest`.
-2. Tox: If you are using `pyenv` you can use `pdm run tox` to run the tests for all supported python versions.
-3. Code-Style: You can use `pdm check-style` to check code format.
+2. tox: If you are using `pyenv` you can use `pdm run tox` to run the tests for all supported Python versions.
+3. Code Style: You can use `pdm check-style` to check code format.
 4. Format: You can use `pdm format` to format your code.
-5. Commit messages: You can run `pdm check-commits` to run `gitlint` across your commit messages.
+5. Commit messages: You can run `pdm check-commits` to run `gitlint` on your commit messages.
 
-Before opening a Pull Request, make sure, that the quality gates should succeed.
+Before opening a Pull Request make sure that the quality gates are passed.
```

### Comparing `pdm-bump-0.6.9/pyproject.toml` & `pdm-bump-0.7.0a1/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 [project]
 name = "pdm-bump"
-version = "0.6.9"
+version = "0.7.0a1"
 readme = "README.md"
 description = "A plugin for PDM providing the ability to modify the version according to PEP440"
 authors = [
     { name = "Carsten Igel", email = "cig@bite-that-bit.de" },
 ]
 dependencies = [
     "pdm>=2.00",
     "annotated-types>=0.2.0",
     "typing-extensions>=4; python_version<='3.9'",
+    "tomlkit>=0.11.6",
+    "tomli>=2.0.1; python_version<='3.10'",
+    "pyproject-metadata>=0.6.1",
+    "tomli-w>=1.0.0",
 ]
 requires-python = ">=3.9"
 license = "MIT"
 
 [project.license-files]
 paths = [
     "LICENSE",
@@ -54,45 +58,80 @@
     "pylint>=2.14.5",
     "pycodestyle>=2.7.0",
 ]
 formatting = [
     "black>=22.6.0",
     "isort>=5.10.1",
     "licenseheaders>=0.8.8",
+    "autoflake>=2.0.2",
 ]
 release = [
     "gitlint>=0.17.0",
     "pip-audit>=2.4.4",
 ]
+static-code-analysis = [
+    "radon>=5.1.0",
+    "vulture>=2.7",
+    "bandit>=1.7.4",
+    "prospector>=0.12.2",
+]
+checkstyle = [
+    "pep8-naming>=0.13.3",
+]
 
 [tool.pdm.scripts]
 flake = "flake518 src/"
 mypy = "mypy src/"
 pylint = "pylint src/"
 isort = "isort src/"
 black = "black src/"
-copyright-headers = "licenseheaders -y 2021-2022 -o 'Carsten Igel' -n pdm-bump -d . -u https://github.com/carstencodes/pdm-bump -x src/pdm_bump/dynamic.py -t ./.licenseheader.j2 -E .py"
+autoflake = "autoflake --ignore-pass-statements --remove-all-unused-imports --in-place --recursive src"
+radon_cc = "radon cc --total-average --show-complexity --json --output-file radon.cc.json src/"
+radon_mi = "radon mi --show --json --output-file radon.mi.json src/"
+radon_hal = "radon hal --functions --json --output-file radon.hal.json src/"
+vulture = "vulture src/"
+bandit = "bandit src/"
+prospector = "prospector src/"
+copyright-headers = "licenseheaders -y 2021-2023 -o 'Carsten Igel' -n pdm-bump -d . -u https://github.com/carstencodes/pdm-bump -x src/pdm_bump/dynamic.py -t ./.licenseheader.j2 -E .py"
 
 [tool.pdm.scripts.check-style]
 composite = [
     "flake",
     "pylint",
     "mypy",
 ]
 
 [tool.pdm.scripts.format]
 composite = [
     "copyright-headers",
     "isort",
     "black",
+    "autoflake",
+]
+
+[tool.pdm.scripts.radon]
+composite = [
+    "radon_cc",
+    "radon_mi",
+    "radon_hal",
+]
+
+[tool.pdm.scripts.static-analysis]
+composite = [
+    "radon",
+    "vulture",
+    "bandit",
+    "prospector",
 ]
 
 [tool.pdm.scripts.check-commits]
 shell = "gitlint --commits $(git describe --tags --abbrev=0)..HEAD lint"
 
+[tool.pdm.plugins]
+
 [tool.pylint.MAIN]
 fail-under = 9
 ignore = "vcs"
 
 [tool.pylint."MESSAGES CONTROL"]
 disable = [
     "C0114",
```

### Comparing `pdm-bump-0.6.9/src/pdm_bump/__init__.py` & `pdm-bump-0.7.0a1/src/pdm_bump/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #
-# Copyright (c) 2021-2022 Carsten Igel.
+# SPDX-License-Identifier: MIT
+#
+# Copyright (c) 2021-2023 Carsten Igel.
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 from importlib.metadata import PackageNotFoundError
 from importlib.metadata import version as __get_version
-from typing import Final, List
+from typing import Final
 
 from .cli import main as register_plugin
 
 main = register_plugin
 
 
 def _get_version(name: str) -> str:
@@ -22,8 +24,8 @@
     except PackageNotFoundError:
         # Only occurs in development, since package is not installed properly
         return "0.0.0"
 
 
 __version__: Final[str] = _get_version(__package__ or __name__)
 
-__all__: List[str] = [main.__name__]
+__all__: list[str] = [main.__name__]
```

### Comparing `pdm-bump-0.6.9/src/pdm_bump/cli.py` & `pdm-bump-0.7.0a1/src/pdm_bump/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 #
-# Copyright (c) 2021-2022 Carsten Igel.
+# SPDX-License-Identifier: MIT
+#
+# Copyright (c) 2021-2023 Carsten Igel.
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
-from typing import Optional, Protocol, Type
+from typing import Optional, Protocol
 
 # MyPy cannot resolve this during pull request
 from pdm.project.config import ConfigItem as _ConfigItem  # type: ignore
 
 from .plugin import BumpCommand as _Command
 
 
 class _CoreLike(Protocol):
     def register_command(
-        self, command: Type[_Command], name: Optional[str] = None
+        self, command: type[_Command], name: Optional[str] = None
     ) -> None:
         # Method empty: Only a protocol stub
         pass
 
     @staticmethod
     def add_config(name: str, config_item: _ConfigItem) -> None:
         # Method empty: Only a protocol stub
```

### Comparing `pdm-bump-0.6.9/src/pdm_bump/dynamic.py` & `pdm-bump-0.7.0a1/src/pdm_bump/dynamic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 #
-# Copyright (c) 2021-2022 Carsten Igel, Chase Sterling.
+# SPDX-License-Identifier: MIT
+#
+# Copyright (c) 2021-2023 Carsten Igel, Chase Sterling.
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 from functools import cached_property
 from pathlib import Path
-from re import M as MultilinePattern
+from re import M as MultilinePattern  # noqa: N811
 from re import Match, Pattern
 from re import compile as compile_re
 from typing import Final, Optional, cast
 
-from .config import Config
-from .version import Pep440VersionFormatter, Version
+from .core.config import Config, ConfigKeys, ConfigValues
+from .core.version import Pep440VersionFormatter, Version
 
 DEFAULT_REGEX: Final[Pattern[str]] = compile_re(
     r"^__version__\s*=\s*[\"'](?P<version>.+?)[\"']\s*(?:#.*)?$",
     MultilinePattern,
 )
 
 
@@ -44,67 +46,65 @@
         return self.__pattern
 
     @cached_property
     def dynamic_version(self) -> Optional[str]:
         with self.__file.open("r", encoding=self.__file_encoding) as file_ptr:
             match = self.__pattern.search(file_ptr.read())
         if match is not None:
-            return match.group("version")
+            return match.group(ConfigKeys.VERSION)
         return None
 
     def replace_dynamic_version(self, new_version: str) -> None:
         with self.__file.open("r", encoding=self.__file_encoding) as file_ptr:
             version_file = file_ptr.read()
             match = self.__pattern.search(version_file)
             if match is None:
                 raise ValueError("Failed to fetch version")
             match = cast(Match[str], match)
-            version_start, version_end = match.span("version")
+            version_start, version_end = match.span(ConfigKeys.VERSION)
             new_version_file = (
                 version_file[:version_start]
                 + new_version
                 + version_file[version_end:]
             )
         with self.__file.open("w", encoding=self.__file_encoding) as file_ptr:
             file_ptr.write(new_version_file)
 
     @staticmethod
     def find_dynamic_config(
         root_path: Path, project_config: Config
     ) -> Optional["DynamicVersionConfig"]:
         if (
-            project_config.get_pyproject_value("build-system", "build-backend")
-            == "pdm.pep517.api"
-            and project_config.get_pyproject_value(
-                "tool", "pdm", "version", "source"
+            project_config.get_pyproject_build_system(ConfigKeys.BUILD_BACKEND)
+            == ConfigValues.BUILD_BACKEND_PDM_PEP517_API
+            and project_config.get_pyproject_tool_config(
+                ConfigKeys.VERSION, ConfigKeys.VERSION_SOURCE
             )
-            == "file"
+            == ConfigValues.VERSION_SOURCE_FILE
         ):
-            file_path = project_config.get_pyproject_value(
-                "tool", "pdm", "version", "path"
+            file_path = project_config.get_pyproject_tool_config(
+                ConfigKeys.VERSION, ConfigKeys.VERSION_SOURCE_FILE_PATH
             )
             return DynamicVersionConfig(
                 file_path=root_path / file_path,
                 pattern=DEFAULT_REGEX,
             )
         return None
 
 
-class DynamicVersionSource:
+# Justification: Implementation of minimal protocol
+class DynamicVersionSource:  # pylint: disable=R0903
     def __init__(self, project_root: Path, config: Config) -> None:
         self.__project_root = project_root
         self.__config = config
         self.__current_version: Optional[Version] = None
 
     @property
     def is_enabled(self) -> bool:
-        dynamic_items: Optional[list[str]] = cast(
-            list[str], self.__config.get_pyproject_value("project", "dynamic")
-        )
-        return dynamic_items is not None and "version" in dynamic_items
+        return self.__config.meta_data.is_dynamic_version
 
     def __get_current_version(self) -> Version:
         if self.__current_version is not None:
             return cast(Version, self.__current_version)
 
         dynamic: DynamicVersionConfig = self.__get_dynamic_version()
         version: Optional[str] = dynamic.dynamic_version
@@ -114,25 +114,20 @@
         raise ValueError(
             f"Failed to find version in {dynamic.file}. "
             f"Make sure it matches {dynamic.pattern}"
         )
 
     def __set_current_version(self, version: Version) -> None:
         self.__current_version = version
-
-    current_version = property(__get_current_version, __set_current_version)
-
-    def save_value(self) -> None:
-        if self.__current_version is None:
-            raise ValueError("No current value set")
-        version: Version = cast(Version, self.__current_version)
         ver: str = Pep440VersionFormatter().format(version)
         config: DynamicVersionConfig = self.__get_dynamic_version()
         config.replace_dynamic_version(ver)
 
+    current_version = property(__get_current_version, __set_current_version)
+
     def __get_dynamic_version(self) -> DynamicVersionConfig:
         dynamic_version: Optional[
             DynamicVersionConfig
         ] = DynamicVersionConfig.find_dynamic_config(
             self.__project_root, self.__config
         )
         if dynamic_version is not None:
```

### Comparing `pdm-bump-0.6.9/src/pdm_bump/logging.py` & `pdm-bump-0.7.0a1/src/pdm_bump/core/logging.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 #
-# Copyright (c) 2021-2022 Carsten Igel.
+# SPDX-License-Identifier: MIT
+#
+# Copyright (c) 2021-2023 Carsten Igel.
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
+from collections.abc import Mapping
 from logging import (
     CRITICAL,
     DEBUG,
     ERROR,
     INFO,
     NOTSET,
     WARN,
@@ -19,28 +22,28 @@
     Handler,
     Logger,
     LogRecord,
     StreamHandler,
     getLogger,
 )
 from sys import stderr, stdout
-from typing import Any, Dict, Final, Mapping, Optional, Tuple, cast
+from typing import Any, Final, Optional, cast
 
 # MyPy does not recognize this during pull requests
 from pdm.termui import UI, Verbosity  # type: ignore
 
 
 def _get_has_rich():
     try:
         # Justification: Required to find module, not more
         import rich  # noqa: F401 pylint: disable=C0415,W0611
     except ImportError:
         return False
-    else:
-        return True
+
+    return True
 
 
 HAS_RICH: Final[bool] = _get_has_rich()
 
 if HAS_RICH:
     from rich.console import Console
     from rich.default_styles import DEFAULT_STYLES
@@ -77,28 +80,28 @@
 # Justification: Only one method to override
 class _ErrorWarningsFilter(Filter):  # pylint: disable=R0903
     def __init__(self, invert: Optional[bool] = False) -> None:
         self.__invert: bool = invert or False
         super().__init__()
 
     def filter(self, record: LogRecord) -> bool:
-        warning_and_above: Tuple[int, ...] = (WARN, WARNING, ERROR, CRITICAL)
+        warning_and_above: tuple[int, ...] = (WARN, WARNING, ERROR, CRITICAL)
         return (
             record.levelno in warning_and_above
             if not self.__invert
             else record.levelno not in warning_and_above
         )
 
 
 class TracingLogger(Logger):
     def trace(self, msg: str, *args: Any, **kwargs) -> None:
         self.log(TRACE, msg, *args, **kwargs)
 
     # Justification: Overriding inherited method
-    def makeRecord(  # pylint: disable=R0913
+    def makeRecord(  # noqa: N802 pylint: disable=R0913
         self,
         name: str,
         level: int,
         fn: str,
         lno: int,
         msg: Any,
         args: Any,
@@ -118,15 +121,15 @@
 
 Logger.manager.setLoggerClass(TracingLogger)
 
 
 def _get_rich_logger() -> TracingLogger:
     _logger: TracingLogger = cast(TracingLogger, getLogger("pdm-bump"))
 
-    styles: Dict[str, StyleType] = {}
+    styles: dict[str, StyleType] = {}
     styles.update(DEFAULT_STYLES)
     styles.update(
         {
             "logging.level.notset": Style(dim=True),
             "logging.level.trace": Style(dim=True, color="bright_black"),
             "logging.level.debug": Style(dim=True, color="white"),
             "logging.level.info": Style(color="blue"),
```

### Comparing `pdm-bump-0.6.9/src/pdm_bump/source.py` & `pdm-bump-0.7.0a1/src/pdm_bump/source.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,49 +1,68 @@
 #
-# Copyright (c) 2021-2022 Carsten Igel.
+# SPDX-License-Identifier: MIT
+#
+# Copyright (c) 2021-2023 Carsten Igel.
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 
-from typing import Protocol, cast
+from typing import Protocol, Union, cast, runtime_checkable
 
-from .config import Config
-from .version import Pep440VersionFormatter, Version
+from .core.config import Config, ConfigKeys
+from .core.logging import logger
+from .core.version import Pep440VersionFormatter, Version
 
 
 # Justification: Minimal protocol
 class _ProjectWriter(Protocol):  # pylint: disable=R0903
+    def write(self, show_message: bool) -> None:
+        # Method empty: Only a protocol stub
+        pass
+
+
+@runtime_checkable
+class _ProjectWriterClassic(Protocol):  # pylint: disable=R0903
     def write_pyproject(self, show_message: bool) -> None:
         # Method empty: Only a protocol stub
         pass
 
 
-class StaticPep621VersionSource:
-    def __init__(self, project: _ProjectWriter, config: Config) -> None:
-        self.__project = project
+# Justification: Minimal protocol
+@runtime_checkable
+class _ProjectWriterHolder(Protocol):  # pylint: disable=R0903
+    pyproject: _ProjectWriter
+
+
+# Justification: Implementation of minimal protocol
+class StaticPep621VersionSource:  # pylint: disable=R0903
+    def __init__(
+        self,
+        _: Union[_ProjectWriterHolder, _ProjectWriterClassic],
+        config: Config,
+    ) -> None:
         self.__config = config
 
     @property
     def is_enabled(self) -> bool:
         return (
-            self.__config.get_pyproject_value("project", "version") is not None
+            self.__config.get_pyproject_metadata(ConfigKeys.VERSION)
+            is not None
         )
 
     def __get_current_version(self) -> Version:
         version: str = cast(
-            str, self.__config.get_pyproject_value("project", "version")
+            str, self.__config.get_pyproject_metadata(ConfigKeys.VERSION)
         )
         return Version.from_string(version)
 
     def __set_current_version(self, ver: Version) -> None:
         formatter: Pep440VersionFormatter = Pep440VersionFormatter()
         version: str = formatter.format(ver)
-        self.__config.set_pyproject_value(version, "project", "version")
+        logger.debug("Setting new version %s", version)
+        self.__config.set_pyproject_metadata(version, ConfigKeys.VERSION)
 
     current_version = property(__get_current_version, __set_current_version)
-
-    def save_value(self) -> None:
-        self.__project.write_pyproject(True)
```

### Comparing `pdm-bump-0.6.9/src/pdm_bump/vcs/__init__.py` & `pdm-bump-0.7.0a1/src/pdm_bump/vcs/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 #
-# Copyright (c) 2021-2022 Carsten Igel.
+# SPDX-License-Identifier: MIT
+#
+# Copyright (c) 2021-2023 Carsten Igel.
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 from .core import (
     DefaultVcsProvider,
     VcsProvider,
+    VcsProviderAggregator,
     VcsProviderFactory,
     VcsProviderRegistry,
     vcs_provider,
     vcs_providers,
 )
 
 # Justification: Add items to registry
 from .gitcli import *  # noqa: disable=F401,F403
 
 __all__ = (
     "vcs_provider",
     "vcs_providers",
     "VcsProvider",
+    "VcsProviderAggregator",
     "VcsProviderFactory",
     "VcsProviderRegistry",
     "DefaultVcsProvider",
 )
```

### Comparing `pdm-bump-0.6.9/src/pdm_bump/vcs/core.py` & `pdm-bump-0.7.0a1/src/pdm_bump/vcs/core.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,33 +1,24 @@
 #
-# Copyright (c) 2021-2022 Carsten Igel.
+# SPDX-License-Identifier: MIT
+#
+# Copyright (c) 2021-2023 Carsten Igel.
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 from abc import ABC, abstractmethod
+from collections.abc import Iterator
 from pathlib import Path
-from typing import (
-    AnyStr,
-    Callable,
-    Dict,
-    Final,
-    Iterator,
-    NamedTuple,
-    Optional,
-    Tuple,
-    Type,
-    Union,
-    cast,
-)
+from typing import AnyStr, Callable, Final, NamedTuple, Optional, Union, cast
 
-from ..version import Pep440VersionFormatter, Version
+from ..core.version import Pep440VersionFormatter, Version
 
 _Pathlike = Union[Path, AnyStr]
 
 
 class _PathLikeConverter(ABC):
     @staticmethod
     def _pathlike_to_path(path: _Pathlike) -> Path:
@@ -62,15 +53,15 @@
 
     @property
     @abstractmethod
     def is_clean(self) -> bool:
         raise NotImplementedError()
 
     @abstractmethod
-    def check_in_items(self, message: str, *files: Tuple[Path, ...]) -> None:
+    def check_in_items(self, message: str, *files: tuple[Path, ...]) -> None:
         raise NotImplementedError()
 
     def create_tag_from_version(
         self, version: Version, prepend_letter_v: bool = True
     ) -> None:
         version_formatted: str = Pep440VersionFormatter().format(version)
         if prepend_letter_v:
@@ -90,14 +81,23 @@
         raise NotImplementedError()
 
     @abstractmethod
     def get_changes_not_checked_in(self) -> int:
         raise NotImplementedError()
 
 
+class VcsProviderAggregator:
+    def __init__(self, vcs_provider: VcsProvider, **kwargs) -> None:
+        self.__vcs_provider: VcsProvider = vcs_provider
+
+    @property
+    def vcs_provider(self) -> VcsProvider:
+        return self.__vcs_provider
+
+
 class VcsProviderFactory(_PathLikeConverter, ABC):
     def force_create_provider(self, path: Path) -> VcsProvider:
         return self._create_provider(path)
 
     @abstractmethod
     def _create_provider(self, path: Path) -> VcsProvider:
         raise NotImplementedError()
@@ -154,15 +154,15 @@
                 is_valid_root_by_dir and is_valid_root_by_file
             )
 
         return is_repository_root
 
 
 class VcsProviderRegistry(
-    Dict[str, Callable[..., VcsProviderFactory]], _PathLikeConverter
+    dict[str, Callable[..., VcsProviderFactory]], _PathLikeConverter
 ):
     def find_repository_root(self, path: _Pathlike) -> Optional[VcsProvider]:
         real_path: Path = _PathLikeConverter._pathlike_to_path(path)
         return self.find_repository_root_by_path(real_path)
 
     def find_repository_root_by_path(
         self, path: Path
@@ -174,15 +174,15 @@
             ] = factory.find_repository_root_from_path(path)
             if result is not None:
                 return result
 
         return None
 
     def register(self, name: str) -> Callable:
-        def decorator(clazz: Type[VcsProvider]):
+        def decorator(clazz: type[VcsProvider]):
             if not issubclass(clazz, VcsProviderFactory):
                 raise ValueError(
                     f"{clazz.__name__} is not an sub-type of "
                     f"{VcsProviderFactory.__name__}"
                 )
 
             self[name] = clazz
@@ -205,15 +205,15 @@
     def is_available(self) -> bool:
         return True
 
     @property
     def is_clean(self) -> bool:
         return True
 
-    def check_in_items(self, message: str, *files: Tuple[Path, ...]) -> None:
+    def check_in_items(self, message: str, *files: tuple[Path, ...]) -> None:
         # Must not be provided
         pass
 
     def create_tag_from_string(self, version_formatted: str) -> None:
         # Must not be provided
         pass
```

### Comparing `pdm-bump-0.6.9/src/pdm_bump/vcs/git.py` & `pdm-bump-0.7.0a1/src/pdm_bump/vcs/git.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 #
-# Copyright (c) 2021-2022 Carsten Igel.
+# SPDX-License-Identifier: MIT
+#
+# Copyright (c) 2021-2023 Carsten Igel.
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 from abc import abstractmethod
+from collections.abc import Iterator
 from pathlib import Path
-from typing import Iterator
 
 from .core import VcsFileSystemIdentifier, VcsProvider, VcsProviderFactory
 
 
 class GitCommonVcsProviderFactory(VcsProviderFactory):
     __git_dir_provider = VcsFileSystemIdentifier(
         file_name=None, dir_name=".git"
```

### Comparing `pdm-bump-0.6.9/src/pdm_bump/vcs/gitcli.py` & `pdm-bump-0.7.0a1/src/pdm_bump/vcs/gitcli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 #
-# Copyright (c) 2021-2022 Carsten Igel.
+# SPDX-License-Identifier: MIT
+#
+# Copyright (c) 2021-2023 Carsten Igel.
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 from functools import cached_property
 from pathlib import Path
 from subprocess import CalledProcessError
-from typing import List, Optional, Tuple, cast
+from typing import Optional, cast
 
-from ..logging import logger
-from ..version import Version
+from ..core.logging import logger
+from ..core.version import Version
 from .core import VcsProvider, VcsProviderError, vcs_provider
 from .git import GitCommonVcsProviderFactory
 from .mixins import CliRunnerMixin
 
 
 class GitCliVcsProvider(VcsProvider, CliRunnerMixin):
     __GIT_EXECUTABLE_NAME = "git"
@@ -70,17 +72,17 @@
             return len(dirty_files) == 0
         except CalledProcessError as cpe:
             raise VcsProviderError(
                 f"Failed to check if {self.current_path} is a clean "
                 f"git repository. Reason: {cpe.stderr}"
             ) from cpe
 
-    def check_in_items(self, message: str, *files: Tuple[Path, ...]) -> None:
+    def check_in_items(self, message: str, *files: tuple[Path, ...]) -> None:
         try:
-            args: List[str] = ["add", "--update"]
+            args: list[str] = ["add", "--update"]
             args.extend(str(f) for f in files)
             logger.debug(
                 "Checking in the following files: \n%s",
                 ", ".join([str(f) for f in files]),
             )
             _ = self.run(
                 self.git_executable_path,
```

### Comparing `pdm-bump-0.6.9/src/pdm_bump/vcs/mixins.py` & `pdm-bump-0.7.0a1/src/pdm_bump/vcs/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 #
-# Copyright (c) 2021-2022 Carsten Igel.
+# SPDX-License-Identifier: MIT
+#
+# Copyright (c) 2021-2023 Carsten Igel.
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 
 from os import environ, pathsep
 from pathlib import Path
 from subprocess import run as stdlib_run_process
 from sys import platform
-from typing import Optional, Protocol, Tuple, Union, cast
+from typing import Optional, Protocol, Union, cast
 
-from ..logging import logger
+from ..core.logging import logger
 
 
 class _CompletedProcessLike(Protocol):
     @property
     def returncode(self) -> int:
         raise NotImplementedError()
 
@@ -105,19 +107,19 @@
         logger.debug("Could not find %s", executable_full_name)
         return None
 
     def run(
         self,
         /,
         executable: Path,
-        args: Tuple[str, ...],
+        args: tuple[str, ...],
         *,
         raise_on_exit: bool = False,
         cwd: Optional[Path] = None,
-    ) -> Tuple[int, str, str]:
+    ) -> tuple[int, str, str]:
         cmd = []
         cmd.append(str(executable))
         for arg in args:
             cmd.append(arg)
 
         logger.debug(
             "Running command '%s' with args [%s]",
```

### Comparing `pdm-bump-0.6.9/src/pdm_bump/version.py` & `pdm-bump-0.7.0a1/src/pdm_bump/core/version.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,23 @@
 #
-# Copyright (c) 2021-2022 Carsten Igel.
+# SPDX-License-Identifier: MIT
+#
+# Copyright (c) 2021-2023 Carsten Igel.
 #
 # This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
 # This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 
 # Implementation of the PEP 440 version.
 from dataclasses import dataclass, field
 from functools import total_ordering
-from typing import (
-    Annotated,
-    Any,
-    Final,
-    List,
-    Literal,
-    Optional,
-    Tuple,
-    cast,
-    final,
-)
+from typing import Annotated, Any, Final, Literal, Optional, cast, final
 
 from annotated_types import Ge
 from packaging.version import InvalidVersion
 from packaging.version import Version as BaseVersion
 
 from .logging import traced_function
 
@@ -43,24 +35,24 @@
 @final
 @dataclass(eq=False, order=False, frozen=True)
 @total_ordering
 class Version:
     epoch: NonNegativeInteger = field(
         default=0, repr=True, hash=True, compare=True
     )
-    release_tuple: Tuple[NonNegativeInteger, ...] = field(default=(1, 0, 0))
+    release_tuple: tuple[NonNegativeInteger, ...] = field(default=(1, 0, 0))
     preview: Optional[
-        Tuple[
+        tuple[
             Literal["a", "b", "c", "alpha", "beta", "rc"], NonNegativeInteger
         ]
     ] = field(default=None, repr=True, hash=True, compare=True)
-    post: Optional[Tuple[Literal["post"], NonNegativeInteger]] = field(
+    post: Optional[tuple[Literal["post"], NonNegativeInteger]] = field(
         default=None, repr=True, hash=True, compare=True
     )
-    dev: Optional[Tuple[Literal["dev"], NonNegativeInteger]] = field(
+    dev: Optional[tuple[Literal["dev"], NonNegativeInteger]] = field(
         default=None, repr=True, hash=True, compare=True
     )
     local: Optional[str] = field(
         default=None, repr=True, hash=True, compare=True
     )
 
     def __post_init__(self):
@@ -81,15 +73,15 @@
     @property
     def micro(self) -> NonNegativeInteger:
         return self.release_tuple[2] if len(self.release_tuple) >= 3 else 0
 
     @property
     def release(
         self,
-    ) -> Tuple[NonNegativeInteger, NonNegativeInteger, NonNegativeInteger]:
+    ) -> tuple[NonNegativeInteger, NonNegativeInteger, NonNegativeInteger]:
         return (
             self.major,
             self.minor,
             self.micro,
         )
 
     @property
@@ -106,30 +98,30 @@
 
     @property
     def is_local_version(self) -> bool:
         return self.local is not None
 
     @property
     def is_alpha(self) -> bool:
-        alpha_part: Final[Tuple[str, ...]] = ("a", "alpha")
+        alpha_part: Final[tuple[str, ...]] = ("a", "alpha")
         return self.preview is not None and self.__compare_preview(alpha_part)
 
     @property
     def is_beta(self) -> bool:
-        beta_part: Final[Tuple[str, ...]] = ("b", "beta")
+        beta_part: Final[tuple[str, ...]] = ("b", "beta")
         return self.preview is not None and self.__compare_preview(beta_part)
 
     @property
     def is_release_candidate(self) -> bool:
-        rc_part: Final[Tuple[str, ...]] = ("c", "rc")
+        rc_part: Final[tuple[str, ...]] = ("c", "rc")
         return self.preview is not None and self.__compare_preview(rc_part)
 
-    def __compare_preview(self, valid_parts: Tuple[str, ...]) -> bool:
+    def __compare_preview(self, valid_parts: tuple[str, ...]) -> bool:
         if self.preview is not None:
-            pre: Tuple[str, int] = cast(Tuple[str, int], self.preview)
+            pre: tuple[str, int] = cast(tuple[str, int], self.preview)
             return pre[0] in valid_parts
         return False
 
     def __eq__(self, other: Any) -> bool:
         if not isinstance(other, Version):
             raise ValueError(f"{other} must be an instance of Version")
         other_version: Version = cast(Version, other)
@@ -177,15 +169,15 @@
             _version: BaseVersion = BaseVersion(version)
 
             return Version(
                 _version.epoch,
                 _version.release,
                 cast(
                     Optional[
-                        Tuple[
+                        tuple[
                             Literal["a", "b", "c", "alpha", "beta", "rc"], int
                         ]
                     ],
                     _version.pre,
                 ),
                 ("post", _version.post) if _version.post is not None else None,
                 ("dev", _version.dev) if _version.dev is not None else None,
@@ -206,15 +198,15 @@
 
 
 @final
 # Justification: Only method to provide
 class Pep440VersionFormatter:  # pylint: disable=R0903
     @traced_function
     def format(self, version: Version) -> str:
-        parts: List[str] = []
+        parts: list[str] = []
 
         if version.epoch > 0:
             parts.append(f"{version.epoch}!")
 
         parts.append(".".join(str(part) for part in version.release))
 
         if version.preview is not None:
```

### Comparing `pdm-bump-0.6.9/tests/plugin_test.py` & `pdm-bump-0.7.0a1/tests/plugin_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 #
-# Copyright (c) 2021-2022 Carsten Igel.
+# SPDX-License-Identifier: MIT
 #
-# This file is part of pdm-bump 
+# Copyright (c) 2021-2023 Carsten Igel.
+#
+# This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
-# This file is published using the MIT license. 
+# This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 
 from unittest import TestCase
-from typing import Type, Optional, Dict, List, Tuple, Iterable
+from typing import Optional
+from collections.abc import Iterable
 from argparse import ArgumentParser, Namespace, ArgumentError
 
-from pdm.core import Core
 from pdm.project.config import ConfigItem
 from pdm.cli.commands.base import BaseCommand
 
 from pdm_bump.cli import main
 from pdm_bump.plugin import BumpCommand
 
 
-_registered_configurations: Dict[str, ConfigItem] = {}
+_registered_configurations: dict[str, ConfigItem] = {}
 
 
-class _CoreStub(object):
-    registered_command: Optional[Type[BaseCommand]] = None
+class _CoreStub:
+    registered_command: Optional[type[BaseCommand]] = None
     registered_name: Optional[str] = None
 
-    def register_command(self, command: Type[BaseCommand], name: Optional[str] = None) -> None:
+    def register_command(
+        self, command: type[BaseCommand], name: Optional[str] = None
+    ) -> None:
         self.registered_command = command
         self.registered_name = name
 
     @staticmethod
     def add_config(name: str, config_item: ConfigItem) -> None:
         _registered_configurations[str] = config_item
 
@@ -39,46 +43,52 @@
 class CliRegistrationTest(TestCase):
     def tearDown(self) -> None:
         _registered_configurations.clear()
 
     def test_registration_command_type(self) -> None:
         core: _CoreStub = _CoreStub()
         main(core)
-        self.assertEqual(core.registered_command, BumpCommand, "The command is registered correctly")
+        self.assertEqual(
+            core.registered_command,
+            BumpCommand,
+            "The command is registered correctly",
+        )
 
     def test_registration_command_name(self) -> None:
         core: _CoreStub = _CoreStub()
         main(core)
         self.assertIsNone(core.registered_name, "No name has been supplied")
 
     def test_registered_config_items(self) -> None:
         core: _CoreStub = _CoreStub()
         main(core)
-        self.assert_(len(_registered_configurations) == 0, "No config item has been registered")
+        self.assertTrue(
+            len(_registered_configurations) == 0,
+            "No config item has been registered",
+        )
 
 
 class BumpVersionCommandParserTests(TestCase):
-    SUB_TEST_PARAMS_WHAT_SUCCESS: Iterable[Tuple[str, str]] = [
-
+    SUB_TEST_PARAMS_WHAT_SUCCESS: Iterable[tuple[str, str]] = [
         ("major", "major"),
         ("minor", "minor"),
         ("micro", "micro"),
         ("patch", "patch"),
         ("pre-release", "pre-release"),
         ("no-pre-release", "no-pre-release"),
         ("post", "post"),
         ("dev", "dev"),
     ]
-    SUB_TEST_PARAMS_PRE_SUCCESS: Iterable[Tuple[str, str]] = [
+    SUB_TEST_PARAMS_PRE_SUCCESS: Iterable[tuple[str, str]] = [
         ("alpha", "alpha"),
         ("beta", "beta"),
         ("c", "c"),
         ("rc", "rc"),
     ]
-    SUB_TEST_PARAMS_FAIL: Iterable[Tuple[str, List[str]]] = [
+    SUB_TEST_PARAMS_FAIL: Iterable[tuple[str, list[str]]] = [
         ("major", ["maj"]),
         ("minor", ["min"]),
         ("micro", ["mic"]),
         ("patch", ["pa"]),
         ("pre-release", ["pre"]),
         ("no-pre-release", ["no-pre"]),
         ("alpha", ["pre-release", "--pre", "a"]),
@@ -89,25 +99,33 @@
 
     def test_parser_setup_what_success(self) -> None:
         parser: ArgumentParser = ArgumentParser()
         _ = BumpCommand(parser)
 
         for msg, what_success in self.SUB_TEST_PARAMS_WHAT_SUCCESS:
             with self.subTest(msg, what=what_success):
-                options: Namespace = parser.parse_args([ what_success ])
-                self.assertEqual(options.what, what_success, "The first item is only matched")
+                options: Namespace = parser.parse_args([what_success])
+                self.assertEqual(
+                    options.selected_command,
+                    what_success,
+                    "The first item is only matched",
+                )
 
     def test_parser_setup_pre_success(self) -> None:
         parser: ArgumentParser = ArgumentParser()
         _ = BumpCommand(parser)
 
         for msg, pre_success in self.SUB_TEST_PARAMS_PRE_SUCCESS:
             with self.subTest(msg, pre=pre_success):
-                options: Namespace = parser.parse_args([ "pre-release", "--pre", pre_success ])
-                self.assertEqual(options.pre, pre_success, "The second item is only matched")
+                options: Namespace = parser.parse_args(
+                    ["pre-release", "--pre", pre_success]
+                )
+                self.assertEqual(
+                    options.pre_release_part, pre_success, "The second item is only matched"
+                )
 
     def test_parser_setup_fail(self) -> None:
         parser: ArgumentParser = ArgumentParser(exit_on_error=False)
         _ = BumpCommand(parser)
 
         for msg, options in self.SUB_TEST_PARAMS_FAIL:
             with self.subTest(msg, options=options):
```

### Comparing `pdm-bump-0.6.9/tests/version_test.py` & `pdm-bump-0.7.0a1/tests/version_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,36 @@
 #
-# Copyright (c) 2021-2022 Carsten Igel.
+# SPDX-License-Identifier: MIT
 #
-# This file is part of pdm-bump 
+# Copyright (c) 2021-2023 Carsten Igel.
+#
+# This file is part of pdm-bump
 # (see https://github.com/carstencodes/pdm-bump).
 #
-# This file is published using the MIT license. 
+# This file is published using the MIT license.
 # Refer to LICENSE for more information
 #
 
 import unittest
 
-from typing import Tuple, List, Final, final
+from typing import Final, final
+
+from pdm_bump.core.version import (
+    Version,
+    VersionParserError,
+    Pep440VersionFormatter,
+    BaseVersion,
+)
 
-from pdm_bump.version import Version, VersionParserError, Pep440VersionFormatter, BaseVersion
 
 @final
 class ParseVersionTest(unittest.TestCase):
-    SUB_TESTS_VERSION_FROM_STR_RLS: Final[List[Tuple[str, str, Tuple[int, int, int]]]] = [
+    SUB_TESTS_VERSION_FROM_STR_RLS: Final[
+        list[tuple[str, str, tuple[int, int, int]]]
+    ] = [
         ("Regular default version", "1.0.0", (1, 0, 0)),
         ("Regular default version no micro", "1.0", (1, 0, 0)),
         ("Regular default version no minor and no micro", "1", (1, 0, 0)),
         ("Pre-fixed default version", "v1.0.0", (1, 0, 0)),
         ("Pre-fixed default version no micro", "v1.0", (1, 0, 0)),
         ("Pre-fixed default version no minor and no micro", "v1", (1, 0, 0)),
         ("Regular non-final version", "0.1.0", (0, 1, 0)),
@@ -31,25 +41,35 @@
         ("Regular version no micro", "6.2", (6, 2, 0)),
         ("Regular version no minor and no micro", "6", (6, 0, 0)),
         ("Pre-fixed version", "v6.2.13", (6, 2, 13)),
         ("Pre-fixed version no micro", "v6.2", (6, 2, 0)),
         ("Pre-fixed version no minor and no micro", "v6", (6, 0, 0)),
         ("Regular double-digit version", "19.22.83", (19, 22, 83)),
         ("Regular double-digit version no micro", "19.22", (19, 22, 0)),
-        ("Regular double-digit version no minor and no micro", "19", (19, 0, 0)),
+        (
+            "Regular double-digit version no minor and no micro",
+            "19",
+            (19, 0, 0),
+        ),
         ("Pre-fixed double-digit version", "v19.22.83", (19, 22, 83)),
         ("Pre-fixed double-digit version no micro", "v19.22", (19, 22, 0)),
-        ("Pre-fixed double-digit version no minor and no micro", "v19", (19, 0, 0)),
+        (
+            "Pre-fixed double-digit version no minor and no micro",
+            "v19",
+            (19, 0, 0),
+        ),
     ]
-    SUB_TESTS_VERSION_FROM_STR_EPOCH: Final[List[Tuple[str, str, int]]] = [
+    SUB_TESTS_VERSION_FROM_STR_EPOCH: Final[list[tuple[str, str, int]]] = [
         ("No epoch set", "1.0.0", 0),
         ("Epoch is one", "1!1.0.0", 1),
         ("Epoch is double-digit", "17!1.0.0", 17),
     ]
-    SUB_TESTS_VERSION_FROM_STR_PRE: Final[List[Tuple[str, str, Tuple[str, int]]]] = [
+    SUB_TESTS_VERSION_FROM_STR_PRE: Final[
+        list[tuple[str, str, tuple[str, int]]]
+    ] = [
         ("None: Alpha short single digit no prefix", "0.1.0a1", ("a", 1)),
         ("None: Alpha long single digit no prefix", "0.1.0alpha1", ("a", 1)),
         ("None: Alpha short single digit prefix", "v0.1.0a1", ("a", 1)),
         ("None: Alpha long single digit prefix", "v0.1.0alpha1", ("a", 1)),
         ("None: Alpha short double digit no prefix", "0.1.0a23", ("a", 23)),
         ("None: Alpha long double digit no prefix", "0.1.0alpha23", ("a", 23)),
         ("None: Alpha short double digit prefix", "v0.1.0a23", ("a", 23)),
@@ -58,22 +78,54 @@
         ("None: Beta long single digit no prefix", "0.1.0beta1", ("b", 1)),
         ("None: Beta short single digit prefix", "v0.1.0b1", ("b", 1)),
         ("None: Beta long single digit prefix", "v0.1.0beta1", ("b", 1)),
         ("None: Beta short double digit no prefix", "0.1.0b42", ("b", 42)),
         ("None: Beta long double digit no prefix", "0.1.0beta42", ("b", 42)),
         ("None: Beta short double digit prefix", "v0.1.0b42", ("b", 42)),
         ("None: Beta long double digit prefix", "v0.1.0beta42", ("b", 42)),
-        ("None: Release-candidate short single digit no prefix", "0.1.0rc1", ("rc", 1)),
-        ("None: Release-candidate long single digit no prefix", "0.1.0rc1", ("rc", 1)),
-        ("None: Release-candidate short single digit prefix", "v0.1.0c1", ("rc", 1)),
-        ("None: Release-candidate long single digit prefix", "v0.1.0rc1", ("rc", 1)),
-        ("None: Release-candidate short double digit no prefix", "0.1.0rc99", ("rc", 99)),
-        ("None: Release-candidate long double digit no prefix", "0.1.0rc99", ("rc", 99)),
-        ("None: Release-candidate short double digit prefix", "v0.1.0c99", ("rc", 99)),
-        ("None: Release-candidate long double digit prefix", "v0.1.0rc99", ("rc", 99)),
+        (
+            "None: Release-candidate short single digit no prefix",
+            "0.1.0rc1",
+            ("rc", 1),
+        ),
+        (
+            "None: Release-candidate long single digit no prefix",
+            "0.1.0rc1",
+            ("rc", 1),
+        ),
+        (
+            "None: Release-candidate short single digit prefix",
+            "v0.1.0c1",
+            ("rc", 1),
+        ),
+        (
+            "None: Release-candidate long single digit prefix",
+            "v0.1.0rc1",
+            ("rc", 1),
+        ),
+        (
+            "None: Release-candidate short double digit no prefix",
+            "0.1.0rc99",
+            ("rc", 99),
+        ),
+        (
+            "None: Release-candidate long double digit no prefix",
+            "0.1.0rc99",
+            ("rc", 99),
+        ),
+        (
+            "None: Release-candidate short double digit prefix",
+            "v0.1.0c99",
+            ("rc", 99),
+        ),
+        (
+            "None: Release-candidate long double digit prefix",
+            "v0.1.0rc99",
+            ("rc", 99),
+        ),
         ("Dot: Alpha short single digit no prefix", "0.1.0.a1", ("a", 1)),
         ("Dot: Alpha long single digit no prefix", "0.1.0.alpha1", ("a", 1)),
         ("Dot: Alpha short single digit prefix", "v0.1.0.a1", ("a", 1)),
         ("Dot: Alpha long single digit prefix", "v0.1.0.alpha1", ("a", 1)),
         ("Dot: Alpha short double digit no prefix", "0.1.0.a23", ("a", 23)),
         ("Dot: Alpha long double digit no prefix", "0.1.0.alpha23", ("a", 23)),
         ("Dot: Alpha short double digit prefix", "v0.1.0.a23", ("a", 23)),
@@ -82,72 +134,242 @@
         ("Dot: Beta long single digit no prefix", "0.1.0.beta1", ("b", 1)),
         ("Dot: Beta short single digit prefix", "v0.1.0.b1", ("b", 1)),
         ("Dot: Beta long single digit prefix", "v0.1.0.beta1", ("b", 1)),
         ("Dot: Beta short double digit no prefix", "0.1.0.b42", ("b", 42)),
         ("Dot: Beta long double digit no prefix", "0.1.0.beta42", ("b", 42)),
         ("Dot: Beta short double digit prefix", "v0.1.0.b42", ("b", 42)),
         ("Dot: Beta long double digit prefix", "v0.1.0.beta42", ("b", 42)),
-        ("Dot: Release-candidate short single digit no prefix", "0.1.0.rc1", ("rc", 1)),
-        ("Dot: Release-candidate long single digit no prefix", "0.1.0.rc1", ("rc", 1)),
-        ("Dot: Release-candidate short single digit prefix", "v0.1.0.c1", ("rc", 1)),
-        ("Dot: Release-candidate long single digit prefix", "v0.1.0.rc1", ("rc", 1)),
-        ("Dot: Release-candidate short double digit no prefix", "0.1.0.rc99", ("rc", 99)),
-        ("Dot: Release-candidate long double digit no prefix", "0.1.0.rc99", ("rc", 99)),
-        ("Dot: Release-candidate short double digit prefix", "v0.1.0.c99", ("rc", 99)),
-        ("Dot: Release-candidate long double digit prefix", "v0.1.0.rc99", ("rc", 99)),
+        (
+            "Dot: Release-candidate short single digit no prefix",
+            "0.1.0.rc1",
+            ("rc", 1),
+        ),
+        (
+            "Dot: Release-candidate long single digit no prefix",
+            "0.1.0.rc1",
+            ("rc", 1),
+        ),
+        (
+            "Dot: Release-candidate short single digit prefix",
+            "v0.1.0.c1",
+            ("rc", 1),
+        ),
+        (
+            "Dot: Release-candidate long single digit prefix",
+            "v0.1.0.rc1",
+            ("rc", 1),
+        ),
+        (
+            "Dot: Release-candidate short double digit no prefix",
+            "0.1.0.rc99",
+            ("rc", 99),
+        ),
+        (
+            "Dot: Release-candidate long double digit no prefix",
+            "0.1.0.rc99",
+            ("rc", 99),
+        ),
+        (
+            "Dot: Release-candidate short double digit prefix",
+            "v0.1.0.c99",
+            ("rc", 99),
+        ),
+        (
+            "Dot: Release-candidate long double digit prefix",
+            "v0.1.0.rc99",
+            ("rc", 99),
+        ),
         ("Hyphen: Alpha short single digit no prefix", "0.1.0-a1", ("a", 1)),
-        ("Hyphen: Alpha long single digit no prefix", "0.1.0-alpha1", ("a", 1)),
+        (
+            "Hyphen: Alpha long single digit no prefix",
+            "0.1.0-alpha1",
+            ("a", 1),
+        ),
         ("Hyphen: Alpha short single digit prefix", "v0.1.0-a1", ("a", 1)),
         ("Hyphen: Alpha long single digit prefix", "v0.1.0-alpha1", ("a", 1)),
         ("Hyphen: Alpha short double digit no prefix", "0.1.0-a23", ("a", 23)),
-        ("Hyphen: Alpha long double digit no prefix", "0.1.0-alpha23", ("a", 23)),
+        (
+            "Hyphen: Alpha long double digit no prefix",
+            "0.1.0-alpha23",
+            ("a", 23),
+        ),
         ("Hyphen: Alpha short double digit prefix", "v0.1.0-a23", ("a", 23)),
-        ("Hyphen: Alpha long double digit prefix", "v0.1.0-alpha23", ("a", 23)),
+        (
+            "Hyphen: Alpha long double digit prefix",
+            "v0.1.0-alpha23",
+            ("a", 23),
+        ),
         ("Hyphen: Beta short single digit no prefix", "0.1.0-b1", ("b", 1)),
         ("Hyphen: Beta long single digit no prefix", "0.1.0-beta1", ("b", 1)),
         ("Hyphen: Beta short single digit prefix", "v0.1.0-b1", ("b", 1)),
         ("Hyphen: Beta long single digit prefix", "v0.1.0-beta1", ("b", 1)),
         ("Hyphen: Beta short double digit no prefix", "0.1.0-b42", ("b", 42)),
-        ("Hyphen: Beta long double digit no prefix", "0.1.0-beta42", ("b", 42)),
+        (
+            "Hyphen: Beta long double digit no prefix",
+            "0.1.0-beta42",
+            ("b", 42),
+        ),
         ("Hyphen: Beta short double digit prefix", "v0.1.0-b42", ("b", 42)),
         ("Hyphen: Beta long double digit prefix", "v0.1.0-beta42", ("b", 42)),
-        ("Hyphen: Release-candidate short single digit no prefix", "0.1.0-rc1", ("rc", 1)),
-        ("Hyphen: Release-candidate long single digit no prefix", "0.1.0-rc1", ("rc", 1)),
-        ("Hyphen: Release-candidate short single digit prefix", "v0.1.0-c1", ("rc", 1)),
-        ("Hyphen: Release-candidate long single digit prefix", "v0.1.0-rc1", ("rc", 1)),
-        ("Hyphen: Release-candidate short double digit no prefix", "0.1.0-rc99", ("rc", 99)),
-        ("Hyphen: Release-candidate long double digit no prefix", "0.1.0-rc99", ("rc", 99)),
-        ("Hyphen: Release-candidate short double digit prefix", "v0.1.0-c99", ("rc", 99)),
-        ("Hyphen: Release-candidate long double digit prefix", "v0.1.0-rc99", ("rc", 99)),
-        ("Underscore: Alpha short single digit no prefix", "0.1.0_a1", ("a", 1)),
-        ("Underscore: Alpha long single digit no prefix", "0.1.0_alpha1", ("a", 1)),
+        (
+            "Hyphen: Release-candidate short single digit no prefix",
+            "0.1.0-rc1",
+            ("rc", 1),
+        ),
+        (
+            "Hyphen: Release-candidate long single digit no prefix",
+            "0.1.0-rc1",
+            ("rc", 1),
+        ),
+        (
+            "Hyphen: Release-candidate short single digit prefix",
+            "v0.1.0-c1",
+            ("rc", 1),
+        ),
+        (
+            "Hyphen: Release-candidate long single digit prefix",
+            "v0.1.0-rc1",
+            ("rc", 1),
+        ),
+        (
+            "Hyphen: Release-candidate short double digit no prefix",
+            "0.1.0-rc99",
+            ("rc", 99),
+        ),
+        (
+            "Hyphen: Release-candidate long double digit no prefix",
+            "0.1.0-rc99",
+            ("rc", 99),
+        ),
+        (
+            "Hyphen: Release-candidate short double digit prefix",
+            "v0.1.0-c99",
+            ("rc", 99),
+        ),
+        (
+            "Hyphen: Release-candidate long double digit prefix",
+            "v0.1.0-rc99",
+            ("rc", 99),
+        ),
+        (
+            "Underscore: Alpha short single digit no prefix",
+            "0.1.0_a1",
+            ("a", 1),
+        ),
+        (
+            "Underscore: Alpha long single digit no prefix",
+            "0.1.0_alpha1",
+            ("a", 1),
+        ),
         ("Underscore: Alpha short single digit prefix", "v0.1.0_a1", ("a", 1)),
-        ("Underscore: Alpha long single digit prefix", "v0.1.0_alpha1", ("a", 1)),
-        ("Underscore: Alpha short double digit no prefix", "0.1.0_a23", ("a", 23)),
-        ("Underscore: Alpha long double digit no prefix", "0.1.0_alpha23", ("a", 23)),
-        ("Underscore: Alpha short double digit prefix", "v0.1.0_a23", ("a", 23)),
-        ("Underscore: Alpha long double digit prefix", "v0.1.0_alpha23", ("a", 23)),
-        ("Underscore: Beta short single digit no prefix", "0.1.0_b1", ("b", 1)),
-        ("Underscore: Beta long single digit no prefix", "0.1.0_beta1", ("b", 1)),
+        (
+            "Underscore: Alpha long single digit prefix",
+            "v0.1.0_alpha1",
+            ("a", 1),
+        ),
+        (
+            "Underscore: Alpha short double digit no prefix",
+            "0.1.0_a23",
+            ("a", 23),
+        ),
+        (
+            "Underscore: Alpha long double digit no prefix",
+            "0.1.0_alpha23",
+            ("a", 23),
+        ),
+        (
+            "Underscore: Alpha short double digit prefix",
+            "v0.1.0_a23",
+            ("a", 23),
+        ),
+        (
+            "Underscore: Alpha long double digit prefix",
+            "v0.1.0_alpha23",
+            ("a", 23),
+        ),
+        (
+            "Underscore: Beta short single digit no prefix",
+            "0.1.0_b1",
+            ("b", 1),
+        ),
+        (
+            "Underscore: Beta long single digit no prefix",
+            "0.1.0_beta1",
+            ("b", 1),
+        ),
         ("Underscore: Beta short single digit prefix", "v0.1.0_b1", ("b", 1)),
-        ("Underscore: Beta long single digit prefix", "v0.1.0_beta1", ("b", 1)),
-        ("Underscore: Beta short double digit no prefix", "0.1.0_b42", ("b", 42)),
-        ("Underscore: Beta long double digit no prefix", "0.1.0_beta42", ("b", 42)),
-        ("Underscore: Beta short double digit prefix", "v0.1.0_b42", ("b", 42)),
-        ("Underscore: Beta long double digit prefix", "v0.1.0_beta42", ("b", 42)),
-        ("Underscore: Release-candidate short single digit no prefix", "0.1.0_rc1", ("rc", 1)),
-        ("Underscore: Release-candidate long single digit no prefix", "0.1.0_rc1", ("rc", 1)),
-        ("Underscore: Release-candidate short single digit prefix", "v0.1.0_c1", ("rc", 1)),
-        ("Underscore: Release-candidate long single digit prefix", "v0.1.0_rc1", ("rc", 1)),
-        ("Underscore: Release-candidate short double digit no prefix", "0.1.0_rc99", ("rc", 99)),
-        ("Underscore: Release-candidate long double digit no prefix", "0.1.0_rc99", ("rc", 99)),
-        ("Underscore: Release-candidate short double digit prefix", "v0.1.0_c99", ("rc", 99)),
-        ("Underscore: Release-candidate long double digit prefix", "v0.1.0_rc99", ("rc", 99)),
+        (
+            "Underscore: Beta long single digit prefix",
+            "v0.1.0_beta1",
+            ("b", 1),
+        ),
+        (
+            "Underscore: Beta short double digit no prefix",
+            "0.1.0_b42",
+            ("b", 42),
+        ),
+        (
+            "Underscore: Beta long double digit no prefix",
+            "0.1.0_beta42",
+            ("b", 42),
+        ),
+        (
+            "Underscore: Beta short double digit prefix",
+            "v0.1.0_b42",
+            ("b", 42),
+        ),
+        (
+            "Underscore: Beta long double digit prefix",
+            "v0.1.0_beta42",
+            ("b", 42),
+        ),
+        (
+            "Underscore: Release-candidate short single digit no prefix",
+            "0.1.0_rc1",
+            ("rc", 1),
+        ),
+        (
+            "Underscore: Release-candidate long single digit no prefix",
+            "0.1.0_rc1",
+            ("rc", 1),
+        ),
+        (
+            "Underscore: Release-candidate short single digit prefix",
+            "v0.1.0_c1",
+            ("rc", 1),
+        ),
+        (
+            "Underscore: Release-candidate long single digit prefix",
+            "v0.1.0_rc1",
+            ("rc", 1),
+        ),
+        (
+            "Underscore: Release-candidate short double digit no prefix",
+            "0.1.0_rc99",
+            ("rc", 99),
+        ),
+        (
+            "Underscore: Release-candidate long double digit no prefix",
+            "0.1.0_rc99",
+            ("rc", 99),
+        ),
+        (
+            "Underscore: Release-candidate short double digit prefix",
+            "v0.1.0_c99",
+            ("rc", 99),
+        ),
+        (
+            "Underscore: Release-candidate long double digit prefix",
+            "v0.1.0_rc99",
+            ("rc", 99),
+        ),
     ]
-    SUB_TESTS_VERSION_FROM_STR_DEV: Final[List[Tuple[str, str, Tuple[str, int]]]] = [
+    SUB_TESTS_VERSION_FROM_STR_DEV: Final[
+        list[tuple[str, str, tuple[str, int]]]
+    ] = [
         ("Regular version zero digit none", "0.0.1dev0", ("dev", 0)),
         ("Regular version zero digit dot", "0.0.1.dev0", ("dev", 0)),
         ("Regular version zero digit hyphen", "0.0.1-dev0", ("dev", 0)),
         ("Regular version zero digit underscore", "0.0.1_dev0", ("dev", 0)),
         ("Regular version no digit none", "0.0.1dev", ("dev", 0)),
         ("Regular version no digit dot", "0.0.1.dev", ("dev", 0)),
         ("Regular version no digit hyphen", "0.0.1-dev", ("dev", 0)),
@@ -155,86 +377,155 @@
         ("Regular version single digit none", "0.0.1dev1", ("dev", 1)),
         ("Regular version single digit dot", "0.0.1.dev1", ("dev", 1)),
         ("Regular version single digit hyphen", "0.0.1-dev1", ("dev", 1)),
         ("Regular version single digit underscore", "0.0.1_dev1", ("dev", 1)),
         ("Regular version double digit none", "0.0.1dev57", ("dev", 57)),
         ("Regular version double digit dot", "0.0.1.dev57", ("dev", 57)),
         ("Regular version double digit hyphen", "0.0.1-dev57", ("dev", 57)),
-        ("Regular version double digit underscore", "0.0.1_dev57", ("dev", 57)),
+        (
+            "Regular version double digit underscore",
+            "0.0.1_dev57",
+            ("dev", 57),
+        ),
         ("Pre-fixed version single digit none", "v0.0.1dev1", ("dev", 1)),
         ("Pre-fixed version single digit dot", "v0.0.1.dev1", ("dev", 1)),
         ("Pre-fixed version single digit hyphen", "v0.0.1-dev1", ("dev", 1)),
-        ("Pre-fixed version single digit underscore", "v0.0.1_dev1", ("dev", 1)),
+        (
+            "Pre-fixed version single digit underscore",
+            "v0.0.1_dev1",
+            ("dev", 1),
+        ),
         ("Pre-fixed version double digit none", "v0.0.1dev57", ("dev", 57)),
         ("Pre-fixed version double digit dot", "v0.0.1.dev57", ("dev", 57)),
         ("Pre-fixed version double digit hyphen", "v0.0.1-dev57", ("dev", 57)),
-        ("Pre-fixed version double digit underscore", "v0.0.1_dev57", ("dev", 57)),
+        (
+            "Pre-fixed version double digit underscore",
+            "v0.0.1_dev57",
+            ("dev", 57),
+        ),
     ]
-    SUB_TESTS_VERSION_FROM_STR_POST: Final[List[Tuple[str, str, Tuple[str, int]]]] = [
+    SUB_TESTS_VERSION_FROM_STR_POST: Final[
+        list[tuple[str, str, tuple[str, int]]]
+    ] = [
         ("Regular version zero digit none", "2.0.0post0", ("post", 0)),
         ("Regular version zero digit dot", "2.0.0.post0", ("post", 0)),
         ("Regular version zero digit hyphen", "2.0.0-post0", ("post", 0)),
         ("Regular version zero digit underscore", "2.0.0_post0", ("post", 0)),
         ("Regular version no digit none", "2.0.0post", ("post", 0)),
         ("Regular version no digit dot", "2.0.0.post", ("post", 0)),
         ("Regular version no digit hyphen", "2.0.0-post", ("post", 0)),
         ("Regular version no digit underscore", "2.0.0_post", ("post", 0)),
         ("Regular version single digit none", "2.0.0post7", ("post", 7)),
         ("Regular version single digit dot", "2.0.0.post7", ("post", 7)),
         ("Regular version single digit hyphen", "2.0.0-post7", ("post", 7)),
-        ("Regular version single digit underscore", "2.0.0_post7", ("post", 7)),
+        (
+            "Regular version single digit underscore",
+            "2.0.0_post7",
+            ("post", 7),
+        ),
         ("Regular version double digit none", "2.0.0post63", ("post", 63)),
         ("Regular version double digit dot", "2.0.0.post63", ("post", 63)),
         ("Regular version double digit hyphen", "2.0.0-post63", ("post", 63)),
-        ("Regular version double digit underscore", "2.0.0_post63", ("post", 63)),
+        (
+            "Regular version double digit underscore",
+            "2.0.0_post63",
+            ("post", 63),
+        ),
         ("Regular version single digit special form", "2.0.0-3", ("post", 3)),
-        ("Regular version double digit special form", "2.0.0-78", ("post", 78)),
+        (
+            "Regular version double digit special form",
+            "2.0.0-78",
+            ("post", 78),
+        ),
         ("Pre-fixed version zero digit none", "v2.0.0post0", ("post", 0)),
         ("Pre-fixed version zero digit dot", "v2.0.0.post0", ("post", 0)),
         ("Pre-fixed version zero digit hyphen", "v2.0.0-post0", ("post", 0)),
-        ("Pre-fixed version zero digit underscore", "v2.0.0_post0", ("post", 0)),
+        (
+            "Pre-fixed version zero digit underscore",
+            "v2.0.0_post0",
+            ("post", 0),
+        ),
         ("Pre-fixed version no digit none", "v2.0.0post", ("post", 0)),
         ("Pre-fixed version no digit dot", "v2.0.0.post", ("post", 0)),
         ("Pre-fixed version no digit hyphen", "v2.0.0-post", ("post", 0)),
         ("Pre-fixed version no digit underscore", "v2.0.0_post", ("post", 0)),
         ("Pre-fixed version single digit none", "v2.0.0post7", ("post", 7)),
         ("Pre-fixed version single digit dot", "v2.0.0.post7", ("post", 7)),
         ("Pre-fixed version single digit hyphen", "v2.0.0-post7", ("post", 7)),
-        ("Pre-fixed version single digit underscore", "v2.0.0_post7", ("post", 7)),
+        (
+            "Pre-fixed version single digit underscore",
+            "v2.0.0_post7",
+            ("post", 7),
+        ),
         ("Pre-fixed version double digit none", "v2.0.0post63", ("post", 63)),
         ("Pre-fixed version double digit dot", "v2.0.0.post63", ("post", 63)),
-        ("Pre-fixed version double digit hyphen", "v2.0.0-post63", ("post", 63)),
-        ("Pre-fixed version double digit underscore", "v2.0.0_post63", ("post", 63)),
-        ("Pre-fixed version single digit special form", "v2.0.0-3", ("post", 3)),
-        ("Pre-fixed version double digit special form", "v2.0.0-78", ("post", 78)),
+        (
+            "Pre-fixed version double digit hyphen",
+            "v2.0.0-post63",
+            ("post", 63),
+        ),
+        (
+            "Pre-fixed version double digit underscore",
+            "v2.0.0_post63",
+            ("post", 63),
+        ),
+        (
+            "Pre-fixed version single digit special form",
+            "v2.0.0-3",
+            ("post", 3),
+        ),
+        (
+            "Pre-fixed version double digit special form",
+            "v2.0.0-78",
+            ("post", 78),
+        ),
     ]  # TODO: rev/r
-    SUB_TESTS_VERSION_FROM_STR_LOCAL: Final[List[Tuple[str, str, str]]] = [
+    SUB_TESTS_VERSION_FROM_STR_LOCAL: Final[list[tuple[str, str, str]]] = [
         ("Regular version single digit plus", "3.1.4+2", "2"),
         ("Regular version double digit plus", "3.1.4+12", "12"),
         ("Regular version alpha-numeric plus", "3.1.4+af2b", "af2b"),
-        ("Regular version hyphen plus", "3.1.4+just-my-2-cents", "just.my.2.cents"),
-        ("Regular version hyphen underscore plus", "3.1.4+just_my-2_cents", "just.my.2.cents"),
+        (
+            "Regular version hyphen plus",
+            "3.1.4+just-my-2-cents",
+            "just.my.2.cents",
+        ),
+        (
+            "Regular version hyphen underscore plus",
+            "3.1.4+just_my-2_cents",
+            "just.my.2.cents",
+        ),
         ("Pre-fixed version single digit plus", "v3.1.4+2", "2"),
         ("Pre-fixed version double digit plus", "v3.1.4+12", "12"),
         ("Pre-fixed version alpha-numeric plus", "v3.1.4+af2b", "af2b"),
-        ("Pre-fixed version hyphen plus", "v3.1.4+just-my-2-cents", "just.my.2.cents"),
-        ("Pre-fixed version hyphen underscore plus", "v3.1.4+just_my-2_cents", "just.my.2.cents"),
+        (
+            "Pre-fixed version hyphen plus",
+            "v3.1.4+just-my-2-cents",
+            "just.my.2.cents",
+        ),
+        (
+            "Pre-fixed version hyphen underscore plus",
+            "v3.1.4+just_my-2_cents",
+            "just.my.2.cents",
+        ),
     ]
-    SUB_TESTS_VERSION_PARSE_SUCCESS: Final[List[Tuple[str, str]]] = [
+    SUB_TESTS_VERSION_PARSE_SUCCESS: Final[list[tuple[str, str]]] = [
         ("Regular version", "1.2.3"),
         ("Prefixed version", "v1.2.3"),
         ("Prefixed version with alpha", "v1.2.3a4"),
         ("Prefixed version with beta", "v1.2.3b4"),
         ("Prefixed version with rc", "v1.2.3rc4"),
         ("Prefixed version with rc as post", "v1.2.3a4post5"),
         ("Prefixed version with rc as post alternative", "v1.2.3a4-5"),
         ("Prefixed version with rc as post and dev", "v1.2.3a4-post5.dev17"),
-        ("Prefixed version with rc as post and dev and local", "v1.2.3a4-post5.dev17+erg.13"),
+        (
+            "Prefixed version with rc as post and dev and local",
+            "v1.2.3a4-post5.dev17+erg.13",
+        ),
     ]
-    SUB_TESTS_VERSION_PARSE_FAIL: Final[List[Tuple[str, str]]] = [
+    SUB_TESTS_VERSION_PARSE_FAIL: Final[list[tuple[str, str]]] = [
         ("Wrong prefix", "a0.1.0+2"),
         ("Negative epoch", "-2!v0.1.0+2"),
         ("Alpha epoch", "f!v0.1.0+2"),
         ("Wrong separators", "0-1-0"),
         ("Wrong alpha", "0.1.0alp1"),
         ("Wrong beta", "0.1.0bet2"),
         ("Wrong release candidate", "0.1.0relca3"),
@@ -242,15 +533,15 @@
         ("Negative minor", "1.-2.0"),
         ("Negative micro", "1.2.-3"),
     ]
 
     def test_default_version_is_one(self) -> None:
         v1: Version = Version.default()
         v2: Version = Version.from_string("1")
-        self.assertEquals(v1, v2)
+        self.assertEqual(v1, v2)
 
     def test_create_version_from_str_epoch_part(self) -> None:
         for message, version, epoch in self.SUB_TESTS_VERSION_FROM_STR_EPOCH:
             with self.subTest(message, version=version):
                 v: Version = Version.from_string(version)
                 self.assertEqual(v.epoch, epoch)
 
@@ -368,23 +659,23 @@
     def test_version_is_local_true(self) -> None:
         v = self._create_version(as_local=True)
         self._assure_pre_matches(v, False, False, False, False, False)
         self.assertTrue(v.is_local_version)
         self.assertFalse(v.is_post_release and v.is_local_version)
 
     def _create_version(
-            self,
-            *,
-            as_alpha: bool = False,
-            as_beta: bool = False,
-            as_rc: bool = False,
-            as_dev: bool = False,
-            as_post: bool = False,
-            as_local: bool = False
-            )-> Version:
+        self,
+        *,
+        as_alpha: bool = False,
+        as_beta: bool = False,
+        as_rc: bool = False,
+        as_dev: bool = False,
+        as_post: bool = False,
+        as_local: bool = False,
+    ) -> Version:
         epoch = 1
         release = (2, 3, 4)
         dev = None if not as_dev else ("dev", 5)
         post = None if not as_post else ("post", 6)
         local = None if not as_local else "as.local7"
 
         items = int(as_alpha) + int(as_beta) + int(as_rc)
@@ -396,21 +687,24 @@
         elif as_beta:
             pre = ("b", 9)
         elif as_rc:
             pre = ("rc", 10)
 
         return Version(epoch, release, pre, post, dev, local)
 
-    def _assure_pre_matches(self, version: Version, is_alpha, is_beta, is_rc, is_pre, is_dev) -> None:
+    def _assure_pre_matches(
+        self, version: Version, is_alpha, is_beta, is_rc, is_pre, is_dev
+    ) -> None:
         self.assertEqual(version.is_alpha, is_alpha)
         self.assertEqual(version.is_beta, is_beta)
         self.assertEqual(version.is_release_candidate, is_rc)
         self.assertEqual(version.is_pre_release, is_pre)
         self.assertEqual(version.is_development_version, is_dev)
 
+
 @final
 class VersionOrderingTest(unittest.TestCase):
     pass  # TODO implement
 
 
 @final
 class FormatVersionTest(unittest.TestCase):
```

### Comparing `pdm-bump-0.6.9/PKG-INFO` & `pdm-bump-0.7.0a1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 Metadata-Version: 2.1
 Name: pdm-bump
-Version: 0.6.9
+Version: 0.7.0a1
 Summary: A plugin for PDM providing the ability to modify the version according to PEP440
 License: MIT
 Author-email: Carsten Igel <cig@bite-that-bit.de>
 Requires-Python: >=3.9
 Project-URL: homepage, https://github.com/carstencodes/pdm-bump
 Description-Content-Type: text/markdown
 
 # pdm-bump
 
 ![PyPI](https://img.shields.io/pypi/v/pdm-bump?logo=python&logoColor=%23cccccc)
 [![pdm-managed](https://img.shields.io/badge/pdm-managed-blueviolet)](https://pdm.fming.dev)
 
-A small PEP440 compliant bump utility for the [Python development master](https://pdm.fming.dev/)
+A small PEP440 compliant bump utility for PDM, the [Python Development Master](https://pdm.fming.dev/).
 
-## Why ?
+## Why?
 
-As of PEP621, the pyproject.toml supports project metadata including a project version. If you are using the PDM build backend (according to PEP517), you can also use a file provider that contains your version, which is often referred to as `dynamic` versions.
+As of PEP621, the pyproject.toml supports project metadata including a project version. If you are using the PDM build backend (according to PEP517), you can also use a file provider that contains your version, which is often referred to as a `dynamic` version.
 
 The project version itself must comply to PEP440, which tells us, that it must consist of
 
 * an optional epoch
 * a mandatory major version part
 * a mandatory minor version part
 * a mandatory micro version part
 * an optional pre-release part supporting alpha, beta or release-candidate part.
 
-Tools like bumpversion or bump2version use their own configuration an their own configuration and might not consider the PEP440 specifications.
+Tools like `bumpversion` or `bump2version` use their own configuration and might not conform to the PEP440 specification.
 
 ## Installation
 
-You can install it using either pip (`pip install [--user] pdm-bump`) or using the pdm cli (`pdm plugin add [--pip-args=--user] pdm-bump`).
+You can install it using either pip (`pip install [--user] pdm-bump`) or using the PDM CLI (`pdm self add [--pip-args=--user] pdm-bump`).
 
 ## Usage
 
 You can use it the following way:
 
 ```shell
 $ grep version= pyproject.toml
@@ -52,24 +52,24 @@
 ## VCS based actions
 
 **NOTE**: Currently, only `git` is supported as VCS provider.
 
 You can create tags based on your `pyproject.toml` version (or dynamic version) using the following command.
 
 ```shell
-$ pdm bump tag # Creates a git tag with a leading v
+$ pdm bump tag # creates a git tag with a leading v
 ```
 
 ## Contributing
 
 Feel free to submit issues and pull requests. Contributions are welcome.
 
 ## Pre-checks
 
 1. Tests: To run the tests for your current checks, run `pdm run pytest`.
-2. Tox: If you are using `pyenv` you can use `pdm run tox` to run the tests for all supported python versions.
-3. Code-Style: You can use `pdm check-style` to check code format.
+2. tox: If you are using `pyenv` you can use `pdm run tox` to run the tests for all supported Python versions.
+3. Code Style: You can use `pdm check-style` to check code format.
 4. Format: You can use `pdm format` to format your code.
-5. Commit messages: You can run `pdm check-commits` to run `gitlint` across your commit messages.
+5. Commit messages: You can run `pdm check-commits` to run `gitlint` on your commit messages.
 
-Before opening a Pull Request, make sure, that the quality gates should succeed.
+Before opening a Pull Request make sure that the quality gates are passed.
```

