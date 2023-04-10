# Comparing `tmp/petljadoc-1.3.0.tar.gz` & `tmp/petljadoc-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petljadoc-1.3.0.tar", last modified: Mon Mar  6 12:48:51 2023, max compression
+gzip compressed data, was "petljadoc-1.3.1.tar", last modified: Mon Apr 10 05:44:09 2023, max compression
```

## Comparing `petljadoc-1.3.0.tar` & `petljadoc-1.3.1.tar`

### file list

```diff
@@ -1,969 +1,969 @@
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:51.051372 petljadoc-1.3.0/
--rw-rw-rw-   0        0        0     1084 2019-09-29 18:46:11.000000 petljadoc-1.3.0/LICENSE
--rw-rw-rw-   0        0        0      475 2022-11-20 11:14:54.000000 petljadoc-1.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2389 2023-03-06 12:48:51.050373 petljadoc-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     1803 2022-11-06 13:07:30.000000 petljadoc-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.325355 petljadoc-1.3.0/petljadoc/
--rw-rw-rw-   0        0        0       67 2023-03-06 12:31:02.000000 petljadoc-1.3.0/petljadoc/__init__.py
--rw-rw-rw-   0        0        0       39 2020-12-07 14:32:36.000000 petljadoc-1.3.0/petljadoc/__main__.py
--rw-rw-rw-   0        0        0    43045 2023-03-06 12:31:02.000000 petljadoc-1.3.0/petljadoc/cli.py
--rw-rw-rw-   0        0        0    15820 2023-03-06 12:31:02.000000 petljadoc-1.3.0/petljadoc/course.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.241356 petljadoc-1.3.0/petljadoc/nb-templates/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.349355 petljadoc-1.3.0/petljadoc/nb-templates/classic2/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.355358 petljadoc-1.3.0/petljadoc/nb-templates/classic2/base/
--rw-rw-rw-   0        0        0     7752 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/nb-templates/classic2/base/base.html.j2
--rw-rw-rw-   0        0        0      220 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/nb-templates/classic2/base/celltags.j2
--rw-rw-rw-   0        0        0     1634 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/nb-templates/classic2/base/display_priority.j2
--rw-rw-rw-   0        0        0      993 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/nb-templates/classic2/base/jupyter_widgets.html.j2
--rw-rw-rw-   0        0        0     1386 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/nb-templates/classic2/base/mathjax.html.j2
--rw-rw-rw-   0        0        0     6340 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/nb-templates/classic2/base/null.j2
--rw-rw-rw-   0        0        0      401 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/nb-templates/classic2/index.html.j2
--rw-rw-rw-   0        0        0    40964 2023-03-06 12:31:02.000000 petljadoc-1.3.0/petljadoc/package.py
--rw-rw-rw-   0        0        0     2282 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/petlja_builder.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.245355 petljadoc-1.3.0/petljadoc/project-templates/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.387374 petljadoc-1.3.0/petljadoc/project-templates/course/
--rw-rw-rw-   0        0        0      142 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/project-templates/course/.t.gitignore
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.388374 petljadoc-1.3.0/petljadoc/project-templates/course/_images/
--rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.0/petljadoc/project-templates/course/_images/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.389373 petljadoc-1.3.0/petljadoc/project-templates/course/_includes/
--rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.0/petljadoc/project-templates/course/_includes/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.389373 petljadoc-1.3.0/petljadoc/project-templates/course/_sources/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.391374 petljadoc-1.3.0/petljadoc/project-templates/course/_sources/1_Lesson/
--rw-rw-rw-   0        0        0     2096 2020-11-30 16:13:38.000000 petljadoc-1.3.0/petljadoc/project-templates/course/_sources/1_Lesson/intro.rst
--rw-rw-rw-   0        0        0     1564 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/project-templates/course/_sources/1_Lesson/quiz.rst
--rw-rw-rw-   0        0        0     1368 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/project-templates/course/_sources/index.t.yaml
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.391374 petljadoc-1.3.0/petljadoc/project-templates/course/_static/
--rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.0/petljadoc/project-templates/course/_static/.gitkeep
--rw-rw-rw-   0        0        0       75 2023-03-06 12:31:02.000000 petljadoc-1.3.0/petljadoc/project-templates/course/conf-petljadoc.t.json
--rw-rw-rw-   0        0        0     6291 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/project-templates/course/conf.t.py
--rw-rw-rw-   0        0        0       33 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/project-templates/course/package-conf.json
--rw-rw-rw-   0        0        0      777 2020-12-09 14:48:07.000000 petljadoc-1.3.0/petljadoc/project-templates/course/pavement.t.py
--rw-rw-rw-   0        0        0      110 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/project-templates/course/template_settings.t.json
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.394372 petljadoc-1.3.0/petljadoc/project-templates/runestone/
--rw-rw-rw-   0        0        0       56 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/.t.gitignore
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.395373 petljadoc-1.3.0/petljadoc/project-templates/runestone/_images/
--rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_images/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.395373 petljadoc-1.3.0/petljadoc/project-templates/runestone/_includes/
--rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_includes/.gitkeep
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.396372 petljadoc-1.3.0/petljadoc/project-templates/runestone/_sources/
--rw-rw-rw-   0        0        0       90 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_sources/index-item.t.md
--rw-rw-rw-   0        0        0     3337 2020-11-30 16:13:38.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_sources/index.rst
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.404374 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/
--rw-rw-rw-   0        0        0        0 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/.gitignore
--rw-rw-rw-   0        0        0    92708 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/activecodethumb.png
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.410372 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/audio/
--rw-rw-rw-   0        0        0    87168 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.mp3
--rw-rw-rw-   0        0        0   273068 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.wav
--rw-rw-rw-   0        0        0   115328 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.mp3
--rw-rw-rw-   0        0        0   361772 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.wav
--rw-rw-rw-   0        0        0   310985 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.mp3
--rw-rw-rw-   0        0        0   978092 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.wav
--rw-rw-rw-   0        0        0    23942 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/clock.png
--rw-rw-rw-   0        0        0     4497 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/close.png
--rw-rw-rw-   0        0        0    16165 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/first.png
--rw-rw-rw-   0        0        0    15899 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/last.png
--rw-rw-rw-   0        0        0    15743 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/next.png
--rw-rw-rw-   0        0        0    15344 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/pause.png
--rw-rw-rw-   0        0        0    15719 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/prev.png
--rw-rw-rw-   0        0        0       75 2023-03-06 12:31:02.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/conf-petljadoc.t.json
--rw-rw-rw-   0        0        0    10633 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/conf.t.py
--rw-rw-rw-   0        0        0      770 2020-12-09 14:48:07.000000 petljadoc-1.3.0/petljadoc/project-templates/runestone/pavement.t.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.412373 petljadoc-1.3.0/petljadoc/runestone_ext/
--rw-rw-rw-   0        0        0     1782 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/runestone_ext/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.413374 petljadoc-1.3.0/petljadoc/runestone_ext/associations/
--rw-rw-rw-   0        0        0       29 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/associations/__init__.py
--rw-rw-rw-   0        0        0     4629 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/runestone_ext/associations/associations.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.414373 petljadoc-1.3.0/petljadoc/runestone_ext/associations/css/
--rw-rw-rw-   0        0        0     3204 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/associations/css/associations.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.419376 petljadoc-1.3.0/petljadoc/runestone_ext/associations/js/
--rw-rw-rw-   0        0        0      147 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/associations/js/associations-i18n.en.js
--rw-rw-rw-   0        0        0      164 2022-11-06 13:07:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/associations/js/associations-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0      144 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/associations/js/associations-i18n.sr-Latn.js
--rw-rw-rw-   0        0        0      159 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/associations/js/associations-i18n.sr.js
--rw-rw-rw-   0        0        0     5682 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/associations/js/associations.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.420376 petljadoc-1.3.0/petljadoc/runestone_ext/audio/
--rw-rw-rw-   0        0        0       20 2019-12-21 09:53:52.000000 petljadoc-1.3.0/petljadoc/runestone_ext/audio/__init__.py
--rw-rw-rw-   0        0        0     1297 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/audio/audio.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.421373 petljadoc-1.3.0/petljadoc/runestone_ext/audio/test/
--rw-rw-rw-   0        0        0        0 2019-12-21 09:53:52.000000 petljadoc-1.3.0/petljadoc/runestone_ext/audio/test/sphinx-enki-info.txt
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.422372 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/
--rw-rw-rw-   0        0        0       27 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/__init__.py
--rw-rw-rw-   0        0        0     6947 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/blocklykarel.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.423375 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/css/
--rw-rw-rw-   0        0        0     2065 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/css/karelBlockly.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.429373 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/
--rw-rw-rw-   0        0        0    80180 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/acorn_interpreter.js
--rw-rw-rw-   0        0        0   929342 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/blockly_compressed.js
--rw-rw-rw-   0        0        0    90975 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/blocks_compressed.js
--rw-rw-rw-   0        0        0    46593 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/javascript_compressed.js
--rw-rw-rw-   0        0        0    17846 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/karelBlockly.js
--rw-rw-rw-   0        0        0    10007 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/karelBlocks.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.430373 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/msg/
--rw-rw-rw-   0        0        0    32475 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/msg/en.js
--rw-rw-rw-   0        0        0    40621 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/msg/sr.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.432373 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/
--rw-rw-rw-   0        0        0       25 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/__init__.py
--rw-rw-rw-   0        0        0     1299 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/blockpylib.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.433375 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.438374 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockly/
--rw-rw-rw-   0        0        0   683169 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockly/blockly_compressed.js
--rw-rw-rw-   0        0        0    92505 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockly/blocks_compressed.js
--rw-rw-rw-   0        0        0    61781 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockly/msg-sr.js
--rw-rw-rw-   0        0        0    40010 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockly/python_compressed.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.444374 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/
--rw-rw-rw-   0        0        0    35053 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter.js
--rw-rw-rw-   0        0        0     6384 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter_definitions.js
--rw-rw-rw-   0        0        0     3736 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/ast_node_visitor.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.456374 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/
--rw-rw-rw-   0        0        0     1888 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/class.js
--rw-rw-rw-   0        0        0     2178 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comment.js
--rw-rw-rw-   0        0        0     1116 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comprehensions.js
--rw-rw-rw-   0        0        0      522 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/decorator.js
--rw-rw-rw-   0        0        0     3777 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/dict.js
--rw-rw-rw-   0        0        0     7891 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/if.js
--rw-rw-rw-   0        0        0     1922 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/io.js
--rw-rw-rw-   0        0        0    12589 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/lists.js
--rw-rw-rw-   0        0        0     1799 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/loops.js
--rw-rw-rw-   0        0        0     8787 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/parking.js
--rw-rw-rw-   0        0        0      609 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/plots.js
--rw-rw-rw-   0        0        0     1718 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/sets.js
--rw-rw-rw-   0        0        0     1263 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/text.js
--rw-rw-rw-   0        0        0     1831 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/tuple.js
--rw-rw-rw-   0        0        0     6969 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/turtles.js
--rw-rw-rw-   0        0        0     4701 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/imported.js
--rw-rw-rw-   0        0        0     7255 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/python_errors.js
--rw-rw-rw-   0        0        0    51813 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/python_to_blockly.js
--rw-rw-rw-   0        0        0    59429 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/pytifa.js
--rw-rw-rw-   0        0        0     8165 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/utilities.js
--rw-rw-rw-   0        0        0     9503 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy-modal.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.253358 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/test/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.253358 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/test/_templates/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.253358 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.254355 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.457373 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.255356 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.458373 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
--rw-rw-rw-   0        0        0    97346 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.459374 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
--rw-rw-rw-   0        0        0    27731 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
--rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.460373 petljadoc-1.3.0/petljadoc/runestone_ext/dbDirective/
--rw-rw-rw-   0        0        0       28 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/dbDirective/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.461374 petljadoc-1.3.0/petljadoc/runestone_ext/dbDirective/css/
--rw-rw-rw-   0        0        0     2423 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/dbDirective/css/dbDirective.css
--rw-rw-rw-   0        0        0     4636 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/runestone_ext/dbDirective/dbDirective.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.462373 petljadoc-1.3.0/petljadoc/runestone_ext/dbDirective/js/
--rw-rw-rw-   0        0        0    16828 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/runestone_ext/dbDirective/js/dbDirective.js
--rw-rw-rw-   0        0        0    48501 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/dbDirective/js/sql.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.465375 petljadoc-1.3.0/petljadoc/runestone_ext/editor/
--rw-rw-rw-   0        0        0       21 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/editor/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.466373 petljadoc-1.3.0/petljadoc/runestone_ext/editor/css/
--rw-rw-rw-   0        0        0     1771 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/editor/css/editor.css
--rw-rw-rw-   0        0        0     5287 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/runestone_ext/editor/editor.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.470373 petljadoc-1.3.0/petljadoc/runestone_ext/editor/js/
--rw-rw-rw-   0        0        0       72 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/editor/js/editor-i18n.en.js
--rw-rw-rw-   0        0        0      102 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/editor/js/editor-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0       88 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/editor/js/editor-i18n.sr-Latn.js
--rw-rw-rw-   0        0        0       97 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/editor/js/editor-i18n.sr.js
--rw-rw-rw-   0        0        0    10712 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/editor/js/editor.js
--rw-rw-rw-   0        0        0   385745 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/editor/js/jszip.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.472373 petljadoc-1.3.0/petljadoc/runestone_ext/gallery/
--rw-rw-rw-   0        0        0       24 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/gallery/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.473374 petljadoc-1.3.0/petljadoc/runestone_ext/gallery/css/
--rw-rw-rw-   0        0        0      589 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/gallery/css/gallery.css
--rw-rw-rw-   0        0        0     4012 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/runestone_ext/gallery/gallery.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.473374 petljadoc-1.3.0/petljadoc/runestone_ext/gallery/js/
--rw-rw-rw-   0        0        0     2096 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/gallery/js/gallery.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.474372 petljadoc-1.3.0/petljadoc/runestone_ext/karel/
--rw-rw-rw-   0        0        0       20 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.475374 petljadoc-1.3.0/petljadoc/runestone_ext/karel/css/
--rw-rw-rw-   0        0        0     1080 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/css/karel.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.484377 petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/
--rw-rw-rw-   0        0        0      438 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karel-i18n.en.js
--rw-rw-rw-   0        0        0      557 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karel-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0      560 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karel-i18n.sr.js
--rw-rw-rw-   0        0        0     3676 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karel.js
--rw-rw-rw-   0        0        0     1689 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karelChat.js
--rw-rw-rw-   0        0        0     1105 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karelCorner.js
--rw-rw-rw-   0        0        0     6683 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karelRobot.js
--rw-rw-rw-   0        0        0    14438 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karelRobotDrawer.js
--rw-rw-rw-   0        0        0     9995 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karelUI.js
--rw-rw-rw-   0        0        0     4647 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karelWorld.js
--rw-rw-rw-   0        0        0     5241 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/karel.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.485372 petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.262355 petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/_templates/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.262355 petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.262355 petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.485372 petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.263358 petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.486373 petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
--rw-rw-rw-   0        0        0    97346 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.487372 petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
--rw-rw-rw-   0        0        0    27731 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
--rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
--rw-rw-rw-   0        0        0        0 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/sphinx-enki-info.txt
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.488374 petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/
--rw-rw-rw-   0        0        0       24 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.489372 petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/css/
--rw-rw-rw-   0        0        0     3729 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/css/nimgame.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.492374 petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/js/
--rw-rw-rw-   0        0        0      406 2022-11-06 13:07:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.en.js
--rw-rw-rw-   0        0        0      565 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0      455 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr-Latn.js
--rw-rw-rw-   0        0        0      560 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr.js
--rw-rw-rw-   0        0        0    13205 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/js/nimgame.js
--rw-rw-rw-   0        0        0     4655 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/nimgame.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.494373 petljadoc-1.3.0/petljadoc/runestone_ext/notes/
--rw-rw-rw-   0        0        0       20 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.495376 petljadoc-1.3.0/petljadoc/runestone_ext/notes/css/
--rw-rw-rw-   0        0        0     3334 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/css/notes.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.496372 petljadoc-1.3.0/petljadoc/runestone_ext/notes/js/
--rw-rw-rw-   0        0        0     1101 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/js/notes.js
--rw-rw-rw-   0        0        0     5293 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/notes.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.497373 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.267356 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/_templates/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.267356 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.268355 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.497373 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.269356 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.498373 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
--rw-rw-rw-   0        0        0    97346 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.499374 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
--rw-rw-rw-   0        0        0    27731 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
--rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.269356 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.500372 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.501373 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_sources/
--rw-rw-rw-   0        0        0      265 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.614377 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/
--rw-rw-rw-   0        0        0     6355 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/Blob.js
--rw-rw-rw-   0        0        0     5120 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/FileSaver.min.js
--rw-rw-rw-   0        0        0     1511 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/LICENSE.txt
--rw-rw-rw-   0        0        0     3439 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibility.css
--rw-rw-rw-   0        0        0     3445 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitydarkest.css
--rw-rw-rw-   0        0        0     2669 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitylight.css
--rw-rw-rw-   0        0        0     9490 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.en.js
--rw-rw-rw-   0        0        0    14677 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0     2096 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.css
--rw-rw-rw-   0        0        0   103165 2020-02-25 19:14:39.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.js
--rw-rw-rw-   0        0        0     3903 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/animationbase.js
--rw-rw-rw-   0        0        0    10912 2020-03-17 13:54:33.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/basic.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.618373 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/
--rw-rw-rw-   0        0        0   683169 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blockly_compressed.js
--rw-rw-rw-   0        0        0    92505 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blocks_compressed.js
--rw-rw-rw-   0        0        0    61781 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/msg-sr.js
--rw-rw-rw-   0        0        0    40010 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/python_compressed.js
--rw-rw-rw-   0        0        0   471577 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly_compressed.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.626372 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/
--rw-rw-rw-   0        0        0    35053 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter.js
--rw-rw-rw-   0        0        0     6384 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter_definitions.js
--rw-rw-rw-   0        0        0     3736 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/ast_node_visitor.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.636373 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/
--rw-rw-rw-   0        0        0     1888 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/class.js
--rw-rw-rw-   0        0        0     2178 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comment.js
--rw-rw-rw-   0        0        0     1116 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comprehensions.js
--rw-rw-rw-   0        0        0      522 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/decorator.js
--rw-rw-rw-   0        0        0     3777 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/dict.js
--rw-rw-rw-   0        0        0     7891 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/if.js
--rw-rw-rw-   0        0        0     1922 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/io.js
--rw-rw-rw-   0        0        0    12589 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/lists.js
--rw-rw-rw-   0        0        0     1799 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/loops.js
--rw-rw-rw-   0        0        0     8787 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/parking.js
--rw-rw-rw-   0        0        0      609 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/plots.js
--rw-rw-rw-   0        0        0     1718 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/sets.js
--rw-rw-rw-   0        0        0     1263 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/text.js
--rw-rw-rw-   0        0        0     1831 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/tuple.js
--rw-rw-rw-   0        0        0     6969 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/turtles.js
--rw-rw-rw-   0        0        0     4701 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/imported.js
--rw-rw-rw-   0        0        0     7255 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_errors.js
--rw-rw-rw-   0        0        0    51813 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_to_blockly.js
--rw-rw-rw-   0        0        0    59429 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/pytifa.js
--rw-rw-rw-   0        0        0     8165 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/utilities.js
--rw-rw-rw-   0        0        0     9298 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy-modal.js
--rw-rw-rw-   0        0        0    55934 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blocks_compressed.js
--rw-rw-rw-   0        0        0    10606 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bookfuncs.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.272355 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.637373 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/css/
--rw-rw-rw-   0        0        0   144838 2022-02-03 12:41:00.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.641373 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/
--rw-rw-rw-   0        0        0    67698 2022-02-03 12:41:15.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0    48907 2022-02-03 12:41:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.min.js
--rw-rw-rw-   0        0        0      425 2020-03-17 13:54:33.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-sphinx.css
--rw-rw-rw-   0        0        0     3776 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-sphinx.js
--rw-rw-rw-   0        0        0    97348 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap.min.css
--rw-rw-rw-   0        0        0     1123 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.css
--rw-rw-rw-   0        0        0    16404 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.js
--rw-rw-rw-   0        0        0    18265 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clike.js
--rw-rw-rw-   0        0        0     2037 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codelens.js
--rw-rw-rw-   0        0        0     7507 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.css
--rw-rw-rw-   0        0        0   320980 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.641373 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css/
--rw-rw-rw-   0        0        0    31004 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css/font-awesome.min.css
--rw-rw-rw-   0        0        0    32373 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css.js
--rw-rw-rw-   0        0        0   111549 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/d3.v2.min.js
--rw-rw-rw-   0        0        0       95 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/datafile.css
--rw-rw-rw-   0        0        0     3000 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/datafile.js
--rw-rw-rw-   0        0        0    19241 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/diff_match_patch.js
--rw-rw-rw-   0        0        0     6868 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/doctools.js
--rw-rw-rw-   0        0        0      306 2020-03-17 13:54:33.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/documentation_options.js
--rw-rw-rw-   0        0        0      310 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop-i18n.en.js
--rw-rw-rw-   0        0        0      394 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0     1480 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.css
--rw-rw-rw-   0        0        0    18311 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.js
--rw-rw-rw-   0        0        0     1756 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/external.css
--rw-rw-rw-   0        0        0      130 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb-i18n.en.js
--rw-rw-rw-   0        0        0      147 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0      182 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb.css
--rw-rw-rw-   0        0        0    13759 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb.js
--rw-rw-rw-   0        0        0   127331 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/flatly.min.css
--rw-rw-rw-   0        0        0    21378 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.css
--rw-rw-rw-   0        0        0    20664 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.js
--rw-rw-rw-   0        0        0     5108 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/htmlmixed.js
--rw-rw-rw-   0        0        0    24396 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript.js
--rw-rw-rw-   0        0        0    41074 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript_compressed.js
--rw-rw-rw-   0        0        0   268039 2019-03-09 15:07:37.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-3.2.1.js
--rw-rw-rw-   0        0        0      204 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-fix.js
--rw-rw-rw-   0        0        0     7200 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-migrate-1.2.1.min.js
--rw-rw-rw-   0        0        0    26010 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.css
--rw-rw-rw-   0        0        0   217071 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.js
--rw-rw-rw-   0        0        0     4255 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.ba-bbq.min.js
--rw-rw-rw-   0        0        0     1418 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.highlight.js
--rw-rw-rw-   0        0        0     1996 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.hotkey.js
--rw-rw-rw-   0        0        0     8182 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.idle-timer.js
--rw-rw-rw-   0        0        0    93069 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.js
--rw-rw-rw-   0        0        0   120545 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.jsPlumb-1.3.10-all-min.js
--rw-rw-rw-   0        0        0    40914 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.tablesorter.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.647373 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/
--rw-rw-rw-   0        0        0    13334 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/CLDRPluralRuleParser.js
--rw-rw-rw-   0        0        0    13513 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js
--rw-rw-rw-   0        0        0     5561 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.js
--rw-rw-rw-   0        0        0     4261 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.fallbacks.js
--rw-rw-rw-   0        0        0     9027 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.js
--rw-rw-rw-   0        0        0    12427 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.language.js
--rw-rw-rw-   0        0        0     3749 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.messagestore.js
--rw-rw-rw-   0        0        0     8483 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.parser.js
--rw-rw-rw-   0        0        0      380 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel-i18n.en.js
--rw-rw-rw-   0        0        0      484 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0      984 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.css
--rw-rw-rw-   0        0        0     3676 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.js
--rw-rw-rw-   0        0        0     1105 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelCorner.js
--rw-rw-rw-   0        0        0     6290 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobot.js
--rw-rw-rw-   0        0        0    12016 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobotDrawer.js
--rw-rw-rw-   0        0        0     9995 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelUI.js
--rw-rw-rw-   0        0        0     4647 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelWorld.js
--rw-rw-rw-   0        0        0    10847 2020-03-17 13:54:33.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/language_data.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.649375 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/
--rw-rw-rw-   0        0        0    20731 2022-02-03 12:41:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/hammer.min.js
--rw-rw-rw-   0        0        0      469 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/prettify.css
--rw-rw-rw-   0        0        0    17033 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/prettify.js
--rw-rw-rw-   0        0        0     2541 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.css
--rw-rw-rw-   0        0        0    27123 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.js
--rw-rw-rw-   0        0        0      264 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice-i18n.en.js
--rw-rw-rw-   0        0        0      207 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0    20787 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice.js
--rw-rw-rw-   0        0        0     3014 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.css
--rw-rw-rw-   0        0        0    20969 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.js
--rw-rw-rw-   0        0        0     1335 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/modal-basic.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.276355 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.650374 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/js/
--rw-rw-rw-   0        0        0    28326 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/js/en.js
--rw-rw-rw-   0        0        0     7117 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/navhelp.js
--rw-rw-rw-   0        0        0      252 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/notes.css
--rw-rw-rw-   0        0        0      216 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/notes.js
--rw-rw-rw-   0        0        0      319 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons-i18n.en.js
--rw-rw-rw-   0        0        0      370 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0     8848 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.css
--rw-rw-rw-   0        0        0    97344 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.js
--rw-rw-rw-   0        0        0     2666 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/petlja.css
--rw-rw-rw-   0        0        0      417 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/poll.css
--rw-rw-rw-   0        0        0     6877 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/poll.js
--rw-rw-rw-   0        0        0     3664 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.css
--rw-rw-rw-   0        0        0     6290 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.js
--rw-rw-rw-   0        0        0   231869 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/processing-1.4.1.min.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.660373 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/
--rw-rw-rw-   0        0        0    84233 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/__init__.js
--rw-rw-rw-   0        0        0     1888 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/display.js
--rw-rw-rw-   0        0        0     8368 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/draw.js
--rw-rw-rw-   0        0        0     3473 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/event.js
--rw-rw-rw-   0        0        0    11479 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/font.js
--rw-rw-rw-   0        0        0     4240 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/image.js
--rw-rw-rw-   0        0        0     6069 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/key.js
--rw-rw-rw-   0        0        0     1632 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/mouse.js
--rw-rw-rw-   0        0        0       47 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/pygame.js
--rw-rw-rw-   0        0        0     6205 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/time.js
--rw-rw-rw-   0        0        0     5597 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/transform.js
--rw-rw-rw-   0        0        0      254 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/version.js
--rw-rw-rw-   0        0        0     1315 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib-init.js
--rw-rw-rw-   0        0        0     4463 2020-03-17 13:54:33.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygments.css
--rw-rw-rw-   0        0        0    12629 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python.js
--rw-rw-rw-   0        0        0    30613 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python_compressed.js
--rw-rw-rw-   0        0        0    18580 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.css
--rw-rw-rw-   0        0        0   159859 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.js
--rw-rw-rw-   0        0        0    44234 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-core.js
--rw-rw-rw-   0        0        0    26515 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-cssclassapplier.js
--rw-rw-rw-   0        0        0    14204 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-textrange.js
--rw-rw-rw-   0        0        0     7907 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/reveal.js
--rw-rw-rw-   0        0        0    13625 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestone-custom-sphinx-bootstrap.css
--rw-rw-rw-   0        0        0     4326 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonebase.js
--rw-rw-rw-   0        0        0     2181 2019-12-21 09:54:12.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonevideo.js
--rw-rw-rw-   0        0        0    15059 2019-03-10 08:47:02.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/searchtools.js
--rw-rw-rw-   0        0        0   106155 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sharedb.js
--rw-rw-rw-   0        0        0        0 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/shortanswer.css
--rw-rw-rw-   0        0        0     8135 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/shortanswer.js
--rw-rw-rw-   0        0        0      631 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.css
--rw-rw-rw-   0        0        0     5939 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.js
--rw-rw-rw-   0        0        0   472567 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt-stdlib.js
--rw-rw-rw-   0        0        0   483003 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt.min.js
--rw-rw-rw-   0        0        0    14765 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortmodels.js
--rw-rw-rw-   0        0        0     1314 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortviewers.js
--rw-rw-rw-   0        0        0     6509 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/style.css
--rw-rw-rw-   0        0        0      526 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.css
--rw-rw-rw-   0        0        0     6176 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.js
--rw-rw-rw-   0        0        0    34671 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed.js
--rw-rw-rw-   0        0        0     2781 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_activecode.js
--rw-rw-rw-   0        0        0     1380 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_shortanswer.js
--rw-rw-rw-   0        0        0     1913 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedclickable.js
--rw-rw-rw-   0        0        0     1885 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timeddnd.js
--rw-rw-rw-   0        0        0     1806 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedfitb.js
--rw-rw-rw-   0        0        0     5551 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedmc.js
--rw-rw-rw-   0        0        0      578 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedparsons.js
--rw-rw-rw-   0        0        0    35168 2019-03-03 11:08:43.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore-1.3.1.js
--rw-rw-rw-   0        0        0    12140 2019-03-03 11:08:43.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore.js
--rw-rw-rw-   0        0        0     1839 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.css
--rw-rw-rw-   0        0        0     9337 2019-12-21 09:54:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.js
--rw-rw-rw-   0        0        0      489 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/video.css
--rw-rw-rw-   0        0        0     8051 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/waypoints.min.js
--rw-rw-rw-   0        0        0      275 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webgldemo.css
--rw-rw-rw-   0        0        0     4541 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.css
--rw-rw-rw-   0        0        0    18025 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.js
--rw-rw-rw-   0        0        0    25355 2019-03-10 08:47:02.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/websupport.js
--rw-rw-rw-   0        0        0    12741 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/xml.js
--rw-rw-rw-   0        0        0      445 2020-03-17 13:54:34.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/searchindex.js
--rw-rw-rw-   0        0        0        0 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/sphinx-enki-info.txt
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.661373 petljadoc-1.3.0/petljadoc/runestone_ext/p5js/
--rw-rw-rw-   0        0        0       21 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/p5js/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.662375 petljadoc-1.3.0/petljadoc/runestone_ext/p5js/css/
--rw-rw-rw-   0        0        0      164 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/p5js/css/p5js.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.663374 petljadoc-1.3.0/petljadoc/runestone_ext/p5js/js/
--rw-rw-rw-   0        0        0     1646 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/p5js/js/p5js.js
--rw-rw-rw-   0        0        0     5321 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/runestone_ext/p5js/p5js.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.664372 petljadoc-1.3.0/petljadoc/runestone_ext/pycode/
--rw-rw-rw-   0        0        0       23 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pycode/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.665374 petljadoc-1.3.0/petljadoc/runestone_ext/pycode/css/
--rw-rw-rw-   0        0        0     2816 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pycode/css/pycode.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.666377 petljadoc-1.3.0/petljadoc/runestone_ext/pycode/js/
--rw-rw-rw-   0        0        0    27491 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pycode/js/pycode.js
--rw-rw-rw-   0        0        0     4032 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pycode/pycode.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.668375 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/
--rw-rw-rw-   0        0        0       24 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.668375 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.679372 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/
--rw-rw-rw-   0        0        0    84233 2019-09-27 19:15:50.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/__init__.js
--rw-rw-rw-   0        0        0     1888 2021-11-01 13:09:37.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/display.js
--rw-rw-rw-   0        0        0     8368 2021-11-01 13:09:37.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/draw.js
--rw-rw-rw-   0        0        0     3473 2021-11-01 13:09:37.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/event.js
--rw-rw-rw-   0        0        0    11479 2021-11-01 13:09:37.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/font.js
--rw-rw-rw-   0        0        0     4240 2021-11-01 13:09:37.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/image.js
--rw-rw-rw-   0        0        0     6069 2019-09-27 19:15:50.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/key.js
--rw-rw-rw-   0        0        0     1632 2021-11-01 13:09:37.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/mouse.js
--rw-rw-rw-   0        0        0       47 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/pygame.js
--rw-rw-rw-   0        0        0     6205 2021-11-01 13:09:37.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/time.js
--rw-rw-rw-   0        0        0     5597 2021-11-01 13:09:37.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/transform.js
--rw-rw-rw-   0        0        0      254 2021-11-01 13:09:37.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/version.js
--rw-rw-rw-   0        0        0     1315 2021-02-02 16:03:37.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib-init.js
--rw-rw-rw-   0        0        0       57 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/pygamelib.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.681373 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.281355 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/_templates/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.281355 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.282355 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.682373 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.283355 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.682373 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
--rw-rw-rw-   0        0        0    97346 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.683374 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
--rw-rw-rw-   0        0        0    27731 2019-09-29 18:46:11.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
--rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
--rw-rw-rw-   0        0        0     8444 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/conf.py
--rw-rw-rw-   0        0        0     1822 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/pavement.py
--rw-rw-rw-   0        0        0        0 2019-11-01 17:26:30.000000 petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/sphinx-enki-info.txt
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.685372 petljadoc-1.3.0/petljadoc/runestone_ext/quizq/
--rw-rw-rw-   0        0        0       22 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/quizq/__init__.py
--rw-rw-rw-   0        0        0     1396 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/quizq/quizq.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.688377 petljadoc-1.3.0/petljadoc/runestone_ext/regexcheck/
--rw-rw-rw-   0        0        0       27 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/regexcheck/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.688377 petljadoc-1.3.0/petljadoc/runestone_ext/regexcheck/css/
--rw-rw-rw-   0        0        0     2809 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/regexcheck/css/regex-check.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.693374 petljadoc-1.3.0/petljadoc/runestone_ext/regexcheck/js/
--rw-rw-rw-   0        0        0      297 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.en.js
--rw-rw-rw-   0        0        0      379 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0      316 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.sr-Latn.js
--rw-rw-rw-   0        0        0      374 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.sr.js
--rw-rw-rw-   0        0        0     5874 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/regexcheck/js/regex-check.js
--rw-rw-rw-   0        0        0     3703 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/runestone_ext/regexcheck/regexcheck.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.694374 petljadoc-1.3.0/petljadoc/runestone_ext/simanim/
--rw-rw-rw-   0        0        0       24 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/simanim/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.695373 petljadoc-1.3.0/petljadoc/runestone_ext/simanim/css/
--rw-rw-rw-   0        0        0     2332 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/runestone_ext/simanim/css/simanim.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.695373 petljadoc-1.3.0/petljadoc/runestone_ext/simanim/js/
--rw-rw-rw-   0        0        0    21064 2023-03-06 12:31:02.000000 petljadoc-1.3.0/petljadoc/runestone_ext/simanim/js/simanim.js
--rw-rw-rw-   0        0        0     4137 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/runestone_ext/simanim/simanim.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.286355 petljadoc-1.3.0/petljadoc/runestone_ext/video/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.286355 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.287355 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.696373 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.697373 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_sources/
--rw-rw-rw-   0        0        0      254 2019-10-06 19:56:26.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_sources/index.rst.txt
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.827373 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/
--rw-rw-rw-   0        0        0     6355 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/Blob.js
--rw-rw-rw-   0        0        0     5120 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/FileSaver.min.js
--rw-rw-rw-   0        0        0     1511 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/LICENSE.txt
--rw-rw-rw-   0        0        0     3439 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibility.css
--rw-rw-rw-   0        0        0     3445 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitydarkest.css
--rw-rw-rw-   0        0        0     2669 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitylight.css
--rw-rw-rw-   0        0        0     9490 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.en.js
--rw-rw-rw-   0        0        0    14672 2020-12-09 10:35:50.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0     2096 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.css
--rw-rw-rw-   0        0        0   102910 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.js
--rw-rw-rw-   0        0        0     3903 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/animationbase.js
--rw-rw-rw-   0        0        0    10912 2019-10-06 20:19:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/basic.css
--rw-rw-rw-   0        0        0   471577 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blockly_compressed.js
--rw-rw-rw-   0        0        0    55934 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blocks_compressed.js
--rw-rw-rw-   0        0        0    10606 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bookfuncs.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.288354 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.827373 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/css/
--rw-rw-rw-   0        0        0    97346 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.828374 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/js/
--rw-rw-rw-   0        0        0    27731 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/js/bootstrap.min.js
--rw-rw-rw-   0        0        0      425 2019-10-06 20:19:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-sphinx.css
--rw-rw-rw-   0        0        0     3776 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-sphinx.js
--rw-rw-rw-   0        0        0    97348 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap.min.css
--rw-rw-rw-   0        0        0     1123 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.css
--rw-rw-rw-   0        0        0    16404 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.js
--rw-rw-rw-   0        0        0    18265 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clike.js
--rw-rw-rw-   0        0        0     2037 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codelens.js
--rw-rw-rw-   0        0        0     7507 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.css
--rw-rw-rw-   0        0        0   320980 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.js
--rw-rw-rw-   0        0        0    32373 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/css.js
--rw-rw-rw-   0        0        0   111549 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/d3.v2.min.js
--rw-rw-rw-   0        0        0       95 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/datafile.css
--rw-rw-rw-   0        0        0     3000 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/datafile.js
--rw-rw-rw-   0        0        0    19241 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/diff_match_patch.js
--rw-rw-rw-   0        0        0     6868 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/doctools.js
--rw-rw-rw-   0        0        0      307 2019-10-06 20:19:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/documentation_options.js
--rw-rw-rw-   0        0        0      310 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop-i18n.en.js
--rw-rw-rw-   0        0        0      389 2020-12-09 10:35:50.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0     1480 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.css
--rw-rw-rw-   0        0        0    18311 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.js
--rw-rw-rw-   0        0        0     1756 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/external.css
--rw-rw-rw-   0        0        0      130 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb-i18n.en.js
--rw-rw-rw-   0        0        0      142 2020-12-09 10:35:50.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0      182 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb.css
--rw-rw-rw-   0        0        0    13759 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb.js
--rw-rw-rw-   0        0        0    21378 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.css
--rw-rw-rw-   0        0        0    20664 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.js
--rw-rw-rw-   0        0        0     5108 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/htmlmixed.js
--rw-rw-rw-   0        0        0    24396 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript.js
--rw-rw-rw-   0        0        0    41074 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript_compressed.js
--rw-rw-rw-   0        0        0   268039 2019-03-09 15:07:37.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-3.2.1.js
--rw-rw-rw-   0        0        0      204 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-fix.js
--rw-rw-rw-   0        0        0     7200 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-migrate-1.2.1.min.js
--rw-rw-rw-   0        0        0    26010 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.css
--rw-rw-rw-   0        0        0   217071 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.js
--rw-rw-rw-   0        0        0     4255 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.ba-bbq.min.js
--rw-rw-rw-   0        0        0     1418 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.highlight.js
--rw-rw-rw-   0        0        0     1996 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.hotkey.js
--rw-rw-rw-   0        0        0     8182 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.idle-timer.js
--rw-rw-rw-   0        0        0    93069 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.js
--rw-rw-rw-   0        0        0   120545 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.jsPlumb-1.3.10-all-min.js
--rw-rw-rw-   0        0        0    40914 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.tablesorter.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.835373 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/
--rw-rw-rw-   0        0        0    13334 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/CLDRPluralRuleParser.js
--rw-rw-rw-   0        0        0    13513 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js
--rw-rw-rw-   0        0        0     5561 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.js
--rw-rw-rw-   0        0        0     4261 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.fallbacks.js
--rw-rw-rw-   0        0        0     9027 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.js
--rw-rw-rw-   0        0        0    12427 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.language.js
--rw-rw-rw-   0        0        0     3749 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.messagestore.js
--rw-rw-rw-   0        0        0     8483 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.parser.js
--rw-rw-rw-   0        0        0    10847 2019-10-06 20:19:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/language_data.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.838374 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/
--rw-rw-rw-   0        0        0    20731 2022-02-03 12:41:37.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/hammer.min.js
--rw-rw-rw-   0        0        0      469 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/prettify.css
--rw-rw-rw-   0        0        0    17033 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/prettify.js
--rw-rw-rw-   0        0        0     2541 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.css
--rw-rw-rw-   0        0        0    27123 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.js
--rw-rw-rw-   0        0        0      264 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice-i18n.en.js
--rw-rw-rw-   0        0        0      202 2020-12-09 10:35:50.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0    20787 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice.js
--rw-rw-rw-   0        0        0     3014 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.css
--rw-rw-rw-   0        0        0    20969 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.js
--rw-rw-rw-   0        0        0     1335 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/modal-basic.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.292356 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.839373 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/js/
--rw-rw-rw-   0        0        0    28326 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/js/en.js
--rw-rw-rw-   0        0        0     7117 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/navhelp.js
--rw-rw-rw-   0        0        0      314 2020-12-09 10:35:50.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons-i18n.en.js
--rw-rw-rw-   0        0        0      365 2020-12-09 10:35:50.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons-i18n.sr-Cyrl.js
--rw-rw-rw-   0        0        0     8848 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.css
--rw-rw-rw-   0        0        0    97344 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.js
--rw-rw-rw-   0        0        0      417 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/poll.css
--rw-rw-rw-   0        0        0     6877 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/poll.js
--rw-rw-rw-   0        0        0     3664 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.css
--rw-rw-rw-   0        0        0     6290 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.js
--rw-rw-rw-   0        0        0   231869 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/processing-1.4.1.min.js
--rw-rw-rw-   0        0        0     4463 2019-10-06 20:19:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pygments.css
--rw-rw-rw-   0        0        0    12629 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python.js
--rw-rw-rw-   0        0        0    30613 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python_compressed.js
--rw-rw-rw-   0        0        0    18580 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.css
--rw-rw-rw-   0        0        0   159859 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.js
--rw-rw-rw-   0        0        0    44234 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-core.js
--rw-rw-rw-   0        0        0    26515 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-cssclassapplier.js
--rw-rw-rw-   0        0        0    14204 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-textrange.js
--rw-rw-rw-   0        0        0     7907 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/reveal.js
--rw-rw-rw-   0        0        0    13625 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestone-custom-sphinx-bootstrap.css
--rw-rw-rw-   0        0        0     4326 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonebase.js
--rw-rw-rw-   0        0        0     2181 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonevideo.js
--rw-rw-rw-   0        0        0    15059 2019-03-10 08:47:02.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/searchtools.js
--rw-rw-rw-   0        0        0   106155 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sharedb.js
--rw-rw-rw-   0        0        0        0 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/shortanswer.css
--rw-rw-rw-   0        0        0     8135 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/shortanswer.js
--rw-rw-rw-   0        0        0      631 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.css
--rw-rw-rw-   0        0        0     5939 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.js
--rw-rw-rw-   0        0        0   472567 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt-stdlib.js
--rw-rw-rw-   0        0        0   483003 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt.min.js
--rw-rw-rw-   0        0        0    14765 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortmodels.js
--rw-rw-rw-   0        0        0     1314 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortviewers.js
--rw-rw-rw-   0        0        0     6509 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/style.css
--rw-rw-rw-   0        0        0      526 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.css
--rw-rw-rw-   0        0        0     6176 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.js
--rw-rw-rw-   0        0        0    34671 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed.js
--rw-rw-rw-   0        0        0     2781 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_activecode.js
--rw-rw-rw-   0        0        0     1380 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_shortanswer.js
--rw-rw-rw-   0        0        0     1913 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedclickable.js
--rw-rw-rw-   0        0        0     1885 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timeddnd.js
--rw-rw-rw-   0        0        0     1806 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedfitb.js
--rw-rw-rw-   0        0        0     5551 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedmc.js
--rw-rw-rw-   0        0        0      578 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedparsons.js
--rw-rw-rw-   0        0        0    35168 2019-03-03 11:08:43.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore-1.3.1.js
--rw-rw-rw-   0        0        0    12140 2019-03-03 11:08:43.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore.js
--rw-rw-rw-   0        0        0     1839 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.css
--rw-rw-rw-   0        0        0     9337 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.js
--rw-rw-rw-   0        0        0      489 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/video.css
--rw-rw-rw-   0        0        0     8051 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/waypoints.min.js
--rw-rw-rw-   0        0        0      275 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webgldemo.css
--rw-rw-rw-   0        0        0     4541 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.css
--rw-rw-rw-   0        0        0    18025 2019-09-29 18:45:24.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.js
--rw-rw-rw-   0        0        0    25355 2019-03-10 08:47:02.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/websupport.js
--rw-rw-rw-   0        0        0    12741 2019-09-29 18:45:23.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/xml.js
--rw-rw-rw-   0        0        0      398 2019-10-06 20:19:31.000000 petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/searchindex.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.845374 petljadoc-1.3.0/petljadoc/scorm-proxy-templates/
--rw-rw-rw-   0        0        0     4508 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/scorm-proxy-templates/adlcp_rootv1p2.xsd
--rw-rw-rw-   0        0        0   100404 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/scorm-proxy-templates/bundle.js
--rw-rw-rw-   0        0        0    10462 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/scorm-proxy-templates/favicon.ico
--rw-rw-rw-   0        0        0     1236 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/scorm-proxy-templates/ims_xml.xsd
--rw-rw-rw-   0        0        0    14820 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/scorm-proxy-templates/imscp_rootv1p1p2.xsd
--rw-rw-rw-   0        0        0     1184 2023-03-06 12:31:02.000000 petljadoc-1.3.0/petljadoc/scorm-proxy-templates/imsmanifest.t.xml
--rw-rw-rw-   0        0        0    19397 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/scorm-proxy-templates/imsmd_rootv1p2p1.xsd
--rw-rw-rw-   0        0        0     1525 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/scorm-proxy-templates/index.t.html
--rw-rw-rw-   0        0        0    18985 2023-01-10 11:56:30.000000 petljadoc-1.3.0/petljadoc/scorm-proxy-templates/style-player.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.850375 petljadoc-1.3.0/petljadoc/scorm-templates/
--rw-rw-rw-   0        0        0     4508 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/scorm-templates/adlcp_rootv1p2.xsd
--rw-rw-rw-   0        0        0     1236 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/scorm-templates/ims_xml.xsd
--rw-rw-rw-   0        0        0    14820 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/scorm-templates/imscp_rootv1p1p2.xsd
--rw-rw-rw-   0        0        0    19397 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/scorm-templates/imsmd_rootv1p2p1.xsd
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.850375 petljadoc-1.3.0/petljadoc/themes/
--rw-rw-rw-   0        0        0       83 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.853372 petljadoc-1.3.0/petljadoc/themes/bc_theme/
--rw-rw-rw-   0        0        0      386 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/__init__.py
--rw-rw-rw-   0        0        0     5931 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/layout.html
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.297355 petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.295355 petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/en/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.854374 petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0      968 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/en/LC_MESSAGES/shpinx.mo
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.296355 petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/sr/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.855373 petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/sr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1260 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/sr/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.296355 petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/sr@latn/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.854374 petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/sr@latn/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1007 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.297355 petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/sr_RS/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.856374 petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/sr_RS/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1260 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.856374 petljadoc-1.3.0/petljadoc/themes/bc_theme/platform/
--rw-rw-rw-   0        0        0     8733 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/platform/petljaRTBundle.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.868372 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.299355 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.868372 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/css/
--rw-rw-rw-   0        0        0   144836 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.870374 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/
--rw-rw-rw-   0        0        0    67698 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0    48907 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js
--rw-rw-rw-   0        0        0      906 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bootstrap-sphinx.css_t
--rw-rw-rw-   0        0        0     3776 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bootstrap-sphinx.js
--rw-rw-rw-   0        0        0   100404 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bundle.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.871372 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/css/
--rw-rw-rw-   0        0        0    31004 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/css/font-awesome.min.css
--rw-rw-rw-   0        0        0    10462 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/favicon.ico
--rw-rw-rw-   0        0        0   127331 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/flatly.min.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.877374 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/fonts/
--rw-rw-rw-   0        0        0   134808 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/fonts/FontAwesome.otf
--rw-rw-rw-   0        0        0   165742 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff2
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.884373 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/
--rw-rw-rw-   0        0        0    69642 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/choice-background.svg
--rw-rw-rw-   0        0        0    69619 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/dragndrop-background.svg
--rw-rw-rw-   0        0        0    69642 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/fitb-background.svg
--rw-rw-rw-   0        0        0      715 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/logo.svg
--rw-rw-rw-   0        0        0     1224 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/netkabinet-logo-strelica-wt.svg
--rw-rw-rw-   0        0        0    69646 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/parsons-background.svg
--rw-rw-rw-   0        0        0      782 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/petlja-logo-wt.svg
--rw-rw-rw-   0        0        0     1618 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/play_button.svg
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.912372 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/
--rw-rw-rw-   0        0        0     3152 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/Facebook.png
--rw-rw-rw-   0        0        0     3079 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/Facebook_icon.png
--rw-rw-rw-   0        0        0     3728 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/Twitter.png
--rw-rw-rw-   0        0        0     3177 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/Twitter_icon.png
--rw-rw-rw-   0        0        0      231 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/active.png
--rw-rw-rw-   0        0        0      332 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/completed.png
--rw-rw-rw-   0        0        0     3482 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/dragndrop-img.svg
--rw-rw-rw-   0        0        0    18186 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/favicon.ico
--rw-rw-rw-   0        0        0      640 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/fitb-img.svg
--rw-rw-rw-   0        0        0     5334 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/green-coin.png
--rw-rw-rw-   0        0        0      447 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/infonote-img.svg
--rw-rw-rw-   0        0        0      828 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-ball.png
--rw-rw-rw-   0        0        0     7370 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-east-balls.png
--rw-rw-rw-   0        0        0     5362 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-east.png
--rw-rw-rw-   0        0        0     8203 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-head.png
--rw-rw-rw-   0        0        0     6942 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-hole.png
--rw-rw-rw-   0        0        0     5910 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-north-balls.png
--rw-rw-rw-   0        0        0     7338 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-north.png
--rw-rw-rw-   0        0        0     6842 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-south-balls.png
--rw-rw-rw-   0        0        0    12370 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-south.png
--rw-rw-rw-   0        0        0    65211 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-west-balls.png
--rw-rw-rw-   0        0        0     7920 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-west.png
--rw-rw-rw-   0        0        0     2857 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/learnmorenote-img.svg
--rw-rw-rw-   0        0        0    37014 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/logo.png
--rw-rw-rw-   0        0        0   102151 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/logo_small.png
--rw-rw-rw-   0        0        0     1224 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/netkabinet-logo-strelica-wt.svg
--rw-rw-rw-   0        0        0     1434 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/parsons-img.svg
--rw-rw-rw-   0        0        0      782 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/petlja-logo-wt.svg
--rw-rw-rw-   0        0        0     5841 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/play_overlay_icon.png
--rw-rw-rw-   0        0        0      640 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/qchoice-img.svg
--rw-rw-rw-   0        0        0     4750 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/question-mark-old.png
--rw-rw-rw-   0        0        0     1327 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/question-mark.png
--rw-rw-rw-   0        0        0     1327 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/questionnote-img.svg
--rw-rw-rw-   0        0        0     3186 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/suggestionnote-img.svg
--rw-rw-rw-   0        0        0     3662 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/technicalnote-img.svg
--rw-rw-rw-   0        0        0    24003 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/petlja-course.css
--rw-rw-rw-   0        0        0     4607 2023-03-06 12:31:02.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/petlja.js
--rw-rw-rw-   0        0        0    88628 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/require.js
--rw-rw-rw-   0        0        0    47740 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/simanim-0.0.4-py3-none-any.whl
--rw-rw-rw-   0        0        0   472567 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/skulpt-stdlib.js
--rw-rw-rw-   0        0        0   483003 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/skulpt.min.js
--rw-rw-rw-   0        0        0    18985 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/static/style-player.css
--rw-rw-rw-   0        0        0     1295 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/bc_theme/theme.conf
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.918375 petljadoc-1.3.0/petljadoc/themes/course_theme/
--rw-rw-rw-   0        0        0      390 2022-11-06 09:12:12.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/__init__.py
--rw-rw-rw-   0        0        0     5667 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/basic_layout.html
--rw-rw-rw-   0        0        0     1935 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/course_homepage.html
--rw-rw-rw-   0        0        0     1653 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/globaltoc.html
--rw-rw-rw-   0        0        0     7299 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/layout.html
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.303355 petljadoc-1.3.0/petljadoc/themes/course_theme/locale/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.302355 petljadoc-1.3.0/petljadoc/themes/course_theme/locale/en/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.919374 petljadoc-1.3.0/petljadoc/themes/course_theme/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0      968 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/locale/en/LC_MESSAGES/shpinx.mo
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.303355 petljadoc-1.3.0/petljadoc/themes/course_theme/locale/sr/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.921374 petljadoc-1.3.0/petljadoc/themes/course_theme/locale/sr/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1260 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/locale/sr/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.302355 petljadoc-1.3.0/petljadoc/themes/course_theme/locale/sr@latn/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.920374 petljadoc-1.3.0/petljadoc/themes/course_theme/locale/sr@latn/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1007 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.304355 petljadoc-1.3.0/petljadoc/themes/course_theme/locale/sr_RS/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.921374 petljadoc-1.3.0/petljadoc/themes/course_theme/locale/sr_RS/LC_MESSAGES/
--rw-rw-rw-   0        0        0     1260 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo
--rw-rw-rw-   0        0        0      205 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/localtoc.html
--rw-rw-rw-   0        0        0      810 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/relations.html
--rw-rw-rw-   0        0        0      170 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/sourcelink.html
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.934372 petljadoc-1.3.0/petljadoc/themes/course_theme/static/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.307355 petljadoc-1.3.0/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.935373 petljadoc-1.3.0/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/css/
--rw-rw-rw-   0        0        0   144836 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.937373 petljadoc-1.3.0/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/
--rw-rw-rw-   0        0        0    67698 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0    48907 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js
--rw-rw-rw-   0        0        0      906 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/bootstrap-sphinx.css_t
--rw-rw-rw-   0        0        0     3776 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/bootstrap-sphinx.js
--rw-rw-rw-   0        0        0      401 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/course-errors.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.938374 petljadoc-1.3.0/petljadoc/themes/course_theme/static/css/
--rw-rw-rw-   0        0        0    31004 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/css/font-awesome.min.css
--rw-rw-rw-   0        0        0        0 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/error_log.txt
--rw-rw-rw-   0        0        0    10462 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/favicon.ico
--rw-rw-rw-   0        0        0   127323 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/flatly.min.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.945377 petljadoc-1.3.0/petljadoc/themes/course_theme/static/fonts/
--rw-rw-rw-   0        0        0   134808 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/fonts/FontAwesome.otf
--rw-rw-rw-   0        0        0   165742 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff2
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.952380 petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/
--rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/choice-background.svg
--rw-rw-rw-   0        0        0    69619 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/dragndrop-background.svg
--rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/fitb-background.svg
--rw-rw-rw-   0        0        0      715 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/logo.svg
--rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/netkabinet-logo-strelica-wt.svg
--rw-rw-rw-   0        0        0    69646 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/parsons-background.svg
--rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/petlja-logo-wt.svg
--rw-rw-rw-   0        0        0     1618 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/play_button.svg
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.985375 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/
--rw-rw-rw-   0        0        0     3152 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/Facebook.png
--rw-rw-rw-   0        0        0     3079 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/Facebook_icon.png
--rw-rw-rw-   0        0        0     3728 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/Twitter.png
--rw-rw-rw-   0        0        0     3177 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/Twitter_icon.png
--rw-rw-rw-   0        0        0      231 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/active.png
--rw-rw-rw-   0        0        0      332 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/completed.png
--rw-rw-rw-   0        0        0     3482 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/dragndrop-img.svg
--rw-rw-rw-   0        0        0    18186 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/favicon.ico
--rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/fitb-img.svg
--rw-rw-rw-   0        0        0     5334 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/green-coin.png
--rw-rw-rw-   0        0        0      447 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/infonote-img.svg
--rw-rw-rw-   0        0        0      828 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-ball.png
--rw-rw-rw-   0        0        0     7370 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-east-balls.png
--rw-rw-rw-   0        0        0     5362 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-east.png
--rw-rw-rw-   0        0        0     8203 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-head.png
--rw-rw-rw-   0        0        0     6942 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-hole.png
--rw-rw-rw-   0        0        0     5910 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-north-balls.png
--rw-rw-rw-   0        0        0     7338 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-north.png
--rw-rw-rw-   0        0        0     6842 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-south-balls.png
--rw-rw-rw-   0        0        0    12370 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-south.png
--rw-rw-rw-   0        0        0    65211 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-west-balls.png
--rw-rw-rw-   0        0        0     7920 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-west.png
--rw-rw-rw-   0        0        0     2857 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/learnmorenote-img.svg
--rw-rw-rw-   0        0        0    37014 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/logo.png
--rw-rw-rw-   0        0        0   102151 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/logo_small.png
--rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/netkabinet-logo-strelica-wt.svg
--rw-rw-rw-   0        0        0     1434 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/parsons-img.svg
--rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/petlja-logo-wt.svg
--rw-rw-rw-   0        0        0     5841 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/play_overlay_icon.png
--rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/qchoice-img.svg
--rw-rw-rw-   0        0        0     4750 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/question-mark-old.png
--rw-rw-rw-   0        0        0     1327 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/question-mark.png
--rw-rw-rw-   0        0        0     1327 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/questionnote-img.svg
--rw-rw-rw-   0        0        0     3186 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/suggestionnote-img.svg
--rw-rw-rw-   0        0        0     3662 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/technicalnote-img.svg
--rw-rw-rw-   0        0        0   264982 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/nbstyle.css
--rw-rw-rw-   0        0        0    23457 2022-12-02 13:00:34.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/petlja-course.css
--rw-rw-rw-   0        0        0     7082 2022-11-20 11:14:54.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/petlja.js
--rw-rw-rw-   0        0        0    88628 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/require.js
--rw-rw-rw-   0        0        0    47740 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/simanim-0.0.4-py3-none-any.whl
--rw-rw-rw-   0        0        0   472567 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/skulpt-stdlib.js
--rw-rw-rw-   0        0        0   483003 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/static/skulpt.min.js
--rw-rw-rw-   0        0        0      859 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/subchapter.html
--rw-rw-rw-   0        0        0     1297 2022-11-03 09:45:51.000000 petljadoc-1.3.0/petljadoc/themes/course_theme/theme.conf
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.993373 petljadoc-1.3.0/petljadoc/themes/runestone_theme/
--rw-rw-rw-   0        0        0      537 2020-12-09 14:48:07.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/__init__.py
--rw-rw-rw-   0        0        0     8162 2020-12-29 14:15:02.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/basic_layout.html
--rw-rw-rw-   0        0        0      372 2020-12-04 12:05:37.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/globaltoc.html
--rw-rw-rw-   0        0        0     5342 2023-03-06 12:31:02.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/layout.html
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.312355 petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.310355 petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/en/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.993373 petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0      566 2020-12-09 14:48:07.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/en/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.311355 petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/sr/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.995373 petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/sr/LC_MESSAGES/
--rw-rw-rw-   0        0        0      689 2020-12-09 14:48:07.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/sr/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.311355 petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/sr@latn/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.994373 petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/sr@latn/LC_MESSAGES/
--rw-rw-rw-   0        0        0      655 2020-12-29 14:15:02.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.312355 petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/sr_RS/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.995373 petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/sr_RS/LC_MESSAGES/
--rw-rw-rw-   0        0        0      689 2020-12-29 14:15:02.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo
--rw-rw-rw-   0        0        0      187 2020-12-08 00:51:34.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/localtoc.html
--rw-rw-rw-   0        0        0     1262 2020-12-09 14:48:07.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/relations.html
--rw-rw-rw-   0        0        0      170 2020-12-04 12:05:37.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/sourcelink.html
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:51.007374 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.314356 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:51.008372 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/css/
--rw-rw-rw-   0        0        0   144838 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:51.010373 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/
--rw-rw-rw-   0        0        0    67698 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
--rw-rw-rw-   0        0        0    48907 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js
--rw-rw-rw-   0        0        0      906 2020-12-04 12:05:37.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.css_t
--rw-rw-rw-   0        0        0     3776 2020-12-04 12:05:37.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.js
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:51.011372 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/css/
--rw-rw-rw-   0        0        0    31004 2020-12-04 12:05:37.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/css/font-awesome.min.css
--rw-rw-rw-   0        0        0        0 2020-12-29 14:15:02.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/error_log.txt
--rw-rw-rw-   0        0        0    10462 2020-12-04 12:05:37.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/favicon.ico
--rw-rw-rw-   0        0        0   127331 2020-12-04 12:05:37.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/flatly.min.css
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:51.017375 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/fonts/
--rw-rw-rw-   0        0        0   134808 2020-12-04 12:05:37.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/fonts/FontAwesome.otf
--rw-rw-rw-   0        0        0   165742 2020-12-04 12:05:37.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.eot
--rw-rw-rw-   0        0        0   447050 2020-12-04 12:05:37.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.svg
--rw-rw-rw-   0        0        0   165548 2020-12-04 12:05:37.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.ttf
--rw-rw-rw-   0        0        0    98024 2020-12-04 12:05:37.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff
--rw-rw-rw-   0        0        0    77160 2020-12-04 12:05:37.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff2
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:51.025373 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/
--rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/choice-background.svg
--rw-rw-rw-   0        0        0    69619 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/dragndrop-background.svg
--rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/fitb-background.svg
--rw-rw-rw-   0        0        0      715 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/logo.svg
--rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/netkabinet-logo-strelica-wt.svg
--rw-rw-rw-   0        0        0    69646 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/parsons-background.svg
--rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/petlja-logo-wt.svg
--rw-rw-rw-   0        0        0     1618 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/play_button.svg
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:51.049372 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/
--rw-rw-rw-   0        0        0     3152 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/Facebook.png
--rw-rw-rw-   0        0        0     3079 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/Facebook_icon.png
--rw-rw-rw-   0        0        0     3728 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/Twitter.png
--rw-rw-rw-   0        0        0     3177 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/Twitter_icon.png
--rw-rw-rw-   0        0        0      231 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/active.png
--rw-rw-rw-   0        0        0      332 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/completed.png
--rw-rw-rw-   0        0        0     3482 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/dragndrop-img.svg
--rw-rw-rw-   0        0        0    18186 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/favicon.ico
--rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/fitb-img.svg
--rw-rw-rw-   0        0        0     5334 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/green-coin.png
--rw-rw-rw-   0        0        0      447 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/infonote-img.svg
--rw-rw-rw-   0        0        0    10414 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/karel-ball.png
--rw-rw-rw-   0        0        0    19798 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/karel-east.png
--rw-rw-rw-   0        0        0     8203 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/karel-head.png
--rw-rw-rw-   0        0        0     6942 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/karel-hole.png
--rw-rw-rw-   0        0        0    13690 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/karel-north.png
--rw-rw-rw-   0        0        0    14972 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/karel-south.png
--rw-rw-rw-   0        0        0    19805 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/karel-west.png
--rw-rw-rw-   0        0        0     2857 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/learnmorenote-img.svg
--rw-rw-rw-   0        0        0    37014 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/logo.png
--rw-rw-rw-   0        0        0   102151 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/logo_small.png
--rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/netkabinet-logo-strelica-wt.svg
--rw-rw-rw-   0        0        0     1434 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/parsons-img.svg
--rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/petlja-logo-wt.svg
--rw-rw-rw-   0        0        0     5841 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/play_overlay_icon.png
--rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/qchoice-img.svg
--rw-rw-rw-   0        0        0     4750 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/question-mark-old.png
--rw-rw-rw-   0        0        0     1327 2022-01-26 16:39:18.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/question-mark.png
--rw-rw-rw-   0        0        0     1327 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/questionnote-img.svg
--rw-rw-rw-   0        0        0     3186 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/suggestionnote-img.svg
--rw-rw-rw-   0        0        0     3662 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/technicalnote-img.svg
--rw-rw-rw-   0        0        0   277929 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/nbstyle.css
--rw-rw-rw-   0        0        0     2821 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/petlja-runestone.css
--rw-rw-rw-   0        0        0        0 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/petlja_ruenstone.js
--rw-rw-rw-   0        0        0    88628 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/require.js
--rw-rw-rw-   0        0        0    47740 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/simanim-0.0.4-py3-none-any.whl
--rw-rw-rw-   0        0        0   472567 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/skulpt-stdlib.js
--rw-rw-rw-   0        0        0   483003 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/skulpt.min.js
--rw-rw-rw-   0        0        0     1264 2020-12-09 14:48:07.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/subchapter.html
--rw-rw-rw-   0        0        0     1297 2020-12-04 12:05:37.000000 petljadoc-1.3.0/petljadoc/themes/runestone_theme/theme.conf
--rw-rw-rw-   0        0        0     4478 2022-11-06 13:07:32.000000 petljadoc-1.3.0/petljadoc/util.py
-drwxrwxrwx   0        0        0        0 2023-03-06 12:48:50.348354 petljadoc-1.3.0/petljadoc.egg-info/
--rw-rw-rw-   0        0        0     2389 2023-03-06 12:48:49.000000 petljadoc-1.3.0/petljadoc.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    51038 2023-03-06 12:48:50.000000 petljadoc-1.3.0/petljadoc.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-06 12:48:49.000000 petljadoc-1.3.0/petljadoc.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      293 2023-03-06 12:48:49.000000 petljadoc-1.3.0/petljadoc.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2019-09-30 21:36:41.000000 petljadoc-1.3.0/petljadoc.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      195 2023-03-06 12:48:49.000000 petljadoc-1.3.0/petljadoc.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-03-06 12:48:49.000000 petljadoc-1.3.0/petljadoc.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      210 2023-03-06 12:48:22.000000 petljadoc-1.3.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-03-06 12:48:51.051372 petljadoc-1.3.0/setup.cfg
--rw-rw-rw-   0        0        0     1707 2022-11-20 11:14:54.000000 petljadoc-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:09.215963 petljadoc-1.3.1/
+-rw-rw-rw-   0        0        0     1084 2019-09-29 18:46:11.000000 petljadoc-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0      475 2022-11-20 11:14:54.000000 petljadoc-1.3.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2389 2023-04-10 05:44:09.215963 petljadoc-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1803 2022-11-06 13:07:30.000000 petljadoc-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.727090 petljadoc-1.3.1/petljadoc/
+-rw-rw-rw-   0        0        0       67 2023-04-10 05:07:00.000000 petljadoc-1.3.1/petljadoc/__init__.py
+-rw-rw-rw-   0        0        0       39 2020-12-07 14:32:36.000000 petljadoc-1.3.1/petljadoc/__main__.py
+-rw-rw-rw-   0        0        0    43045 2023-03-06 12:31:02.000000 petljadoc-1.3.1/petljadoc/cli.py
+-rw-rw-rw-   0        0        0    15820 2023-03-06 12:31:02.000000 petljadoc-1.3.1/petljadoc/course.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.546086 petljadoc-1.3.1/petljadoc/nb-templates/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.763088 petljadoc-1.3.1/petljadoc/nb-templates/classic2/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.864437 petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/
+-rw-rw-rw-   0        0        0     7752 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/base.html.j2
+-rw-rw-rw-   0        0        0      220 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/celltags.j2
+-rw-rw-rw-   0        0        0     1634 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/display_priority.j2
+-rw-rw-rw-   0        0        0      993 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/jupyter_widgets.html.j2
+-rw-rw-rw-   0        0        0     1386 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/mathjax.html.j2
+-rw-rw-rw-   0        0        0     6340 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/null.j2
+-rw-rw-rw-   0        0        0      401 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/nb-templates/classic2/index.html.j2
+-rw-rw-rw-   0        0        0    40964 2023-03-06 12:31:02.000000 petljadoc-1.3.1/petljadoc/package.py
+-rw-rw-rw-   0        0        0     2282 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/petlja_builder.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.548086 petljadoc-1.3.1/petljadoc/project-templates/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.921611 petljadoc-1.3.1/petljadoc/project-templates/course/
+-rw-rw-rw-   0        0        0      142 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/project-templates/course/.t.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.922609 petljadoc-1.3.1/petljadoc/project-templates/course/_images/
+-rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.1/petljadoc/project-templates/course/_images/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.923612 petljadoc-1.3.1/petljadoc/project-templates/course/_includes/
+-rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.1/petljadoc/project-templates/course/_includes/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.943872 petljadoc-1.3.1/petljadoc/project-templates/course/_sources/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.971207 petljadoc-1.3.1/petljadoc/project-templates/course/_sources/1_Lesson/
+-rw-rw-rw-   0        0        0     2096 2020-11-30 16:13:38.000000 petljadoc-1.3.1/petljadoc/project-templates/course/_sources/1_Lesson/intro.rst
+-rw-rw-rw-   0        0        0     1564 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/project-templates/course/_sources/1_Lesson/quiz.rst
+-rw-rw-rw-   0        0        0     1368 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/project-templates/course/_sources/index.t.yaml
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.972208 petljadoc-1.3.1/petljadoc/project-templates/course/_static/
+-rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.1/petljadoc/project-templates/course/_static/.gitkeep
+-rw-rw-rw-   0        0        0       75 2023-04-10 05:07:00.000000 petljadoc-1.3.1/petljadoc/project-templates/course/conf-petljadoc.t.json
+-rw-rw-rw-   0        0        0     6291 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/project-templates/course/conf.t.py
+-rw-rw-rw-   0        0        0       33 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/project-templates/course/package-conf.json
+-rw-rw-rw-   0        0        0      777 2020-12-09 14:48:07.000000 petljadoc-1.3.1/petljadoc/project-templates/course/pavement.t.py
+-rw-rw-rw-   0        0        0      110 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/project-templates/course/template_settings.t.json
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.004165 petljadoc-1.3.1/petljadoc/project-templates/runestone/
+-rw-rw-rw-   0        0        0       56 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/.t.gitignore
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.005163 petljadoc-1.3.1/petljadoc/project-templates/runestone/_images/
+-rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_images/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.005163 petljadoc-1.3.1/petljadoc/project-templates/runestone/_includes/
+-rw-rw-rw-   0        0        0        1 2020-11-30 16:13:38.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_includes/.gitkeep
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.033181 petljadoc-1.3.1/petljadoc/project-templates/runestone/_sources/
+-rw-rw-rw-   0        0        0       90 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_sources/index-item.t.md
+-rw-rw-rw-   0        0        0     3337 2020-11-30 16:13:38.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_sources/index.rst
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.128639 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/
+-rw-rw-rw-   0        0        0        0 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/.gitignore
+-rw-rw-rw-   0        0        0    92708 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/activecodethumb.png
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.237152 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/
+-rw-rw-rw-   0        0        0    87168 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.mp3
+-rw-rw-rw-   0        0        0   273068 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.wav
+-rw-rw-rw-   0        0        0   115328 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.mp3
+-rw-rw-rw-   0        0        0   361772 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.wav
+-rw-rw-rw-   0        0        0   310985 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.mp3
+-rw-rw-rw-   0        0        0   978092 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.wav
+-rw-rw-rw-   0        0        0    23942 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/clock.png
+-rw-rw-rw-   0        0        0     4497 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/close.png
+-rw-rw-rw-   0        0        0    16165 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/first.png
+-rw-rw-rw-   0        0        0    15899 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/last.png
+-rw-rw-rw-   0        0        0    15743 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/next.png
+-rw-rw-rw-   0        0        0    15344 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/pause.png
+-rw-rw-rw-   0        0        0    15719 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/prev.png
+-rw-rw-rw-   0        0        0       75 2023-04-10 05:07:00.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/conf-petljadoc.t.json
+-rw-rw-rw-   0        0        0    10633 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/conf.t.py
+-rw-rw-rw-   0        0        0      770 2020-12-09 14:48:07.000000 petljadoc-1.3.1/petljadoc/project-templates/runestone/pavement.t.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.251002 petljadoc-1.3.1/petljadoc/runestone_ext/
+-rw-rw-rw-   0        0        0     1782 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.273348 petljadoc-1.3.1/petljadoc/runestone_ext/associations/
+-rw-rw-rw-   0        0        0       29 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/__init__.py
+-rw-rw-rw-   0        0        0     4629 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/associations.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.274361 petljadoc-1.3.1/petljadoc/runestone_ext/associations/css/
+-rw-rw-rw-   0        0        0     3204 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/css/associations.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.278361 petljadoc-1.3.1/petljadoc/runestone_ext/associations/js/
+-rw-rw-rw-   0        0        0      147 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/js/associations-i18n.en.js
+-rw-rw-rw-   0        0        0      164 2022-11-06 13:07:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/js/associations-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0      144 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/js/associations-i18n.sr-Latn.js
+-rw-rw-rw-   0        0        0      159 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/js/associations-i18n.sr.js
+-rw-rw-rw-   0        0        0     5682 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/associations/js/associations.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.308389 petljadoc-1.3.1/petljadoc/runestone_ext/audio/
+-rw-rw-rw-   0        0        0       20 2019-12-21 09:53:52.000000 petljadoc-1.3.1/petljadoc/runestone_ext/audio/__init__.py
+-rw-rw-rw-   0        0        0     1297 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/audio/audio.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.309392 petljadoc-1.3.1/petljadoc/runestone_ext/audio/test/
+-rw-rw-rw-   0        0        0        0 2019-12-21 09:53:52.000000 petljadoc-1.3.1/petljadoc/runestone_ext/audio/test/sphinx-enki-info.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.326387 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/
+-rw-rw-rw-   0        0        0       27 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/__init__.py
+-rw-rw-rw-   0        0        0     6966 2023-04-07 12:08:56.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/blocklykarel.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.326387 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/css/
+-rw-rw-rw-   0        0        0     2065 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/css/karelBlockly.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.332868 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/
+-rw-rw-rw-   0        0        0    80180 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/acorn_interpreter.js
+-rw-rw-rw-   0        0        0   929342 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/blockly_compressed.js
+-rw-rw-rw-   0        0        0    90975 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/blocks_compressed.js
+-rw-rw-rw-   0        0        0    46593 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/javascript_compressed.js
+-rw-rw-rw-   0        0        0    18815 2023-04-07 22:59:40.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/karelBlockly.js
+-rw-rw-rw-   0        0        0    11952 2023-04-06 17:23:38.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/karelBlocks.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.334878 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/msg/
+-rw-rw-rw-   0        0        0    32475 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/msg/en.js
+-rw-rw-rw-   0        0        0    40621 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/msg/sr.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.363149 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/
+-rw-rw-rw-   0        0        0       25 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/__init__.py
+-rw-rw-rw-   0        0        0     1299 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/blockpylib.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.382745 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.610664 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/
+-rw-rw-rw-   0        0        0   683169 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/blockly_compressed.js
+-rw-rw-rw-   0        0        0    92505 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/blocks_compressed.js
+-rw-rw-rw-   0        0        0    61781 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/msg-sr.js
+-rw-rw-rw-   0        0        0    40010 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/python_compressed.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:58.809358 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/
+-rw-rw-rw-   0        0        0    35053 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter.js
+-rw-rw-rw-   0        0        0     6384 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter_definitions.js
+-rw-rw-rw-   0        0        0     3736 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/ast_node_visitor.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.068357 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/
+-rw-rw-rw-   0        0        0     1888 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/class.js
+-rw-rw-rw-   0        0        0     2178 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comment.js
+-rw-rw-rw-   0        0        0     1116 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comprehensions.js
+-rw-rw-rw-   0        0        0      522 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/decorator.js
+-rw-rw-rw-   0        0        0     3777 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/dict.js
+-rw-rw-rw-   0        0        0     7891 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/if.js
+-rw-rw-rw-   0        0        0     1922 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/io.js
+-rw-rw-rw-   0        0        0    12589 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/lists.js
+-rw-rw-rw-   0        0        0     1799 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/loops.js
+-rw-rw-rw-   0        0        0     8787 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/parking.js
+-rw-rw-rw-   0        0        0      609 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/plots.js
+-rw-rw-rw-   0        0        0     1718 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/sets.js
+-rw-rw-rw-   0        0        0     1263 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/text.js
+-rw-rw-rw-   0        0        0     1831 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/tuple.js
+-rw-rw-rw-   0        0        0     6969 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/turtles.js
+-rw-rw-rw-   0        0        0     4701 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/imported.js
+-rw-rw-rw-   0        0        0     7255 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/python_errors.js
+-rw-rw-rw-   0        0        0    51813 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/python_to_blockly.js
+-rw-rw-rw-   0        0        0    59429 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/pytifa.js
+-rw-rw-rw-   0        0        0     8165 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/utilities.js
+-rw-rw-rw-   0        0        0     9503 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy-modal.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.558088 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.558088 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.559088 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.559088 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.089359 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.560088 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.103361 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
+-rw-rw-rw-   0        0        0    97346 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.133360 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
+-rw-rw-rw-   0        0        0    27731 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.152363 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/
+-rw-rw-rw-   0        0        0       28 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.154359 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/css/
+-rw-rw-rw-   0        0        0     2423 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/css/dbDirective.css
+-rw-rw-rw-   0        0        0     4636 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/dbDirective.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.168357 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/js/
+-rw-rw-rw-   0        0        0    16828 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/js/dbDirective.js
+-rw-rw-rw-   0        0        0    48501 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/js/sql.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.189361 petljadoc-1.3.1/petljadoc/runestone_ext/editor/
+-rw-rw-rw-   0        0        0       21 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.190360 petljadoc-1.3.1/petljadoc/runestone_ext/editor/css/
+-rw-rw-rw-   0        0        0     1771 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/css/editor.css
+-rw-rw-rw-   0        0        0     5287 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/editor.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.196359 petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/
+-rw-rw-rw-   0        0        0       72 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/editor-i18n.en.js
+-rw-rw-rw-   0        0        0      102 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/editor-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0       88 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/editor-i18n.sr-Latn.js
+-rw-rw-rw-   0        0        0       97 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/editor-i18n.sr.js
+-rw-rw-rw-   0        0        0    10712 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/editor.js
+-rw-rw-rw-   0        0        0   385745 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/jszip.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.231359 petljadoc-1.3.1/petljadoc/runestone_ext/gallery/
+-rw-rw-rw-   0        0        0       24 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/gallery/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.232359 petljadoc-1.3.1/petljadoc/runestone_ext/gallery/css/
+-rw-rw-rw-   0        0        0      589 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/gallery/css/gallery.css
+-rw-rw-rw-   0        0        0     4012 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/gallery/gallery.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.233360 petljadoc-1.3.1/petljadoc/runestone_ext/gallery/js/
+-rw-rw-rw-   0        0        0     2096 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/gallery/js/gallery.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.245359 petljadoc-1.3.1/petljadoc/runestone_ext/karel/
+-rw-rw-rw-   0        0        0       20 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.246373 petljadoc-1.3.1/petljadoc/runestone_ext/karel/css/
+-rw-rw-rw-   0        0        0     1080 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/css/karel.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.255090 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/
+-rw-rw-rw-   0        0        0      438 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karel-i18n.en.js
+-rw-rw-rw-   0        0        0      557 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karel-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0      560 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karel-i18n.sr.js
+-rw-rw-rw-   0        0        0     3676 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karel.js
+-rw-rw-rw-   0        0        0     1689 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelChat.js
+-rw-rw-rw-   0        0        0     1455 2023-04-07 12:31:14.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelCorner.js
+-rw-rw-rw-   0        0        0     6683 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelRobot.js
+-rw-rw-rw-   0        0        0    14648 2023-04-07 11:34:03.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelRobotDrawer.js
+-rw-rw-rw-   0        0        0     9995 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelUI.js
+-rw-rw-rw-   0        0        0     5047 2023-04-07 12:30:39.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelWorld.js
+-rw-rw-rw-   0        0        0     5241 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/karel.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.256102 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.566085 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.566085 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.567086 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.266226 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.570087 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.286959 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
+-rw-rw-rw-   0        0        0    97346 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.316960 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
+-rw-rw-rw-   0        0        0    27731 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
+-rw-rw-rw-   0        0        0        0 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/sphinx-enki-info.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.344080 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/
+-rw-rw-rw-   0        0        0       24 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.345079 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/css/
+-rw-rw-rw-   0        0        0     3729 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/css/nimgame.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.352079 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/
+-rw-rw-rw-   0        0        0      406 2022-11-06 13:07:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.en.js
+-rw-rw-rw-   0        0        0      565 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0      455 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr-Latn.js
+-rw-rw-rw-   0        0        0      560 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr.js
+-rw-rw-rw-   0        0        0    13205 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame.js
+-rw-rw-rw-   0        0        0     4655 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/nimgame.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.369833 petljadoc-1.3.1/petljadoc/runestone_ext/notes/
+-rw-rw-rw-   0        0        0       20 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.370845 petljadoc-1.3.1/petljadoc/runestone_ext/notes/css/
+-rw-rw-rw-   0        0        0     3334 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/css/notes.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.371844 petljadoc-1.3.1/petljadoc/runestone_ext/notes/js/
+-rw-rw-rw-   0        0        0     1101 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/js/notes.js
+-rw-rw-rw-   0        0        0     5293 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/notes.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.371844 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.573087 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.574087 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.574087 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.381845 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.575086 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.397940 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
+-rw-rw-rw-   0        0        0    97346 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.416940 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
+-rw-rw-rw-   0        0        0    27731 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.576087 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.423941 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:59.428939 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_sources/
+-rw-rw-rw-   0        0        0      265 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_sources/index.rst.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.080782 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/
+-rw-rw-rw-   0        0        0     6355 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/Blob.js
+-rw-rw-rw-   0        0        0     5120 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/FileSaver.min.js
+-rw-rw-rw-   0        0        0     1511 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/LICENSE.txt
+-rw-rw-rw-   0        0        0     3439 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibility.css
+-rw-rw-rw-   0        0        0     3445 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitydarkest.css
+-rw-rw-rw-   0        0        0     2669 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitylight.css
+-rw-rw-rw-   0        0        0     9490 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.en.js
+-rw-rw-rw-   0        0        0    14677 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0     2096 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.css
+-rw-rw-rw-   0        0        0   103165 2020-02-25 19:14:39.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.js
+-rw-rw-rw-   0        0        0     3903 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/animationbase.js
+-rw-rw-rw-   0        0        0    10912 2020-03-17 13:54:33.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/basic.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.261777 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/
+-rw-rw-rw-   0        0        0   683169 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blockly_compressed.js
+-rw-rw-rw-   0        0        0    92505 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blocks_compressed.js
+-rw-rw-rw-   0        0        0    61781 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/msg-sr.js
+-rw-rw-rw-   0        0        0    40010 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/python_compressed.js
+-rw-rw-rw-   0        0        0   471577 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly_compressed.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.397022 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/
+-rw-rw-rw-   0        0        0    35053 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter.js
+-rw-rw-rw-   0        0        0     6384 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter_definitions.js
+-rw-rw-rw-   0        0        0     3736 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/ast_node_visitor.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.570529 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/
+-rw-rw-rw-   0        0        0     1888 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/class.js
+-rw-rw-rw-   0        0        0     2178 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comment.js
+-rw-rw-rw-   0        0        0     1116 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comprehensions.js
+-rw-rw-rw-   0        0        0      522 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/decorator.js
+-rw-rw-rw-   0        0        0     3777 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/dict.js
+-rw-rw-rw-   0        0        0     7891 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/if.js
+-rw-rw-rw-   0        0        0     1922 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/io.js
+-rw-rw-rw-   0        0        0    12589 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/lists.js
+-rw-rw-rw-   0        0        0     1799 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/loops.js
+-rw-rw-rw-   0        0        0     8787 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/parking.js
+-rw-rw-rw-   0        0        0      609 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/plots.js
+-rw-rw-rw-   0        0        0     1718 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/sets.js
+-rw-rw-rw-   0        0        0     1263 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/text.js
+-rw-rw-rw-   0        0        0     1831 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/tuple.js
+-rw-rw-rw-   0        0        0     6969 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/turtles.js
+-rw-rw-rw-   0        0        0     4701 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/imported.js
+-rw-rw-rw-   0        0        0     7255 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_errors.js
+-rw-rw-rw-   0        0        0    51813 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_to_blockly.js
+-rw-rw-rw-   0        0        0    59429 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/pytifa.js
+-rw-rw-rw-   0        0        0     8165 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/utilities.js
+-rw-rw-rw-   0        0        0     9298 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy-modal.js
+-rw-rw-rw-   0        0        0    55934 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blocks_compressed.js
+-rw-rw-rw-   0        0        0    10606 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bookfuncs.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.579086 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.588321 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/css/
+-rw-rw-rw-   0        0        0   144838 2022-02-03 12:41:00.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.662959 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/
+-rw-rw-rw-   0        0        0    67698 2022-02-03 12:41:15.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0    48907 2022-02-03 12:41:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0      425 2020-03-17 13:54:33.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-sphinx.css
+-rw-rw-rw-   0        0        0     3776 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-sphinx.js
+-rw-rw-rw-   0        0        0    97348 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap.min.css
+-rw-rw-rw-   0        0        0     1123 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.css
+-rw-rw-rw-   0        0        0    16404 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.js
+-rw-rw-rw-   0        0        0    18265 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clike.js
+-rw-rw-rw-   0        0        0     2037 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codelens.js
+-rw-rw-rw-   0        0        0     7507 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.css
+-rw-rw-rw-   0        0        0   320980 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.688962 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css/
+-rw-rw-rw-   0        0        0    31004 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css/font-awesome.min.css
+-rw-rw-rw-   0        0        0    32373 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css.js
+-rw-rw-rw-   0        0        0   111549 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/d3.v2.min.js
+-rw-rw-rw-   0        0        0       95 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/datafile.css
+-rw-rw-rw-   0        0        0     3000 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/datafile.js
+-rw-rw-rw-   0        0        0    19241 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/diff_match_patch.js
+-rw-rw-rw-   0        0        0     6868 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/doctools.js
+-rw-rw-rw-   0        0        0      306 2020-03-17 13:54:33.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      310 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop-i18n.en.js
+-rw-rw-rw-   0        0        0      394 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0     1480 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.css
+-rw-rw-rw-   0        0        0    18311 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.js
+-rw-rw-rw-   0        0        0     1756 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/external.css
+-rw-rw-rw-   0        0        0      130 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb-i18n.en.js
+-rw-rw-rw-   0        0        0      147 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0      182 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb.css
+-rw-rw-rw-   0        0        0    13759 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb.js
+-rw-rw-rw-   0        0        0   127331 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/flatly.min.css
+-rw-rw-rw-   0        0        0    21378 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.css
+-rw-rw-rw-   0        0        0    20664 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.js
+-rw-rw-rw-   0        0        0     5108 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/htmlmixed.js
+-rw-rw-rw-   0        0        0    24396 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript.js
+-rw-rw-rw-   0        0        0    41074 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript_compressed.js
+-rw-rw-rw-   0        0        0   268039 2019-03-09 15:07:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-3.2.1.js
+-rw-rw-rw-   0        0        0      204 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-fix.js
+-rw-rw-rw-   0        0        0     7200 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-migrate-1.2.1.min.js
+-rw-rw-rw-   0        0        0    26010 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.css
+-rw-rw-rw-   0        0        0   217071 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.js
+-rw-rw-rw-   0        0        0     4255 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.ba-bbq.min.js
+-rw-rw-rw-   0        0        0     1418 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.highlight.js
+-rw-rw-rw-   0        0        0     1996 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.hotkey.js
+-rw-rw-rw-   0        0        0     8182 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.idle-timer.js
+-rw-rw-rw-   0        0        0    93069 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.js
+-rw-rw-rw-   0        0        0   120545 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.jsPlumb-1.3.10-all-min.js
+-rw-rw-rw-   0        0        0    40914 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.tablesorter.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.815307 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/
+-rw-rw-rw-   0        0        0    13334 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/CLDRPluralRuleParser.js
+-rw-rw-rw-   0        0        0    13513 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js
+-rw-rw-rw-   0        0        0     5561 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.js
+-rw-rw-rw-   0        0        0     4261 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.fallbacks.js
+-rw-rw-rw-   0        0        0     9027 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.js
+-rw-rw-rw-   0        0        0    12427 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.language.js
+-rw-rw-rw-   0        0        0     3749 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.messagestore.js
+-rw-rw-rw-   0        0        0     8483 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.parser.js
+-rw-rw-rw-   0        0        0      380 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel-i18n.en.js
+-rw-rw-rw-   0        0        0      484 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0      984 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.css
+-rw-rw-rw-   0        0        0     3676 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.js
+-rw-rw-rw-   0        0        0     1105 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelCorner.js
+-rw-rw-rw-   0        0        0     6290 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobot.js
+-rw-rw-rw-   0        0        0    12016 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobotDrawer.js
+-rw-rw-rw-   0        0        0     9995 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelUI.js
+-rw-rw-rw-   0        0        0     4647 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelWorld.js
+-rw-rw-rw-   0        0        0    10847 2020-03-17 13:54:33.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/language_data.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.868354 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/
+-rw-rw-rw-   0        0        0    20731 2022-02-03 12:41:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/hammer.min.js
+-rw-rw-rw-   0        0        0      469 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/prettify.css
+-rw-rw-rw-   0        0        0    17033 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/prettify.js
+-rw-rw-rw-   0        0        0     2541 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.css
+-rw-rw-rw-   0        0        0    27123 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.js
+-rw-rw-rw-   0        0        0      264 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice-i18n.en.js
+-rw-rw-rw-   0        0        0      207 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0    20787 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice.js
+-rw-rw-rw-   0        0        0     3014 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.css
+-rw-rw-rw-   0        0        0    20969 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.js
+-rw-rw-rw-   0        0        0     1335 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/modal-basic.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.581087 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:02.892800 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/js/
+-rw-rw-rw-   0        0        0    28326 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/js/en.js
+-rw-rw-rw-   0        0        0     7117 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/navhelp.js
+-rw-rw-rw-   0        0        0      252 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/notes.css
+-rw-rw-rw-   0        0        0      216 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/notes.js
+-rw-rw-rw-   0        0        0      319 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons-i18n.en.js
+-rw-rw-rw-   0        0        0      370 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0     8848 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.css
+-rw-rw-rw-   0        0        0    97344 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.js
+-rw-rw-rw-   0        0        0     2666 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/petlja.css
+-rw-rw-rw-   0        0        0      417 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/poll.css
+-rw-rw-rw-   0        0        0     6877 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/poll.js
+-rw-rw-rw-   0        0        0     3664 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.css
+-rw-rw-rw-   0        0        0     6290 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.js
+-rw-rw-rw-   0        0        0   231869 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/processing-1.4.1.min.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.067723 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/
+-rw-rw-rw-   0        0        0    84233 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/__init__.js
+-rw-rw-rw-   0        0        0     1888 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/display.js
+-rw-rw-rw-   0        0        0     8368 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/draw.js
+-rw-rw-rw-   0        0        0     3473 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/event.js
+-rw-rw-rw-   0        0        0    11479 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/font.js
+-rw-rw-rw-   0        0        0     4240 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/image.js
+-rw-rw-rw-   0        0        0     6069 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/key.js
+-rw-rw-rw-   0        0        0     1632 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/mouse.js
+-rw-rw-rw-   0        0        0       47 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/pygame.js
+-rw-rw-rw-   0        0        0     6205 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/time.js
+-rw-rw-rw-   0        0        0     5597 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/transform.js
+-rw-rw-rw-   0        0        0      254 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/version.js
+-rw-rw-rw-   0        0        0     1315 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib-init.js
+-rw-rw-rw-   0        0        0     4463 2020-03-17 13:54:33.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygments.css
+-rw-rw-rw-   0        0        0    12629 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python.js
+-rw-rw-rw-   0        0        0    30613 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python_compressed.js
+-rw-rw-rw-   0        0        0    18580 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.css
+-rw-rw-rw-   0        0        0   159859 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.js
+-rw-rw-rw-   0        0        0    44234 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-core.js
+-rw-rw-rw-   0        0        0    26515 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-cssclassapplier.js
+-rw-rw-rw-   0        0        0    14204 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-textrange.js
+-rw-rw-rw-   0        0        0     7907 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/reveal.js
+-rw-rw-rw-   0        0        0    13625 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestone-custom-sphinx-bootstrap.css
+-rw-rw-rw-   0        0        0     4326 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonebase.js
+-rw-rw-rw-   0        0        0     2181 2019-12-21 09:54:12.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonevideo.js
+-rw-rw-rw-   0        0        0    15059 2019-03-10 08:47:02.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/searchtools.js
+-rw-rw-rw-   0        0        0   106155 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sharedb.js
+-rw-rw-rw-   0        0        0        0 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/shortanswer.css
+-rw-rw-rw-   0        0        0     8135 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/shortanswer.js
+-rw-rw-rw-   0        0        0      631 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.css
+-rw-rw-rw-   0        0        0     5939 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.js
+-rw-rw-rw-   0        0        0   472567 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt-stdlib.js
+-rw-rw-rw-   0        0        0   483003 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt.min.js
+-rw-rw-rw-   0        0        0    14765 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortmodels.js
+-rw-rw-rw-   0        0        0     1314 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortviewers.js
+-rw-rw-rw-   0        0        0     6509 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/style.css
+-rw-rw-rw-   0        0        0      526 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.css
+-rw-rw-rw-   0        0        0     6176 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.js
+-rw-rw-rw-   0        0        0    34671 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed.js
+-rw-rw-rw-   0        0        0     2781 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_activecode.js
+-rw-rw-rw-   0        0        0     1380 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_shortanswer.js
+-rw-rw-rw-   0        0        0     1913 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedclickable.js
+-rw-rw-rw-   0        0        0     1885 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timeddnd.js
+-rw-rw-rw-   0        0        0     1806 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedfitb.js
+-rw-rw-rw-   0        0        0     5551 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedmc.js
+-rw-rw-rw-   0        0        0      578 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedparsons.js
+-rw-rw-rw-   0        0        0    35168 2019-03-03 11:08:43.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore-1.3.1.js
+-rw-rw-rw-   0        0        0    12140 2019-03-03 11:08:43.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore.js
+-rw-rw-rw-   0        0        0     1839 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.css
+-rw-rw-rw-   0        0        0     9337 2019-12-21 09:54:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.js
+-rw-rw-rw-   0        0        0      489 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/video.css
+-rw-rw-rw-   0        0        0     8051 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/waypoints.min.js
+-rw-rw-rw-   0        0        0      275 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webgldemo.css
+-rw-rw-rw-   0        0        0     4541 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.css
+-rw-rw-rw-   0        0        0    18025 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.js
+-rw-rw-rw-   0        0        0    25355 2019-03-10 08:47:02.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/websupport.js
+-rw-rw-rw-   0        0        0    12741 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/xml.js
+-rw-rw-rw-   0        0        0      445 2020-03-17 13:54:34.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/searchindex.js
+-rw-rw-rw-   0        0        0        0 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/sphinx-enki-info.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.091723 petljadoc-1.3.1/petljadoc/runestone_ext/p5js/
+-rw-rw-rw-   0        0        0       21 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/p5js/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.096723 petljadoc-1.3.1/petljadoc/runestone_ext/p5js/css/
+-rw-rw-rw-   0        0        0      164 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/p5js/css/p5js.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.110724 petljadoc-1.3.1/petljadoc/runestone_ext/p5js/js/
+-rw-rw-rw-   0        0        0     1646 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/p5js/js/p5js.js
+-rw-rw-rw-   0        0        0     5321 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/runestone_ext/p5js/p5js.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.130723 petljadoc-1.3.1/petljadoc/runestone_ext/pycode/
+-rw-rw-rw-   0        0        0       23 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pycode/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.143723 petljadoc-1.3.1/petljadoc/runestone_ext/pycode/css/
+-rw-rw-rw-   0        0        0     2816 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pycode/css/pycode.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.160723 petljadoc-1.3.1/petljadoc/runestone_ext/pycode/js/
+-rw-rw-rw-   0        0        0    27491 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pycode/js/pycode.js
+-rw-rw-rw-   0        0        0     4032 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pycode/pycode.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.171723 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/
+-rw-rw-rw-   0        0        0       24 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.172724 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.183724 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/
+-rw-rw-rw-   0        0        0    84233 2019-09-27 19:15:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/__init__.js
+-rw-rw-rw-   0        0        0     1888 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/display.js
+-rw-rw-rw-   0        0        0     8368 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/draw.js
+-rw-rw-rw-   0        0        0     3473 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/event.js
+-rw-rw-rw-   0        0        0    11479 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/font.js
+-rw-rw-rw-   0        0        0     4240 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/image.js
+-rw-rw-rw-   0        0        0     6069 2019-09-27 19:15:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/key.js
+-rw-rw-rw-   0        0        0     1632 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/mouse.js
+-rw-rw-rw-   0        0        0       47 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/pygame.js
+-rw-rw-rw-   0        0        0     6205 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/time.js
+-rw-rw-rw-   0        0        0     5597 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/transform.js
+-rw-rw-rw-   0        0        0      254 2021-11-01 13:09:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/version.js
+-rw-rw-rw-   0        0        0     1315 2021-02-02 16:03:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib-init.js
+-rw-rw-rw-   0        0        0       57 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/pygamelib.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.217724 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.588088 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.589086 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.589086 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.230724 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.590087 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.247960 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/
+-rw-rw-rw-   0        0        0    97346 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.271960 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/
+-rw-rw-rw-   0        0        0    27731 2019-09-29 18:46:11.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0     3776 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js
+-rw-rw-rw-   0        0        0     8444 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/conf.py
+-rw-rw-rw-   0        0        0     1822 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/pavement.py
+-rw-rw-rw-   0        0        0        0 2019-11-01 17:26:30.000000 petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/sphinx-enki-info.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.293811 petljadoc-1.3.1/petljadoc/runestone_ext/quizq/
+-rw-rw-rw-   0        0        0       22 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/quizq/__init__.py
+-rw-rw-rw-   0        0        0     1396 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/quizq/quizq.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.312750 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/
+-rw-rw-rw-   0        0        0       27 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.325895 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/css/
+-rw-rw-rw-   0        0        0     2809 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/css/regex-check.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.369363 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/js/
+-rw-rw-rw-   0        0        0      297 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.en.js
+-rw-rw-rw-   0        0        0      379 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0      316 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.sr-Latn.js
+-rw-rw-rw-   0        0        0      374 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/js/regex-check-i18n.sr.js
+-rw-rw-rw-   0        0        0     5874 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/js/regex-check.js
+-rw-rw-rw-   0        0        0     3703 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/regexcheck.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.386142 petljadoc-1.3.1/petljadoc/runestone_ext/simanim/
+-rw-rw-rw-   0        0        0       24 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/simanim/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.387149 petljadoc-1.3.1/petljadoc/runestone_ext/simanim/css/
+-rw-rw-rw-   0        0        0     2332 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/runestone_ext/simanim/css/simanim.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.387149 petljadoc-1.3.1/petljadoc/runestone_ext/simanim/js/
+-rw-rw-rw-   0        0        0    21064 2023-03-06 12:31:02.000000 petljadoc-1.3.1/petljadoc/runestone_ext/simanim/js/simanim.js
+-rw-rw-rw-   0        0        0     4137 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/runestone_ext/simanim/simanim.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.594087 petljadoc-1.3.1/petljadoc/runestone_ext/video/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.594087 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.595087 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.394142 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:03.399141 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_sources/
+-rw-rw-rw-   0        0        0      254 2019-10-06 19:56:26.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_sources/index.rst.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:05.603366 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/
+-rw-rw-rw-   0        0        0     6355 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/Blob.js
+-rw-rw-rw-   0        0        0     5120 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/FileSaver.min.js
+-rw-rw-rw-   0        0        0     1511 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/LICENSE.txt
+-rw-rw-rw-   0        0        0     3439 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibility.css
+-rw-rw-rw-   0        0        0     3445 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitydarkest.css
+-rw-rw-rw-   0        0        0     2669 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitylight.css
+-rw-rw-rw-   0        0        0     9490 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.en.js
+-rw-rw-rw-   0        0        0    14672 2020-12-09 10:35:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0     2096 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.css
+-rw-rw-rw-   0        0        0   102910 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.js
+-rw-rw-rw-   0        0        0     3903 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/animationbase.js
+-rw-rw-rw-   0        0        0    10912 2019-10-06 20:19:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/basic.css
+-rw-rw-rw-   0        0        0   471577 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blockly_compressed.js
+-rw-rw-rw-   0        0        0    55934 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blocks_compressed.js
+-rw-rw-rw-   0        0        0    10606 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bookfuncs.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.597088 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:05.618383 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/css/
+-rw-rw-rw-   0        0        0    97346 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:05.636383 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/js/
+-rw-rw-rw-   0        0        0    27731 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0      425 2019-10-06 20:19:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-sphinx.css
+-rw-rw-rw-   0        0        0     3776 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-sphinx.js
+-rw-rw-rw-   0        0        0    97348 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap.min.css
+-rw-rw-rw-   0        0        0     1123 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.css
+-rw-rw-rw-   0        0        0    16404 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.js
+-rw-rw-rw-   0        0        0    18265 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clike.js
+-rw-rw-rw-   0        0        0     2037 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codelens.js
+-rw-rw-rw-   0        0        0     7507 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.css
+-rw-rw-rw-   0        0        0   320980 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.js
+-rw-rw-rw-   0        0        0    32373 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/css.js
+-rw-rw-rw-   0        0        0   111549 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/d3.v2.min.js
+-rw-rw-rw-   0        0        0       95 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/datafile.css
+-rw-rw-rw-   0        0        0     3000 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/datafile.js
+-rw-rw-rw-   0        0        0    19241 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/diff_match_patch.js
+-rw-rw-rw-   0        0        0     6868 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/doctools.js
+-rw-rw-rw-   0        0        0      307 2019-10-06 20:19:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/documentation_options.js
+-rw-rw-rw-   0        0        0      310 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop-i18n.en.js
+-rw-rw-rw-   0        0        0      389 2020-12-09 10:35:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0     1480 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.css
+-rw-rw-rw-   0        0        0    18311 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.js
+-rw-rw-rw-   0        0        0     1756 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/external.css
+-rw-rw-rw-   0        0        0      130 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb-i18n.en.js
+-rw-rw-rw-   0        0        0      142 2020-12-09 10:35:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0      182 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb.css
+-rw-rw-rw-   0        0        0    13759 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb.js
+-rw-rw-rw-   0        0        0    21378 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.css
+-rw-rw-rw-   0        0        0    20664 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.js
+-rw-rw-rw-   0        0        0     5108 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/htmlmixed.js
+-rw-rw-rw-   0        0        0    24396 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript.js
+-rw-rw-rw-   0        0        0    41074 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript_compressed.js
+-rw-rw-rw-   0        0        0   268039 2019-03-09 15:07:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-3.2.1.js
+-rw-rw-rw-   0        0        0      204 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-fix.js
+-rw-rw-rw-   0        0        0     7200 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-migrate-1.2.1.min.js
+-rw-rw-rw-   0        0        0    26010 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.css
+-rw-rw-rw-   0        0        0   217071 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.js
+-rw-rw-rw-   0        0        0     4255 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.ba-bbq.min.js
+-rw-rw-rw-   0        0        0     1418 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.highlight.js
+-rw-rw-rw-   0        0        0     1996 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.hotkey.js
+-rw-rw-rw-   0        0        0     8182 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.idle-timer.js
+-rw-rw-rw-   0        0        0    93069 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.js
+-rw-rw-rw-   0        0        0   120545 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.jsPlumb-1.3.10-all-min.js
+-rw-rw-rw-   0        0        0    40914 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.tablesorter.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:05.831444 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/
+-rw-rw-rw-   0        0        0    13334 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/CLDRPluralRuleParser.js
+-rw-rw-rw-   0        0        0    13513 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js
+-rw-rw-rw-   0        0        0     5561 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.js
+-rw-rw-rw-   0        0        0     4261 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.fallbacks.js
+-rw-rw-rw-   0        0        0     9027 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.js
+-rw-rw-rw-   0        0        0    12427 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.language.js
+-rw-rw-rw-   0        0        0     3749 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.messagestore.js
+-rw-rw-rw-   0        0        0     8483 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.parser.js
+-rw-rw-rw-   0        0        0    10847 2019-10-06 20:19:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/language_data.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:05.887540 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/
+-rw-rw-rw-   0        0        0    20731 2022-02-03 12:41:37.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/hammer.min.js
+-rw-rw-rw-   0        0        0      469 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/prettify.css
+-rw-rw-rw-   0        0        0    17033 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/prettify.js
+-rw-rw-rw-   0        0        0     2541 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.css
+-rw-rw-rw-   0        0        0    27123 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.js
+-rw-rw-rw-   0        0        0      264 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice-i18n.en.js
+-rw-rw-rw-   0        0        0      202 2020-12-09 10:35:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0    20787 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice.js
+-rw-rw-rw-   0        0        0     3014 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.css
+-rw-rw-rw-   0        0        0    20969 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.js
+-rw-rw-rw-   0        0        0     1335 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/modal-basic.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.598087 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:05.908193 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/js/
+-rw-rw-rw-   0        0        0    28326 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/js/en.js
+-rw-rw-rw-   0        0        0     7117 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/navhelp.js
+-rw-rw-rw-   0        0        0      314 2020-12-09 10:35:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons-i18n.en.js
+-rw-rw-rw-   0        0        0      365 2020-12-09 10:35:50.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons-i18n.sr-Cyrl.js
+-rw-rw-rw-   0        0        0     8848 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.css
+-rw-rw-rw-   0        0        0    97344 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.js
+-rw-rw-rw-   0        0        0      417 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/poll.css
+-rw-rw-rw-   0        0        0     6877 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/poll.js
+-rw-rw-rw-   0        0        0     3664 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.css
+-rw-rw-rw-   0        0        0     6290 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.js
+-rw-rw-rw-   0        0        0   231869 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/processing-1.4.1.min.js
+-rw-rw-rw-   0        0        0     4463 2019-10-06 20:19:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pygments.css
+-rw-rw-rw-   0        0        0    12629 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python.js
+-rw-rw-rw-   0        0        0    30613 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python_compressed.js
+-rw-rw-rw-   0        0        0    18580 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.css
+-rw-rw-rw-   0        0        0   159859 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.js
+-rw-rw-rw-   0        0        0    44234 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-core.js
+-rw-rw-rw-   0        0        0    26515 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-cssclassapplier.js
+-rw-rw-rw-   0        0        0    14204 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-textrange.js
+-rw-rw-rw-   0        0        0     7907 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/reveal.js
+-rw-rw-rw-   0        0        0    13625 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestone-custom-sphinx-bootstrap.css
+-rw-rw-rw-   0        0        0     4326 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonebase.js
+-rw-rw-rw-   0        0        0     2181 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonevideo.js
+-rw-rw-rw-   0        0        0    15059 2019-03-10 08:47:02.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/searchtools.js
+-rw-rw-rw-   0        0        0   106155 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sharedb.js
+-rw-rw-rw-   0        0        0        0 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/shortanswer.css
+-rw-rw-rw-   0        0        0     8135 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/shortanswer.js
+-rw-rw-rw-   0        0        0      631 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.css
+-rw-rw-rw-   0        0        0     5939 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.js
+-rw-rw-rw-   0        0        0   472567 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt-stdlib.js
+-rw-rw-rw-   0        0        0   483003 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt.min.js
+-rw-rw-rw-   0        0        0    14765 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortmodels.js
+-rw-rw-rw-   0        0        0     1314 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortviewers.js
+-rw-rw-rw-   0        0        0     6509 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/style.css
+-rw-rw-rw-   0        0        0      526 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.css
+-rw-rw-rw-   0        0        0     6176 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.js
+-rw-rw-rw-   0        0        0    34671 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed.js
+-rw-rw-rw-   0        0        0     2781 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_activecode.js
+-rw-rw-rw-   0        0        0     1380 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_shortanswer.js
+-rw-rw-rw-   0        0        0     1913 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedclickable.js
+-rw-rw-rw-   0        0        0     1885 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timeddnd.js
+-rw-rw-rw-   0        0        0     1806 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedfitb.js
+-rw-rw-rw-   0        0        0     5551 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedmc.js
+-rw-rw-rw-   0        0        0      578 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedparsons.js
+-rw-rw-rw-   0        0        0    35168 2019-03-03 11:08:43.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore-1.3.1.js
+-rw-rw-rw-   0        0        0    12140 2019-03-03 11:08:43.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore.js
+-rw-rw-rw-   0        0        0     1839 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.css
+-rw-rw-rw-   0        0        0     9337 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.js
+-rw-rw-rw-   0        0        0      489 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/video.css
+-rw-rw-rw-   0        0        0     8051 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/waypoints.min.js
+-rw-rw-rw-   0        0        0      275 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webgldemo.css
+-rw-rw-rw-   0        0        0     4541 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.css
+-rw-rw-rw-   0        0        0    18025 2019-09-29 18:45:24.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.js
+-rw-rw-rw-   0        0        0    25355 2019-03-10 08:47:02.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/websupport.js
+-rw-rw-rw-   0        0        0    12741 2019-09-29 18:45:23.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/xml.js
+-rw-rw-rw-   0        0        0      398 2019-10-06 20:19:31.000000 petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/searchindex.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.010388 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/
+-rw-rw-rw-   0        0        0     4508 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/adlcp_rootv1p2.xsd
+-rw-rw-rw-   0        0        0   100404 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/bundle.js
+-rw-rw-rw-   0        0        0    10462 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/favicon.ico
+-rw-rw-rw-   0        0        0     1236 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/ims_xml.xsd
+-rw-rw-rw-   0        0        0    14820 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/imscp_rootv1p1p2.xsd
+-rw-rw-rw-   0        0        0     1184 2023-03-06 12:31:02.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/imsmanifest.t.xml
+-rw-rw-rw-   0        0        0    19397 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/imsmd_rootv1p2p1.xsd
+-rw-rw-rw-   0        0        0     1525 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/index.t.html
+-rw-rw-rw-   0        0        0    18985 2023-01-10 11:56:30.000000 petljadoc-1.3.1/petljadoc/scorm-proxy-templates/style-player.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.066388 petljadoc-1.3.1/petljadoc/scorm-templates/
+-rw-rw-rw-   0        0        0     4508 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/scorm-templates/adlcp_rootv1p2.xsd
+-rw-rw-rw-   0        0        0     1236 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/scorm-templates/ims_xml.xsd
+-rw-rw-rw-   0        0        0    14820 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/scorm-templates/imscp_rootv1p1p2.xsd
+-rw-rw-rw-   0        0        0    19397 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/scorm-templates/imsmd_rootv1p2p1.xsd
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.071388 petljadoc-1.3.1/petljadoc/themes/
+-rw-rw-rw-   0        0        0       83 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.120388 petljadoc-1.3.1/petljadoc/themes/bc_theme/
+-rw-rw-rw-   0        0        0      386 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/__init__.py
+-rw-rw-rw-   0        0        0     5931 2023-03-15 11:59:27.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/layout.html
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.604086 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.602087 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/en/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.139219 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      968 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/en/LC_MESSAGES/shpinx.mo
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.604086 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.159734 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1260 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.603086 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr@latn/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.148725 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr@latn/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1007 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.605086 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr_RS/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.170158 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr_RS/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1260 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.190761 petljadoc-1.3.1/petljadoc/themes/bc_theme/platform/
+-rw-rw-rw-   0        0        0     8733 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/platform/petljaRTBundle.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.479169 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.606086 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.495169 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/css/
+-rw-rw-rw-   0        0        0   144836 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.555166 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/
+-rw-rw-rw-   0        0        0    67698 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0    48907 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0      906 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-sphinx.css_t
+-rw-rw-rw-   0        0        0     3776 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-sphinx.js
+-rw-rw-rw-   0        0        0   100404 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bundle.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.571167 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/css/
+-rw-rw-rw-   0        0        0    31004 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/css/font-awesome.min.css
+-rw-rw-rw-   0        0        0    10462 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/favicon.ico
+-rw-rw-rw-   0        0        0   127331 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/flatly.min.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.668167 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/
+-rw-rw-rw-   0        0        0   134808 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/FontAwesome.otf
+-rw-rw-rw-   0        0        0   165742 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff2
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:06.862203 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/
+-rw-rw-rw-   0        0        0    69642 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/choice-background.svg
+-rw-rw-rw-   0        0        0    69619 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/dragndrop-background.svg
+-rw-rw-rw-   0        0        0    69642 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/fitb-background.svg
+-rw-rw-rw-   0        0        0      715 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/logo.svg
+-rw-rw-rw-   0        0        0     1224 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/netkabinet-logo-strelica-wt.svg
+-rw-rw-rw-   0        0        0    69646 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/parsons-background.svg
+-rw-rw-rw-   0        0        0      782 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/petlja-logo-wt.svg
+-rw-rw-rw-   0        0        0     1618 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/play_button.svg
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:07.890469 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/
+-rw-rw-rw-   0        0        0     3152 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Facebook.png
+-rw-rw-rw-   0        0        0     3079 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Facebook_icon.png
+-rw-rw-rw-   0        0        0     3728 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Twitter.png
+-rw-rw-rw-   0        0        0     3177 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Twitter_icon.png
+-rw-rw-rw-   0        0        0      231 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/active.png
+-rw-rw-rw-   0        0        0      332 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/completed.png
+-rw-rw-rw-   0        0        0     3482 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/dragndrop-img.svg
+-rw-rw-rw-   0        0        0    18186 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/favicon.ico
+-rw-rw-rw-   0        0        0      640 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/fitb-img.svg
+-rw-rw-rw-   0        0        0     5334 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/green-coin.png
+-rw-rw-rw-   0        0        0      447 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/infonote-img.svg
+-rw-rw-rw-   0        0        0      828 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-ball.png
+-rw-rw-rw-   0        0        0     7370 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-east-balls.png
+-rw-rw-rw-   0        0        0     5362 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-east.png
+-rw-rw-rw-   0        0        0     8203 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-head.png
+-rw-rw-rw-   0        0        0     6942 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-hole.png
+-rw-rw-rw-   0        0        0     5910 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-north-balls.png
+-rw-rw-rw-   0        0        0     7338 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-north.png
+-rw-rw-rw-   0        0        0     6842 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-south-balls.png
+-rw-rw-rw-   0        0        0    12370 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-south.png
+-rw-rw-rw-   0        0        0    65211 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-west-balls.png
+-rw-rw-rw-   0        0        0     7920 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-west.png
+-rw-rw-rw-   0        0        0     2857 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/learnmorenote-img.svg
+-rw-rw-rw-   0        0        0    37014 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/logo.png
+-rw-rw-rw-   0        0        0   102151 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/logo_small.png
+-rw-rw-rw-   0        0        0     1224 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/netkabinet-logo-strelica-wt.svg
+-rw-rw-rw-   0        0        0     1434 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/parsons-img.svg
+-rw-rw-rw-   0        0        0      782 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/petlja-logo-wt.svg
+-rw-rw-rw-   0        0        0     5841 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/play_overlay_icon.png
+-rw-rw-rw-   0        0        0      640 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/qchoice-img.svg
+-rw-rw-rw-   0        0        0     4750 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/question-mark-old.png
+-rw-rw-rw-   0        0        0     1327 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/question-mark.png
+-rw-rw-rw-   0        0        0     1327 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/questionnote-img.svg
+-rw-rw-rw-   0        0        0     3186 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/suggestionnote-img.svg
+-rw-rw-rw-   0        0        0     3662 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/technicalnote-img.svg
+-rw-rw-rw-   0        0        0    24003 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/petlja-course.css
+-rw-rw-rw-   0        0        0     4607 2023-03-06 12:31:02.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/petlja.js
+-rw-rw-rw-   0        0        0    88628 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/require.js
+-rw-rw-rw-   0        0        0    47740 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/simanim-0.0.4-py3-none-any.whl
+-rw-rw-rw-   0        0        0   472567 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/skulpt-stdlib.js
+-rw-rw-rw-   0        0        0   483003 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/skulpt.min.js
+-rw-rw-rw-   0        0        0    18985 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/static/style-player.css
+-rw-rw-rw-   0        0        0     1295 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/bc_theme/theme.conf
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:07.958964 petljadoc-1.3.1/petljadoc/themes/course_theme/
+-rw-rw-rw-   0        0        0      390 2022-11-06 09:12:12.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/__init__.py
+-rw-rw-rw-   0        0        0     5667 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/basic_layout.html
+-rw-rw-rw-   0        0        0     1935 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/course_homepage.html
+-rw-rw-rw-   0        0        0     1653 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/globaltoc.html
+-rw-rw-rw-   0        0        0     7299 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/layout.html
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.611087 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.610088 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/en/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.063336 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      968 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/en/LC_MESSAGES/shpinx.mo
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.611087 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.068346 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1260 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.610088 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr@latn/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.068346 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr@latn/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1007 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.612087 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr_RS/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.074334 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr_RS/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     1260 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo
+-rw-rw-rw-   0        0        0      205 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/localtoc.html
+-rw-rw-rw-   0        0        0      810 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/relations.html
+-rw-rw-rw-   0        0        0      170 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/sourcelink.html
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.229806 petljadoc-1.3.1/petljadoc/themes/course_theme/static/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.613086 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.230805 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/css/
+-rw-rw-rw-   0        0        0   144836 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.233807 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/
+-rw-rw-rw-   0        0        0    67698 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0    48907 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0      906 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-sphinx.css_t
+-rw-rw-rw-   0        0        0     3776 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-sphinx.js
+-rw-rw-rw-   0        0        0      401 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/course-errors.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.234809 petljadoc-1.3.1/petljadoc/themes/course_theme/static/css/
+-rw-rw-rw-   0        0        0    31004 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/css/font-awesome.min.css
+-rw-rw-rw-   0        0        0        0 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/error_log.txt
+-rw-rw-rw-   0        0        0    10462 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/favicon.ico
+-rw-rw-rw-   0        0        0   127323 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/flatly.min.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.240806 petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/
+-rw-rw-rw-   0        0        0   134808 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/FontAwesome.otf
+-rw-rw-rw-   0        0        0   165742 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff2
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.247806 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/
+-rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/choice-background.svg
+-rw-rw-rw-   0        0        0    69619 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/dragndrop-background.svg
+-rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/fitb-background.svg
+-rw-rw-rw-   0        0        0      715 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/logo.svg
+-rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/netkabinet-logo-strelica-wt.svg
+-rw-rw-rw-   0        0        0    69646 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/parsons-background.svg
+-rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/petlja-logo-wt.svg
+-rw-rw-rw-   0        0        0     1618 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/play_button.svg
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.282246 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/
+-rw-rw-rw-   0        0        0     3152 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Facebook.png
+-rw-rw-rw-   0        0        0     3079 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Facebook_icon.png
+-rw-rw-rw-   0        0        0     3728 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Twitter.png
+-rw-rw-rw-   0        0        0     3177 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Twitter_icon.png
+-rw-rw-rw-   0        0        0      231 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/active.png
+-rw-rw-rw-   0        0        0      332 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/completed.png
+-rw-rw-rw-   0        0        0     3482 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/dragndrop-img.svg
+-rw-rw-rw-   0        0        0    18186 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/favicon.ico
+-rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/fitb-img.svg
+-rw-rw-rw-   0        0        0     5334 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/green-coin.png
+-rw-rw-rw-   0        0        0      447 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/infonote-img.svg
+-rw-rw-rw-   0        0        0      828 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-ball.png
+-rw-rw-rw-   0        0        0     7370 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-east-balls.png
+-rw-rw-rw-   0        0        0     5362 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-east.png
+-rw-rw-rw-   0        0        0     8203 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-head.png
+-rw-rw-rw-   0        0        0     6942 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-hole.png
+-rw-rw-rw-   0        0        0     5910 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-north-balls.png
+-rw-rw-rw-   0        0        0     7338 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-north.png
+-rw-rw-rw-   0        0        0     6842 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-south-balls.png
+-rw-rw-rw-   0        0        0    12370 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-south.png
+-rw-rw-rw-   0        0        0    65211 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-west-balls.png
+-rw-rw-rw-   0        0        0     7920 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-west.png
+-rw-rw-rw-   0        0        0     2857 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/learnmorenote-img.svg
+-rw-rw-rw-   0        0        0    37014 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/logo.png
+-rw-rw-rw-   0        0        0   102151 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/logo_small.png
+-rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/netkabinet-logo-strelica-wt.svg
+-rw-rw-rw-   0        0        0     1434 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/parsons-img.svg
+-rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/petlja-logo-wt.svg
+-rw-rw-rw-   0        0        0     5841 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/play_overlay_icon.png
+-rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/qchoice-img.svg
+-rw-rw-rw-   0        0        0     4750 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/question-mark-old.png
+-rw-rw-rw-   0        0        0     1327 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/question-mark.png
+-rw-rw-rw-   0        0        0     1327 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/questionnote-img.svg
+-rw-rw-rw-   0        0        0     3186 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/suggestionnote-img.svg
+-rw-rw-rw-   0        0        0     3662 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/technicalnote-img.svg
+-rw-rw-rw-   0        0        0   264982 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/nbstyle.css
+-rw-rw-rw-   0        0        0    23457 2022-12-02 13:00:34.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/petlja-course.css
+-rw-rw-rw-   0        0        0     7082 2022-11-20 11:14:54.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/petlja.js
+-rw-rw-rw-   0        0        0    88628 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/require.js
+-rw-rw-rw-   0        0        0    47740 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/simanim-0.0.4-py3-none-any.whl
+-rw-rw-rw-   0        0        0   472567 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/skulpt-stdlib.js
+-rw-rw-rw-   0        0        0   483003 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/static/skulpt.min.js
+-rw-rw-rw-   0        0        0      859 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/subchapter.html
+-rw-rw-rw-   0        0        0     1297 2022-11-03 09:45:51.000000 petljadoc-1.3.1/petljadoc/themes/course_theme/theme.conf
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.383962 petljadoc-1.3.1/petljadoc/themes/runestone_theme/
+-rw-rw-rw-   0        0        0      537 2020-12-09 14:48:07.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/__init__.py
+-rw-rw-rw-   0        0        0     8162 2020-12-29 14:15:02.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/basic_layout.html
+-rw-rw-rw-   0        0        0      372 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/globaltoc.html
+-rw-rw-rw-   0        0        0     5342 2023-03-06 12:31:02.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/layout.html
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.619087 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.618087 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/en/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.389963 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      566 2020-12-09 14:48:07.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/en/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.619087 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.400717 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      689 2020-12-09 14:48:07.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.618087 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr@latn/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.394961 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr@latn/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      655 2020-12-29 14:15:02.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.620086 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr_RS/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.401732 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr_RS/LC_MESSAGES/
+-rw-rw-rw-   0        0        0      689 2020-12-29 14:15:02.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo
+-rw-rw-rw-   0        0        0      187 2020-12-08 00:51:34.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/localtoc.html
+-rw-rw-rw-   0        0        0     1262 2020-12-09 14:48:07.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/relations.html
+-rw-rw-rw-   0        0        0      170 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/sourcelink.html
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.651963 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.621086 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.679961 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/css/
+-rw-rw-rw-   0        0        0   144838 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.738043 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/
+-rw-rw-rw-   0        0        0    67698 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0        0        0    48907 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js
+-rw-rw-rw-   0        0        0      906 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.css_t
+-rw-rw-rw-   0        0        0     3776 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.js
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.749061 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/css/
+-rw-rw-rw-   0        0        0    31004 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/css/font-awesome.min.css
+-rw-rw-rw-   0        0        0        0 2020-12-29 14:15:02.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/error_log.txt
+-rw-rw-rw-   0        0        0    10462 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/favicon.ico
+-rw-rw-rw-   0        0        0   127331 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/flatly.min.css
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.847176 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/
+-rw-rw-rw-   0        0        0   134808 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/FontAwesome.otf
+-rw-rw-rw-   0        0        0   165742 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.eot
+-rw-rw-rw-   0        0        0   447050 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.svg
+-rw-rw-rw-   0        0        0   165548 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.ttf
+-rw-rw-rw-   0        0        0    98024 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff
+-rw-rw-rw-   0        0        0    77160 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff2
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:08.946294 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/
+-rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/choice-background.svg
+-rw-rw-rw-   0        0        0    69619 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/dragndrop-background.svg
+-rw-rw-rw-   0        0        0    69642 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/fitb-background.svg
+-rw-rw-rw-   0        0        0      715 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/logo.svg
+-rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/netkabinet-logo-strelica-wt.svg
+-rw-rw-rw-   0        0        0    69646 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/parsons-background.svg
+-rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/petlja-logo-wt.svg
+-rw-rw-rw-   0        0        0     1618 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/play_button.svg
+drwxrwxrwx   0        0        0        0 2023-04-10 05:44:09.214965 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/
+-rw-rw-rw-   0        0        0     3152 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Facebook.png
+-rw-rw-rw-   0        0        0     3079 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Facebook_icon.png
+-rw-rw-rw-   0        0        0     3728 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Twitter.png
+-rw-rw-rw-   0        0        0     3177 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Twitter_icon.png
+-rw-rw-rw-   0        0        0      231 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/active.png
+-rw-rw-rw-   0        0        0      332 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/completed.png
+-rw-rw-rw-   0        0        0     3482 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/dragndrop-img.svg
+-rw-rw-rw-   0        0        0    18186 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/favicon.ico
+-rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/fitb-img.svg
+-rw-rw-rw-   0        0        0     5334 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/green-coin.png
+-rw-rw-rw-   0        0        0      447 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/infonote-img.svg
+-rw-rw-rw-   0        0        0    10414 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-ball.png
+-rw-rw-rw-   0        0        0    19798 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-east.png
+-rw-rw-rw-   0        0        0     8203 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-head.png
+-rw-rw-rw-   0        0        0     6942 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-hole.png
+-rw-rw-rw-   0        0        0    13690 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-north.png
+-rw-rw-rw-   0        0        0    14972 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-south.png
+-rw-rw-rw-   0        0        0    19805 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-west.png
+-rw-rw-rw-   0        0        0     2857 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/learnmorenote-img.svg
+-rw-rw-rw-   0        0        0    37014 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/logo.png
+-rw-rw-rw-   0        0        0   102151 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/logo_small.png
+-rw-rw-rw-   0        0        0     1224 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/netkabinet-logo-strelica-wt.svg
+-rw-rw-rw-   0        0        0     1434 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/parsons-img.svg
+-rw-rw-rw-   0        0        0      782 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/petlja-logo-wt.svg
+-rw-rw-rw-   0        0        0     5841 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/play_overlay_icon.png
+-rw-rw-rw-   0        0        0      640 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/qchoice-img.svg
+-rw-rw-rw-   0        0        0     4750 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/question-mark-old.png
+-rw-rw-rw-   0        0        0     1327 2022-01-26 16:39:18.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/question-mark.png
+-rw-rw-rw-   0        0        0     1327 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/questionnote-img.svg
+-rw-rw-rw-   0        0        0     3186 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/suggestionnote-img.svg
+-rw-rw-rw-   0        0        0     3662 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/technicalnote-img.svg
+-rw-rw-rw-   0        0        0   277929 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/nbstyle.css
+-rw-rw-rw-   0        0        0     2821 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/petlja-runestone.css
+-rw-rw-rw-   0        0        0        0 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/petlja_ruenstone.js
+-rw-rw-rw-   0        0        0    88628 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/require.js
+-rw-rw-rw-   0        0        0    47740 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/simanim-0.0.4-py3-none-any.whl
+-rw-rw-rw-   0        0        0   472567 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/skulpt-stdlib.js
+-rw-rw-rw-   0        0        0   483003 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/skulpt.min.js
+-rw-rw-rw-   0        0        0     1264 2020-12-09 14:48:07.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/subchapter.html
+-rw-rw-rw-   0        0        0     1297 2020-12-04 12:05:37.000000 petljadoc-1.3.1/petljadoc/themes/runestone_theme/theme.conf
+-rw-rw-rw-   0        0        0     4478 2022-11-06 13:07:32.000000 petljadoc-1.3.1/petljadoc/util.py
+drwxrwxrwx   0        0        0        0 2023-04-10 05:43:57.757089 petljadoc-1.3.1/petljadoc.egg-info/
+-rw-rw-rw-   0        0        0     2389 2023-04-10 05:43:56.000000 petljadoc-1.3.1/petljadoc.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    51038 2023-04-10 05:43:57.000000 petljadoc-1.3.1/petljadoc.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 05:43:56.000000 petljadoc-1.3.1/petljadoc.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      293 2023-04-10 05:43:56.000000 petljadoc-1.3.1/petljadoc.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2019-09-30 21:36:41.000000 petljadoc-1.3.1/petljadoc.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      195 2023-04-10 05:43:56.000000 petljadoc-1.3.1/petljadoc.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-10 05:43:56.000000 petljadoc-1.3.1/petljadoc.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      210 2023-03-06 12:48:22.000000 petljadoc-1.3.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-04-10 05:44:09.215963 petljadoc-1.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1707 2022-11-20 11:14:54.000000 petljadoc-1.3.1/setup.py
```

### Comparing `petljadoc-1.3.0/LICENSE` & `petljadoc-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/PKG-INFO` & `petljadoc-1.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petljadoc
-Version: 1.3.0
+Version: 1.3.1
 Summary: Petlja's command-line interface for learning content
 Home-page: https://github.com/Petlja/PetljaDoc
 Author: Fondacija Petlja
 Author-email: team@petlja.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `petljadoc-1.3.0/README.md` & `petljadoc-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/cli.py` & `petljadoc-1.3.1/petljadoc/cli.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/course.py` & `petljadoc-1.3.1/petljadoc/course.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/nb-templates/classic2/base/base.html.j2` & `petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/base.html.j2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/nb-templates/classic2/base/display_priority.j2` & `petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/display_priority.j2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/nb-templates/classic2/base/jupyter_widgets.html.j2` & `petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/jupyter_widgets.html.j2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/nb-templates/classic2/base/mathjax.html.j2` & `petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/mathjax.html.j2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/nb-templates/classic2/base/null.j2` & `petljadoc-1.3.1/petljadoc/nb-templates/classic2/base/null.j2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/package.py` & `petljadoc-1.3.1/petljadoc/package.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/petlja_builder.py` & `petljadoc-1.3.1/petljadoc/petlja_builder.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/course/_sources/1_Lesson/intro.rst` & `petljadoc-1.3.1/petljadoc/project-templates/course/_sources/1_Lesson/intro.rst`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/course/_sources/1_Lesson/quiz.rst` & `petljadoc-1.3.1/petljadoc/project-templates/course/_sources/1_Lesson/quiz.rst`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/course/_sources/index.t.yaml` & `petljadoc-1.3.1/petljadoc/project-templates/course/_sources/index.t.yaml`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/course/conf.t.py` & `petljadoc-1.3.1/petljadoc/project-templates/course/conf.t.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/course/pavement.t.py` & `petljadoc-1.3.1/petljadoc/project-templates/course/pavement.t.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_sources/index.rst` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_sources/index.rst`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/activecodethumb.png` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/activecodethumb.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.mp3` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.mp3`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.wav` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line01.wav`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.mp3` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.mp3`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.wav` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line02.wav`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.mp3` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.mp3`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.wav` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/audio/Example04_Tour01_Line03.wav`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/clock.png` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/clock.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/close.png` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/close.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/first.png` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/first.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/last.png` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/last.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/next.png` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/next.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/pause.png` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/pause.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/_static/prev.png` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/_static/prev.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/conf.t.py` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/conf.t.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/project-templates/runestone/pavement.t.py` & `petljadoc-1.3.1/petljadoc/project-templates/runestone/pavement.t.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/__init__.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/__init__.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/associations/associations.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/associations/associations.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/associations/css/associations.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/associations/css/associations.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/associations/js/associations.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/associations/js/associations.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/audio/audio.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/audio/audio.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockly/blocklykarel.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/blocklykarel.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         """
         generate html to include Karel box.
         :param self:
         :return:
         """
 
         env = self.state.document.settings.env
-        categories = ["KarelCommands", "BeginnerKarelCommands","KarelBrain","Values", "Branching", "KarelBranching", "Loops", "KarelLoops", "Logic", "KarelSays", "Arithmetic"]
+        categories = ["KarelCommands", "BeginnerKarelCommands","KarelBrain","Values", "Branching", "KarelBranching", "Loops", "KarelLoops", "Arithmetic", "Logic", "KarelSays", "AskUser", "Vars"]
         self.options['name'] = self.arguments[0].strip()
         self.options['divid'] = self.arguments[0]
 
         if not self.options['divid']:
             raise Exception("No divid")
```

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockly/css/karelBlockly.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/css/karelBlockly.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/acorn_interpreter.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/acorn_interpreter.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/blockly_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/blockly_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/blocks_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/blocks_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/javascript_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/javascript_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/karelBlockly.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/karelBlockly.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,13 @@
 "use strict";
 
 function WrappingBlicky() {
     var ScrollDebounce = {};
     var ScrollDebounceLog = {};
+    var resetInterpreter = {};
     $(document).ready(function() {
         var errorText = {};
 
         errorText.ErrorTitle = $.i18n("msg_activecode_error_title");
         errorText.DescriptionTitle = $.i18n("msg_activecode_description_title");
         errorText.ToFixTitle = $.i18n("msg_activecode_to_fix_title");
         errorText.ParseError = $.i18n("msg_activecode_parse_error");
@@ -109,15 +110,15 @@
                     "kind": "block",
                     "type": "count_balls",
                 }, ]
             },
             'Values': {
                 "kind": "category",
                 "name": "Вредности",
-                "colour": 110,
+                "colour": 250,
                 "contents": [{
                     "kind": "block",
                     "type": "math_number",
                 }, ]
             },
             'Branching': {
                 "kind": "category",
@@ -139,73 +140,97 @@
                     "kind": "block",
                     "type": "controls_if_simple",
                 }, {
                     "kind": "block",
                     "type": "controls_ifelse_simple",
                 }, ]
             },
+            'Vars': {
+                "kind": "category",
+                "colour": 310,
+                "name": "Променљиве",
+                "custom": "VARIABLE",
+            },
             'Loops': {
                 "kind": "category",
                 "name": "Петље",
                 "colour": 190,
                 "contents": [{
                     "kind": "block",
                     "type": "controls_repeat"
                 }, {
                     "kind": "block",
+                    "type": "controls_repeat_ext",
+                }, {
+                    "kind": "block",
                     "type": "controls_whileUntil"
-                }]
+                }, ]
             },
             'KarelLoops': {
                 "kind": "category",
                 "name": "Петље робот",
                 "colour": 210,
                 "contents": [{
                     "kind": "block",
                     "type": "karel_controls_whileUntil"
                 }, ]
             },
             'Logic': {
                 "kind": "category",
                 "name": "Логички оператори",
-                "colour": 240,
+                "colour": 220,
                 "contents": [{
                     "kind": "block",
                     "type": "logic_compare",
                 }, {
                     "kind": "block",
                     "type": "logic_operation",
                 }, {
                     "kind": "block",
                     "type": "logic_negate",
                 }, ]
             },
             'Arithmetic': {
                 "kind": "category",
                 "name": "Аритметикa",
-                "colour": 270,
+                "colour": 215,
                 "contents": [{
                     "kind": "block",
                     "type": "math_number",
                 }, {
                     "kind": "block",
                     "type": "math_arithmetic",
                 }, ]
             },
             'KarelSays': {
                 "kind": "category",
                 "name": "Поруке роботу",
-                "colour": 290,
+                "colour": 245,
                 "contents": [{
                     "kind": "block",
                     "type": "text_print",
                 }, ]
             },
+            'AskUser': {
+                "kind": "category",
+                "name": "Помози роботу",
+                "colour": 290,
+                "contents": [{
+                    "kind": "block",
+                    "type": "number_prompt",
+                }]
+            }
         }
 
+        const startBlocks = {
+            "variables": [{
+                "name": "x",
+                "id": "x"
+            }]
+        };
 
         $('[data-component=blocklyKarel]').each(function(index) {
             var toolboxType = "";
             if (this.hasAttribute("data-flyoutToolbox"))
                 toolboxType = "flyoutToolbox"
             else
                 toolboxType = "categoryToolbox"
@@ -237,21 +262,23 @@
                 for (var i = 0; i < categoriesFilter.length; i++)
                     toolbox.contents.push(categories[categoriesFilter[i]]);
             }
             var workspace = Blockly.inject(karelConfigDiv, {
                 toolbox: toolbox,
                 trashcan: true
             });
+            Blockly.serialization.workspaces.load(startBlocks, workspace);
 
             var setup = config.setup();
             if (setup.hasOwnProperty('domXml')) {
                 var domXml = setup.domXml;
                 Blockly.Xml.domToWorkspace(workspace, Blockly.Xml.textToDom(domXml))
             }
-            ScrollDebounce[workspace.id] = true
+            ScrollDebounce[workspace.id] = true;
+            resetInterpreter[workspace.id] = false;
 
             var robot = setup.robot;
             var world = setup.world;
             var node = this.querySelector(".chat-window");
             var chat = new Chat(node);
             robot.setChat(chat);
             robot.setWorld(world);
@@ -342,24 +369,27 @@
                 drawer.drawFrame(robot);
                 var code = Blockly.JavaScript.workspaceToCode(workspace);
                 var myInterpreter = new Interpreter(code, initApi);
                 drawer.start()
 
                 function nextStep() {
                     try {
-                        if (myInterpreter.step()) {
+                        if (myInterpreter.step() && !resetInterpreter[workspace.id]) {
                             setTimeout(nextStep, 65);
                         } else {
                             $('.run-button').removeAttr('disabled', 'disabled');
                             var result = config.isSuccess(robot, world);
                             if (result) {
                                 showEndMessageSuccess();
                             } else {
-                                showEndMessageError($.i18n("msg_karel_incorrect"));
+                                if (!resetInterpreter[workspace.id])
+                                    showEndMessageError($.i18n("msg_karel_incorrect"));
                             }
+                            if (resetInterpreter[workspace.id])
+                                resetInterpreter[workspace.id] = false
                         }
                     } catch (err) {
                         $('.run-button').removeAttr('disabled', 'disabled');
                         drawer.stop(function() {
                             var message = "";
                             var otherError = false;
                             if ((err == "crashed") || (err == "no_ball") || (err == "out_of_bounds") || (err == "no_balls_with_robot"))
@@ -375,14 +405,15 @@
                     }
                 }
                 nextStep();
             });
 
             karelCongrolosDiv.querySelector(".reset-button").addEventListener("click", function() {
                 workspace.getAllBlocks().forEach(a => a.setHighlighted(!1));
+                resetInterpreter[workspace.id] = true;
                 clearError();
                 reset();
             });
             document.getElementsByClassName("lectureContentMaterial")[0].addEventListener('scroll', function() {
                 if (ScrollDebounce[workspace.id]) {
                     ScrollDebounce[workspace.id] = false;
                     workspace.updateScreenCalculations_();
```

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/karelBlocks.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/karelBlocks.js`

 * *Files 10% similar despite different names*

#### js-beautify {}

```diff
@@ -350,8 +350,65 @@
             'style': 'logic_blocks',
             'tooltip': '%{BKYCONTROLS_IF_TOOLTIP_2}',
             'helpUrl': '%{BKY_CONTROLS_IF_HELPURL}',
             'suppressPrefixSuffix': true,
             'extensions': ['controls_if_tooltip'],
         }, )
     }
-}
+}
+Blockly.Blocks['variables_get'] = {
+    init: function() {
+        this.jsonInit({
+            'type': 'variables_get',
+            'message0': '%1',
+            'args0': [{
+                'type': 'field_variable',
+                'name': 'VAR',
+                'variable': 'x',
+            }, ],
+            'output': null,
+            'style': 'variable_blocks',
+            'helpUrl': '%{BKY_VARIABLES_GET_HELPURL}',
+            'tooltip': '%{BKY_VARIABLES_GET_TOOLTIP}',
+            'extensions': ['contextMenu_variableSetterGetter'],
+        }, )
+    }
+}
+Blockly.Blocks['variables_set'] = {
+    init: function() {
+        this.jsonInit({
+            'type': 'variables_set',
+            'message0': 'У %1 постави %2',
+            'args0': [{
+                'type': 'field_variable',
+                'name': 'VAR',
+                'variable': 'x',
+            }, {
+                'type': 'input_value',
+                'name': 'VALUE',
+            }, ],
+            'previousStatement': null,
+            'nextStatement': null,
+            'style': 'variable_blocks',
+            'tooltip': '%{BKY_VARIABLES_SET_TOOLTIP}',
+            'helpUrl': '%{BKY_VARIABLES_SET_HELPURL}',
+            'extensions': ['contextMenu_variableSetterGetter'],
+        }, )
+    }
+}
+Blockly.Blocks['number_prompt'] = {
+    init: function() {
+        this.appendDummyInput()
+            .appendField("Питај ")
+            .appendField(new Blockly.FieldTextInput(""), "PROMPT");
+        this.setOutput(true, "Number");
+        this.setColour(230);
+        this.setTooltip("");
+        this.setHelpUrl("");
+    }
+};
+
+Blockly.JavaScript['number_prompt'] = function(block) {
+    var promptText = block.getFieldValue('PROMPT');
+    var code = 'parseFloat(window.prompt(' + JSON.stringify(promptText) + '))';
+    return [code, Blockly.JavaScript.ORDER_ATOMIC];
+};
```

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/msg/en.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/msg/en.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockly/js/msg/sr.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockly/js/msg/sr.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/blockpylib.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/blockpylib.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockly/blockly_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/blockly_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockly/blocks_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/blocks_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockly/msg-sr.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/msg-sr.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockly/python_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockly/python_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter_definitions.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/abstract_interpreter_definitions.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/ast_node_visitor.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/ast_node_visitor.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/class.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/class.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comment.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comment.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comprehensions.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/comprehensions.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/decorator.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/decorator.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/dict.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/dict.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/if.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/if.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/io.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/io.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/lists.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/lists.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/loops.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/loops.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/parking.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/parking.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/plots.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/plots.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/sets.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/sets.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/text.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/text.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/tuple.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/tuple.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/turtles.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/blocks/turtles.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/imported.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/imported.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/python_errors.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/python_errors.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/python_to_blockly.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/python_to_blockly.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/pytifa.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/pytifa.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy/utilities.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy/utilities.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/js/blockpy-modal.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/js/blockpy-modal.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/blockpylib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/dbDirective/css/dbDirective.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/css/dbDirective.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/dbDirective/dbDirective.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/dbDirective.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/dbDirective/js/dbDirective.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/js/dbDirective.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/dbDirective/js/sql.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/dbDirective/js/sql.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/editor/css/editor.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/editor/css/editor.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/editor/editor.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/editor/editor.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/editor/js/editor.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/editor.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/editor/js/jszip.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/editor/js/jszip.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/gallery/css/gallery.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/gallery/css/gallery.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/gallery/gallery.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/gallery/gallery.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/gallery/js/gallery.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/gallery/js/gallery.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/karel/css/karel.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/karel/css/karel.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karel-i18n.sr-Cyrl.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karel-i18n.sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karel-i18n.sr.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karel-i18n.sr.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karel.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karel.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karelChat.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelChat.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karelCorner.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelCorner.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karelRobot.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelRobot.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karelRobotDrawer.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelRobotDrawer.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -302,30 +302,35 @@
         var ctx = this.context;
 
 
         for (var a = 1; a <= world.getAvenues(); a++) {
             for (var s = 1; s <= world.getStreets(); s++) {
                 if (world.checkBall(a, s) || world.checkHole(a, s)) {
                     var pt = worldToScreen.call(this, a, s);
-                    var img, width, height;
+                    var img, width, height, has_balls;
                     if (world.checkBall(a, s)) {
                         width = 0.4 * this.cell_width;
                         height = 0.4 * this.cell_height;
                         img = KarelImages.get().images().ball;
                         fontStyle = "black";
+                        has_balls = true
                     } else {
                         width = 0.8 * this.cell_width;
                         height = 0.8 * this.cell_height;
                         img = KarelImages.get().images().hole;
                         fontStyle = "white";
                     }
                     ctx.drawImage(img, pt.x - width / 2, pt.y - height / 2, width, height);
 
                     var fontSize = 15;
-                    var nb = Math.abs(world.getBalls(a, s)).toString();
+                    var nb;
+                    if (has_balls && world.showNumberOfBalls(a, s))
+                        nb = Math.abs(world.getBalls(a, s)).toString();
+                    else
+                        nb = '?'
 
                     while (true) {
                         ctx.fillStyle = fontStyle;
                         ctx.font = fontSize + "px Arial";
                         var text_width = ctx.measureText(nb).width;
                         var text_height = getTextHeight(ctx.font).ascent; // this text is digits only, so ascent is enough
                         if (fontSize <= 8) break;
```

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karelUI.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelUI.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/karel/js/karelWorld.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelWorld.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/karel/karel.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/karel/karel.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/karel/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/css/nimgame.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/css/nimgame.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr-Cyrl.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame-i18n.sr.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/js/nimgame.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/js/nimgame.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/nimgame/nimgame.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/nimgame/nimgame.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/css/notes.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/css/notes.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/js/notes.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/js/notes.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/notes.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/notes.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/Blob.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/Blob.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/FileSaver.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/FileSaver.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/LICENSE.txt` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibility.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibility.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitydarkest.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitydarkest.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitylight.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/accessibilitylight.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.en.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.en.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.sr-Cyrl.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode-i18n.sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/activecode.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/animationbase.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/animationbase.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/basic.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/basic.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blockly_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blockly_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blocks_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/blocks_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/msg-sr.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/msg-sr.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/python_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly/python_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockly_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter_definitions.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/abstract_interpreter_definitions.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/ast_node_visitor.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/ast_node_visitor.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/class.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/class.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comment.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comment.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comprehensions.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/comprehensions.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/decorator.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/decorator.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/dict.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/dict.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/if.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/if.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/io.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/io.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/lists.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/lists.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/loops.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/loops.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/parking.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/parking.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/plots.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/plots.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/sets.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/sets.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/text.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/text.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/tuple.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/tuple.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/turtles.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/blocks/turtles.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/imported.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/imported.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_errors.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_errors.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_to_blockly.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/python_to_blockly.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/pytifa.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/pytifa.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/utilities.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy/utilities.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy-modal.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blockpy-modal.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blocks_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/blocks_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bookfuncs.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bookfuncs.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/css/bootstrap.min.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-4.0.0-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-sphinx.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap.min.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clickable.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clike.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/clike.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codelens.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codelens.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/codemirror.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css/font-awesome.min.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/css.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/d3.v2.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/d3.v2.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/datafile.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/datafile.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/diff_match_patch.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/diff_match_patch.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/doctools.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/dragndrop.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/external.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/external.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/fitb.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/flatly.min.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/flatly.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/guiders-1.3.0.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/htmlmixed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/htmlmixed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/javascript_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-3.2.1.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-migrate-1.2.1.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-migrate-1.2.1.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery-ui-1.10.3.custom.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.ba-bbq.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.ba-bbq.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.highlight.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.highlight.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.hotkey.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.hotkey.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.idle-timer.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.idle-timer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.jsPlumb-1.3.10-all-min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.jsPlumb-1.3.10-all-min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.tablesorter.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery.tablesorter.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/CLDRPluralRuleParser.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/CLDRPluralRuleParser.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.emitter.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.fallbacks.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.fallbacks.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.language.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.language.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.messagestore.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.messagestore.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.parser.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/jquery_i18n/jquery.i18n.parser.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karel.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelCorner.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelCorner.js`

 * *Files 20% similar despite different names*

#### js-beautify {}

```diff
@@ -1,12 +1,13 @@
 var Corner = (function() {
     function Corner(a, s) {
         this.avenue = a;
         this.street = s;
         this.numBalls = 0;
+        this.areBallsVisible = true;
         this.wallToNorth = false;
         this.wallToEast = false;
     }
 
     Corner.prototype.clone = function() {
         var c = new Corner(this.avenue, this.street);
 
@@ -19,16 +20,21 @@
         return c;
     };
 
     Corner.prototype.setBalls = function(n) {
         this.numBalls = n;
     };
 
+    Corner.prototype.setHiddenBalls = function(n) {
+        this.numBalls = n;
+        this.areBallsVisible = false;
+    };
+
     Corner.prototype.getBalls = function() {
-        return this.numBalls;
+        return this.numBalls
     };
 
     Corner.prototype.setNorthWall = function(w) {
         this.wallToNorth = w;
     };
 
     Corner.prototype.hasNorthWall = function() {
@@ -39,9 +45,15 @@
         this.wallToEast = w;
     };
 
     Corner.prototype.hasEastWall = function() {
         return this.wallToEast;
     };
 
+    Corner.prototype.showNumberOfBalls = function() {
+        var returnValue = this.areBallsVisible;
+        this.areBallsVisible = false;
+        return returnValue;
+    };
+
     return Corner;
 })();
```

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobot.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobot.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobotDrawer.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelRobotDrawer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelUI.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelUI.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/karelWorld.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/karel/js/karelWorld.js`

 * *Files 5% similar despite different names*

#### js-beautify {}

```diff
@@ -3,14 +3,15 @@
         this.numAvenues = avenues;
         this.numStreets = streets;
         this.corners = [];
         this.robotStartAvenue = 0;
         this.robotStartStreet = 0;
         this.robotStartDirection = "N";
         this.robotStartBalls = 0;
+        this.args = {}
 
         for (var av = 0; av < avenues; av++) {
             var avenue = [];
             for (var st = 0; st < streets; st++) {
                 avenue.push(new Corner(av + 1, st + 1));
             }
             this.corners.push(avenue);
@@ -120,14 +121,18 @@
         if (this.getBalls(a, s) > 0) {
             this.setBalls(a, s, this.getBalls(a, s) - 1);
             return true;
         }
         throw "no_ball";
     };
 
+    World.prototype.putHiddenNumberOfBalls = function(a, s, n) {
+        return this.getCorner(a, s).setHiddenBalls(n);
+    }
+
     World.prototype.putBall = function(a, s) {
         this.setBalls(a, s, this.getBalls(a, s) + 1);
     };
 
     World.prototype.putBalls = function(a, s, n) {
         for (var i = 0; i < n; i++)
             this.putBall(a, s);
@@ -150,9 +155,17 @@
         return this.getCorner(a, s).getBalls();
     };
 
     World.prototype.getHoles = function(a, s) {
         return this.getCorner(a, s).getHoles();
     };
 
+    World.prototype.showNumberOfBalls = function(a, s) {
+        return this.getCorner(a, s).showNumberOfBalls();
+    };
+
+    World.prototype.getRandomNumber = function(range = 3) {
+        return Math.floor(Math.random() * range) + 1;
+    };
+
     return World;
 })();
```

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/language_data.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/hammer.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/hammer.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/prettify.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/lib/prettify.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/matrixeq.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/mchoice.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/merge.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/modal-basic.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/modal-basic.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/js/en.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/msg/js/en.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/navhelp.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/navhelp.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/parsons.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/petlja.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/petlja.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/poll.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/poll.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/presenter_mode.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/processing-1.4.1.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/processing-1.4.1.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/__init__.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/__init__.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/display.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/display.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/draw.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/draw.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/event.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/event.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/font.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/font.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/image.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/image.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/key.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/key.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/mouse.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/mouse.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/time.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/time.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/transform.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib/transform.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib-init.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygamelib-init.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygments.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/python_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/pytutor.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-core.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-core.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-cssclassapplier.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-cssclassapplier.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-textrange.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/rangy-textrange.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/reveal.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/reveal.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestone-custom-sphinx-bootstrap.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestone-custom-sphinx-bootstrap.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonebase.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonebase.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonevideo.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/runestonevideo.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/searchtools.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sharedb.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sharedb.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/shortanswer.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/shortanswer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/showEval.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt-stdlib.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt-stdlib.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/skulpt.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortmodels.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortmodels.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortviewers.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/sortviewers.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/style.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/style.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/tabbedstuff.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_activecode.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_activecode.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_shortanswer.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timed_shortanswer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedclickable.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedclickable.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timeddnd.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timeddnd.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedfitb.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedfitb.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedmc.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedmc.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedparsons.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/timedparsons.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore-1.3.1.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/user-highlights.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/waypoints.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/waypoints.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/webglinteractive.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/websupport.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/notes/test/build/noteTests/_static/xml.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/notes/test/build/noteTests/_static/xml.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/p5js/js/p5js.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/p5js/js/p5js.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/p5js/p5js.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/p5js/p5js.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pycode/css/pycode.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/pycode/css/pycode.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pycode/js/pycode.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/pycode/js/pycode.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pycode/pycode.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/pycode/pycode.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/__init__.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/__init__.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/display.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/display.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/draw.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/draw.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/event.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/event.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/font.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/font.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/image.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/image.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/key.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/key.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/mouse.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/mouse.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/time.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/time.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib/transform.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib/transform.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/js/pygamelib-init.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/js/pygamelib-init.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-3.0.0/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/_templates/plugin_layouts/sphinx_bootstrap/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/conf.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/conf.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/pygamelib/test/pavement.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/pygamelib/test/pavement.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/quizq/quizq.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/quizq/quizq.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/regexcheck/css/regex-check.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/css/regex-check.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/regexcheck/js/regex-check.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/js/regex-check.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/regexcheck/regexcheck.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/regexcheck/regexcheck.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/simanim/css/simanim.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/simanim/css/simanim.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/simanim/js/simanim.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/simanim/js/simanim.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/simanim/simanim.py` & `petljadoc-1.3.1/petljadoc/runestone_ext/simanim/simanim.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/Blob.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/Blob.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/FileSaver.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/FileSaver.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/LICENSE.txt` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibility.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibility.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitydarkest.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitydarkest.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitylight.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/accessibilitylight.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.en.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.en.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.sr-Cyrl.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode-i18n.sr-Cyrl.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/activecode.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/animationbase.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/animationbase.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/basic.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/basic.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blockly_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blockly_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blocks_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/blocks_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bookfuncs.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bookfuncs.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/css/bootstrap.min.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/js/bootstrap.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-3.0.0/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-sphinx.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap.min.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clickable.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clike.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/clike.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codelens.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codelens.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/codemirror.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/css.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/css.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/d3.v2.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/d3.v2.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/datafile.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/datafile.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/diff_match_patch.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/diff_match_patch.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/doctools.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/doctools.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/dragndrop.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/external.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/external.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/fitb.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/guiders-1.3.0.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/htmlmixed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/htmlmixed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/javascript_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-3.2.1.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-3.2.1.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-migrate-1.2.1.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-migrate-1.2.1.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery-ui-1.10.3.custom.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.ba-bbq.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.ba-bbq.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.highlight.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.highlight.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.hotkey.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.hotkey.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.idle-timer.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.idle-timer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.jsPlumb-1.3.10-all-min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.jsPlumb-1.3.10-all-min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.tablesorter.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery.tablesorter.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/CLDRPluralRuleParser.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/CLDRPluralRuleParser.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.bidi.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.emitter.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.fallbacks.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.fallbacks.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.language.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.language.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.messagestore.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.messagestore.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.parser.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/jquery_i18n/jquery.i18n.parser.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/language_data.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/language_data.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/hammer.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/hammer.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/prettify.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/lib/prettify.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/matrixeq.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/mchoice.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/merge.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/modal-basic.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/modal-basic.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/js/en.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/msg/js/en.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/navhelp.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/navhelp.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/parsons.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/poll.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/poll.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/presenter_mode.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/processing-1.4.1.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/processing-1.4.1.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pygments.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pygments.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python_compressed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/python_compressed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/pytutor.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-core.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-core.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-cssclassapplier.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-cssclassapplier.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-textrange.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/rangy-textrange.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/reveal.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/reveal.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestone-custom-sphinx-bootstrap.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestone-custom-sphinx-bootstrap.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonebase.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonebase.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonevideo.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/runestonevideo.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/searchtools.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/searchtools.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sharedb.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sharedb.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/shortanswer.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/shortanswer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/showEval.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt-stdlib.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt-stdlib.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/skulpt.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortmodels.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortmodels.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortviewers.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/sortviewers.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/style.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/style.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/tabbedstuff.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_activecode.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_activecode.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_shortanswer.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timed_shortanswer.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedclickable.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedclickable.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timeddnd.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timeddnd.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedfitb.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedfitb.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedmc.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedmc.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedparsons.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/timedparsons.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore-1.3.1.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore-1.3.1.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/underscore.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/user-highlights.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/waypoints.min.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/waypoints.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.css` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/webglinteractive.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/websupport.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/websupport.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/runestone_ext/video/test/build/VideoTests/_static/xml.js` & `petljadoc-1.3.1/petljadoc/runestone_ext/video/test/build/VideoTests/_static/xml.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/scorm-proxy-templates/adlcp_rootv1p2.xsd` & `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/adlcp_rootv1p2.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/scorm-proxy-templates/bundle.js` & `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/bundle.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/scorm-proxy-templates/favicon.ico` & `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/scorm-proxy-templates/ims_xml.xsd` & `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/ims_xml.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/scorm-proxy-templates/imscp_rootv1p1p2.xsd` & `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/imscp_rootv1p1p2.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/scorm-proxy-templates/imsmanifest.t.xml` & `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/imsmanifest.t.xml`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/scorm-proxy-templates/imsmd_rootv1p2p1.xsd` & `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/imsmd_rootv1p2p1.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/scorm-proxy-templates/index.t.html` & `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/index.t.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/scorm-proxy-templates/style-player.css` & `petljadoc-1.3.1/petljadoc/scorm-proxy-templates/style-player.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/scorm-templates/adlcp_rootv1p2.xsd` & `petljadoc-1.3.1/petljadoc/scorm-templates/adlcp_rootv1p2.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/scorm-templates/ims_xml.xsd` & `petljadoc-1.3.1/petljadoc/scorm-templates/ims_xml.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/scorm-templates/imscp_rootv1p1p2.xsd` & `petljadoc-1.3.1/petljadoc/scorm-templates/imscp_rootv1p1p2.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/scorm-templates/imsmd_rootv1p2p1.xsd` & `petljadoc-1.3.1/petljadoc/scorm-templates/imsmd_rootv1p2p1.xsd`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/layout.html` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/layout.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/en/LC_MESSAGES/shpinx.mo` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/en/LC_MESSAGES/shpinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/sr/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/platform/petljaRTBundle.js` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/platform/petljaRTBundle.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bootstrap-sphinx.css_t` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-sphinx.css_t`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bootstrap-sphinx.js` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/bundle.js` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/bundle.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/css/font-awesome.min.css` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/favicon.ico` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/flatly.min.css` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/flatly.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/fonts/FontAwesome.otf` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.eot` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.ttf` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff2` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/choice-background.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/choice-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/dragndrop-background.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/dragndrop-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/fitb-background.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/fitb-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/logo.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/netkabinet-logo-strelica-wt.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/netkabinet-logo-strelica-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/parsons-background.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/parsons-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/petlja-logo-wt.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/petlja-logo-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/images/play_button.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/images/play_button.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/Facebook.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Facebook.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/Facebook_icon.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Facebook_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/Twitter.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Twitter.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/Twitter_icon.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/Twitter_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/dragndrop-img.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/dragndrop-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/favicon.ico` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/fitb-img.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/fitb-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/green-coin.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/green-coin.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-ball.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-ball.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-east-balls.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-east-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-east.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-east.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-head.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-head.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-hole.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-hole.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-north-balls.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-north-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-north.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-north.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-south-balls.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-south-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-south.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-south.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-west-balls.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-west-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/karel-west.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/karel-west.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/learnmorenote-img.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/learnmorenote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/logo.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/logo_small.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/logo_small.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/netkabinet-logo-strelica-wt.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/netkabinet-logo-strelica-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/parsons-img.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/parsons-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/petlja-logo-wt.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/petlja-logo-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/play_overlay_icon.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/play_overlay_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/qchoice-img.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/qchoice-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/question-mark-old.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/question-mark-old.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/question-mark.png` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/question-mark.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/questionnote-img.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/questionnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/suggestionnote-img.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/suggestionnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/img/technicalnote-img.svg` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/img/technicalnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/petlja-course.css` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/petlja-course.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/petlja.js` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/petlja.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/require.js` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/require.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/simanim-0.0.4-py3-none-any.whl` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/simanim-0.0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/skulpt-stdlib.js` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/skulpt-stdlib.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/skulpt.min.js` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/skulpt.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/static/style-player.css` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/static/style-player.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/bc_theme/theme.conf` & `petljadoc-1.3.1/petljadoc/themes/bc_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/basic_layout.html` & `petljadoc-1.3.1/petljadoc/themes/course_theme/basic_layout.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/course_homepage.html` & `petljadoc-1.3.1/petljadoc/themes/course_theme/course_homepage.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/globaltoc.html` & `petljadoc-1.3.1/petljadoc/themes/course_theme/globaltoc.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/layout.html` & `petljadoc-1.3.1/petljadoc/themes/course_theme/layout.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/locale/en/LC_MESSAGES/shpinx.mo` & `petljadoc-1.3.1/petljadoc/themes/course_theme/locale/en/LC_MESSAGES/shpinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/locale/sr/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.1/petljadoc/themes/course_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/relations.html` & `petljadoc-1.3.1/petljadoc/themes/course_theme/relations.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/bootstrap-sphinx.css_t` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-sphinx.css_t`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/bootstrap-sphinx.js` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/css/font-awesome.min.css` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/favicon.ico` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/flatly.min.css` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/flatly.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/fonts/FontAwesome.otf` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.eot` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.ttf` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff2` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/choice-background.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/choice-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/dragndrop-background.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/dragndrop-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/fitb-background.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/fitb-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/logo.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/netkabinet-logo-strelica-wt.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/netkabinet-logo-strelica-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/parsons-background.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/parsons-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/petlja-logo-wt.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/petlja-logo-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/images/play_button.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/images/play_button.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/Facebook.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Facebook.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/Facebook_icon.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Facebook_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/Twitter.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Twitter.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/Twitter_icon.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/Twitter_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/dragndrop-img.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/dragndrop-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/favicon.ico` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/fitb-img.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/fitb-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/green-coin.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/green-coin.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-ball.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-ball.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-east-balls.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-east-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-east.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-east.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-head.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-head.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-hole.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-hole.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-north-balls.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-north-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-north.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-north.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-south-balls.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-south-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-south.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-south.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-west-balls.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-west-balls.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/karel-west.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/karel-west.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/learnmorenote-img.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/learnmorenote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/logo.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/logo_small.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/logo_small.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/netkabinet-logo-strelica-wt.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/netkabinet-logo-strelica-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/parsons-img.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/parsons-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/petlja-logo-wt.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/petlja-logo-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/play_overlay_icon.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/play_overlay_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/qchoice-img.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/qchoice-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/question-mark-old.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/question-mark-old.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/question-mark.png` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/question-mark.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/questionnote-img.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/questionnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/suggestionnote-img.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/suggestionnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/img/technicalnote-img.svg` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/img/technicalnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/nbstyle.css` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/nbstyle.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/petlja-course.css` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/petlja-course.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/petlja.js` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/petlja.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/require.js` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/require.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/simanim-0.0.4-py3-none-any.whl` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/simanim-0.0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/skulpt-stdlib.js` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/skulpt-stdlib.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/static/skulpt.min.js` & `petljadoc-1.3.1/petljadoc/themes/course_theme/static/skulpt.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/subchapter.html` & `petljadoc-1.3.1/petljadoc/themes/course_theme/subchapter.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/course_theme/theme.conf` & `petljadoc-1.3.1/petljadoc/themes/course_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/__init__.py` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/__init__.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/basic_layout.html` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/basic_layout.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/layout.html` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/layout.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/en/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/en/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/sr/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr@latn/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/locale/sr_RS/LC_MESSAGES/sphinx.mo`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/relations.html` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/relations.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-4.0.0-dist/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.css_t` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.css_t`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.js` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/bootstrap-sphinx.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/css/font-awesome.min.css` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/css/font-awesome.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/favicon.ico` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/flatly.min.css` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/flatly.min.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/fonts/FontAwesome.otf` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/FontAwesome.otf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.eot` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.eot`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.ttf` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.ttf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff2` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/fonts/fontawesome-webfont.woff2`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/choice-background.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/choice-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/dragndrop-background.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/dragndrop-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/fitb-background.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/fitb-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/logo.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/logo.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/netkabinet-logo-strelica-wt.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/netkabinet-logo-strelica-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/parsons-background.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/parsons-background.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/petlja-logo-wt.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/petlja-logo-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/images/play_button.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/images/play_button.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/Facebook.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Facebook.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/Facebook_icon.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Facebook_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/Twitter.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Twitter.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/Twitter_icon.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/Twitter_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/dragndrop-img.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/dragndrop-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/favicon.ico` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/fitb-img.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/fitb-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/green-coin.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/green-coin.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/karel-ball.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-ball.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/karel-east.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-east.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/karel-head.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-head.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/karel-hole.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-hole.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/karel-north.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-north.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/karel-south.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-south.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/karel-west.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/karel-west.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/learnmorenote-img.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/learnmorenote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/logo.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/logo.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/logo_small.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/logo_small.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/netkabinet-logo-strelica-wt.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/netkabinet-logo-strelica-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/parsons-img.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/parsons-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/petlja-logo-wt.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/petlja-logo-wt.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/play_overlay_icon.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/play_overlay_icon.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/qchoice-img.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/qchoice-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/question-mark-old.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/question-mark-old.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/question-mark.png` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/question-mark.png`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/questionnote-img.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/questionnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/suggestionnote-img.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/suggestionnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/img/technicalnote-img.svg` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/img/technicalnote-img.svg`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/nbstyle.css` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/nbstyle.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/petlja-runestone.css` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/petlja-runestone.css`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/require.js` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/require.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/simanim-0.0.4-py3-none-any.whl` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/simanim-0.0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/skulpt-stdlib.js` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/skulpt-stdlib.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/static/skulpt.min.js` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/static/skulpt.min.js`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/subchapter.html` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/subchapter.html`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/themes/runestone_theme/theme.conf` & `petljadoc-1.3.1/petljadoc/themes/runestone_theme/theme.conf`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc/util.py` & `petljadoc-1.3.1/petljadoc/util.py`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/petljadoc.egg-info/PKG-INFO` & `petljadoc-1.3.1/petljadoc.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petljadoc
-Version: 1.3.0
+Version: 1.3.1
 Summary: Petlja's command-line interface for learning content
 Home-page: https://github.com/Petlja/PetljaDoc
 Author: Fondacija Petlja
 Author-email: team@petlja.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `petljadoc-1.3.0/petljadoc.egg-info/SOURCES.txt` & `petljadoc-1.3.1/petljadoc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petljadoc-1.3.0/setup.py` & `petljadoc-1.3.1/setup.py`

 * *Files identical despite different names*

