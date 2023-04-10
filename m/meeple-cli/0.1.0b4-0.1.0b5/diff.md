# Comparing `tmp/meeple-cli-0.1.0b4.tar.gz` & `tmp/meeple-cli-0.1.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "meeple-cli-0.1.0b4.tar", last modified: Fri Apr  7 19:59:06 2023, max compression
+gzip compressed data, was "meeple-cli-0.1.0b5.tar", last modified: Mon Apr 10 18:07:10 2023, max compression
```

## Comparing `meeple-cli-0.1.0b4.tar` & `meeple-cli-0.1.0b5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
--rw-r--r--   0        0        0       66 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/.flake8
--rw-r--r--   0        0        0     1146 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     1035 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/.github/workflows/python-test.yml
--rw-r--r--   0        0        0      289 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/.gitignore
--rw-r--r--   0        0        0      168 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/.markdownlint.yaml
--rw-r--r--   0        0        0     1174 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1073 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/LICENSE
--rw-r--r--   0        0        0     6207 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/README.md
--rw-r--r--   0        0        0     4380 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/docs/changelog.md
--rw-r--r--   0        0        0      876 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/justfile
--rw-r--r--   0        0        0     1014 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/pyproject.toml
--rw-r--r--   0        0        0      112 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/__init__.py
--rw-r--r--   0        0        0      639 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/__init__.py
--rw-r--r--   0        0        0     1498 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/add.py
--rw-r--r--   0        0        0     2039 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/collections.py
--rw-r--r--   0        0        0     1052 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/completions.py
--rw-r--r--   0        0        0     1385 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/delete.py
--rw-r--r--   0        0        0     1489 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/drop.py
--rw-r--r--   0        0        0     5040 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/find.py
--rw-r--r--   0        0        0      628 2023-04-07 19:58:57.701596 meeple-cli-0.1.0b4/src/meeple/command/hot.py
--rw-r--r--   0        0        0     1229 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/info.py
--rw-r--r--   0        0        0     3357 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/list.py
--rw-r--r--   0        0        0     2394 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/move.py
--rw-r--r--   0        0        0      658 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/new.py
--rw-r--r--   0        0        0     1158 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/open.py
--rw-r--r--   0        0        0     1179 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/rename.py
--rw-r--r--   0        0        0      966 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/search.py
--rw-r--r--   0        0        0     3403 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/stats.py
--rw-r--r--   0        0        0     2634 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/command/update.py
--rw-r--r--   0        0        0     1153 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/root.py
--rw-r--r--   0        0        0        0 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/type/__init__.py
--rw-r--r--   0        0        0      226 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/type/collection.py
--rw-r--r--   0        0        0     3977 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/type/item.py
--rw-r--r--   0        0        0        0 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/__init__.py
--rw-r--r--   0        0        0     1594 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/api_util.py
--rw-r--r--   0        0        0      697 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/cmd_util.py
--rw-r--r--   0        0        0     2024 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/collection_util.py
--rw-r--r--   0        0        0      235 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/completion_util.py
--rw-r--r--   0        0        0     2596 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/data_util.py
--rw-r--r--   0        0        0      938 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/filter_util.py
--rw-r--r--   0        0        0      652 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/fs_util.py
--rw-r--r--   0        0        0      352 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/input_util.py
--rw-r--r--   0        0        0     2549 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/output_util.py
--rw-r--r--   0        0        0     1538 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/src/meeple/util/sort_util.py
--rw-r--r--   0        0        0        0 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/tests/__init__.py
--rw-r--r--   0        0        0      313 2023-04-07 19:58:57.705596 meeple-cli-0.1.0b4/tests/test_root.py
--rw-r--r--   0        0        0     7207 1970-01-01 00:00:00.000000 meeple-cli-0.1.0b4/PKG-INFO
+-rw-r--r--   0        0        0       66 2023-04-10 18:07:01.108505 meeple-cli-0.1.0b5/.flake8
+-rw-r--r--   0        0        0     1146 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1035 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/.github/workflows/python-test.yml
+-rw-r--r--   0        0        0      289 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/.gitignore
+-rw-r--r--   0        0        0      168 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/.markdownlint.yaml
+-rw-r--r--   0        0        0     1174 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1073 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/LICENSE
+-rw-r--r--   0        0        0     4293 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/README.md
+-rw-r--r--   0        0        0     4834 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/docs/changelog.md
+-rw-r--r--   0        0        0      876 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/justfile
+-rw-r--r--   0        0        0     1014 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/pyproject.toml
+-rw-r--r--   0        0        0      112 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/__init__.py
+-rw-r--r--   0        0        0      639 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/__init__.py
+-rw-r--r--   0        0        0     1498 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/add.py
+-rw-r--r--   0        0        0     1983 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/collections.py
+-rw-r--r--   0        0        0      941 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/completions.py
+-rw-r--r--   0        0        0     1385 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/delete.py
+-rw-r--r--   0        0        0     1489 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/drop.py
+-rw-r--r--   0        0        0     4990 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/find.py
+-rw-r--r--   0        0        0      566 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/hot.py
+-rw-r--r--   0        0        0     1490 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/info.py
+-rw-r--r--   0        0        0     3027 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/list.py
+-rw-r--r--   0        0        0     2394 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/move.py
+-rw-r--r--   0        0        0      658 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/new.py
+-rw-r--r--   0        0        0     1182 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/open.py
+-rw-r--r--   0        0        0     1179 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/rename.py
+-rw-r--r--   0        0        0      848 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/search.py
+-rw-r--r--   0        0        0     3403 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/stats.py
+-rw-r--r--   0        0        0     2634 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/command/update.py
+-rw-r--r--   0        0        0     1153 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/root.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/type/__init__.py
+-rw-r--r--   0        0        0      278 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/type/collection.py
+-rw-r--r--   0        0        0     4385 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/type/item.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/__init__.py
+-rw-r--r--   0        0        0     1450 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/api_util.py
+-rw-r--r--   0        0        0      697 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/cmd_util.py
+-rw-r--r--   0        0        0     2024 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/collection_util.py
+-rw-r--r--   0        0        0      235 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/completion_util.py
+-rw-r--r--   0        0        0     2596 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/data_util.py
+-rw-r--r--   0        0        0      935 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/filter_util.py
+-rw-r--r--   0        0        0      652 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/fs_util.py
+-rw-r--r--   0        0        0      352 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/input_util.py
+-rw-r--r--   0        0        0     2489 2023-04-10 18:07:01.112505 meeple-cli-0.1.0b5/src/meeple/util/output_util.py
+-rw-r--r--   0        0        0     1940 2023-04-10 18:07:01.116505 meeple-cli-0.1.0b5/src/meeple/util/sort_util.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:07:01.116505 meeple-cli-0.1.0b5/tests/__init__.py
+-rw-r--r--   0        0        0      313 2023-04-10 18:07:01.116505 meeple-cli-0.1.0b5/tests/test_root.py
+-rw-r--r--   0        0        0     5293 1970-01-01 00:00:00.000000 meeple-cli-0.1.0b5/PKG-INFO
```

### Comparing `meeple-cli-0.1.0b4/.github/workflows/python-publish.yml` & `meeple-cli-0.1.0b5/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/.github/workflows/python-test.yml` & `meeple-cli-0.1.0b5/.github/workflows/python-test.yml`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/.pre-commit-config.yaml` & `meeple-cli-0.1.0b5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/LICENSE` & `meeple-cli-0.1.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/docs/changelog.md` & `meeple-cli-0.1.0b5/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,31 @@
 The format is based on
 [Keep a Changelog](https://keepachangelog.com/en/1.1.0/ "Keep a Changelog"),
 and this project adheres to
 [Semantic Versioning](https://semver.org/spec/v2.0.0.html "Semantic Versioning").
 
 ## [Unreleased]
 
+## [v0.1.0b5] - 2023-04-10
+
+### Added
+
+- `meeple info`: `-v/--verbose` - Output additional details.
+- `meeple open`: `-y/--yes` - Bypass confirmation.
+- `meeple find`/`meeple list`: `--sort` - Sort output by _time_.
+
+### Changed
+
+- `GENERAL` - Output _Play Time_ values as expected duration instead of a range.
+- `GENERAL` - Update _Time_ column header text to _Play Time_.
+
+### Removed
+
+- `ROADMAP` - Remove roadmap from README. Move to GitHub issues.
+
 ## [v0.1.0b4] - 2023-04-07
 
 ### Added
 
 - `meeple find` - Search collections for board games and expansions.
   - Search in just one, multiple, or all collections at once.
   - `-b/--boardgames` - Output only board games.
```

### Comparing `meeple-cli-0.1.0b4/justfile` & `meeple-cli-0.1.0b5/justfile`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/pyproject.toml` & `meeple-cli-0.1.0b5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/__init__.py` & `meeple-cli-0.1.0b5/src/meeple/command/__init__.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/add.py` & `meeple-cli-0.1.0b5/src/meeple/command/add.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/collections.py` & `meeple-cli-0.1.0b5/src/meeple/command/collections.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,14 @@
             Collection(collection, boardgames, expansions, last_updated(collection))
         )
 
     # sort output
     collection_list = sort_collections(collection_list, sort)
 
     # prepare table data
-    # TODO: add indicator to currently sorted by column
     headers = ["Name"]
     if verbose:
         headers.extend(["Boardgames", "Expansions", "Last Updated"])
 
     rows = []
     for collection in collection_list:
         cols = [collection.name]
```

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/completions.py` & `meeple-cli-0.1.0b5/src/meeple/command/completions.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from meeple.util.output_util import print_info
 
 SHELLS = ["bash", "zsh", "fish"]
 
 
 @click.command()
 @click.argument("shell", type=click.Choice(SHELLS, case_sensitive=False))
-# TODO: add --install option to automatically install completions
-# TODO: add -y option to bypass confirmation
 @click.help_option("-h", "--help")
 def completions(shell: str) -> None:
     """Setup meeple shell completions.
 
     - SHELL is the shell for which to setup completions.
     """
     match shell.lower():
```

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/delete.py` & `meeple-cli-0.1.0b5/src/meeple/command/delete.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/drop.py` & `meeple-cli-0.1.0b5/src/meeple/command/drop.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/find.py` & `meeple-cli-0.1.0b5/src/meeple/command/find.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     fmt_rating,
     fmt_type,
     fmt_weight,
     fmt_year,
     print_error,
     print_table,
 )
-from meeple.util.sort_util import sort_items
+from meeple.util.sort_util import ITEM_SORT_KEYS, sort_items
 
 
 @click.command()
 @click.argument("collections", nargs=-1, shell_complete=complete_collections)
 @click.option(
     "-b",
     "--boardgames",
@@ -42,17 +42,15 @@
 @click.option(
     "--players",
     type=int,
     help="Output only board games/expansions that support the provided player count.",
 )
 @click.option(
     "--sort",
-    type=click.Choice(
-        ["rank", "rating", "weight", "year", "name", "id"], case_sensitive=False
-    ),
+    type=click.Choice(ITEM_SORT_KEYS, case_sensitive=False),
     default="rating",
     show_default=True,
     help="Sort output by the provided column.",
 )
 @click.option(
     "--max-time",
     type=int,
@@ -121,15 +119,15 @@
     if item_type not in ("bg", "ex"):
         headers.append("Type")
     # include collections column if more than one collection was included
     if len(collections) > 1:
         headers.append("Collection(s)")
     # include additional columns if verbose flag present
     if verbose:
-        headers.extend(["Year", "Rank", "Rating", "Weight", "Players", "Time"])
+        headers.extend(["Year", "Rank", "Rating", "Weight", "Players", "Play Time"])
 
     # prepare table data
     rows = []
     for item in result_items:
         cols = [str(item.id), item.name]
         # include type data if neither type is ommitted
         if item_type not in ("bg", "ex"):
@@ -150,13 +148,13 @@
             cols.extend(
                 [
                     fmt_year(item.year),
                     fmt_rank(item.rank),
                     fmt_rating(item.rating),
                     fmt_weight(item.weight),
                     fmt_players(item.minplayers, item.maxplayers),
-                    fmt_playtime(item.minplaytime, item.maxplaytime),
+                    fmt_playtime(item.playtime),
                 ]
             )
         rows.append(cols)
 
     print_table(rows, headers)
```

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/info.py` & `meeple-cli-0.1.0b5/src/meeple/command/info.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,16 +13,17 @@
     print_error,
     print_table,
 )
 
 
 @click.command()
 @click.argument("id", type=int)
+@click.option("-v", "--verbose", is_flag=True, help="Output additional details.")
 @click.help_option("-h", "--help")
-def info(id: int) -> None:
+def info(id: int, verbose: bool) -> None:
     """Print out the details of an item.
 
     - ID is the BoardGameGeek ID of the board game/expansion to be detailed.
     """
     # check that the given id is a valid one
     bgg_id = id
     bgg_item = get_bgg_item(bgg_id)
@@ -33,13 +34,20 @@
         [
             f"Rating: {fmt_rating(bgg_item.rating)}",
             f"Players: {fmt_players(bgg_item.minplayers, bgg_item.maxplayers)}",
             f"Min Age: {bgg_item.minage}",
         ],
         [
             f"Rank: {fmt_rank(bgg_item.rank)}",
-            f"Time: {fmt_playtime(bgg_item.minplaytime, bgg_item.maxplaytime)}",
+            f"Play Time: {fmt_playtime(bgg_item.playtime)}",
             f"Weight: {fmt_weight(bgg_item.weight)}",
         ],
     ]
     print_table([[f"{bgg_item.id}", f"{bgg_item.name} ({fmt_year(bgg_item.year)})"]])
     print_table(info_rows, lines=True)
+    # include additional data if verbose flag present
+    if verbose:
+        print_table(
+            [
+                ["Description", bgg_item.description],
+            ]
+        )
```

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/list.py` & `meeple-cli-0.1.0b5/src/meeple/command/list.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     fmt_rating,
     fmt_weight,
     fmt_year,
     print_error,
     print_table,
     print_warning,
 )
-from meeple.util.sort_util import sort_items
+from meeple.util.sort_util import ITEM_SORT_KEYS, sort_items
 
 
 @click.command(name="list")
 @click.argument("collection", shell_complete=complete_collections)
 @click.option(
     "-b",
     "--boardgames",
@@ -35,26 +35,22 @@
     "item_type",
     is_flag=True,
     flag_value="ex",
     help="Output only expansions.",
 )
 @click.option(
     "--sort",
-    type=click.Choice(
-        ["rank", "rating", "weight", "year", "name", "id"], case_sensitive=False
-    ),
+    type=click.Choice(ITEM_SORT_KEYS, case_sensitive=False),
     default="rating",
     show_default=True,
     help="Sort output by the provided column.",
 )
 @click.option("-v", "--verbose", is_flag=True, help="Output additional details.")
 @click.help_option("-h", "--help")
-# TODO: add option to run update on the collection prior to list
 # TODO: add option to show grid lines or not in the table
-# TODO: implement paging/scrolling for long lists? not sure how rich will like that
 def list_collection(collection: str, item_type: str, sort: str, verbose: bool) -> None:
     """List contents of a collection.
 
     - COLLECTION is the name of the collection to be listed.
     """
     # check that the given collection is a valid collection
     if not is_collection(collection):
@@ -78,32 +74,30 @@
     else:
         out_list = boardgames + expansions
 
     # sort output
     out_list = sort_items(out_list, sort)
 
     # prepare table data
-    # TODO: add indicator to currently sorted by column
     headers = ["ID", "Name"]
     if verbose:
-        headers.extend(["Year", "Rank", "Rating", "Weight", "Players", "Time"])
+        headers.extend(["Year", "Rank", "Rating", "Weight", "Players", "Play Time"])
 
     rows = []
     for item in out_list:
         cols = [str(item.id), item.name]
         # include additional data if the user chose verbose output
         if verbose:
             cols.extend(
                 [
                     fmt_year(item.year),
                     fmt_rank(str(item.rank)),
                     fmt_rating(item.rating),
                     fmt_weight(item.weight),
                     fmt_players(item.minplayers, item.maxplayers),
-                    fmt_playtime(item.minplaytime, item.maxplaytime),
+                    fmt_playtime(item.playtime),
                 ]
             )
 
         rows.append(cols)
 
-    # TODO: add "Showing all ___ in ___ collection." printout above table?
     print_table(rows, headers)
```

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/move.py` & `meeple-cli-0.1.0b5/src/meeple/command/move.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/new.py` & `meeple-cli-0.1.0b5/src/meeple/command/new.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/rename.py` & `meeple-cli-0.1.0b5/src/meeple/command/rename.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/search.py` & `meeple-cli-0.1.0b5/src/meeple/command/search.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,16 +3,14 @@
 from meeple.util.api_util import search_bgg
 from meeple.util.output_util import fmt_year, print_table
 
 
 @click.command()
 @click.argument("query")
 @click.help_option("-h", "--help")
-# TODO: add option to sort output by different columns
-# TODO: add verbosity flag to show more info about each result
 def search(query: str) -> None:
     """Search BoardGameGeek for items.
 
     - QUERY is the text to be searched for on BoardGameGeek. If searching multiple words, surround with quotes.
     """
     # search BoardGameGeek with user provided query
     api_result = search_bgg(query)
```

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/stats.py` & `meeple-cli-0.1.0b5/src/meeple/command/stats.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/command/update.py` & `meeple-cli-0.1.0b5/src/meeple/command/update.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/root.py` & `meeple-cli-0.1.0b5/src/meeple/root.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/util/api_util.py` & `meeple-cli-0.1.0b5/src/meeple/util/api_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -40,12 +40,10 @@
 
 
 def get_bgg_hot() -> List[Item]:
     url = f"{API2_BASE_URL}/hot?type={BOARDGAME_TYPE}"
     return _bgg_api_get_items(url)
 
 
-# TODO: figure out how to allow user to only search for board games or expansions
-# current api returns both as board game type for some reason
 def search_bgg(query: str) -> List[Item]:
     url = f"{API2_BASE_URL}/search?type={BOARDGAME_TYPE}&query={query}"
     return _bgg_api_get_items(url)
```

### Comparing `meeple-cli-0.1.0b4/src/meeple/util/cmd_util.py` & `meeple-cli-0.1.0b5/src/meeple/util/cmd_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/util/collection_util.py` & `meeple-cli-0.1.0b5/src/meeple/util/collection_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/util/data_util.py` & `meeple-cli-0.1.0b5/src/meeple/util/data_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/util/filter_util.py` & `meeple-cli-0.1.0b5/src/meeple/util/filter_util.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         and int(item.maxplayers) >= players,
         item_list,
     )
 
 
 def filterby_playtime(item_list: [Item], max_time: int) -> [Item]:
     return filter(
-        lambda item: int(item.maxplaytime) <= max_time,
+        lambda item: int(item.playtime) <= max_time,
         item_list,
     )
 
 
 def filterby_weight(item_list: [Item], weight_key: str) -> [Item]:
     min_weight, max_weight = _weight_range(int(weight_key))
     return filter(
```

### Comparing `meeple-cli-0.1.0b4/src/meeple/util/fs_util.py` & `meeple-cli-0.1.0b5/src/meeple/util/fs_util.py`

 * *Files identical despite different names*

### Comparing `meeple-cli-0.1.0b4/src/meeple/util/output_util.py` & `meeple-cli-0.1.0b5/src/meeple/util/output_util.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 def fmt_players(minplayers: str, maxplayers: str) -> str:
     if int(minplayers) == int(maxplayers) == 0:
         return NA
     return f"{minplayers}-{maxplayers}"
 
 
-def fmt_playtime(minplaytime: str, maxplaytime: str) -> str:
-    if int(minplaytime) == int(maxplaytime) == 0:
+def fmt_playtime(playtime: str) -> str:
+    if int(playtime) == 0:
         return NA
-    return f"{minplaytime}-{maxplaytime} Min"
+    return f"~{playtime} Min"
 
 
 def fmt_avg_rank(rank: str) -> str:
     if not isinstance(rank, numbers.Number) or int(rank) == 0:
         return NA
     rank_str = f"{rank:.2f}"
     return rank_str
```

### Comparing `meeple-cli-0.1.0b4/src/meeple/util/sort_util.py` & `meeple-cli-0.1.0b5/src/meeple/util/sort_util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from meeple.type.collection import Collection
 from meeple.type.item import Item
 
+ITEM_SORT_KEYS = ["rank", "rating", "weight", "year", "name", "id", "time"]
+
 
 def _handle_str_rank(item: Item):
     try:
         return int(item.rank)
     except ValueError:
         return float("inf")
 
@@ -29,19 +31,30 @@
         collection_list,
         key=lambda collection: collection.last_updated,
         reverse=True,
     )
 
 
 def sort_items(item_list: [Item], sort_key: str) -> [Item]:
+    """Sort the given item list by the given key. Defaults to sort by rating.
+
+    Args:
+        item_list (Item]): list of Items.
+        sort_key (str): key to sort by.
+
+    Returns:
+        [Item]: sorted list of Item.
+    """
     match sort_key:
         case "rank":
             return sorted(item_list, key=_handle_str_rank)
         case "weight":
             return sorted(item_list, key=lambda item: item.weight, reverse=True)
         case "year":
             return sorted(item_list, key=lambda item: item.year)
         case "name":
             return sorted(item_list, key=lambda item: item.name)
         case "id":
             return sorted(item_list, key=lambda item: int(item.id))
+        case "time":
+            return sorted(item_list, key=lambda item: int(item.playtime))
     return sorted(item_list, key=lambda item: item.rating, reverse=True)
```

### Comparing `meeple-cli-0.1.0b4/PKG-INFO` & `meeple-cli-0.1.0b5/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: meeple-cli
-Version: 0.1.0b4
+Version: 0.1.0b5
 Summary: Local board game collection manager. Powered by BoardGameGeek.
 Author-email: Bradley Wojcik <bradleycwojcik@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: click >=8
 Requires-Dist: rich >=13
@@ -35,17 +35,15 @@
 
 <!-- [![codecov](https://codecov.io/gh/boldandbrad/meeple-cli/branch/main/graph/badge.svg)](https://codecov.io/gh/boldandbrad/meeple-cli) -->
 <!-- [![Docs](https://img.shields.io/website?down_message=down&label=docs&up_message=online&url=https%3A%2F%2Fboldandbrad.github.io%2Fmeeple-cli%2F)](https://boldandbrad.github.io/meeple-cli/) -->
 
 **Local board game collection manager. Powered by
 [BoardGameGeek](https://boardgamegeek.com).**
 
-## Disclaimer
-
-> Neither `meeple-cli` nor its maintainers are affiliated with
+> Disclaimer: Neither `meeple-cli` nor its maintainers are affiliated with
 > [BoardGameGeek](https://boardgamegeek.com).
 
 ## Install
 
 Global isolated install via [pipx](https://pypa.github.io/pipx/) (recommended):
 
 ```sh
@@ -54,14 +52,16 @@
 
 Local python environment install:
 
 ```sh
 pip install meeple-cli
 ```
 
+<!-- Homebrew install: -->
+
 <!-- ```zsh
 brew tap boldandbrad/homebrew-tap
 brew install meeple-cli
 ```-->
 
 <!-- > For more details, read the **meeple-cli**
 > [install guide](https://boldandbrad.github.io/meeple-cli/#/install). -->
@@ -138,62 +138,23 @@
 
 ```sh
 _MEEPLE_COMPLETE=fish_source meeple > ~/.config/fish/completions/meeple.fish
 ```
 
 </details>
 
-## Roadmap
+## Changelog
 
-See a list of already implemented features/changes in the
+See a history of implemented features/changes in the
 [Changelog](docs/changelog.md).
 
-### Planned Features
+## Roadmap
 
-- [ ] Verbose option on `meeple info` that includes additional info such as
-      description, publishers, etc
-- [ ] Export a collection to csv or another format -> `meeple export`
-- [ ] Import a collection from a variety of formats -> `meeple import`
-
-### Potential Features (May or may not happen)
-
-- [ ] Ability to assign and manage personal ratings of board games/expansions
-- [ ] Copy a collection -> `meeple copy`
-- [ ] Copy option `-c` on most commands that allows you to interactively select
-      and copy text from the command output (for grabbing IDs) - similar to yank
-- [ ] Manage user preferences/configs -> `meeple config` stored at
-      `~/.meeple/config.json` or something
-  - [ ] Toggle colorized output
-  - [ ] Set custom default output sorts
-  - [ ] Set custom data location
-- [ ] Show elegant data diffs on `meeple update` (individual board game stat
-      changes/collection stat changes)
-- [ ] Output pagination for long lists?
-  - [ ] Ability to display only a given number of output rows
-- [ ] Identify when changes have been made to a collection and an update has not
-      occurred yet
-- [ ] Service or job that runs once a day to automatically update local data
-  - [ ] Ability to output graphs/visuals to show change in collections over time
-  - [ ] Ability to output graphs/visuals to show a board game's changes on
-        BoardGameGeek over time
-- [ ] Ability to record and manage plays of board games - would be nuts.
-  - [ ] Ability to calculate and surface play statistics for a board game
-- [ ] Ability to interact with discord services to show that you are currently
-      playing a board game?
-- [ ] Ability to actually interact with BoardGameGeek user
-      profile/settings/collections (not all currently possible via the API)
-
-### Other Todos
-
-- [ ] Unit tests
-- [ ] Documentation site (via vitepress?)
-- [ ] Homebrew formula (will be available
-      [here](https://github.com/boldandbrad/homebrew-tap))
-- [ ] Implement simple logging for debugging (local, not telemetry) (via
-      loguru?)
+See a list of planned features and milestones
+[here](https://github.com/boldandbrad/meeple-cli/milestones).
 
 ## FAQ
 
 ### Why local only collections?
 
 Currently, the
 [BoardGameGeek Public API](https://boardgamegeek.com/wiki/page/BGG_XML_API2)
```

