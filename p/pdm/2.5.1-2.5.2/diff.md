# Comparing `tmp/pdm-2.5.1.tar.gz` & `tmp/pdm-2.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-2.5.1.tar", last modified: Sun Apr  9 12:06:18 2023, max compression
+gzip compressed data, was "pdm-2.5.2.tar", last modified: Mon Apr 10 11:51:49 2023, max compression
```

## Comparing `pdm-2.5.1.tar` & `pdm-2.5.2.tar`

### file list

```diff
@@ -1,270 +1,270 @@
--rw-r--r--   0        0        0   115263 2023-04-09 12:06:04.912886 pdm-2.5.1/CHANGELOG.md
--rw-r--r--   0        0        0     1075 2023-04-09 12:06:04.912886 pdm-2.5.1/LICENSE
--rw-r--r--   0        0        0     1075 2023-04-09 12:06:04.912886 pdm-2.5.1/LICENSE
--rw-r--r--   0        0        0     8229 2023-04-09 12:06:04.912886 pdm-2.5.1/README.md
--rw-r--r--   0        0        0     8229 2023-04-09 12:06:04.912886 pdm-2.5.1/README.md
--rw-r--r--   0        0        0     4423 2023-04-09 12:06:18.708810 pdm-2.5.1/pyproject.toml
--rw-r--r--   0        0        0       65 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/__main__.py
--rw-r--r--   0        0        0      316 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/__version__.py
--rw-r--r--   0        0        0     2432 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/_types.py
--rw-r--r--   0        0        0      237 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/builders/__init__.py
--rw-r--r--   0        0        0    11738 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/builders/base.py
--rw-r--r--   0        0        0     1755 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/builders/editable.py
--rw-r--r--   0        0        0      656 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/builders/sdist.py
--rw-r--r--   0        0        0     1073 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/builders/wheel.py
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/__init__.py
--rw-r--r--   0        0        0    33643 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/actions.py
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/__init__.py
--rw-r--r--   0        0        0     2404 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/add.py
--rw-r--r--   0        0        0     2255 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/base.py
--rw-r--r--   0        0        0     2380 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/build.py
--rw-r--r--   0        0        0     6529 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/cache.py
--rw-r--r--   0        0        0     1324 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/completion.py
--rw-r--r--   0        0        0     6102 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/config.py
--rw-r--r--   0        0        0     2948 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/export.py
--rw-r--r--   0        0        0     3034 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/fix/__init__.py
--rw-r--r--   0        0        0     2309 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/fix/fixers.py
--rw-r--r--   0        0        0     1071 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/import_cmd.py
--rw-r--r--   0        0        0     2318 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/info.py
--rw-r--r--   0        0        0     5963 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/init.py
--rw-r--r--   0        0        0     2263 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/install.py
--rw-r--r--   0        0        0    15743 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/list.py
--rw-r--r--   0        0        0     1912 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/lock.py
--rw-r--r--   0        0        0     6161 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/publish/__init__.py
--rw-r--r--   0        0        0     7904 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/publish/package.py
--rw-r--r--   0        0        0     4644 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/publish/repository.py
--rw-r--r--   0        0        0     1672 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/remove.py
--rw-r--r--   0        0        0    14018 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/run.py
--rw-r--r--   0        0        0     2436 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/search.py
--rw-r--r--   0        0        0     9364 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/self_cmd.py
--rw-r--r--   0        0        0     2896 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/show.py
--rw-r--r--   0        0        0     1447 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/sync.py
--rw-r--r--   0        0        0     2392 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/update.py
--rw-r--r--   0        0        0     1318 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/use.py
--rw-r--r--   0        0        0     1848 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/venv/__init__.py
--rw-r--r--   0        0        0     2416 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/venv/activate.py
--rw-r--r--   0        0        0     6171 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/venv/backends.py
--rw-r--r--   0        0        0     2155 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/venv/create.py
--rw-r--r--   0        0        0      809 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/venv/list.py
--rw-r--r--   0        0        0     2195 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/venv/purge.py
--rw-r--r--   0        0        0     1276 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/venv/remove.py
--rw-r--r--   0        0        0     3027 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/commands/venv/utils.py
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/completions/__init__.py
--rw-r--r--   0        0        0     5025 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/completions/pdm.bash
--rw-r--r--   0        0        0    37111 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/completions/pdm.fish
--rw-r--r--   0        0        0    18492 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/completions/pdm.ps1
--rw-r--r--   0        0        0    24801 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/completions/pdm.zsh
--rw-r--r--   0        0        0     3553 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/filters.py
--rw-r--r--   0        0        0     1481 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/hooks.py
--rw-r--r--   0        0        0    10330 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/options.py
--rw-r--r--   0        0        0    24464 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/cli/utils.py
--rw-r--r--   0        0        0     2409 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/compat.py
--rw-r--r--   0        0        0     9245 2023-04-09 12:06:04.916886 pdm-2.5.1/src/pdm/core.py
--rw-r--r--   0        0        0      904 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/environments/__init__.py
--rw-r--r--   0        0        0     8889 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/environments/base.py
--rw-r--r--   0        0        0     3560 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/environments/local.py
--rw-r--r--   0        0        0      808 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/environments/prefix.py
--rw-r--r--   0        0        0     1614 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/environments/python.py
--rw-r--r--   0        0        0     1377 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/exceptions.py
--rw-r--r--   0        0        0     1086 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/formats/__init__.py
--rw-r--r--   0        0        0     3215 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/formats/base.py
--rw-r--r--   0        0        0     5741 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/formats/flit.py
--rw-r--r--   0        0        0     2349 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/formats/pipfile.py
--rw-r--r--   0        0        0     7289 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/formats/poetry.py
--rw-r--r--   0        0        0     7131 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/formats/requirements.py
--rw-r--r--   0        0        0     2271 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/formats/setup_py.py
--rw-r--r--   0        0        0      119 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/installers/__init__.py
--rw-r--r--   0        0        0     1853 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/installers/core.py
--rw-r--r--   0        0        0    10908 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/installers/installers.py
--rw-r--r--   0        0        0     2091 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/installers/manager.py
--rw-r--r--   0        0        0     2226 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/installers/packages.py
--rw-r--r--   0        0        0    17107 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/installers/synchronizers.py
--rw-r--r--   0        0        0    10903 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/installers/uninstallers.py
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/__init__.py
--rw-r--r--   0        0        0     2111 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/auth.py
--rw-r--r--   0        0        0     4394 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/backends.py
--rw-r--r--   0        0        0     9886 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/caches.py
--rw-r--r--   0        0        0    24220 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/candidates.py
--rw-r--r--   0        0        0      287 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/environment.py
--rw-r--r--   0        0        0     1714 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/in_process/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/in_process/get_abi_tag.py
--rw-r--r--   0        0        0     6182 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/in_process/parse_setup.py
--rw-r--r--   0        0        0     1165 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/in_process/pep508.py
--rw-r--r--   0        0        0     1653 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/in_process/sysconfig_get_paths.py
--rw-r--r--   0        0        0     5701 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/markers.py
--rw-r--r--   0        0        0     3507 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/project_info.py
--rw-r--r--   0        0        0     2120 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/python.py
--rw-r--r--   0        0        0      318 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/python_max_versions.json
--rw-r--r--   0        0        0    20760 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/repositories.py
--rw-r--r--   0        0        0    17969 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/requirements.py
--rw-r--r--   0        0        0     2313 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/search.py
--rw-r--r--   0        0        0     1344 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/session.py
--rw-r--r--   0        0        0    14482 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/setup.py
--rw-r--r--   0        0        0    16337 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/specifiers.py
--rw-r--r--   0        0        0     5899 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/versions.py
--rw-r--r--   0        0        0     2721 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/models/working_set.py
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/pep582/__init__.py
--rw-r--r--   0        0        0     4481 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/pep582/sitecustomize.py
--rw-r--r--   0        0        0      134 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/project/__init__.py
--rw-r--r--   0        0        0    16212 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/project/config.py
--rw-r--r--   0        0        0    26927 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/project/core.py
--rw-r--r--   0        0        0     1320 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/project/lockfile.py
--rw-r--r--   0        0        0     3046 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/project/project_file.py
--rw-r--r--   0        0        0     1009 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/project/toml_file.py
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/py.typed
--rw-r--r--   0        0        0    19636 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/pytest.py
--rw-r--r--   0        0        0       61 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/resolver/__init__.py
--rw-r--r--   0        0        0     1954 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/resolver/core.py
--rw-r--r--   0        0        0    12796 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/resolver/providers.py
--rw-r--r--   0        0        0     1580 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/resolver/python.py
--rw-r--r--   0        0        0     3742 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/resolver/reporters.py
--rw-r--r--   0        0        0     4027 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/signals.py
--rw-r--r--   0        0        0     7966 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/termui.py
--rw-r--r--   0        0        0    13510 2023-04-09 12:06:04.920886 pdm-2.5.1/src/pdm/utils.py
--rw-r--r--   0        0        0       72 2023-04-09 12:06:04.920886 pdm-2.5.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.920886 pdm-2.5.1/tests/cli/__init__.py
--rw-r--r--   0        0        0     2631 2023-04-09 12:06:04.920886 pdm-2.5.1/tests/cli/conftest.py
--rw-r--r--   0        0        0    12370 2023-04-09 12:06:04.920886 pdm-2.5.1/tests/cli/test_add.py
--rw-r--r--   0        0        0     5811 2023-04-09 12:06:04.920886 pdm-2.5.1/tests/cli/test_build.py
--rw-r--r--   0        0        0     5277 2023-04-09 12:06:04.920886 pdm-2.5.1/tests/cli/test_cache.py
--rw-r--r--   0        0        0     7603 2023-04-09 12:06:04.920886 pdm-2.5.1/tests/cli/test_config.py
--rw-r--r--   0        0        0     1131 2023-04-09 12:06:04.920886 pdm-2.5.1/tests/cli/test_fix.py
--rw-r--r--   0        0        0    10432 2023-04-09 12:06:04.920886 pdm-2.5.1/tests/cli/test_hooks.py
--rw-r--r--   0        0        0     4505 2023-04-09 12:06:04.920886 pdm-2.5.1/tests/cli/test_init.py
--rw-r--r--   0        0        0    11265 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/cli/test_install.py
--rw-r--r--   0        0        0    28998 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/cli/test_list.py
--rw-r--r--   0        0        0     4675 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/cli/test_lock.py
--rw-r--r--   0        0        0     7188 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/cli/test_others.py
--rw-r--r--   0        0        0     5740 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/cli/test_publish.py
--rw-r--r--   0        0        0     3872 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/cli/test_remove.py
--rw-r--r--   0        0        0    26440 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/cli/test_run.py
--rw-r--r--   0        0        0     3641 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/cli/test_self_command.py
--rw-r--r--   0        0        0     8806 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/cli/test_update.py
--rw-r--r--   0        0        0     2960 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/cli/test_use.py
--rw-r--r--   0        0        0    10565 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/cli/test_venv.py
--rw-r--r--   0        0        0     3172 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/conftest.py
--rw-r--r--   0        0        0      235 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/fixtures/Pipfile
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0    49497 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
--rw-r--r--   0        0        0      546 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
--rw-r--r--   0        0        0   422824 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1254 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
--rw-r--r--   0        0        0     1254 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     1038 2023-04-09 12:06:04.924886 pdm-2.5.1/tests/fixtures/artifacts/demo-0.0.1.tar.gz
--rw-r--r--   0        0        0     2615 2023-04-09 12:06:04.928887 pdm-2.5.1/tests/fixtures/artifacts/demo-0.0.1.zip
--rw-r--r--   0        0        0     4595 2023-04-09 12:06:04.928887 pdm-2.5.1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
--rw-r--r--   0        0        0     5359 2023-04-09 12:06:04.928887 pdm-2.5.1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
--rw-r--r--   0        0        0    56715 2023-04-09 12:06:04.928887 pdm-2.5.1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
--rw-r--r--   0        0        0     6138 2023-04-09 12:06:04.928887 pdm-2.5.1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5786 2023-04-09 12:06:04.928887 pdm-2.5.1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
--rw-r--r--   0        0        0    17978 2023-04-09 12:06:04.928887 pdm-2.5.1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
--rw-r--r--   0        0        0    24489 2023-04-09 12:06:04.928887 pdm-2.5.1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0   156727 2023-04-09 12:06:04.928887 pdm-2.5.1/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
--rw-r--r--   0        0        0   305481 2023-04-09 12:06:04.928887 pdm-2.5.1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
--rw-r--r--   0        0        0   531270 2023-04-09 12:06:04.932886 pdm-2.5.1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
--rw-r--r--   0        0        0  1232518 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
--rw-r--r--   0        0        0    26662 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
--rw-r--r--   0        0        0    35301 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
--rw-r--r--   0        0        0     5312 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
--rw-r--r--   0        0        0      326 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/index/demo.html
--rw-r--r--   0        0        0      511 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/index/future-fstrings.html
--rw-r--r--   0        0        0      262 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/index/pep345-legacy.html
--rw-r--r--   0        0        0      262 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/index/wheel.html
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/__init__.py
--rw-r--r--   0        0        0       42 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-#-with-hash/demo.py
--rw-r--r--   0        0        0      332 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-#-with-hash/setup.py
--rw-r--r--   0        0        0       26 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-combined-extras/demo.py
--rw-r--r--   0        0        0      462 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-combined-extras/pyproject.toml
--rw-r--r--   0        0        0       42 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-failure-no-dep/demo.py
--rw-r--r--   0        0        0      246 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-failure-no-dep/setup.py
--rw-r--r--   0        0        0       42 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-failure/demo.py
--rw-r--r--   0        0        0      345 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-failure/setup.py
--rw-r--r--   0        0        0       12 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-module/LICENSE
--rw-r--r--   0        0        0       24 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-module/README.md
--rw-r--r--   0        0        0       14 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-module/bar_module.py
--rw-r--r--   0        0        0       36 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-module/foo_module.py
--rw-r--r--   0        0        0      442 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-module/pyproject.toml
--rw-r--r--   0        0        0     3983 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
--rw-r--r--   0        0        0      318 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
--rw-r--r--   0        0        0      157 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
--rw-r--r--   0        0        0       12 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package/LICENSE
--rw-r--r--   0        0        0       24 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package/README.md
--rw-r--r--   0        0        0       16 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package/data_out.json
--rw-r--r--   0        0        0       22 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package/my_package/data.json
--rw-r--r--   0        0        0    29800 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package/pdm.lock
--rw-r--r--   0        0        0      574 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package/pyproject.toml
--rw-r--r--   0        0        0      122 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package/requirements.ini
--rw-r--r--   0        0        0     7521 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package/requirements.txt
--rw-r--r--   0        0        0      211 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package/requirements_simple.txt
--rw-r--r--   0        0        0      728 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package/setup.txt
--rw-r--r--   0        0        0       21 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-package/single_module.py
--rw-r--r--   0        0        0       18 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-parent-package/README.md
--rw-r--r--   0        0        0       22 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-parent-package/package-a/foo.py
--rw-r--r--   0        0        0      120 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-parent-package/package-a/setup.py
--rw-r--r--   0        0        0       22 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-parent-package/package-b/bar.py
--rw-r--r--   0        0        0      197 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
--rw-r--r--   0        0        0       42 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-prerelease/demo.py
--rw-r--r--   0        0        0      334 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-prerelease/setup.py
--rw-r--r--   0        0        0       12 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-src-package/LICENSE
--rw-r--r--   0        0        0       24 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-src-package/README.md
--rw-r--r--   0        0        0       16 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-src-package/data_out.json
--rw-r--r--   0        0        0      456 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-src-package/pyproject.toml
--rw-r--r--   0        0        0       21 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-src-package/single_module.py
--rw-r--r--   0        0        0       22 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
--rw-r--r--   0        0        0       24 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo-src-package/src/my_package/data.json
--rw-r--r--   0        0        0       42 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo/demo.py
--rw-r--r--   0        0        0      332 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo/setup.py
--rw-r--r--   0        0        0       26 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo_extras/demo.py
--rw-r--r--   0        0        0      250 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/demo_extras/setup.py
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/flit-demo/README.rst
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/flit-demo/doc/index.html
--rw-r--r--   0        0        0       49 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/flit-demo/flit.py
--rw-r--r--   0        0        0      969 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/flit-demo/pyproject.toml
--rw-r--r--   0        0        0       12 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/poetry-demo/mylib.py
--rw-r--r--   0        0        0      863 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/poetry-demo/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-hatch-static/README.md
--rw-r--r--   0        0        0      386 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-hatch-static/pyproject.toml
--rw-r--r--   0        0        0       11 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-monorepo/README.md
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-monorepo/core/core.py
--rw-r--r--   0        0        0      179 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-monorepo/core/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-monorepo/package_a/alice.py
--rw-r--r--   0        0        0      231 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-monorepo/package_b/bob.py
--rw-r--r--   0        0        0      231 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
--rw-r--r--   0        0        0      237 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-monorepo/pyproject.toml
--rw-r--r--   0        0        0      380 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-plugin-pdm/hello.py
--rw-r--r--   0        0        0      312 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
--rw-r--r--   0        0        0      380 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-plugin/hello.py
--rw-r--r--   0        0        0      168 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-plugin/setup.py
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-removal/__init__.py
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-removal/bar.py
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-removal/foo.py
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-removal/subdir/__init__.py
--rw-r--r--   0        0        0       10 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-setuptools/AUTHORS
--rw-r--r--   0        0        0       12 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-setuptools/README.md
--rw-r--r--   0        0        0       22 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-setuptools/mymodule.py
--rw-r--r--   0        0        0      398 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-setuptools/setup.cfg
--rw-r--r--   0        0        0      308 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/projects/test-setuptools/setup.py
--rw-r--r--   0        0        0     1525 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/pypi.json
--rw-r--r--   0        0        0     1329 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/pyproject.toml
--rw-r--r--   0        0        0       20 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/requirements-include.txt
--rw-r--r--   0        0        0      502 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/fixtures/requirements.txt
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/models/__init__.py
--rw-r--r--   0        0        0     3820 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/models/test_backends.py
--rw-r--r--   0        0        0    12991 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/models/test_candidates.py
--rw-r--r--   0        0        0     1971 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/models/test_marker.py
--rw-r--r--   0        0        0     2679 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/models/test_requirements.py
--rw-r--r--   0        0        0     2526 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/models/test_setup_parsing.py
--rw-r--r--   0        0        0     3418 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/models/test_specifiers.py
--rw-r--r--   0        0        0     2703 2023-04-09 12:06:04.940886 pdm-2.5.1/tests/models/test_versions.py
--rw-r--r--   0        0        0        0 2023-04-09 12:06:04.944886 pdm-2.5.1/tests/resolver/__init__.py
--rw-r--r--   0        0        0    11567 2023-04-09 12:06:04.944886 pdm-2.5.1/tests/resolver/test_resolve.py
--rw-r--r--   0        0        0     7187 2023-04-09 12:06:04.944886 pdm-2.5.1/tests/test_formats.py
--rw-r--r--   0        0        0     7240 2023-04-09 12:06:04.944886 pdm-2.5.1/tests/test_installer.py
--rw-r--r--   0        0        0     1862 2023-04-09 12:06:04.944886 pdm-2.5.1/tests/test_integration.py
--rw-r--r--   0        0        0     2859 2023-04-09 12:06:04.944886 pdm-2.5.1/tests/test_plugin.py
--rw-r--r--   0        0        0    11182 2023-04-09 12:06:04.944886 pdm-2.5.1/tests/test_project.py
--rw-r--r--   0        0        0     1109 2023-04-09 12:06:04.944886 pdm-2.5.1/tests/test_signals.py
--rw-r--r--   0        0        0     4364 2023-04-09 12:06:04.944886 pdm-2.5.1/tests/test_utils.py
--rw-r--r--   0        0        0     9912 1970-01-01 00:00:00.000000 pdm-2.5.1/PKG-INFO
+-rw-r--r--   0        0        0   115658 2023-04-10 11:51:36.625334 pdm-2.5.2/CHANGELOG.md
+-rw-r--r--   0        0        0     1075 2023-04-10 11:51:36.625334 pdm-2.5.2/LICENSE
+-rw-r--r--   0        0        0     1075 2023-04-10 11:51:36.625334 pdm-2.5.2/LICENSE
+-rw-r--r--   0        0        0     8229 2023-04-10 11:51:36.625334 pdm-2.5.2/README.md
+-rw-r--r--   0        0        0     8229 2023-04-10 11:51:36.625334 pdm-2.5.2/README.md
+-rw-r--r--   0        0        0     4423 2023-04-10 11:51:49.381577 pdm-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0       65 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/__main__.py
+-rw-r--r--   0        0        0      316 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/__version__.py
+-rw-r--r--   0        0        0     2432 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/_types.py
+-rw-r--r--   0        0        0      237 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/builders/__init__.py
+-rw-r--r--   0        0        0    11738 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/builders/base.py
+-rw-r--r--   0        0        0     1755 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/builders/editable.py
+-rw-r--r--   0        0        0      656 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/builders/sdist.py
+-rw-r--r--   0        0        0     1073 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/builders/wheel.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/__init__.py
+-rw-r--r--   0        0        0    33643 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/actions.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/__init__.py
+-rw-r--r--   0        0        0     2404 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/add.py
+-rw-r--r--   0        0        0     2255 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/base.py
+-rw-r--r--   0        0        0     2380 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/build.py
+-rw-r--r--   0        0        0     6529 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/cache.py
+-rw-r--r--   0        0        0     1324 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/completion.py
+-rw-r--r--   0        0        0     6102 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/config.py
+-rw-r--r--   0        0        0     2948 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/export.py
+-rw-r--r--   0        0        0     3034 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/fix/__init__.py
+-rw-r--r--   0        0        0     2309 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/fix/fixers.py
+-rw-r--r--   0        0        0     1071 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/import_cmd.py
+-rw-r--r--   0        0        0     2318 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/info.py
+-rw-r--r--   0        0        0     5979 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/init.py
+-rw-r--r--   0        0        0     2263 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/install.py
+-rw-r--r--   0        0        0    15743 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/list.py
+-rw-r--r--   0        0        0     1912 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/lock.py
+-rw-r--r--   0        0        0     6161 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/publish/__init__.py
+-rw-r--r--   0        0        0     7904 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/publish/package.py
+-rw-r--r--   0        0        0     4644 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/publish/repository.py
+-rw-r--r--   0        0        0     1672 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/remove.py
+-rw-r--r--   0        0        0    14018 2023-04-10 11:51:36.629335 pdm-2.5.2/src/pdm/cli/commands/run.py
+-rw-r--r--   0        0        0     2436 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/commands/search.py
+-rw-r--r--   0        0        0     9364 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/commands/self_cmd.py
+-rw-r--r--   0        0        0     2896 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/commands/show.py
+-rw-r--r--   0        0        0     1447 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/commands/sync.py
+-rw-r--r--   0        0        0     2392 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/commands/update.py
+-rw-r--r--   0        0        0     1318 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/commands/use.py
+-rw-r--r--   0        0        0     1848 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/commands/venv/__init__.py
+-rw-r--r--   0        0        0     2416 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/commands/venv/activate.py
+-rw-r--r--   0        0        0     6171 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/commands/venv/backends.py
+-rw-r--r--   0        0        0     2155 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/commands/venv/create.py
+-rw-r--r--   0        0        0      809 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/commands/venv/list.py
+-rw-r--r--   0        0        0     2195 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/commands/venv/purge.py
+-rw-r--r--   0        0        0     1276 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/commands/venv/remove.py
+-rw-r--r--   0        0        0     3027 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/commands/venv/utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/completions/__init__.py
+-rw-r--r--   0        0        0     5025 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/completions/pdm.bash
+-rw-r--r--   0        0        0    37102 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/completions/pdm.fish
+-rw-r--r--   0        0        0    18492 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/completions/pdm.ps1
+-rw-r--r--   0        0        0    24792 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/completions/pdm.zsh
+-rw-r--r--   0        0        0     3553 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/filters.py
+-rw-r--r--   0        0        0     1481 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/hooks.py
+-rw-r--r--   0        0        0    10328 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/options.py
+-rw-r--r--   0        0        0    24464 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/cli/utils.py
+-rw-r--r--   0        0        0     2409 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/compat.py
+-rw-r--r--   0        0        0     9245 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/core.py
+-rw-r--r--   0        0        0      904 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/environments/__init__.py
+-rw-r--r--   0        0        0     8889 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/environments/base.py
+-rw-r--r--   0        0        0     3560 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/environments/local.py
+-rw-r--r--   0        0        0      808 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/environments/prefix.py
+-rw-r--r--   0        0        0     1614 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/environments/python.py
+-rw-r--r--   0        0        0     1377 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/exceptions.py
+-rw-r--r--   0        0        0     1086 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/formats/__init__.py
+-rw-r--r--   0        0        0     3215 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/formats/base.py
+-rw-r--r--   0        0        0     5741 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/formats/flit.py
+-rw-r--r--   0        0        0     2349 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/formats/pipfile.py
+-rw-r--r--   0        0        0     7289 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/formats/poetry.py
+-rw-r--r--   0        0        0     7131 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/formats/requirements.py
+-rw-r--r--   0        0        0     2271 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/formats/setup_py.py
+-rw-r--r--   0        0        0      119 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/installers/__init__.py
+-rw-r--r--   0        0        0     1853 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/installers/core.py
+-rw-r--r--   0        0        0    10908 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/installers/installers.py
+-rw-r--r--   0        0        0     2091 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/installers/manager.py
+-rw-r--r--   0        0        0     2226 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/installers/packages.py
+-rw-r--r--   0        0        0    17107 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/installers/synchronizers.py
+-rw-r--r--   0        0        0    10903 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/installers/uninstallers.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/__init__.py
+-rw-r--r--   0        0        0     2111 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/auth.py
+-rw-r--r--   0        0        0     4394 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/backends.py
+-rw-r--r--   0        0        0     9886 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/caches.py
+-rw-r--r--   0        0        0    24220 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/candidates.py
+-rw-r--r--   0        0        0      287 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/environment.py
+-rw-r--r--   0        0        0     1714 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/in_process/__init__.py
+-rw-r--r--   0        0        0     2049 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/in_process/get_abi_tag.py
+-rw-r--r--   0        0        0     6182 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/in_process/parse_setup.py
+-rw-r--r--   0        0        0     1165 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/in_process/pep508.py
+-rw-r--r--   0        0        0     1653 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/in_process/sysconfig_get_paths.py
+-rw-r--r--   0        0        0     5701 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/markers.py
+-rw-r--r--   0        0        0     3507 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/project_info.py
+-rw-r--r--   0        0        0     2120 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/python.py
+-rw-r--r--   0        0        0      318 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/python_max_versions.json
+-rw-r--r--   0        0        0    20760 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/repositories.py
+-rw-r--r--   0        0        0    17969 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/requirements.py
+-rw-r--r--   0        0        0     2313 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/search.py
+-rw-r--r--   0        0        0     1344 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/session.py
+-rw-r--r--   0        0        0    14482 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/setup.py
+-rw-r--r--   0        0        0    16337 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/specifiers.py
+-rw-r--r--   0        0        0     5899 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/versions.py
+-rw-r--r--   0        0        0     2721 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/models/working_set.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/pep582/__init__.py
+-rw-r--r--   0        0        0     4481 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/pep582/sitecustomize.py
+-rw-r--r--   0        0        0      134 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/project/__init__.py
+-rw-r--r--   0        0        0    16212 2023-04-10 11:51:36.633334 pdm-2.5.2/src/pdm/project/config.py
+-rw-r--r--   0        0        0    26927 2023-04-10 11:51:36.637334 pdm-2.5.2/src/pdm/project/core.py
+-rw-r--r--   0        0        0     1320 2023-04-10 11:51:36.637334 pdm-2.5.2/src/pdm/project/lockfile.py
+-rw-r--r--   0        0        0     3046 2023-04-10 11:51:36.637334 pdm-2.5.2/src/pdm/project/project_file.py
+-rw-r--r--   0        0        0     1009 2023-04-10 11:51:36.637334 pdm-2.5.2/src/pdm/project/toml_file.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.637334 pdm-2.5.2/src/pdm/py.typed
+-rw-r--r--   0        0        0    19636 2023-04-10 11:51:36.637334 pdm-2.5.2/src/pdm/pytest.py
+-rw-r--r--   0        0        0       61 2023-04-10 11:51:36.637334 pdm-2.5.2/src/pdm/resolver/__init__.py
+-rw-r--r--   0        0        0     1954 2023-04-10 11:51:36.637334 pdm-2.5.2/src/pdm/resolver/core.py
+-rw-r--r--   0        0        0    12796 2023-04-10 11:51:36.637334 pdm-2.5.2/src/pdm/resolver/providers.py
+-rw-r--r--   0        0        0     1580 2023-04-10 11:51:36.637334 pdm-2.5.2/src/pdm/resolver/python.py
+-rw-r--r--   0        0        0     3742 2023-04-10 11:51:36.637334 pdm-2.5.2/src/pdm/resolver/reporters.py
+-rw-r--r--   0        0        0     4027 2023-04-10 11:51:36.637334 pdm-2.5.2/src/pdm/signals.py
+-rw-r--r--   0        0        0     7966 2023-04-10 11:51:36.637334 pdm-2.5.2/src/pdm/termui.py
+-rw-r--r--   0        0        0    13510 2023-04-10 11:51:36.637334 pdm-2.5.2/src/pdm/utils.py
+-rw-r--r--   0        0        0       72 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/__init__.py
+-rw-r--r--   0        0        0     2631 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/conftest.py
+-rw-r--r--   0        0        0    12370 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_add.py
+-rw-r--r--   0        0        0     5811 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_build.py
+-rw-r--r--   0        0        0     5277 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_cache.py
+-rw-r--r--   0        0        0     7603 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_config.py
+-rw-r--r--   0        0        0     1131 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_fix.py
+-rw-r--r--   0        0        0    10432 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_hooks.py
+-rw-r--r--   0        0        0     4505 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_init.py
+-rw-r--r--   0        0        0    11265 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_install.py
+-rw-r--r--   0        0        0    28998 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_list.py
+-rw-r--r--   0        0        0     4675 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_lock.py
+-rw-r--r--   0        0        0     7187 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_others.py
+-rw-r--r--   0        0        0     5740 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_publish.py
+-rw-r--r--   0        0        0     3872 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_remove.py
+-rw-r--r--   0        0        0    26440 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_run.py
+-rw-r--r--   0        0        0     3641 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_self_command.py
+-rw-r--r--   0        0        0     8806 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_update.py
+-rw-r--r--   0        0        0     2960 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_use.py
+-rw-r--r--   0        0        0    10565 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/cli/test_venv.py
+-rw-r--r--   0        0        0     3172 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/conftest.py
+-rw-r--r--   0        0        0      235 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/fixtures/Pipfile
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0    49497 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl
+-rw-r--r--   0        0        0      546 2023-04-10 11:51:36.637334 pdm-2.5.2/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz
+-rw-r--r--   0        0        0   422824 2023-04-10 11:51:36.641335 pdm-2.5.2/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1254 2023-04-10 11:51:36.641335 pdm-2.5.2/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl
+-rw-r--r--   0        0        0     1254 2023-04-10 11:51:36.641335 pdm-2.5.2/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     1038 2023-04-10 11:51:36.641335 pdm-2.5.2/tests/fixtures/artifacts/demo-0.0.1.tar.gz
+-rw-r--r--   0        0        0     2615 2023-04-10 11:51:36.641335 pdm-2.5.2/tests/fixtures/artifacts/demo-0.0.1.zip
+-rw-r--r--   0        0        0     4595 2023-04-10 11:51:36.641335 pdm-2.5.2/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl
+-rw-r--r--   0        0        0     5359 2023-04-10 11:51:36.641335 pdm-2.5.2/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl
+-rw-r--r--   0        0        0    56715 2023-04-10 11:51:36.641335 pdm-2.5.2/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl
+-rw-r--r--   0        0        0     6138 2023-04-10 11:51:36.641335 pdm-2.5.2/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5786 2023-04-10 11:51:36.641335 pdm-2.5.2/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz
+-rw-r--r--   0        0        0    17978 2023-04-10 11:51:36.641335 pdm-2.5.2/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl
+-rw-r--r--   0        0        0    24489 2023-04-10 11:51:36.641335 pdm-2.5.2/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   156727 2023-04-10 11:51:36.641335 pdm-2.5.2/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl
+-rw-r--r--   0        0        0   305481 2023-04-10 11:51:36.641335 pdm-2.5.2/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl
+-rw-r--r--   0        0        0   531270 2023-04-10 11:51:36.645335 pdm-2.5.2/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl
+-rw-r--r--   0        0        0  1232518 2023-04-10 11:51:36.649335 pdm-2.5.2/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl
+-rw-r--r--   0        0        0    26662 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl
+-rw-r--r--   0        0        0    35301 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl
+-rw-r--r--   0        0        0     5312 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl
+-rw-r--r--   0        0        0      326 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/index/demo.html
+-rw-r--r--   0        0        0      511 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/index/future-fstrings.html
+-rw-r--r--   0        0        0      262 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/index/pep345-legacy.html
+-rw-r--r--   0        0        0      262 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/index/wheel.html
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/__init__.py
+-rw-r--r--   0        0        0       42 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-#-with-hash/demo.py
+-rw-r--r--   0        0        0      332 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-#-with-hash/setup.py
+-rw-r--r--   0        0        0       26 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-combined-extras/demo.py
+-rw-r--r--   0        0        0      462 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-combined-extras/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-failure-no-dep/demo.py
+-rw-r--r--   0        0        0      246 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-failure-no-dep/setup.py
+-rw-r--r--   0        0        0       42 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-failure/demo.py
+-rw-r--r--   0        0        0      345 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-failure/setup.py
+-rw-r--r--   0        0        0       12 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-module/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-module/README.md
+-rw-r--r--   0        0        0       14 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-module/bar_module.py
+-rw-r--r--   0        0        0       36 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-module/foo_module.py
+-rw-r--r--   0        0        0      442 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-module/pyproject.toml
+-rw-r--r--   0        0        0     3983 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock
+-rw-r--r--   0        0        0      318 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package-has-dep-with-extras/pyproject.toml
+-rw-r--r--   0        0        0      157 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package-has-dep-with-extras/requirements.txt
+-rw-r--r--   0        0        0       12 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package/README.md
+-rw-r--r--   0        0        0       16 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package/data_out.json
+-rw-r--r--   0        0        0       22 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package/my_package/data.json
+-rw-r--r--   0        0        0    29800 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package/pdm.lock
+-rw-r--r--   0        0        0      574 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package/pyproject.toml
+-rw-r--r--   0        0        0      122 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package/requirements.ini
+-rw-r--r--   0        0        0     7521 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package/requirements.txt
+-rw-r--r--   0        0        0      211 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package/requirements_simple.txt
+-rw-r--r--   0        0        0      728 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package/setup.txt
+-rw-r--r--   0        0        0       21 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-package/single_module.py
+-rw-r--r--   0        0        0       18 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-parent-package/README.md
+-rw-r--r--   0        0        0       22 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-parent-package/package-a/foo.py
+-rw-r--r--   0        0        0      120 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-parent-package/package-a/setup.py
+-rw-r--r--   0        0        0       22 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-parent-package/package-b/bar.py
+-rw-r--r--   0        0        0      197 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-parent-package/package-b/pyproject.toml
+-rw-r--r--   0        0        0       42 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-prerelease/demo.py
+-rw-r--r--   0        0        0      334 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-prerelease/setup.py
+-rw-r--r--   0        0        0       12 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-src-package/LICENSE
+-rw-r--r--   0        0        0       24 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-src-package/README.md
+-rw-r--r--   0        0        0       16 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-src-package/data_out.json
+-rw-r--r--   0        0        0      456 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-src-package/pyproject.toml
+-rw-r--r--   0        0        0       21 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-src-package/single_module.py
+-rw-r--r--   0        0        0       22 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-src-package/src/my_package/__init__.py
+-rw-r--r--   0        0        0       24 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo-src-package/src/my_package/data.json
+-rw-r--r--   0        0        0       42 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo/demo.py
+-rw-r--r--   0        0        0      332 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo/setup.py
+-rw-r--r--   0        0        0       26 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo_extras/demo.py
+-rw-r--r--   0        0        0      250 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/demo_extras/setup.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/flit-demo/README.rst
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/flit-demo/doc/index.html
+-rw-r--r--   0        0        0       49 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/flit-demo/flit.py
+-rw-r--r--   0        0        0      969 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/flit-demo/pyproject.toml
+-rw-r--r--   0        0        0       12 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/poetry-demo/mylib.py
+-rw-r--r--   0        0        0      863 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/poetry-demo/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-hatch-static/README.md
+-rw-r--r--   0        0        0      386 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-hatch-static/pyproject.toml
+-rw-r--r--   0        0        0       11 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-monorepo/README.md
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-monorepo/core/core.py
+-rw-r--r--   0        0        0      179 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-monorepo/core/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-monorepo/package_a/alice.py
+-rw-r--r--   0        0        0      231 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-monorepo/package_a/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-monorepo/package_b/bob.py
+-rw-r--r--   0        0        0      231 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-monorepo/package_b/pyproject.toml
+-rw-r--r--   0        0        0      237 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-monorepo/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-plugin-pdm/hello.py
+-rw-r--r--   0        0        0      312 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-plugin-pdm/pyproject.toml
+-rw-r--r--   0        0        0      380 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-plugin/hello.py
+-rw-r--r--   0        0        0      168 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-plugin/setup.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-removal/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-removal/bar.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-removal/foo.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-removal/subdir/__init__.py
+-rw-r--r--   0        0        0       10 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-setuptools/AUTHORS
+-rw-r--r--   0        0        0       12 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-setuptools/README.md
+-rw-r--r--   0        0        0       22 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-setuptools/mymodule.py
+-rw-r--r--   0        0        0      398 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-setuptools/setup.cfg
+-rw-r--r--   0        0        0      308 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/projects/test-setuptools/setup.py
+-rw-r--r--   0        0        0     1525 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/pypi.json
+-rw-r--r--   0        0        0     1329 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/pyproject.toml
+-rw-r--r--   0        0        0       20 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/requirements-include.txt
+-rw-r--r--   0        0        0      502 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/fixtures/requirements.txt
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/models/__init__.py
+-rw-r--r--   0        0        0     3820 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/models/test_backends.py
+-rw-r--r--   0        0        0    12991 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/models/test_candidates.py
+-rw-r--r--   0        0        0     1971 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/models/test_marker.py
+-rw-r--r--   0        0        0     2679 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/models/test_requirements.py
+-rw-r--r--   0        0        0     2526 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/models/test_setup_parsing.py
+-rw-r--r--   0        0        0     3418 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/models/test_specifiers.py
+-rw-r--r--   0        0        0     2703 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/models/test_versions.py
+-rw-r--r--   0        0        0        0 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/resolver/__init__.py
+-rw-r--r--   0        0        0    11567 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/resolver/test_resolve.py
+-rw-r--r--   0        0        0     7187 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/test_formats.py
+-rw-r--r--   0        0        0     7240 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/test_installer.py
+-rw-r--r--   0        0        0     1862 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/test_integration.py
+-rw-r--r--   0        0        0     2859 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/test_plugin.py
+-rw-r--r--   0        0        0    11182 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/test_project.py
+-rw-r--r--   0        0        0     1109 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/test_signals.py
+-rw-r--r--   0        0        0     4364 2023-04-10 11:51:36.653334 pdm-2.5.2/tests/test_utils.py
+-rw-r--r--   0        0        0     9912 1970-01-01 00:00:00.000000 pdm-2.5.2/PKG-INFO
```

### Comparing `pdm-2.5.1/CHANGELOG.md` & `pdm-2.5.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,16 @@
+Release v2.5.2 (2023-04-10)
+---------------------------
+
+### Bug Fixes
+
+- Regression(#1710): Don't crash when trying to update the shebang in a binary script [#1827](https://github.com/pdm-project/pdm/issues/1827)
+- Rename the env var `PDM_USE_VENV` as `PDM_IN_VENV` for `--venv` flag as it mistakenly override another existing env var. [#1829](https://github.com/pdm-project/pdm/issues/1829)
+
+
 Release v2.5.1 (2023-04-09)
 ---------------------------
 
 ### Bug Fixes
 
 - Fix a bug that `pdm --pep582` raises an argument error. [#1823](https://github.com/pdm-project/pdm/issues/1823)
```

### Comparing `pdm-2.5.1/LICENSE` & `pdm-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/README.md` & `pdm-2.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/pyproject.toml` & `pdm-2.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
-version = "2.5.1"
+version = "2.5.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://pdm.fming.dev"
 Repository = "https://github.com/pdm-project/pdm"
```

### Comparing `pdm-2.5.1/src/pdm/_types.py` & `pdm-2.5.2/src/pdm/_types.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/builders/base.py` & `pdm-2.5.2/src/pdm/builders/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/builders/editable.py` & `pdm-2.5.2/src/pdm/builders/editable.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/builders/sdist.py` & `pdm-2.5.2/src/pdm/builders/sdist.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/builders/wheel.py` & `pdm-2.5.2/src/pdm/builders/wheel.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/actions.py` & `pdm-2.5.2/src/pdm/cli/actions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/add.py` & `pdm-2.5.2/src/pdm/cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/base.py` & `pdm-2.5.2/src/pdm/cli/commands/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/build.py` & `pdm-2.5.2/src/pdm/cli/commands/build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/cache.py` & `pdm-2.5.2/src/pdm/cli/commands/cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/completion.py` & `pdm-2.5.2/src/pdm/cli/commands/completion.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/config.py` & `pdm-2.5.2/src/pdm/cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/export.py` & `pdm-2.5.2/src/pdm/cli/commands/export.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/fix/__init__.py` & `pdm-2.5.2/src/pdm/cli/commands/fix/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/fix/fixers.py` & `pdm-2.5.2/src/pdm/cli/commands/fix/fixers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/import_cmd.py` & `pdm-2.5.2/src/pdm/cli/commands/import_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/info.py` & `pdm-2.5.2/src/pdm/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/init.py` & `pdm-2.5.2/src/pdm/cli/commands/init.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,16 +90,16 @@
                 "For more info, please visit https://peps.python.org/pep-0582/",
                 style="success",
             )
         is_library = options.lib
         if not is_library and self.interactive:
             is_library = termui.confirm(
                 "Is the project a library that is installable?\n"
-                "A few more questions will be asked to include a project name "
-                "and build backend"
+                "If yes, we will need to ask a few more questions to include "
+                "the project name and build backend"
             )
         build_backend: type[BuildBackend] | None = None
         if is_library:
             name = self.ask("Project name", project.root.name)
             version = self.ask("Project version", "0.1.0")
             description = self.ask("Project description", "")
             if options.backend:
```

### Comparing `pdm-2.5.1/src/pdm/cli/commands/install.py` & `pdm-2.5.2/src/pdm/cli/commands/install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/list.py` & `pdm-2.5.2/src/pdm/cli/commands/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/lock.py` & `pdm-2.5.2/src/pdm/cli/commands/lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/publish/__init__.py` & `pdm-2.5.2/src/pdm/cli/commands/publish/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/publish/package.py` & `pdm-2.5.2/src/pdm/cli/commands/publish/package.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/publish/repository.py` & `pdm-2.5.2/src/pdm/cli/commands/publish/repository.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/remove.py` & `pdm-2.5.2/src/pdm/cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/run.py` & `pdm-2.5.2/src/pdm/cli/commands/run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/search.py` & `pdm-2.5.2/src/pdm/cli/commands/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/self_cmd.py` & `pdm-2.5.2/src/pdm/cli/commands/self_cmd.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/show.py` & `pdm-2.5.2/src/pdm/cli/commands/show.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/sync.py` & `pdm-2.5.2/src/pdm/cli/commands/sync.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/update.py` & `pdm-2.5.2/src/pdm/cli/commands/update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/use.py` & `pdm-2.5.2/src/pdm/cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/venv/__init__.py` & `pdm-2.5.2/src/pdm/cli/commands/venv/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/venv/activate.py` & `pdm-2.5.2/src/pdm/cli/commands/venv/activate.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/venv/backends.py` & `pdm-2.5.2/src/pdm/cli/commands/venv/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/venv/create.py` & `pdm-2.5.2/src/pdm/cli/commands/venv/create.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/venv/list.py` & `pdm-2.5.2/src/pdm/cli/commands/venv/list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/venv/purge.py` & `pdm-2.5.2/src/pdm/cli/commands/venv/purge.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/venv/remove.py` & `pdm-2.5.2/src/pdm/cli/commands/venv/remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/commands/venv/utils.py` & `pdm-2.5.2/src/pdm/cli/commands/venv/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/completions/pdm.bash` & `pdm-2.5.2/src/pdm/cli/completions/pdm.bash`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/completions/pdm.fish` & `pdm-2.5.2/src/pdm/cli/completions/pdm.fish`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l save-minimum -d 'Save minimum version specifiers'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l save-wildcard -d 'Save wildcard version specifiers'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l unconstrained -d 'Ignore the version constraint of packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l update-all -d 'Update all dependencies and sub-dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l update-eager -d 'Try to update the packages and their dependencies recursively'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l update-reuse -d 'Reuse pinned versions already present in lock file if possible'
-complete -c pdm -A -n '__fish_seen_subcommand_from add' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
+complete -c pdm -A -n '__fish_seen_subcommand_from add' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from add' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # build
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l config-setting -d 'Pass options to the backend. options with a value must be specified after "=": "--config-setting=--opt(=value)" or "-C--opt(=value)"'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l dest -d 'Target directory to put artifacts'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l help -d 'show this help message and exit'
 complete -c pdm -A -n '__fish_seen_subcommand_from build' -l no-clean -d 'Do not clean the target directory'
@@ -134,15 +134,15 @@
 # info
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l env -d 'Show PEP 508 environment markers'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l help -d 'show this help message and exit'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l packages -d 'Show the local packages root'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l python -d 'Show the interpreter path'
-complete -c pdm -A -n '__fish_seen_subcommand_from info' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
+complete -c pdm -A -n '__fish_seen_subcommand_from info' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l verbose -d '-v for detailed output and -vv for more detailed'
 complete -c pdm -A -n '__fish_seen_subcommand_from info' -l where -d 'Show the project root path'
 
 # init
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l backend -d 'Specify the build backend'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from init' -l help -d 'show this help message and exit'
@@ -166,15 +166,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-editable -d 'Install non-editable versions for all packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-lock -d 'Don\'t do lock if the lock file is not found or outdated'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l no-self -d 'Don\'t install the project itself'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
-complete -c pdm -A -n '__fish_seen_subcommand_from install' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
+complete -c pdm -A -n '__fish_seen_subcommand_from install' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from install' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # list
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l csv -d 'Output dependencies in CSV document format'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l exclude -d 'Exclude dependency groups from the output'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l fields -d 'Select information to output as a comma separated string. For example: name,version,homepage,licenses,groups.'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l freeze -d 'Show the installed dependencies in pip\'s requirements.txt format'
@@ -184,15 +184,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l include -d 'Dependency groups to include in the output. By default all are included'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l json -d 'Output dependencies in JSON document format'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l markdown -d 'Output dependencies and legal notices in markdown document format - best effort basis'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l resolve -d 'Resolve all requirements to output licenses (instead of just showing those currently installed)'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l reverse -d 'Reverse the dependency graph'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l sort -d 'Sort the output using a given field name. If nothing is set, no sort is applied. Multiple fields can be combined with \',\'.'
-complete -c pdm -A -n '__fish_seen_subcommand_from list' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
+complete -c pdm -A -n '__fish_seen_subcommand_from list' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from list' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # lock
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l check -d 'Check if the lock file is up to date and quit'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from lock' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species.'
@@ -234,25 +234,25 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l lockfile -d 'Specify another lockfile path. Default: pdm.lock. [env var: PDM_LOCKFILE]'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-editable -d 'Install non-editable versions for all packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-self -d 'Don\'t install the project itself'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l no-sync -d 'Only write pyproject.toml and do not uninstall packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
-complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
+complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from remove' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # run
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l help -d 'show this help message and exit'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l list -d 'Show all available scripts defined in pyproject.toml'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l site-packages -d 'Load site-packages from the selected interpreter'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
-complete -c pdm -A -n '__fish_seen_subcommand_from run' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
+complete -c pdm -A -n '__fish_seen_subcommand_from run' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from run' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # search
 complete -c pdm -A -n '__fish_seen_subcommand_from search' -l help -d 'show this help message and exit'
 complete -c pdm -A -n '__fish_seen_subcommand_from search' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # self
@@ -264,15 +264,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l help -d 'show this help message and exit'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l keywords -d 'Show keywords'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l license -d 'Show license'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l name -d 'Show name'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l platform -d 'Show platform'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l summary -d 'Show summary'
-complete -c pdm -A -n '__fish_seen_subcommand_from show' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
+complete -c pdm -A -n '__fish_seen_subcommand_from show' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l verbose -d '-v for detailed output and -vv for more detailed'
 complete -c pdm -A -n '__fish_seen_subcommand_from show' -l version -d 'Show version'
 
 # sync
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l clean -d 'clean packages not in the lockfile'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l dry-run -d 'Show the difference only and don\'t perform any action'
@@ -286,15 +286,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l no-isolation -d 'Do not isolate the build in a clean environment'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l no-self -d 'Don\'t install the project itself'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l only-keep -d 'only keep the selected packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l production -d 'Unselect dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l project -d 'Specify another path as the project root, which changes the base of pyproject.toml and __pypackages__'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l reinstall -d 'Force reinstall existing dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
-complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
+complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from sync' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # update
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l dev -d 'Select dev dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l fail-fast -d 'Abort on first installation error'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l group -d 'Select group of optional-dependencies separated by comma or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species.'
@@ -315,15 +315,15 @@
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l save-wildcard -d 'Save wildcard version specifiers'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l skip -d 'Skip some tasks and/or hooks by their comma-separated names. Can be supplied multiple times. Use ":all" to skip all hooks. Use ":pre" and ":post" to skip all pre or post hooks.'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l top -d 'Only update those listed in pyproject.toml'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l unconstrained -d 'Ignore the version constraint of packages'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l update-all -d 'Update all dependencies and sub-dependencies'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l update-eager -d 'Try to update the packages and their dependencies recursively'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l update-reuse -d 'Reuse pinned versions already present in lock file if possible'
-complete -c pdm -A -n '__fish_seen_subcommand_from update' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]'
+complete -c pdm -A -n '__fish_seen_subcommand_from update' -l venv -d 'Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]'
 complete -c pdm -A -n '__fish_seen_subcommand_from update' -l verbose -d '-v for detailed output and -vv for more detailed'
 
 # use
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l first -d 'Select the first matched interpreter'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l global -d 'Use the global project, supply the project root with `-p` option'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l help -d 'show this help message and exit'
 complete -c pdm -A -n '__fish_seen_subcommand_from use' -l ignore-remembered -d 'Ignore the remembered selection'
```

### Comparing `pdm-2.5.1/src/pdm/cli/completions/pdm.ps1` & `pdm-2.5.2/src/pdm/cli/completions/pdm.ps1`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/completions/pdm.zsh` & `pdm-2.5.2/src/pdm/cli/completions/pdm.zsh`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
         '--save-exact[Save exact version specifiers]'
         '--save-minimum[Save minimum version specifiers]'
         '--update-reuse[Reuse pinned versions already present in lock file if possible]'
         '--update-eager[Try to update the packages and their dependencies recursively]'
         '--update-all[Update all dependencies and sub-dependencies]'
         '--no-editable[Install non-editable versions for all packages]'
         "--no-self[Don't install the project itself]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
+        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]'
         {-u,--unconstrained}'[Ignore the version constraint of packages]'
         {--pre,--prerelease}'[Allow prereleases to be pinned]'
         {-e+,--editable+}'[Specify editable packages]:packages'
         {-x,--fail-fast}'[Abort on first installation error]'
         "--no-isolation[do not isolate the build in a clean environment]"
         "--dry-run[Show the difference only without modifying the lockfile content]"
@@ -170,15 +170,15 @@
     info)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         '--python[Show the interpreter path]'
         '--where[Show the project root path]'
         '--env[Show PEP 508 environment markers]'
         '--packages[Show the packages root]'
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
+        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
       )
       ;;
     init)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-n,--non-interactive}"[Don't ask questions but use default values]"
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]'
@@ -199,15 +199,15 @@
         "--no-default[Don\'t include dependencies from the default group]"
         '--no-editable[Install non-editable versions for all packages]'
         "--no-self[Don't install the project itself]"
         {-x,--fail-fast}'[Abort on first installation error]'
         "--no-isolation[do not isolate the build in a clean environment]"
         "--dry-run[Show the difference only without modifying the lock file content]"
         "--check[Check if the lock file is up to date and fail otherwise]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
+        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
       )
       ;;
     list)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-r,--reverse}'[Reverse the dependency graph]'
         '--fields[Select information to output as a comma separated string.]:fields:'
@@ -216,15 +216,15 @@
         '--csv[Output dependencies in CSV document format]'
         '--markdown[Output dependencies and legal notices in markdown document format - best effort basis]'
         '--graph[Display a graph of dependencies]'
         "--freeze[Show the installed dependencies as pip's requirements.txt format]"
         "--include[Dependency groups to include in the output. By default all are included]:include:"
         "--exclude[Dependency groups to exclude from the output]:exclude:"
         "--resolve[Resolve all requirements to output licenses (instead of just showing those currently installed)"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
+        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
       )
       ;;
     lock)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-L,--lockfile}'[Specify another lockfile path, or use `PDM_LOCKFILE` env variable. Default: pdm.lock]:lockfile:_files'
         "--no-isolation[Do not isolate the build in a clean environment]"
@@ -308,25 +308,25 @@
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]'
         "--no-sync[Only write pyproject.toml and do not uninstall packages]"
         '--no-editable[Install non-editable versions for all packages]'
         "--no-self[Don't install the project itself]"
         {-x,--fail-fast}'[Abort on first installation error]'
         "--no-isolation[do not isolate the build in a clean environment]"
         "--dry-run[Show the difference only without modifying the lockfile content]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
+        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
         "*:packages:_pdm_packages"
       )
       ;;
     run)
       _arguments -s \
         {-g,--global}'[Use the global project, supply the project root with `-p` option]' \
         {-l,--list}'[Show all available scripts defined in pyproject.toml]' \
         {-k,--skip}'[Skip some tasks and/or hooks by their comma-separated names]' \
         {-s,--site-packages}'[Load site-packages from the selected interpreter]' \
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:' \
+        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:' \
         '(-)1:command:->command' \
         '*:arguments: _normal ' && return 0
       if [[ $state == command ]]; then
         _command_names -e
         local local_commands=($(_pdm_scripts))
         _describe "local command" local_commands
         return 0
@@ -342,15 +342,15 @@
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         '--name[Show name]'
         '--version[Show version]'
         '--summary[Show summary]'
         '--license[Show license]'
         '--platform[Show platform]'
         '--keywords[Show keywords]'
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
+        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
         '1:package:'
       )
       ;;
     sync)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-G+,--group+}'[Select group of optional-dependencies or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species]:group:_pdm_groups'
@@ -363,15 +363,15 @@
         '--clean[Clean unused packages]'
         "--only-keep[Only keep the selected packages]"
         "--no-default[Don\'t include dependencies from the default group]"
         {-x,--fail-fast}'[Abort on first installation error]'
         '--no-editable[Install non-editable versions for all packages]'
         "--no-self[Don't install the project itself]"
         "--no-isolation[do not isolate the build in a clean environment]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
+        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
       )
       ;;
     update)
       arguments+=(
         {-g,--global}'[Use the global project, supply the project root with `-p` option]'
         {-G+,--group+}'[Select group of optional-dependencies or dev-dependencies(with -d). Can be supplied multiple times, use ":all" to include all groups under the same species]:group:_pdm_groups'
         {-L,--lockfile}'[Specify another lockfile path, or use `PDM_LOCKFILE` env variable. Default: pdm.lock]:lockfile:_files'
@@ -392,15 +392,15 @@
         {--prod,--production}"[Unselect dev dependencies]"
         "--no-default[Don\'t include dependencies from the default group]"
         {-t,--top}'[Only update those list in pyproject.toml]'
         "--dry-run[Show the difference only without modifying the lockfile content]"
         "--outdated[Show the difference only without modifying the lockfile content]"
         {-x,--fail-fast}'[Abort on first installation error]'
         "--no-isolation[do not isolate the build in a clean environment]"
-        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]]:venv:'
+        '--venv[Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]]:venv:'
         "*:packages:_pdm_packages"
       )
       ;;
     use)
       arguments+=(
         {-f,--first}'[Select the first matched interpreter]'
         {-i,--ignore-remembered}'[Ignore the remembered selection]'
```

### Comparing `pdm-2.5.1/src/pdm/cli/filters.py` & `pdm-2.5.2/src/pdm/cli/filters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/hooks.py` & `pdm-2.5.2/src/pdm/cli/hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/cli/options.py` & `pdm-2.5.2/src/pdm/cli/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,10 +343,10 @@
 
 venv_option = Option(
     "--venv",
     dest="use_venv",
     metavar="NAME",
     nargs="?",
     const="in-project",
-    help="Run the command in the virtual environment with the given key. [env var: PDM_USE_VENV]",
-    default=os.getenv("PDM_USE_VENV"),
+    help="Run the command in the virtual environment with the given key. [env var: PDM_IN_VENV]",
+    default=os.getenv("PDM_IN_VENV"),
 )
```

### Comparing `pdm-2.5.1/src/pdm/cli/utils.py` & `pdm-2.5.2/src/pdm/cli/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/compat.py` & `pdm-2.5.2/src/pdm/compat.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/core.py` & `pdm-2.5.2/src/pdm/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/environments/__init__.py` & `pdm-2.5.2/src/pdm/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/environments/base.py` & `pdm-2.5.2/src/pdm/environments/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/environments/local.py` & `pdm-2.5.2/src/pdm/environments/local.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,31 +23,33 @@
     where the interpreter path is quoted.
     """
     if is_launcher or " " not in executable and (len(executable) + 3) <= 127:
         return executable.encode("utf-8")
     return shlex.quote(executable).encode("utf-8")
 
 
-def _replace_shebang(contents: bytes, new_executable: bytes) -> bytes:
+def _replace_shebang(path: Path, new_executable: bytes) -> None:
     """Replace the python executable from the shebeng line, which can be in two forms:
 
     1. #!python_executable
     2. #!/bin/sh
        '''exec' '/path to/python' "$0" "$@"
        ' '''
     """
     _complex_shebang_re = rb"^'''exec' ('.+?') \"\$0\""
     _simple_shebang_re = rb"^#!(.+?)\s*$"
+    contents = path.read_bytes()
     match = re.search(_complex_shebang_re, contents, flags=re.M)
     if match:
-        return contents.replace(match.group(1), new_executable, 1)
-    else:
-        match = re.search(_simple_shebang_re, contents, flags=re.M)
-        assert match is not None
-        return contents.replace(match.group(1), new_executable, 1)
+        path.write_bytes(contents.replace(match.group(1), new_executable, 1))
+        return
+
+    match = re.search(_simple_shebang_re, contents, flags=re.M)
+    if match:
+        path.write_bytes(contents.replace(match.group(1), new_executable, 1))
 
 
 class PythonLocalEnvironment(BaseEnvironment):
     """A project environment that installs packages into
     the local `__pypackages__` directory(PEP 582).
     """
 
@@ -87,8 +89,8 @@
         """Update the shebang lines"""
         scripts = self.get_paths()["scripts"]
         for child in Path(scripts).iterdir():
             if not child.is_file() or child.suffix not in (".exe", ".py", ""):
                 continue
             is_launcher = child.suffix == ".exe"
             new_shebang = _get_shebang_path(new_path, is_launcher)
-            child.write_bytes(_replace_shebang(child.read_bytes(), new_shebang))
+            _replace_shebang(child, new_shebang)
```

### Comparing `pdm-2.5.1/src/pdm/environments/prefix.py` & `pdm-2.5.2/src/pdm/environments/prefix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/environments/python.py` & `pdm-2.5.2/src/pdm/environments/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/exceptions.py` & `pdm-2.5.2/src/pdm/exceptions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/formats/__init__.py` & `pdm-2.5.2/src/pdm/formats/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/formats/base.py` & `pdm-2.5.2/src/pdm/formats/base.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/formats/flit.py` & `pdm-2.5.2/src/pdm/formats/flit.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/formats/pipfile.py` & `pdm-2.5.2/src/pdm/formats/pipfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/formats/poetry.py` & `pdm-2.5.2/src/pdm/formats/poetry.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/formats/requirements.py` & `pdm-2.5.2/src/pdm/formats/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/formats/setup_py.py` & `pdm-2.5.2/src/pdm/formats/setup_py.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/installers/core.py` & `pdm-2.5.2/src/pdm/installers/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/installers/installers.py` & `pdm-2.5.2/src/pdm/installers/installers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/installers/manager.py` & `pdm-2.5.2/src/pdm/installers/manager.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/installers/packages.py` & `pdm-2.5.2/src/pdm/installers/packages.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/installers/synchronizers.py` & `pdm-2.5.2/src/pdm/installers/synchronizers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/installers/uninstallers.py` & `pdm-2.5.2/src/pdm/installers/uninstallers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/auth.py` & `pdm-2.5.2/src/pdm/models/auth.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/backends.py` & `pdm-2.5.2/src/pdm/models/backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/caches.py` & `pdm-2.5.2/src/pdm/models/caches.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/candidates.py` & `pdm-2.5.2/src/pdm/models/candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/in_process/__init__.py` & `pdm-2.5.2/src/pdm/models/in_process/__init__.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/in_process/get_abi_tag.py` & `pdm-2.5.2/src/pdm/models/in_process/get_abi_tag.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/in_process/parse_setup.py` & `pdm-2.5.2/src/pdm/models/in_process/parse_setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/in_process/pep508.py` & `pdm-2.5.2/src/pdm/models/in_process/pep508.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/in_process/sysconfig_get_paths.py` & `pdm-2.5.2/src/pdm/models/in_process/sysconfig_get_paths.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/markers.py` & `pdm-2.5.2/src/pdm/models/markers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/project_info.py` & `pdm-2.5.2/src/pdm/models/project_info.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/python.py` & `pdm-2.5.2/src/pdm/models/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/repositories.py` & `pdm-2.5.2/src/pdm/models/repositories.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/requirements.py` & `pdm-2.5.2/src/pdm/models/requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/search.py` & `pdm-2.5.2/src/pdm/models/search.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/session.py` & `pdm-2.5.2/src/pdm/models/session.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/setup.py` & `pdm-2.5.2/src/pdm/models/setup.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/specifiers.py` & `pdm-2.5.2/src/pdm/models/specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/versions.py` & `pdm-2.5.2/src/pdm/models/versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/models/working_set.py` & `pdm-2.5.2/src/pdm/models/working_set.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/pep582/sitecustomize.py` & `pdm-2.5.2/src/pdm/pep582/sitecustomize.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/project/config.py` & `pdm-2.5.2/src/pdm/project/config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/project/core.py` & `pdm-2.5.2/src/pdm/project/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/project/lockfile.py` & `pdm-2.5.2/src/pdm/project/lockfile.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/project/project_file.py` & `pdm-2.5.2/src/pdm/project/project_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/project/toml_file.py` & `pdm-2.5.2/src/pdm/project/toml_file.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/pytest.py` & `pdm-2.5.2/src/pdm/pytest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/resolver/core.py` & `pdm-2.5.2/src/pdm/resolver/core.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/resolver/providers.py` & `pdm-2.5.2/src/pdm/resolver/providers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/resolver/python.py` & `pdm-2.5.2/src/pdm/resolver/python.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/resolver/reporters.py` & `pdm-2.5.2/src/pdm/resolver/reporters.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/signals.py` & `pdm-2.5.2/src/pdm/signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/termui.py` & `pdm-2.5.2/src/pdm/termui.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/src/pdm/utils.py` & `pdm-2.5.2/src/pdm/utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/conftest.py` & `pdm-2.5.2/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_add.py` & `pdm-2.5.2/tests/cli/test_add.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_build.py` & `pdm-2.5.2/tests/cli/test_build.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_cache.py` & `pdm-2.5.2/tests/cli/test_cache.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_config.py` & `pdm-2.5.2/tests/cli/test_config.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_fix.py` & `pdm-2.5.2/tests/cli/test_fix.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_hooks.py` & `pdm-2.5.2/tests/cli/test_hooks.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_init.py` & `pdm-2.5.2/tests/cli/test_init.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_install.py` & `pdm-2.5.2/tests/cli/test_install.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_list.py` & `pdm-2.5.2/tests/cli/test_list.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_lock.py` & `pdm-2.5.2/tests/cli/test_lock.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_others.py` & `pdm-2.5.2/tests/cli/test_others.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     project._saved_python = None
     result = pdm(["info", "--python"], obj=project, strict=True)
     assert Path(result.output.strip()).parent.parent == project.root / ".venv"
     venv_location = project.config["venv.location"]
     result = pdm(["info", "--python", "--venv", "test"], obj=project, strict=True)
     assert Path(result.output.strip()).parent.parent.parent == project.root / venv_location
 
-    result = pdm(["info", "--python", "--venv", "test"], obj=project, strict=True, env={"PDM_USE_VENV": "test"})
+    result = pdm(["info", "--python", "--venv", "test"], obj=project, strict=True, env={"PDM_IN_VENV": "test"})
     assert Path(result.output.strip()).parent.parent.parent == project.root / venv_location
     result = pdm(["info", "--python", "--venv", "default"], obj=project)
     assert "No virtualenv with key 'default' is found" in result.stderr
 
 
 def test_global_project_other_location(pdm, project):
     result = pdm(["info", "-g", "-p", project.root.as_posix(), "--where"])
```

### Comparing `pdm-2.5.1/tests/cli/test_publish.py` & `pdm-2.5.2/tests/cli/test_publish.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_remove.py` & `pdm-2.5.2/tests/cli/test_remove.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_run.py` & `pdm-2.5.2/tests/cli/test_run.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_self_command.py` & `pdm-2.5.2/tests/cli/test_self_command.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_update.py` & `pdm-2.5.2/tests/cli/test_update.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_use.py` & `pdm-2.5.2/tests/cli/test_use.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/cli/test_venv.py` & `pdm-2.5.2/tests/cli/test_venv.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/conftest.py` & `pdm-2.5.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/PyFunctional-1.4.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz` & `pdm-2.5.2/tests/fixtures/artifacts/caj2pdf-restructured-0.1.0a6.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/celery-4.4.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl` & `pdm-2.5.2/tests/fixtures/artifacts/demo-0.0.1-cp36-cp36m-win_amd64.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/demo-0.0.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/demo-0.0.1.tar.gz` & `pdm-2.5.2/tests/fixtures/artifacts/demo-0.0.1.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/demo-0.0.1.zip` & `pdm-2.5.2/tests/fixtures/artifacts/demo-0.0.1.zip`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/editables-0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/first-2.0.2-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/flit_core-3.6.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/future_fstrings-1.2.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz` & `pdm-2.5.2/tests/fixtures/artifacts/future_fstrings-1.2.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/importlib_metadata-4.8.3-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/jmespath-0.10.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/pdm_backend-2.0.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/pdm_pep517-1.0.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/poetry_core-1.3.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/setuptools-65.4.1-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/typing_extensions-4.4.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/wheel-0.37.1-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl` & `pdm-2.5.2/tests/fixtures/artifacts/zipp-3.7.0-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock` & `pdm-2.5.2/tests/fixtures/projects/demo-package-has-dep-with-extras/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/projects/demo-package/pdm.lock` & `pdm-2.5.2/tests/fixtures/projects/demo-package/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/projects/demo-package/pyproject.toml` & `pdm-2.5.2/tests/fixtures/projects/demo-package/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/projects/demo-package/requirements.txt` & `pdm-2.5.2/tests/fixtures/projects/demo-package/requirements.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/projects/demo-package/setup.txt` & `pdm-2.5.2/tests/fixtures/projects/demo-package/setup.txt`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/projects/flit-demo/pyproject.toml` & `pdm-2.5.2/tests/fixtures/projects/flit-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/projects/poetry-demo/pyproject.toml` & `pdm-2.5.2/tests/fixtures/projects/poetry-demo/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/pypi.json` & `pdm-2.5.2/tests/fixtures/pypi.json`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/fixtures/pyproject.toml` & `pdm-2.5.2/tests/fixtures/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/models/test_backends.py` & `pdm-2.5.2/tests/models/test_backends.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/models/test_candidates.py` & `pdm-2.5.2/tests/models/test_candidates.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/models/test_marker.py` & `pdm-2.5.2/tests/models/test_marker.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/models/test_requirements.py` & `pdm-2.5.2/tests/models/test_requirements.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/models/test_setup_parsing.py` & `pdm-2.5.2/tests/models/test_setup_parsing.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/models/test_specifiers.py` & `pdm-2.5.2/tests/models/test_specifiers.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/models/test_versions.py` & `pdm-2.5.2/tests/models/test_versions.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/resolver/test_resolve.py` & `pdm-2.5.2/tests/resolver/test_resolve.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/test_formats.py` & `pdm-2.5.2/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/test_installer.py` & `pdm-2.5.2/tests/test_installer.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/test_integration.py` & `pdm-2.5.2/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/test_plugin.py` & `pdm-2.5.2/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/test_project.py` & `pdm-2.5.2/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/test_signals.py` & `pdm-2.5.2/tests/test_signals.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/tests/test_utils.py` & `pdm-2.5.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `pdm-2.5.1/PKG-INFO` & `pdm-2.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm
-Version: 2.5.1
+Version: 2.5.2
 Summary: A modern Python package and dependency manager supporting the latest PEP standards
 Keywords: packaging dependency workflow
 Author-Email: Frost Ming <mianghong@gmail.com>
 License: MIT
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pdm Version: 2.5.1 Summary: A modern Python package
+Metadata-Version: 2.1 Name: pdm Version: 2.5.2 Summary: A modern Python package
 and dependency manager supporting the latest PEP standards Keywords: packaging
 dependency workflow Author-Email: Frost Ming
 gmail.com> License: MIT Classifier: Topic :: Software Development :: Build
 Tools Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
```

