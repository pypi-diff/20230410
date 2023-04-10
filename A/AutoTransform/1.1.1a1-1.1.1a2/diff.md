# Comparing `tmp/AutoTransform-1.1.1a1.tar.gz` & `tmp/AutoTransform-1.1.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AutoTransform-1.1.1a1.tar", last modified: Wed Mar 15 09:41:31 2023, max compression
+gzip compressed data, was "AutoTransform-1.1.1a2.tar", last modified: Mon Apr 10 12:23:29 2023, max compression
```

## Comparing `AutoTransform-1.1.1a1.tar` & `AutoTransform-1.1.1a2.tar`

### file list

```diff
@@ -1,178 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.775530 AutoTransform-1.1.1a1/
--rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/BEST_PRACTICES.md
--rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/COMPONENTS.md
--rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/CUSTOM_DEPLOYMENT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/MANAGE_CHANGES.md
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-03-15 09:41:31.775530 AutoTransform-1.1.1a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/SCHEDULED_RUNS.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.751530 AutoTransform-1.1.1a1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.751530 AutoTransform-1.1.1a1/examples/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/examples/docker/Dockerfile
--rwxr-xr-x   0 runner    (1001) docker     (123)      979 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/examples/docker/docker_autotransform.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      993 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/examples/docker/entrypoint.sh
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/examples/manager.json
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/examples/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/examples/scheduler.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.751530 AutoTransform-1.1.1a1/examples/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/examples/schemas/black_format.json
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/examples/schemas/schema_map.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.751530 AutoTransform-1.1.1a1/examples/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/examples/workflows/autotransform.manage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/examples/workflows/autotransform.run.yml
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/examples/workflows/autotransform.schedule.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/examples/workflows/autotransform.update.yml
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-15 09:41:31.775530 AutoTransform-1.1.1a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.743530 AutoTransform-1.1.1a1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.743530 AutoTransform-1.1.1a1/src/python/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.755530 AutoTransform-1.1.1a1/src/python/AutoTransform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-03-15 09:41:31.000000 AutoTransform-1.1.1a1/src/python/AutoTransform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-03-15 09:41:31.000000 AutoTransform-1.1.1a1/src/python/AutoTransform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-15 09:41:31.000000 AutoTransform-1.1.1a1/src/python/AutoTransform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-15 09:41:31.000000 AutoTransform-1.1.1a1/src/python/AutoTransform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-15 09:41:31.000000 AutoTransform-1.1.1a1/src/python/AutoTransform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-03-15 09:41:31.000000 AutoTransform-1.1.1a1/src/python/AutoTransform.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.755530 AutoTransform-1.1.1a1/src/python/autotransform/
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.755530 AutoTransform-1.1.1a1/src/python/autotransform/batcher/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/batcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/batcher/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/batcher/chunk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/batcher/codeowners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/batcher/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/batcher/extradata.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/batcher/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/batcher/single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.755530 AutoTransform-1.1.1a1/src/python/autotransform/change/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/change/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/change/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9757 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/change/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.759530 AutoTransform-1.1.1a1/src/python/autotransform/command/
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/command/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/command/script.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.759530 AutoTransform-1.1.1a1/src/python/autotransform/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19761 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/config/default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/config/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/config/fetcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.763530 AutoTransform-1.1.1a1/src/python/autotransform/event/
--rw-r--r--   0 runner    (1001) docker     (123)      762 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/event/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/event/action.py
--rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/event/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/event/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/event/handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/event/logginglevel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/event/remoterun.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/event/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/event/schedulerun.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/event/type.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/event/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/event/verbose.py
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/event/warning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.763530 AutoTransform-1.1.1a1/src/python/autotransform/filter/
--rw-r--r--   0 runner    (1001) docker     (123)      432 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/filter/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/filter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/filter/codeowners.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/filter/key_hash_shard.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/filter/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/filter/shard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.767530 AutoTransform-1.1.1a1/src/python/autotransform/input/
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/input/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/input/directory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/input/empty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/input/gitgrep.py
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/input/inline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.767530 AutoTransform-1.1.1a1/src/python/autotransform/item/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/item/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/item/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/item/file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.767530 AutoTransform-1.1.1a1/src/python/autotransform/repo/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/repo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/repo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/repo/git.py
--rw-r--r--   0 runner    (1001) docker     (123)     8371 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/repo/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.767530 AutoTransform-1.1.1a1/src/python/autotransform/runner/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/runner/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/runner/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/runner/jenkins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/runner/local.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.767530 AutoTransform-1.1.1a1/src/python/autotransform/schema/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/schema/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/schema/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/schema/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.767530 AutoTransform-1.1.1a1/src/python/autotransform/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.767530 AutoTransform-1.1.1a1/src/python/autotransform/scripts/commands/
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/scripts/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/scripts/commands/initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/scripts/commands/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/scripts/commands/run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/scripts/commands/schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/scripts/commands/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/scripts/commands/update.py
--rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/scripts/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.771530 AutoTransform-1.1.1a1/src/python/autotransform/scripts/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/scripts/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/scripts/migrations/p1_0_1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/scripts/migrations/p1_0_3.py
--rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/scripts/migrations/p1_0_5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.771530 AutoTransform-1.1.1a1/src/python/autotransform/step/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.771530 AutoTransform-1.1.1a1/src/python/autotransform/step/action/
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/action/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/action/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/action/comments.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/action/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/action/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/action/reviewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/action/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.771530 AutoTransform-1.1.1a1/src/python/autotransform/step/condition/
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/condition/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/condition/aggregate.py
--rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/condition/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/condition/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/condition/created.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/condition/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/condition/request.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/condition/reviewers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/condition/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/condition/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/condition/updated.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/step/conditional.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.771530 AutoTransform-1.1.1a1/src/python/autotransform/transformer/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/transformer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/transformer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/transformer/jscodeshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/transformer/libcst.py
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/transformer/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/transformer/script.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/transformer/single.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.775530 AutoTransform-1.1.1a1/src/python/autotransform/util/
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/util/cachedfile.py
--rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/util/component.py
--rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/util/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/util/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/util/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    18520 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/util/github.py
--rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/util/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/util/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/util/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/util/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/util/schema_map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-15 09:41:31.775530 AutoTransform-1.1.1a1/src/python/autotransform/validator/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/validator/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-03-15 09:40:33.000000 AutoTransform-1.1.1a1/src/python/autotransform/validator/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.781783 AutoTransform-1.1.1a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3699 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/BEST_PRACTICES.md
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/COMPONENTS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/CUSTOM_DEPLOYMENT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/MANAGE_CHANGES.md
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-10 12:23:29.781783 AutoTransform-1.1.1a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4698 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/SCHEDULED_RUNS.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.765783 AutoTransform-1.1.1a2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.765783 AutoTransform-1.1.1a2/examples/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/docker/Dockerfile
+-rwxr-xr-x   0 runner    (1001) docker     (123)      979 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/docker/docker_autotransform.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      993 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/docker/entrypoint.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/manager.json
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/scheduler.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.765783 AutoTransform-1.1.1a2/examples/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/schemas/black_format.json
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/schemas/schema_map.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.765783 AutoTransform-1.1.1a2/examples/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/workflows/autotransform.manage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/workflows/autotransform.run.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/workflows/autotransform.schedule.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/examples/workflows/autotransform.update.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-10 12:23:29.781783 AutoTransform-1.1.1a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.761783 AutoTransform-1.1.1a2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.761783 AutoTransform-1.1.1a2/src/python/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.765783 AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5484 2023-04-10 12:23:29.000000 AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6146 2023-04-10 12:23:29.000000 AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-10 12:23:29.000000 AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-10 12:23:29.000000 AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-10 12:23:29.000000 AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-10 12:23:29.000000 AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.765783 AutoTransform-1.1.1a2/src/python/autotransform/
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.769783 AutoTransform-1.1.1a2/src/python/autotransform/batcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2793 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/chunk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7144 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/codeowners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/extradata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/batcher/single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.769783 AutoTransform-1.1.1a2/src/python/autotransform/change/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/change/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6558 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/change/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10075 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/change/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.769783 AutoTransform-1.1.1a2/src/python/autotransform/command/
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1778 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/command/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5972 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/command/script.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.769783 AutoTransform-1.1.1a2/src/python/autotransform/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3816 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19761 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/config/default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/config/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/config/fetcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.769783 AutoTransform-1.1.1a2/src/python/autotransform/event/
+-rw-r--r--   0 runner    (1001) docker     (123)      762 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2846 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4041 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/logginglevel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/remoterun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/schedulerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1752 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/verbose.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/event/warning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.769783 AutoTransform-1.1.1a2/src/python/autotransform/filter/
+-rw-r--r--   0 runner    (1001) docker     (123)      432 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/filter/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2744 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/filter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/filter/codeowners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/filter/key_hash_shard.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/filter/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1508 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/filter/shard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/input/
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/input/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/input/directory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/input/empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1570 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/input/gitgrep.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/input/inline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/item/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/item/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/item/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1336 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/item/file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/repo/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/repo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/repo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7282 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/repo/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9108 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/repo/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/runner/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/runner/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/runner/jenkins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/runner/local.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/schema/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4826 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/schema/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15352 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/schema/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12182 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7073 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3750 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13430 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5301 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/update.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4619 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/p1_0_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3259 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/p1_0_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2901 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/p1_0_5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.773783 AutoTransform-1.1.1a2/src/python/autotransform/step/
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.777783 AutoTransform-1.1.1a2/src/python/autotransform/step/action/
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/action/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/action/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/action/comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/action/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/action/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4614 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/action/reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/action/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.777783 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/aggregate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11990 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2651 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/created.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/reviewers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/condition/updated.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/step/conditional.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.777783 AutoTransform-1.1.1a2/src/python/autotransform/transformer/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/transformer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/transformer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/transformer/jscodeshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3662 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/transformer/libcst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/transformer/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5322 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/transformer/script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/transformer/single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.777783 AutoTransform-1.1.1a2/src/python/autotransform/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/cachedfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15661 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8670 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18520 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8931 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5725 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16845 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5689 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/util/schema_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-10 12:23:29.777783 AutoTransform-1.1.1a2/src/python/autotransform/validator/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/validator/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7186 2023-04-10 12:22:33.000000 AutoTransform-1.1.1a2/src/python/autotransform/validator/script.py
```

### Comparing `AutoTransform-1.1.1a1/BEST_PRACTICES.md` & `AutoTransform-1.1.1a2/BEST_PRACTICES.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/COMPONENTS.md` & `AutoTransform-1.1.1a2/COMPONENTS.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/CONTRIBUTING.md` & `AutoTransform-1.1.1a2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/CUSTOM_DEPLOYMENT.md` & `AutoTransform-1.1.1a2/CUSTOM_DEPLOYMENT.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/LICENSE` & `AutoTransform-1.1.1a2/LICENSE`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/MANAGE_CHANGES.md` & `AutoTransform-1.1.1a2/MANAGE_CHANGES.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/PKG-INFO` & `AutoTransform-1.1.1a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoTransform
-Version: 1.1.1a1
+Version: 1.1.1a2
 Summary: A component based framework for designing automated code modification
 Home-page: https://github.com/nathro/AutoTransform
 Author: Nathan Rockenbach
 Author-email: nathro.software@gmail.com
 Project-URL: Source, https://github.com/nathro/AutoTransform/
 Project-URL: Bug Tracker, https://github.com/nathro/AutoTransform/issues
 Keywords: codemod,automation,code change,codeshift,transformation,maintain
```

### Comparing `AutoTransform-1.1.1a1/README.md` & `AutoTransform-1.1.1a2/README.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/SCHEDULED_RUNS.md` & `AutoTransform-1.1.1a2/SCHEDULED_RUNS.md`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/examples/docker/docker_autotransform.sh` & `AutoTransform-1.1.1a2/examples/docker/docker_autotransform.sh`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/examples/docker/entrypoint.sh` & `AutoTransform-1.1.1a2/examples/docker/entrypoint.sh`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/examples/manager.json` & `AutoTransform-1.1.1a2/examples/manager.json`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/examples/schemas/black_format.json` & `AutoTransform-1.1.1a2/examples/schemas/black_format.json`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/examples/workflows/autotransform.manage.yml` & `AutoTransform-1.1.1a2/examples/workflows/autotransform.manage.yml`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/examples/workflows/autotransform.run.yml` & `AutoTransform-1.1.1a2/examples/workflows/autotransform.run.yml`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/examples/workflows/autotransform.schedule.yml` & `AutoTransform-1.1.1a2/examples/workflows/autotransform.schedule.yml`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/examples/workflows/autotransform.update.yml` & `AutoTransform-1.1.1a2/examples/workflows/autotransform.update.yml`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/setup.py` & `AutoTransform-1.1.1a2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         data_files.append((f"autotransform-{path}", [os.path.join(path, file) for file in files]))
 
     return data_files
 
 
 setuptools.setup(
     name="AutoTransform",
-    version="1.1.1a1",
+    version="1.1.1a2",
     author="Nathan Rockenbach",
     author_email="nathro.software@gmail.com",
     description="A component based framework for designing automated code modification",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/nathro/AutoTransform",
     project_urls={
```

### Comparing `AutoTransform-1.1.1a1/src/python/AutoTransform.egg-info/PKG-INFO` & `AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AutoTransform
-Version: 1.1.1a1
+Version: 1.1.1a2
 Summary: A component based framework for designing automated code modification
 Home-page: https://github.com/nathro/AutoTransform
 Author: Nathan Rockenbach
 Author-email: nathro.software@gmail.com
 Project-URL: Source, https://github.com/nathro/AutoTransform/
 Project-URL: Bug Tracker, https://github.com/nathro/AutoTransform/issues
 Keywords: codemod,automation,code change,codeshift,transformation,maintain
```

### Comparing `AutoTransform-1.1.1a1/src/python/AutoTransform.egg-info/SOURCES.txt` & `AutoTransform-1.1.1a2/src/python/AutoTransform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/__init__.py` & `AutoTransform-1.1.1a2/src/python/autotransform/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/batcher/base.py` & `AutoTransform-1.1.1a2/src/python/autotransform/batcher/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/batcher/chunk.py` & `AutoTransform-1.1.1a2/src/python/autotransform/batcher/chunk.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/batcher/codeowners.py` & `AutoTransform-1.1.1a2/src/python/autotransform/batcher/codeowners.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/batcher/directory.py` & `AutoTransform-1.1.1a2/src/python/autotransform/batcher/directory.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/batcher/extradata.py` & `AutoTransform-1.1.1a2/src/python/autotransform/batcher/extradata.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/batcher/regex.py` & `AutoTransform-1.1.1a2/src/python/autotransform/batcher/regex.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/batcher/single.py` & `AutoTransform-1.1.1a2/src/python/autotransform/batcher/single.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/change/base.py` & `AutoTransform-1.1.1a2/src/python/autotransform/change/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/change/github.py` & `AutoTransform-1.1.1a2/src/python/autotransform/change/github.py`

 * *Files 16% similar despite different names*

```diff
@@ -278,39 +278,44 @@
         """Loads the Schema and Batch data for the GithubChange as a cached property.
 
         Returns:
             Tuple[AutoTransformSchema, Batch]: The Schema and Batch contained
                 in the PullRequest's Body.
         """
 
-        data: Dict[str, str] = {}
         gist_match = re.search("<<<Automation Info Gist: (.*)>>>", self._pull_request.body)
         if gist_match:
-            gist = GithubUtils.get(self.full_github_name).get_gist(gist_match.groups()[0])
-            data["schema"] = gist.get_file_content("schema") or ""
-            data["batch"] = gist.get_file_content("batch") or ""
+            gist_ids = gist_match.groups()[0].split("/")
+            gist = GithubUtils.get(self.full_github_name).get_gist(gist_ids[0])
+            schema_data = gist.get_file_content("schema") or ""
+            batch = json.loads(gist.get_file_content("batch") or "")
+            assert isinstance(batch["items"], List)
+            for i in range(1, len(gist_ids)):
+                gist = GithubUtils.get(self.full_github_name).get_gist(gist_ids[i])
+                items = json.loads(gist.get_file_content("items") or "[]")
+                assert isinstance(items, List)
+                batch["items"].extend(items)
         else:
             cur_line_placement = None
             data_lines: Dict[str, List[str]] = {"schema": [], "batch": []}
             for line in self._pull_request.body.splitlines():
                 if line == GithubUtils.BEGIN_SCHEMA:
                     cur_line_placement = "schema"
                 elif line == GithubUtils.END_SCHEMA:
                     cur_line_placement = None
                 elif line == GithubUtils.BEGIN_BATCH:
                     cur_line_placement = "batch"
                 elif line == GithubUtils.END_BATCH:
                     cur_line_placement = None
                 elif cur_line_placement is not None:
                     data_lines[cur_line_placement].append(line)
-            data["schema"] = "\n".join(data_lines["schema"])
-            data["batch"] = "\n".join(data_lines["batch"])
+            schema_data = "\n".join(data_lines["schema"])
+            batch = json.loads("\n".join(data_lines["batch"]))
 
-        schema = AutoTransformSchema.from_data(json.loads(data["schema"]))
-        batch = json.loads(data["batch"])
+        schema = AutoTransformSchema.from_data(json.loads(schema_data))
         items = [item_factory.get_instance(item) for item in batch["items"]]
         batch = {
             "items": items,
             "metadata": batch["metadata"],
             "title": str(batch["title"]),
         }
         return (schema, batch)
```

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/command/__init__.py` & `AutoTransform-1.1.1a2/src/python/autotransform/command/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/command/base.py` & `AutoTransform-1.1.1a2/src/python/autotransform/command/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/command/script.py` & `AutoTransform-1.1.1a2/src/python/autotransform/command/script.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/config/__init__.py` & `AutoTransform-1.1.1a2/src/python/autotransform/config/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/config/config.py` & `AutoTransform-1.1.1a2/src/python/autotransform/config/config.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/config/default.py` & `AutoTransform-1.1.1a2/src/python/autotransform/config/default.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/config/environment.py` & `AutoTransform-1.1.1a2/src/python/autotransform/config/environment.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/config/fetcher.py` & `AutoTransform-1.1.1a2/src/python/autotransform/config/fetcher.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/event/__init__.py` & `AutoTransform-1.1.1a2/src/python/autotransform/event/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/event/action.py` & `AutoTransform-1.1.1a2/src/python/autotransform/event/action.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/event/base.py` & `AutoTransform-1.1.1a2/src/python/autotransform/event/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/event/debug.py` & `AutoTransform-1.1.1a2/src/python/autotransform/event/debug.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/event/handler.py` & `AutoTransform-1.1.1a2/src/python/autotransform/event/handler.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/event/logginglevel.py` & `AutoTransform-1.1.1a2/src/python/autotransform/event/logginglevel.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/event/remoterun.py` & `AutoTransform-1.1.1a2/src/python/autotransform/event/remoterun.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/event/run.py` & `AutoTransform-1.1.1a2/src/python/autotransform/event/run.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/event/schedulerun.py` & `AutoTransform-1.1.1a2/src/python/autotransform/event/schedulerun.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/event/type.py` & `AutoTransform-1.1.1a2/src/python/autotransform/event/type.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/event/update.py` & `AutoTransform-1.1.1a2/src/python/autotransform/event/update.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/event/verbose.py` & `AutoTransform-1.1.1a2/src/python/autotransform/event/verbose.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/event/warning.py` & `AutoTransform-1.1.1a2/src/python/autotransform/event/warning.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/filter/aggregate.py` & `AutoTransform-1.1.1a2/src/python/autotransform/filter/aggregate.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/filter/base.py` & `AutoTransform-1.1.1a2/src/python/autotransform/filter/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/filter/codeowners.py` & `AutoTransform-1.1.1a2/src/python/autotransform/filter/codeowners.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/filter/key_hash_shard.py` & `AutoTransform-1.1.1a2/src/python/autotransform/filter/key_hash_shard.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/filter/regex.py` & `AutoTransform-1.1.1a2/src/python/autotransform/filter/regex.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/filter/shard.py` & `AutoTransform-1.1.1a2/src/python/autotransform/filter/shard.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/input/base.py` & `AutoTransform-1.1.1a2/src/python/autotransform/input/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/input/directory.py` & `AutoTransform-1.1.1a2/src/python/autotransform/input/directory.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/input/empty.py` & `AutoTransform-1.1.1a2/src/python/autotransform/input/empty.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/input/gitgrep.py` & `AutoTransform-1.1.1a2/src/python/autotransform/input/gitgrep.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/input/inline.py` & `AutoTransform-1.1.1a2/src/python/autotransform/input/inline.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/item/base.py` & `AutoTransform-1.1.1a2/src/python/autotransform/item/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/item/file.py` & `AutoTransform-1.1.1a2/src/python/autotransform/item/file.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/repo/base.py` & `AutoTransform-1.1.1a2/src/python/autotransform/repo/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/repo/git.py` & `AutoTransform-1.1.1a2/src/python/autotransform/repo/git.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/repo/github.py` & `AutoTransform-1.1.1a2/src/python/autotransform/repo/github.py`

 * *Files 10% similar despite different names*

```diff
@@ -183,25 +183,45 @@
 
         files = {}
         # Add schema JSON
         if schema is not None:
             files["schema"] = {"content": json.dumps(schema.bundle(), indent=4)}
 
         # Add batch JSON
+        chunk_size = 5000
+        items = batch["items"]
+        item_chunks = [items[i : i + chunk_size] for i in range(0, len(items), chunk_size)]
+        if not item_chunks:
+            item_chunks = [[]]
         encodable_batch: Dict[str, Any] = {
             "title": batch["title"],
-            "items": [item.bundle() for item in batch["items"]],
+            "items": [item.bundle() for item in item_chunks[0]],
         }
         if "metadata" in batch:
             encodable_batch["metadata"] = batch["metadata"]
         files["batch"] = {"content": json.dumps(encodable_batch, indent=4)}
-        gist = GithubUtils.get(self.full_github_name).create_gist(
-            files, description="Automation info for AutoTransform", public=True
+        gists = [
+            GithubUtils.get(self.full_github_name).create_gist(
+                files, description="Automation info for AutoTransform", public=True
+            )
+        ]
+        for i in range(1, len(item_chunks)):
+            item_file = {
+                "items": {
+                    "content": json.dumps([item.bundle() for item in item_chunks[i]], indent=4)
+                }
+            }
+            gists.append(
+                GithubUtils.get(self.full_github_name).create_gist(
+                    item_file, description="Automation info for AutoTransform", public=True
+                )
+            )
+        automation_info_lines.append(
+            f"<<<Automation Info Gist: {'/'.join([gist.gist_id for gist in gists])}>>>"
         )
-        automation_info_lines.append(f"<<<Automation Info Gist: {gist.gist_id}>>>")
 
         return "\n".join(automation_info_lines)
 
     def get_outstanding_changes(self) -> Sequence[GithubChange]:
         """Gets all outstanding pull requests for the Repo.
 
         Returns:
```

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/runner/base.py` & `AutoTransform-1.1.1a2/src/python/autotransform/runner/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/runner/github.py` & `AutoTransform-1.1.1a2/src/python/autotransform/runner/github.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/runner/jenkins.py` & `AutoTransform-1.1.1a2/src/python/autotransform/runner/jenkins.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/runner/local.py` & `AutoTransform-1.1.1a2/src/python/autotransform/runner/local.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/schema/__init__.py` & `AutoTransform-1.1.1a2/src/python/autotransform/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/schema/builder.py` & `AutoTransform-1.1.1a2/src/python/autotransform/schema/builder.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/schema/config.py` & `AutoTransform-1.1.1a2/src/python/autotransform/schema/config.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/schema/schema.py` & `AutoTransform-1.1.1a2/src/python/autotransform/schema/schema.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/scripts/commands/initialize.py` & `AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/initialize.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/scripts/commands/manage.py` & `AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/manage.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/scripts/commands/run.py` & `AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/run.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/scripts/commands/schedule.py` & `AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/schedule.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/scripts/commands/settings.py` & `AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/settings.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/scripts/commands/update.py` & `AutoTransform-1.1.1a2/src/python/autotransform/scripts/commands/update.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/scripts/main.py` & `AutoTransform-1.1.1a2/src/python/autotransform/scripts/main.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/scripts/migrations/p1_0_1.py` & `AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/p1_0_1.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/scripts/migrations/p1_0_3.py` & `AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/p1_0_3.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/scripts/migrations/p1_0_5.py` & `AutoTransform-1.1.1a2/src/python/autotransform/scripts/migrations/p1_0_5.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/action/base.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/action/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/action/comments.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/action/comments.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/action/labels.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/action/labels.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/action/request.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/action/request.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/action/reviewers.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/action/reviewers.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/action/source.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/action/source.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/base.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/condition/aggregate.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/aggregate.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/condition/base.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/condition/comparison.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/comparison.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/condition/created.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/created.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/condition/labels.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/labels.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/condition/request.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/request.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/condition/reviewers.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/reviewers.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/condition/schema.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/schema.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/condition/state.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/state.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/condition/updated.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/condition/updated.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/step/conditional.py` & `AutoTransform-1.1.1a2/src/python/autotransform/step/conditional.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/transformer/base.py` & `AutoTransform-1.1.1a2/src/python/autotransform/transformer/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/transformer/jscodeshift.py` & `AutoTransform-1.1.1a2/src/python/autotransform/transformer/jscodeshift.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/transformer/libcst.py` & `AutoTransform-1.1.1a2/src/python/autotransform/transformer/libcst.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/transformer/regex.py` & `AutoTransform-1.1.1a2/src/python/autotransform/transformer/regex.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/transformer/script.py` & `AutoTransform-1.1.1a2/src/python/autotransform/transformer/script.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/transformer/single.py` & `AutoTransform-1.1.1a2/src/python/autotransform/transformer/single.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/util/cachedfile.py` & `AutoTransform-1.1.1a2/src/python/autotransform/util/cachedfile.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/util/component.py` & `AutoTransform-1.1.1a2/src/python/autotransform/util/component.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/util/console.py` & `AutoTransform-1.1.1a2/src/python/autotransform/util/console.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/util/enums.py` & `AutoTransform-1.1.1a2/src/python/autotransform/util/enums.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/util/functions.py` & `AutoTransform-1.1.1a2/src/python/autotransform/util/functions.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/util/github.py` & `AutoTransform-1.1.1a2/src/python/autotransform/util/github.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/util/manager.py` & `AutoTransform-1.1.1a2/src/python/autotransform/util/manager.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/util/package.py` & `AutoTransform-1.1.1a2/src/python/autotransform/util/package.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/util/request.py` & `AutoTransform-1.1.1a2/src/python/autotransform/util/request.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/util/scheduler.py` & `AutoTransform-1.1.1a2/src/python/autotransform/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/util/schema_map.py` & `AutoTransform-1.1.1a2/src/python/autotransform/util/schema_map.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/validator/base.py` & `AutoTransform-1.1.1a2/src/python/autotransform/validator/base.py`

 * *Files identical despite different names*

### Comparing `AutoTransform-1.1.1a1/src/python/autotransform/validator/script.py` & `AutoTransform-1.1.1a2/src/python/autotransform/validator/script.py`

 * *Files identical despite different names*

