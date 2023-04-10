# Comparing `tmp/pawpaw-1.0.0a8.tar.gz` & `tmp/pawpaw-1.0.0a9.tar.gz`

## Comparing `pawpaw-1.0.0a8.tar` & `pawpaw-1.0.0a9.tar`

### file list

```diff
@@ -1,103 +1,114 @@
--rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/CONTRIBUTING.md
--rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/SECURITY.md
--rw-r--r--   0        0        0     9034 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tinker.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/.idea/.gitignore
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/.idea/misc.xml
--rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/.idea/modules.xml
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/.idea/pawpaw.iml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/.idea/vcs.xml
--rw-r--r--   0        0        0    34150 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/.idea/workspace.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0     9191 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/docs/0. Introduction.md
--rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/docs/1. Segment and Span.md
--rw-r--r--   0        0        0    23030 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/docs/2. In Text Object.md
--rw-r--r--   0        0        0     9139 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/docs/3. Visualization.md
--rw-r--r--   0        0        0     5358 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/docs/4. Arborform.md
--rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/docs/5. Traversal & Query.md
--rw-r--r--   0        0        0    12922 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/docs/6. Xml.md
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/docs/7. NLP.md
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/docs/8. Serialization.md
--rw-r--r--   0        0        0     1918 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/docs/Using Pawpaw with nltk.md
--rw-r--r--   0        0        0     2229 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/docs/cookbook.md
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/docs/demos/gettysburg_address/gettysburg_address.txt
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/docs/demos/us_constitution/us_constitution.py
--rw-r--r--   0        0        0    26246 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/docs/demos/us_constitution/us_constitution.txt
--rw-r--r--   0        0        0   940341 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/images/pawpaw.png
--rw-r--r--   0        0        0   160416 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/images/pawpaw2.png
--rw-r--r--   0        0        0      671 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/__init__.py
--rw-r--r--   0        0        0     2276 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/_furcation.py
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/_predicated_value.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/_type_magic.py
--rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/_version.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/errors.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/infix.py
--rw-r--r--   0        0        0    50595 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/ito.py
--rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/span.py
--rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/util.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/arborform/__init__.py
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/arborform/itorator/__init__.py
--rw-r--r--   0        0        0      686 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/arborform/itorator/desc.py
--rw-r--r--   0        0        0     3159 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/arborform/itorator/extract.py
--rw-r--r--   0        0        0     5306 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/arborform/itorator/itorator.py
--rw-r--r--   0        0        0      301 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/arborform/itorator/reflect.py
--rw-r--r--   0        0        0     3889 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/arborform/itorator/split.py
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/arborform/postorator/__init__.py
--rw-r--r--   0        0        0      829 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/arborform/postorator/postorator.py
--rw-r--r--   0        0        0     2622 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/arborform/postorator/stacked_reduce.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/arborform/postorator/windowed_join.py
--rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/nlp/__init__.py
--rw-r--r--   0        0        0    14936 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/nlp/nlp.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/query/__init__.py
--rw-r--r--   0        0        0    27591 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/query/query.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/visualization/__init__.py
--rw-r--r--   0        0        0    51546 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/visualization/ascii_box.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/visualization/highlighter.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/visualization/pepo/__init__.py
--rw-r--r--   0        0        0     7221 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/visualization/pepo/pepo.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/visualization/sgr/__init__.py
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/visualization/sgr/sgr.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/visualization/sgr/palettes/__init__.py
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/visualization/sgr/palettes/palettes.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/xml/__init__.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/xml/descriptors.py
--rw-r--r--   0        0        0     8364 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/xml/xml_helper.py
--rw-r--r--   0        0        0     8209 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pawpaw/xml/xml_parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/__init__.py
--rw-r--r--   0        0        0     9091 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_child_itos.py
--rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_furcation.py
--rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_invoke_func.py
--rw-r--r--   0        0        0    18719 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_ito.py
--rw-r--r--   0        0        0    13222 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_ito_ctor.py
--rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_ito_regex_equivalence_methods.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_ito_serialization.py
--rw-r--r--   0        0        0    17476 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_ito_str_equivalence_methods.py
--rw-r--r--   0        0        0     9141 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_itorator.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_itorator_extract.py
--rw-r--r--   0        0        0      388 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_itorator_reflect.py
--rw-r--r--   0        0        0     3628 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_itorator_split.py
--rw-r--r--   0        0        0     9647 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_nlp.py
--rw-r--r--   0        0        0     1594 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_postorator.py
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_postorator_windowed_join.py
--rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_predicated_value.py
--rw-r--r--   0        0        0    40963 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_query_and_traversal.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_sgr.py
--rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_span.py
--rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_type_magic.py
--rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_util.py
--rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_visualization_ascii_box.py
--rw-r--r--   0        0        0     4441 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_xml_helper.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/test_xml_parser.py
--rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/util.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/LICENSE
--rw-r--r--   0        0        0    15606 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/README.md
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/pyproject.toml
--rw-r--r--   0        0        0    16200 2020-02-02 00:00:00.000000 pawpaw-1.0.0a8/PKG-INFO
+-rw-r--r--   0        0        0     5236 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/CONTRIBUTING.md
+-rw-r--r--   0        0        0      534 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/SECURITY.md
+-rw-r--r--   0        0        0     9007 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tinker.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tmp.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      628 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.idea/.gitignore
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.idea/misc.xml
+-rw-r--r--   0        0        0      271 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.idea/modules.xml
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.idea/pawpaw.iml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.idea/vcs.xml
+-rw-r--r--   0        0        0    36360 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.idea/workspace.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     9184 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/0. Introduction.md
+-rw-r--r--   0        0        0     5242 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/1. Segment and Span.md
+-rw-r--r--   0        0        0    23527 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/2. In Text Object.md
+-rw-r--r--   0        0        0     9237 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/3. Visualization.md
+-rw-r--r--   0        0        0    19023 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/4. Arborform.md
+-rw-r--r--   0        0        0    14843 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/5. Traversal & Query.md
+-rw-r--r--   0        0        0    13200 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/6. Xml.md
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/7. NLP.md
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/8. Serialization.md
+-rw-r--r--   0        0        0     3582 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/Pawpaw Cookbook.md
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/Using Pawpaw with nltk.md
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/class_grades/description.md
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/class_grades/input.txt
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/class_grades/parser_compact.py
+-rw-r--r--   0        0        0     1451 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/class_grades/parser_verbose.py
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/class_grades/solution.py
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/gettysburg_address/gettysburg_address.txt
+-rw-r--r--   0        0        0     2764 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/us_constitution/us_constitution.py
+-rw-r--r--   0        0        0    26246 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/docs/demos/us_constitution/us_constitution.txt
+-rw-r--r--   0        0        0   940341 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/images/pawpaw.png
+-rw-r--r--   0        0        0   160416 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/images/pawpaw2.png
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/__init__.py
+-rw-r--r--   0        0        0     2268 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/_furcation.py
+-rw-r--r--   0        0        0      613 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/_predicated_value.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/_type_magic.py
+-rw-r--r--   0        0        0     1092 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/_version.py
+-rw-r--r--   0        0        0     1767 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/errors.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/infix.py
+-rw-r--r--   0        0        0    50592 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/ito.py
+-rw-r--r--   0        0        0     1690 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/span.py
+-rw-r--r--   0        0        0     2636 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/util.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/__init__.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/__init__.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/desc.py
+-rw-r--r--   0        0        0     3611 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/extract.py
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/filter.py
+-rw-r--r--   0        0        0     5330 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/itorator.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/reflect.py
+-rw-r--r--   0        0        0     4199 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/split.py
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/itorator/value_func.py
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/postorator/__init__.py
+-rw-r--r--   0        0        0     1104 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/postorator/postorator.py
+-rw-r--r--   0        0        0     1900 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/postorator/stacked_reduce.py
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/arborform/postorator/windowed_join.py
+-rw-r--r--   0        0        0       46 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/nlp/__init__.py
+-rw-r--r--   0        0        0    15149 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/nlp/nlp.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/query/__init__.py
+-rw-r--r--   0        0        0    27492 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/query/_query.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/__init__.py
+-rw-r--r--   0        0        0    51546 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/ascii_box.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/highlighter.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/pepo/__init__.py
+-rw-r--r--   0        0        0     7217 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/pepo/pepo.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/sgr/__init__.py
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/sgr/sgr.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/sgr/palettes/__init__.py
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/visualization/sgr/palettes/palettes.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/xml/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/xml/descriptors.py
+-rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/xml/xml_helper.py
+-rw-r--r--   0        0        0     8147 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pawpaw/xml/xml_parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/__init__.py
+-rw-r--r--   0        0        0     9091 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_child_itos.py
+-rw-r--r--   0        0        0     3090 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_furcation.py
+-rw-r--r--   0        0        0     2176 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_invoke_func.py
+-rw-r--r--   0        0        0    19841 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_ito.py
+-rw-r--r--   0        0        0    13222 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_ito_ctor.py
+-rw-r--r--   0        0        0     4190 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_ito_regex_equivalence_methods.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_ito_serialization.py
+-rw-r--r--   0        0        0    17476 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_ito_str_equivalence_methods.py
+-rw-r--r--   0        0        0    14565 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_itorator.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_itorator_desc.py
+-rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_itorator_extract.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_itorator_filter.py
+-rw-r--r--   0        0        0      392 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_itorator_reflect.py
+-rw-r--r--   0        0        0     5571 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_itorator_split.py
+-rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_itorator_value_func.py
+-rw-r--r--   0        0        0     9638 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_nlp.py
+-rw-r--r--   0        0        0     1278 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_postorator.py
+-rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_postorator_windowed_join.py
+-rw-r--r--   0        0        0     2162 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_predicated_value.py
+-rw-r--r--   0        0        0    40963 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_query_and_traversal.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_sgr.py
+-rw-r--r--   0        0        0     2092 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_span.py
+-rw-r--r--   0        0        0     7182 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_type_magic.py
+-rw-r--r--   0        0        0     4612 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_util.py
+-rw-r--r--   0        0        0     5907 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_visualization_ascii_box.py
+-rw-r--r--   0        0        0     4444 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_xml_helper.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/test_xml_parser.py
+-rw-r--r--   0        0        0     7558 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/util.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      310 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/.pytest_cache/README.md
+-rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/tests/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     1093 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/LICENSE
+-rw-r--r--   0        0        0    15693 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/README.md
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/pyproject.toml
+-rw-r--r--   0        0        0    16284 2020-02-02 00:00:00.000000 pawpaw-1.0.0a9/PKG-INFO
```

### Comparing `pawpaw-1.0.0a8/CODE_OF_CONDUCT.md` & `pawpaw-1.0.0a9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/CONTRIBUTING.md` & `pawpaw-1.0.0a9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/SECURITY.md` & `pawpaw-1.0.0a9/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tinker.py` & `pawpaw-1.0.0a9/tinker.py`

 * *Files 1% similar despite different names*

```diff
@@ -239,23 +239,23 @@
 
 nltk_tok = nltk.tokenize
 sent_itor = pawpaw.arborform.Itorator.wrap(lambda ito: ito.from_substrings(ito, *nltk_tok.sent_tokenize(str(ito))))
 
 word_itor = pawpaw.arborform.Itorator.wrap(lambda ito: ito.from_substrings(ito, *nltk_tok.word_tokenize(str(ito))))
 sent_itor.itor_children = word_itor
 
-i.children.add(*(sent_itor.traverse(i)))
+i.children.add(*(sent_itor(i)))
 print(v_tree.dumps(i))
 exit(0)
 
 
 ws_tok = nltk.tokenize.WhitespaceTokenizer()
 splitter = pawpaw.arborform.Split(regex.compile(ws_tok._pattern, ws_tok._flags))
 i = pawpaw.Ito('The quick brown fox.')
-[str(i) for i in splitter.traverse(i)]
+[str(i) for i in splitter(i)]
 
 
 
 
 # # VERSION
 #
 # print(pawpaw.__version__)
@@ -285,15 +285,15 @@
 
 wrds_nums = Extract(regex.compile(r'(?P<word>[a-z]+) (?P<number>\d+)'))
 phrases.itor_children = wrds_nums
 
 chrs_digs = Extract(regex.compile(r'(?P<char>[a-z])+|(?P<digit>\d)+'))
 wrds_nums.itor_children = chrs_digs
 
-root.children.add(*phrases.traverse(root))
+root.children.add(*phrases(root))
 
 print(dump.Compact().dumps(root))
 exit(0)
 
     
 # SGR
```

### Comparing `pawpaw-1.0.0a8/.github/ISSUE_TEMPLATE/bug_report.md` & `pawpaw-1.0.0a9/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/.github/ISSUE_TEMPLATE/feature_request.md` & `pawpaw-1.0.0a9/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/.idea/workspace.xml` & `pawpaw-1.0.0a9/.idea/workspace.xml`

 * *Files 5% similar despite different names*

#### Comparing `pawpaw-1.0.0a8/.idea/workspace.xml` & `pawpaw-1.0.0a9/.idea/workspace.xml`

```diff
@@ -52,48 +52,48 @@
       <recent name="C:\Users\rlaye\Documents\PycharmProjects\pawpaw\pawpaw\arborform\itorator"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
       <recent name="C:\Users\rlaye\Documents\PycharmProjects\pawpaw\pawpaw\arborform\itorator"/>
     </key>
   </component>
   <component name="RunManager" selected="Python tests. All Unittests">
-    <configuration name="tinker" type="PythonConfigurationType" factoryName="Python" nameIsGenerated="true">
+    <configuration name="solution" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
-      <option name="SDK_HOME" value="C:\Users\rlaye\anaconda3\envs\pawpaw\python.exe"/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
-      <option name="IS_MODULE_SDK" value="false"/>
+      <option name="SDK_HOME" value=""/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/docs/demos/class_grades"/>
+      <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tinker.py"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/docs/demos/class_grades/solution.py"/>
       <option name="PARAMETERS" value=""/>
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
     </configuration>
-    <configuration name="us_constitution" type="PythonConfigurationType" factoryName="Python" temporary="true" nameIsGenerated="true">
+    <configuration name="tinker" type="PythonConfigurationType" factoryName="Python" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <envs>
         <env name="PYTHONUNBUFFERED" value="1"/>
       </envs>
-      <option name="SDK_HOME" value=""/>
-      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/docs/demos/us_constitution"/>
-      <option name="IS_MODULE_SDK" value="true"/>
+      <option name="SDK_HOME" value="C:\Users\rlaye\anaconda3\envs\pawpaw\python.exe"/>
+      <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
+      <option name="IS_MODULE_SDK" value="false"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
-      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/docs/demos/us_constitution/us_constitution.py"/>
+      <option name="SCRIPT_NAME" value="$PROJECT_DIR$/tinker.py"/>
       <option name="PARAMETERS" value=""/>
       <option name="SHOW_COMMAND_LINE" value="false"/>
       <option name="EMULATE_TERMINAL" value="false"/>
       <option name="MODULE_MODE" value="false"/>
       <option name="REDIRECT_INPUT" value="false"/>
       <option name="INPUT_FILE" value=""/>
       <method v="2"/>
@@ -109,67 +109,67 @@
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <option name="_new_pattern" value="&quot;&quot;"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;$PROJECT_DIR$/tests&quot;"/>
       <option name="_new_targetType" value="&quot;PATH&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_query_and_traversal.TestItoQuery.test_filter_string_casefold_endswith_multiple" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_itorator_extract.TestExtract.test_desc_func" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_query_and_traversal.TestItoQuery.test_filter_string_casefold_endswith_multiple&quot;"/>
+      <option name="_new_target" value="&quot;test_itorator_extract.TestExtract.test_desc_func&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_query_and_traversal.TestItoQuery.test_filter_string_casefold_endswith_scalar" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_itorator_extract.TestExtract.test_group_filter_default" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_query_and_traversal.TestItoQuery.test_filter_string_casefold_endswith_scalar&quot;"/>
+      <option name="_new_target" value="&quot;test_itorator_extract.TestExtract.test_group_filter_default&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_query_and_traversal.TestItoQuery.test_filter_string_casefold_startswith_multiple" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_itorator_filter.TestFilter.test_traverse_partial" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_query_and_traversal.TestItoQuery.test_filter_string_casefold_startswith_multiple&quot;"/>
+      <option name="_new_target" value="&quot;test_itorator_filter.TestFilter.test_traverse_partial&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
-    <configuration name="Python tests for test_query_and_traversal.TestItoQuery.test_filter_string_casefold_startswith_scalar" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
+    <configuration name="Python tests for test_itorator_split.TestSplit.test_limit" type="tests" factoryName="Autodetect" temporary="true" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
       <option name="SDK_HOME" value=""/>
       <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
       <option name="IS_MODULE_SDK" value="true"/>
       <option name="ADD_CONTENT_ROOTS" value="true"/>
       <option name="ADD_SOURCE_ROOTS" value="true"/>
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
-      <option name="_new_target" value="&quot;test_query_and_traversal.TestItoQuery.test_filter_string_casefold_startswith_scalar&quot;"/>
+      <option name="_new_target" value="&quot;test_itorator_split.TestSplit.test_limit&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <configuration name="Unittests for test_type_magic.TestTypeMagic.test_is_callable_exact" type="tests" factoryName="Unittests" nameIsGenerated="true">
       <module name="pawpaw"/>
       <option name="INTERPRETER_OPTIONS" value=""/>
       <option name="PARENT_ENVS" value="true"/>
@@ -182,153 +182,41 @@
       <option name="_new_additionalArguments" value="&quot;&quot;"/>
       <option name="_new_target" value="&quot;test_type_magic.TestTypeMagic.test_is_callable_exact&quot;"/>
       <option name="_new_targetType" value="&quot;PYTHON&quot;"/>
       <method v="2"/>
     </configuration>
     <list>
       <item itemvalue="Python.tinker"/>
-      <item itemvalue="Python.us_constitution"/>
+      <item itemvalue="Python.solution"/>
       <item itemvalue="Python tests.Unittests for test_type_magic.TestTypeMagic.test_is_callable_exact"/>
       <item itemvalue="Python tests. All Unittests"/>
-      <item itemvalue="Python tests.Python tests for test_query_and_traversal.TestItoQuery.test_filter_string_casefold_endswith_multiple"/>
-      <item itemvalue="Python tests.Python tests for test_query_and_traversal.TestItoQuery.test_filter_string_casefold_endswith_scalar"/>
-      <item itemvalue="Python tests.Python tests for test_query_and_traversal.TestItoQuery.test_filter_string_casefold_startswith_multiple"/>
-      <item itemvalue="Python tests.Python tests for test_query_and_traversal.TestItoQuery.test_filter_string_casefold_startswith_scalar"/>
+      <item itemvalue="Python tests.Python tests for test_itorator_extract.TestExtract.test_desc_func"/>
+      <item itemvalue="Python tests.Python tests for test_itorator_extract.TestExtract.test_group_filter_default"/>
+      <item itemvalue="Python tests.Python tests for test_itorator_filter.TestFilter.test_traverse_partial"/>
+      <item itemvalue="Python tests.Python tests for test_itorator_split.TestSplit.test_limit"/>
     </list>
     <recent_temporary>
       <list>
-        <item itemvalue="Python.us_constitution"/>
-        <item itemvalue="Python tests.Python tests for test_query_and_traversal.TestItoQuery.test_filter_string_casefold_startswith_multiple"/>
-        <item itemvalue="Python tests.Python tests for test_query_and_traversal.TestItoQuery.test_filter_string_casefold_startswith_scalar"/>
-        <item itemvalue="Python tests.Python tests for test_query_and_traversal.TestItoQuery.test_filter_string_casefold_endswith_multiple"/>
-        <item itemvalue="Python tests.Python tests for test_query_and_traversal.TestItoQuery.test_filter_string_casefold_endswith_scalar"/>
+        <item itemvalue="Python tests.Python tests for test_itorator_split.TestSplit.test_limit"/>
+        <item itemvalue="Python tests.Python tests for test_itorator_extract.TestExtract.test_group_filter_default"/>
+        <item itemvalue="Python tests.Python tests for test_itorator_filter.TestFilter.test_traverse_partial"/>
+        <item itemvalue="Python tests.Python tests for test_itorator_extract.TestExtract.test_desc_func"/>
+        <item itemvalue="Python.solution"/>
       </list>
     </recent_temporary>
   </component>
   <component name="SpellCheckerSettings" RuntimeDictionaries="0" Folders="0" CustomDictionaries="0" DefaultDictionary="application-level" UseSingleDictionary="true" transferred="true"/>
   <component name="TaskManager">
     <task active="true" id="Default" summary="Default task">
       <changelist id="60f56f5e-2b22-4441-9568-072b306fbfd2" name="Changes" comment=""/>
       <created>1668472305766</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1668472305766</updated>
     </task>
-    <task id="LOCAL-00004" summary="nlp updates">
-      <created>1668983186128</created>
-      <option name="number" value="00004"/>
-      <option name="presentableId" value="LOCAL-00004"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1668983186128</updated>
-    </task>
-    <task id="LOCAL-00005" summary="nlp updates">
-      <created>1668983273268</created>
-      <option name="number" value="00005"/>
-      <option name="presentableId" value="LOCAL-00005"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1668983273268</updated>
-    </task>
-    <task id="LOCAL-00006" summary="nlp updates">
-      <created>1669172543817</created>
-      <option name="number" value="00006"/>
-      <option name="presentableId" value="LOCAL-00006"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1669172543817</updated>
-    </task>
-    <task id="LOCAL-00007" summary="Cleanups">
-      <created>1669260814520</created>
-      <option name="number" value="00007"/>
-      <option name="presentableId" value="LOCAL-00007"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1669260814520</updated>
-    </task>
-    <task id="LOCAL-00008" summary="format strings refactor">
-      <created>1669329330300</created>
-      <option name="number" value="00008"/>
-      <option name="presentableId" value="LOCAL-00008"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1669329330300</updated>
-    </task>
-    <task id="LOCAL-00009" summary="Typos &amp; query test fixes">
-      <created>1669860014773</created>
-      <option name="number" value="00009"/>
-      <option name="presentableId" value="LOCAL-00009"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1669860014773</updated>
-    </task>
-    <task id="LOCAL-00010" summary="Added query tests">
-      <created>1669947529849</created>
-      <option name="number" value="00010"/>
-      <option name="presentableId" value="LOCAL-00010"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1669947529849</updated>
-    </task>
-    <task id="LOCAL-00011" summary="Query tests and fixes; 1.0.0.a5 final">
-      <created>1670082952901</created>
-      <option name="number" value="00011"/>
-      <option name="presentableId" value="LOCAL-00011"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670082952901</updated>
-    </task>
-    <task id="LOCAL-00012" summary="Removed redundant error">
-      <created>1670110905119</created>
-      <option name="number" value="00012"/>
-      <option name="presentableId" value="LOCAL-00012"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670110905119</updated>
-    </task>
-    <task id="LOCAL-00013" summary="subquery consolidation">
-      <created>1670184184626</created>
-      <option name="number" value="00013"/>
-      <option name="presentableId" value="LOCAL-00013"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670184184626</updated>
-    </task>
-    <task id="LOCAL-00014" summary="fixes for all subquery tests">
-      <created>1670188079605</created>
-      <option name="number" value="00014"/>
-      <option name="presentableId" value="LOCAL-00014"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670188079605</updated>
-    </task>
-    <task id="LOCAL-00015" summary="Added subquery tests">
-      <created>1670190071629</created>
-      <option name="number" value="00015"/>
-      <option name="presentableId" value="LOCAL-00015"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670190071629</updated>
-    </task>
-    <task id="LOCAL-00016" summary="Added subquery tests">
-      <created>1670191639813</created>
-      <option name="number" value="00016"/>
-      <option name="presentableId" value="LOCAL-00016"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670191639813</updated>
-    </task>
-    <task id="LOCAL-00017" summary="Added subquery tests">
-      <created>1670294735995</created>
-      <option name="number" value="00017"/>
-      <option name="presentableId" value="LOCAL-00017"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670294735995</updated>
-    </task>
-    <task id="LOCAL-00018" summary="Typos">
-      <created>1670372856179</created>
-      <option name="number" value="00018"/>
-      <option name="presentableId" value="LOCAL-00018"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670372856179</updated>
-    </task>
-    <task id="LOCAL-00019" summary="Typos">
-      <created>1670458446748</created>
-      <option name="number" value="00019"/>
-      <option name="presentableId" value="LOCAL-00019"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1670458446748</updated>
-    </task>
     <task id="LOCAL-00020" summary="Fixes">
       <created>1670458671852</created>
       <option name="number" value="00020"/>
       <option name="presentableId" value="LOCAL-00020"/>
       <option name="project" value="LOCAL"/>
       <updated>1670458671852</updated>
     </task>
@@ -552,44 +440,156 @@
     <task id="LOCAL-00052" summary="Arborform .itor_next &amp; .itor_children now are monads (i.e., class Furcation)">
       <created>1675449044917</created>
       <option name="number" value="00052"/>
       <option name="presentableId" value="LOCAL-00052"/>
       <option name="project" value="LOCAL"/>
       <updated>1675449044917</updated>
     </task>
-    <option name="localTasksCounter" value="53"/>
+    <task id="LOCAL-00053" summary="Unit test fix">
+      <created>1675990493576</created>
+      <option name="number" value="00053"/>
+      <option name="presentableId" value="LOCAL-00053"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1675990493576</updated>
+    </task>
+    <task id="LOCAL-00054" summary="Format string typo">
+      <created>1676083314760</created>
+      <option name="number" value="00054"/>
+      <option name="presentableId" value="LOCAL-00054"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676083314760</updated>
+    </task>
+    <task id="LOCAL-00055" summary="Concrete Itorators all return new or clones">
+      <created>1676086137438</created>
+      <option name="number" value="00055"/>
+      <option name="presentableId" value="LOCAL-00055"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676086137438</updated>
+    </task>
+    <task id="LOCAL-00056" summary="Cleanup + tags">
+      <created>1676086170647</created>
+      <option name="number" value="00056"/>
+      <option name="presentableId" value="LOCAL-00056"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676086170647</updated>
+    </task>
+    <task id="LOCAL-00057" summary="Itorator refactor; postorator roll-back">
+      <created>1676259147809</created>
+      <option name="number" value="00057"/>
+      <option name="presentableId" value="LOCAL-00057"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676259147809</updated>
+    </task>
+    <task id="LOCAL-00058" summary="Itorator function decorations">
+      <created>1676339237212</created>
+      <option name="number" value="00058"/>
+      <option name="presentableId" value="LOCAL-00058"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676339237212</updated>
+    </task>
+    <task id="LOCAL-00059" summary="Grammer, whitespace, and table-formatting">
+      <created>1676339920067</created>
+      <option name="number" value="00059"/>
+      <option name="presentableId" value="LOCAL-00059"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676339920067</updated>
+    </task>
+    <task id="LOCAL-00060" summary="import directive cleanups">
+      <created>1676340047065</created>
+      <option name="number" value="00060"/>
+      <option name="presentableId" value="LOCAL-00060"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676340047065</updated>
+    </task>
+    <task id="LOCAL-00061" summary="import directive cleanups">
+      <created>1676340124266</created>
+      <option name="number" value="00061"/>
+      <option name="presentableId" value="LOCAL-00061"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676340124266</updated>
+    </task>
+    <task id="LOCAL-00062" summary="import directive cleanups">
+      <created>1676340145707</created>
+      <option name="number" value="00062"/>
+      <option name="presentableId" value="LOCAL-00062"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676340145707</updated>
+    </task>
+    <task id="LOCAL-00063" summary="typehint corrections">
+      <created>1676340216892</created>
+      <option name="number" value="00063"/>
+      <option name="presentableId" value="LOCAL-00063"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676340216892</updated>
+    </task>
+    <task id="LOCAL-00064" summary="import cleanups">
+      <created>1676340280650</created>
+      <option name="number" value="00064"/>
+      <option name="presentableId" value="LOCAL-00064"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676340280650</updated>
+    </task>
+    <task id="LOCAL-00065" summary="Unit test count update">
+      <created>1676340314361</created>
+      <option name="number" value="00065"/>
+      <option name="presentableId" value="LOCAL-00065"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676340314361</updated>
+    </task>
+    <task id="LOCAL-00066" summary="Refactor typos &amp; bugfixes">
+      <created>1676602196976</created>
+      <option name="number" value="00066"/>
+      <option name="presentableId" value="LOCAL-00066"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676602196976</updated>
+    </task>
+    <task id="LOCAL-00067" summary="test_limit subtests expansion">
+      <created>1676602496661</created>
+      <option name="number" value="00067"/>
+      <option name="presentableId" value="LOCAL-00067"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676602496661</updated>
+    </task>
+    <task id="LOCAL-00068" summary="Typehint and PEP cleanups">
+      <created>1676602967110</created>
+      <option name="number" value="00068"/>
+      <option name="presentableId" value="LOCAL-00068"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1676602967110</updated>
+    </task>
+    <option name="localTasksCounter" value="69"/>
     <servers/>
   </component>
   <component name="VcsManagerConfiguration">
-    <MESSAGE value="typos"/>
-    <MESSAGE value="Sentence improvements"/>
-    <MESSAGE value="Whitespace PEP fixes"/>
-    <MESSAGE value="Typos"/>
-    <MESSAGE value="Typos and doc edits"/>
-    <MESSAGE value="Xml Doc edits"/>
-    <MESSAGE value="__version__ = '1.0.0.a7'"/>
-    <MESSAGE value="ascii_box updates"/>
-    <MESSAGE value="peduncle -&gt; pepo"/>
-    <MESSAGE value="Documentation arborform stub"/>
-    <MESSAGE value="arborform module structuring"/>
-    <MESSAGE value="itorator import cleanup"/>
-    <MESSAGE value="Pep whitespace cleanups"/>
-    <MESSAGE value="regex expansion"/>
     <MESSAGE value="Documentation spelling and typo fixes"/>
     <MESSAGE value="Ascii box from_corners redo"/>
     <MESSAGE value="Ascii box rotation approach complete"/>
     <MESSAGE value="Ascii box exception on un-mappable corner"/>
     <MESSAGE value="Large refactoring to address circular TypeDef issue"/>
     <MESSAGE value="Typehting pawpaw.Ito -&gt; Ito as appropriate; added .tag to itorator"/>
     <MESSAGE value="Added .tag to postorator"/>
     <MESSAGE value="type_magic cleanup &amp; tests"/>
     <MESSAGE value="Exceeded 4k unit tests"/>
     <MESSAGE value="Whitespace"/>
     <MESSAGE value="Arborform .itor_next &amp; .itor_children now are monads (i.e., class Furcation)"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Arborform .itor_next &amp; .itor_children now are monads (i.e., class Furcation)"/>
+    <MESSAGE value="Unit test fix"/>
+    <MESSAGE value="Format string typo"/>
+    <MESSAGE value="Concrete Itorators all return new or clones"/>
+    <MESSAGE value="Cleanup + tags"/>
+    <MESSAGE value="Itorator refactor; postorator roll-back"/>
+    <MESSAGE value="Itorator function decorations"/>
+    <MESSAGE value="Grammer, whitespace, and table-formatting"/>
+    <MESSAGE value="import directive cleanups"/>
+    <MESSAGE value="typehint corrections"/>
+    <MESSAGE value="import cleanups"/>
+    <MESSAGE value="Unit test count update"/>
+    <MESSAGE value="Refactor typos &amp; bugfixes"/>
+    <MESSAGE value="test_limit subtests expansion"/>
+    <MESSAGE value="Typehint and PEP cleanups"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Typehint and PEP cleanups"/>
   </component>
   <component name="XDebuggerManager">
     <breakpoint-manager>
       <breakpoints>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_xml_parser.py</url>
           <line>15</line>
@@ -623,20 +623,20 @@
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_xml_parser.py</url>
           <line>130</line>
           <option name="timeStamp" value="82"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_ito.py</url>
-          <line>367</line>
+          <line>402</line>
           <option name="timeStamp" value="83"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_ito.py</url>
-          <line>340</line>
+          <line>375</line>
           <option name="timeStamp" value="84"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tinker.py</url>
           <line>189</line>
           <option name="timeStamp" value="91"/>
         </line-breakpoint>
@@ -668,30 +668,79 @@
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_type_magic.py</url>
           <line>144</line>
           <option name="timeStamp" value="133"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/tests/test_itorator.py</url>
-          <line>81</line>
+          <line>97</line>
           <option name="timeStamp" value="134"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
-          <url>file://$PROJECT_DIR$/pawpaw/arborform/itorator/itorator.py</url>
-          <line>114</line>
-          <option name="timeStamp" value="135"/>
+          <url>file://$PROJECT_DIR$/pawpaw/ito.py</url>
+          <line>1351</line>
+          <option name="timeStamp" value="137"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/docs/demos/us_constitution/us_constitution.py</url>
+          <line>72</line>
+          <option name="timeStamp" value="138"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/docs/demos/us_constitution/us_constitution.py</url>
+          <line>71</line>
+          <option name="timeStamp" value="139"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/test_itorator.py</url>
+          <line>135</line>
+          <option name="timeStamp" value="144"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/test_itorator.py</url>
+          <line>217</line>
+          <option name="timeStamp" value="146"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/test_itorator.py</url>
+          <line>287</line>
+          <option name="timeStamp" value="147"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/test_itorator.py</url>
+          <line>294</line>
+          <option name="timeStamp" value="149"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/test_itorator.py</url>
+          <line>307</line>
+          <option name="timeStamp" value="150"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/test_itorator.py</url>
+          <line>305</line>
+          <option name="timeStamp" value="151"/>
         </line-breakpoint>
         <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
           <url>file://$PROJECT_DIR$/pawpaw/arborform/itorator/itorator.py</url>
-          <line>76</line>
-          <option name="timeStamp" value="136"/>
+          <line>127</line>
+          <option name="timeStamp" value="154"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/test_itorator_extract.py</url>
+          <line>43</line>
+          <option name="timeStamp" value="155"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/tests/test_itorator_extract.py</url>
+          <line>42</line>
+          <option name="timeStamp" value="157"/>
+        </line-breakpoint>
+        <line-breakpoint enabled="true" suspend="THREAD" type="python-line">
+          <url>file://$PROJECT_DIR$/pawpaw/arborform/itorator/extract.py</url>
+          <line>71</line>
+          <option name="timeStamp" value="160"/>
         </line-breakpoint>
       </breakpoints>
     </breakpoint-manager>
-    <watches-manager>
-      <configuration name="tests">
-        <watch expression="self.parser"/>
-        <watch expression="func_p" language="Python"/>
-      </configuration>
-    </watches-manager>
   </component>
 </project>
```

### Comparing `pawpaw-1.0.0a8/docs/0. Introduction.md` & `pawpaw-1.0.0a9/docs/0. Introduction.md`

 * *Files 0% similar despite different names*

```diff
@@ -209,19 +209,19 @@
 >>>
 >>> wrds_nums = arborform.Extract(regex.compile(r'(?P<word>[a-z]+) (?P<number>\d+)'))
 >>> phrases.itor_children = wrds_nums
 >>>
 >>> chrs_digs = arborform.Extract(regex.compile(r'(?P<char>[a-z])+|(?P<digit>\d)+'))
 >>> wrds_nums.itor_children = chrs_digs
 >>>
->>> root.children.add(*phrases.traverse(root))
+>>> root.children.add(*phrases(root))
 >>>
 >>> tree_vis = visualization.pepo.Tree()
 >>> print(tree_vis.dumps(root))
-(0, 45) 'root' : 'nine 9 ten 10 eleve…LVE 12 thirteen 13'
+(0, 45) 'root' : 'nine 9 ten 10 eleven…ELVE 12 thirteen 13'
 ├──(0, 6) 'Phrase' : 'nine 9'
 │  ├──(0, 4) 'word' : 'nine'
 │  │  ├──(0, 1) 'char' : 'n'
 │  │  ├──(1, 2) 'char' : 'i'
 │  │  ├──(2, 3) 'char' : 'n'
 │  │  └──(3, 4) 'char' : 'e'
 │  └──(5, 6) 'number' : '9'
```

### Comparing `pawpaw-1.0.0a8/docs/1. Segment and Span.md` & `pawpaw-1.0.0a9/docs/1. Segment and Span.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/docs/2. In Text Object.md` & `pawpaw-1.0.0a9/docs/2. In Text Object.md`

 * *Files 2% similar despite different names*

```diff
@@ -150,15 +150,15 @@
 >>> tree_vis = pawpaw.visualization.pepo.Tree()
 >>> print(tree_vis.dumps(i))
 (0, 8) '0' : 'John Doe'
 ├──(0, 4) 'fn' : 'John'
 └──(5, 8) 'ln' : 'Doe'
 ```
 
-A variable length argument, ``exclude_keys``, can be used to indicate which groups should be excluded from the result.  Note that a ``ValueError`` is raised if you include zero in ``exclude_keys``.  This is because ``.from_match`` returns a single Ito whose root is the entire-match.  Excluding the zero-match could potentially result in a return value consiting of more than one tree, and so it is not allowed.
+A variable length argument, ``exclude_keys``, can be used to indicate which groups should be excluded from the result.  Note that a ``ValueError`` is raised if you include zero in ``exclude_keys``.  This is because ``.from_match`` returns a single Ito whose root is the entire-match.  Excluding the zero-match could potentially result in a return value consisting of more than one tree, and so it is not allowed.
 
 ```python
 >>> i = str(Ito.from_match(m, 'fn'))
 >>> print(tree_vis.dumps(i))
 (0, 8) '0' : 'John Doe'
 └──(5, 8) 'ln' : 'Doe'
 ```
@@ -319,14 +319,22 @@
 >>> j = i.clone(stop=3)
 >>> str(j)
 '123'
 >>> j.value()
 123
 ```
 
+### Indexing
+
+The ``Ito`` class implements the ``__getitem__`` method, which makes it a sequence.  The behavior is consistent with string:
+
+* Accessing by an integer index returns an Ito matching the character at that position
+* Accessing by a slice returns an Ito matching the span of the slice
+  * In the case of a empty slice, e.g. ito[:0] or ito[n:] (where n >= len(ito)), a *zero-width* ito is returned.  This is the same behavior as 'abc'[:0] or 'abc'[3:], both of which return ''
+
 ### Formatting
 
 ``Ito`` offers extensive compite formatting techniques via its implementation of the ``__format__`` method.  See [Visualization](./3.%20Visualization.md) in the docs for more details.
 
 ### .adopt
 
 The ``.adopt`` method synthesizes a parent for an ``Ito`` sequence in which all elements:
@@ -362,15 +370,15 @@
 
 ### .split_iter
 
 The ``.split_iter`` method creates a generator whose elements are synthesized ``Ito`` objects whose
 edges correspond to a matches for a given ``regex.Pattern``.  The edges are computed based on a boolean
 ``keep_seps`` parameter (defaulted to False) as follows:
 
-1. Element edges computed from the ``.start`` and ``.stop`` of match spans; zero-length metches result in adjacent elements, otherwise
+1. Element edges computed from the ``.start`` and ``.stop`` of match spans; zero-length matches result in adjacent elements, otherwise
 the elements are separated by gaps
 2. Element edges correspond to the ``.stop`` of match spans; elements are all adjacent
 
 The resulting objects have empty ``.children`` collections.
 
 ### .split
 
@@ -460,15 +468,15 @@
 
 An ``Ito`` is fully hierarchical through its ``.parent`` and ``.children`` properties.  This allows an ``Ito`` to both represent a segment *and* act as a node within a graph[^is_tree_graph].
 
 The attributes of an ``Ito`` plus its lineage within a graph provide are topologically complete for determining its relevance.  In other words, an ``Ito`` plus its location within a tree are sufficient information for information retrieval tasks.  Pawpaw features powerful search and query operations to facilitate knowledge discovery and traversal of these trees.
 
 Pawpaw trees, however, are not arbitrary data collection.  Rather, they define segments within a basis text.  Because of this, Pawpaw trees have additional qualities over arbitrarily ordered ones.  Pawpaw tree have these three logical requirements:
 
-1. Zero-length segments are not permissable \[***no empty substrings***\]
+1. Zero-length segments are not permissible \[***no empty substrings***\]
    * Given an ``Ito`` **N**:
 
 $$N.span.start < N.span.stop$$
 
 2. A child segment is always contained by its parent. \[***valid substring***\]
   *  Given a parent ``Ito`` **P** and child ``Ito`` **C**:
```

### Comparing `pawpaw-1.0.0a8/docs/3. Visualization.md` & `pawpaw-1.0.0a9/docs/3. Visualization.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,15 @@
 
 ## Introduction
 
 Pawpaw offers basic visualization tools intended to help develop, test, and debug.
 
 ## Format Strings
 
-Pawpaw's ``Ito`` has a well-defined  ``.__format__`` that makes it possible to specify a format string for
-an ``Ito`` object in [formatted string literals](https://docs.python.org/3/reference/lexical_analysis.html#f-strings) and when using ``str.format()``.
-Two categories of formatting directives are available: Integer and String, each with its own vocabulary and modifiers.  Both formatting directives
-can occur within a single f-string expression.
+Pawpaw's ``Ito`` has a well-defined  ``.__format__`` that makes it possible to specify a format string for an ``Ito`` object in [formatted string literals](https://docs.python.org/3/reference/lexical_analysis.html#f-strings) and when using ``str.format()``.  Two categories of formatting directives are available: Integer and String, each with its own vocabulary and modifiers.  Both formatting directives can occur within a single f-string expression.
 
 ### Integer Expressions
 
 An integer expression has the following form:
 
 ```
 integer expression := directive[:[[fill]align][sign][#][0][width][grouping_option][type]]
@@ -60,21 +57,21 @@
 string expression := directive[![lslice]conversion[rslice]][:[abbr_pos]width[abbr]]
 ```
 
 ### **directive**
 
 The *directive* field indicates which ``str`` value you wish to format, and has one of the following values:
 
-| Directive | Meaning                                                       | Example |
-| :---:     |---------------------------------------------------------------|   ---   |
-| ``'%string'`` | ``.string``                                                   | ``' Hello, world! '`` |
-| ``'%desc'`` | ``.desc``                                                     | ``'phrase'`` |
-| ``'%substr'`` | ``.__str__()``                                                | ``'Hello, world!'`` |
-| ``'%value'`` | ``str(.value())``                                             | ``'Hello, world!'`` |
-| ``'% '`` | zero-length whitespace;</br>used to define expression parsing | ``''`` |
+|   Directive   |                             Meaning                             |         Example         |
+|:-------------:|:---------------------------------------------------------------:|:-----------------------:|
+| ``'%string'`` |                           ``.string``                           |  ``' Hello, world! '``  |
+|  ``'%desc'``  |                            ``.desc``                            |      ``'phrase'``       |
+| ``'%substr'`` |                         ``.__str__()``                          |   ``'Hello, world!'``   |
+| ``'%value'``  |                        ``str(.value())``                        |   ``'Hello, world!'``   |
+|   ``'% '``    |  zero-length whitespace;</br>used to define expression parsing  |         ``''``          |
 
 #### Examples
 
 ```python
 >>> from pawpaw import Ito
 >>> i = Ito('ab12cd', 2, -2, 'phrase')
 >>> f'{i:%desc}'  # .desc
```

### Comparing `pawpaw-1.0.0a8/docs/5. Traversal & Query.md` & `pawpaw-1.0.0a9/docs/5. Traversal & Query.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/docs/6. Xml.md` & `pawpaw-1.0.0a9/docs/6. Xml.md`

 * *Files 3% similar despite different names*

```diff
@@ -46,22 +46,22 @@
 
 ```python
 >>> root.find('*').ito.find(f'*[d:{xml.descriptors.TEXT}]')  # Get untransformed text of element
 ```
 
 ### Usage
 
-Pawpaw's ``XmlParser`` dervies from ``xml.ElementTree.XmlParser``, which by default, uses a C implementation.  However, in order to be able
+Pawpaw's ``XmlParser`` derives from ``xml.ElementTree.XmlParser``, which by default, uses a C implementation.  However, in order to be able
 to annotate objects such as ``xml.ElementTree.Element`` as well as correctly hook methods, the Python implementation must be used instead.
 This can be achieved by adding the following statements to you import section before any references are made to ``xml.ElementTree``:
 
 ```python
 >>> import sys
 >>> # Force Python XML parser, not faster C version so that we can hook methods
->>> sys.modules['_elementtree'] is None
+>>> sys.modules['_elementtree'] = None
 ```
 
 From here, using Pawpaw's XmlParser is straightforward:
 
 ```python
 >>> import xml.etree.ElementTree as ET
 >>> from pawpaw import xml
@@ -136,20 +136,31 @@
 
 Note that the ElementTree.XmlParser is *transformational*, i.e., the resulting ``Element`` objects have text that may be altered from the original, underlying xml:
 
 * xmlns attributes are removed
 * Namespace keys for entity tags & attribute names are replaced with full-namespace values
   - 'mb:id' -> '{ht<span>tp://</span>musicbrainz.org/ns/mmd-1.0#}id'
 * Entity references converted to characters
-  - '&amp;' -> '&'
+  - E.g., '\&amp;' -> '&'
 * Comments and processing instructions removed[^TreeBuilder]
   - 'Robson Jorge &amp; Lincoln Olivetti <!-- 1982, Vinyl -->' -> 'Robson Jorge &amp; Lincoln Olivetti'
 
-Most of the time, these types of transformations are exactly what you need.  However, in some cases you may need access to the original underlying text
-(or even just the offsets.)  This is where Pawpaw comes in.  For example, let's say you need to access the xml comment:
+Most of the time, these types of transformations are exactly what you need.  For example, an Xml element containing this text:
+
+```text
+Ben \&amp; Jerry's
+```
+
+will have a ``.text`` property that returns:
+
+```text
+Ben & Jerry's
+```
+
+On the other hand, in some cases you may need access to the original underlying text (or even just the offsets.)  This is where Pawpaw comes in.  For example, let's say you need to access the xml comment:
  
 ```python
 >>> child = root[0]  # First and only child
 >>>
 >>> child.text  # Element.text has entities converted and comments stripped
 '\n        Robson Jorge & Lincoln Olivetti \n    '
 >>>
@@ -160,19 +171,19 @@
 >>> c = i.find(f'*[d:{xml.descriptors.COMMENT}]')  # Get comment
 >>> f'{c:%span %substr!r}  # Display comment (show span and substr repr)
 "(223, 242) '<!-- 1982 Vinyl -->'"
 ```
 
 Certain ``Ito`` objects have their ``.value_func`` set as follows:
 
-| Descriptor | ``.value_func`` |
-| :---:     |  ---    |
-|  ``descriptors.ELEMENT`` | returns associated ``xml.ElementTree.Element`` |
-|  ``descriptors.TAG`` | returns ``pawpaw.xml.QualifiedName`` for this tag |
-|  ``descriptors.ATTRIBUTES`` | returns associated ``xml.ElementTree.Element.attrib`` |
+|         Descriptor         | ``.value_func`` returns                       |
+|:--------------------------:|-----------------------------------------------|
+|  ``descriptors.ELEMENT``   | associated ``xml.ElementTree.Element``        |
+|    ``descriptors.TAG``     | ``pawpaw.xml.QualifiedName`` for this tag     |
+| ``descriptors.ATTRIBUTES`` | associated ``xml.ElementTree.Element.attrib`` |
 
 Note that you can move bi-directionally between an ``'element'`` type ``Ito`` and ``Element`` instances:
 
 * ``Ito`` → ``Element``
   - via ``Ito.value()``
 * ``Element`` → ``Ito``
   - via ``Element.ito`` attribute
@@ -276,8 +287,8 @@
 
 [^f_str_expr]: If this format string looks strange to you, note that as of Python 3.8, format strings support `self-documenting expressions <https://docs.python.org/3/whatsnew/3.8.html#f-strings-support-for-self-documenting-expressions-and-debugging>`_.
 
 [^add_dict_attr]: As of Python 3.10, there is no way to add an arbitrary attribute to the instances of the base ``dict``.
 
 [^TreeBuilder]: As of Python 3.8, you can pass a reference to a ``TreeBuilder`` to ``ElementTree.XmlParser`` to define how you want comments and processing
 instructions handled.  However, this behavior results in additional ``Element`` objects containing the comments and/or processing instructions, which
-results in an awkward tree structure that has less correspondance to the underlying XML document
+results in an awkward tree structure that has less correspondence to the underlying XML document
```

### Comparing `pawpaw-1.0.0a8/docs/7. NLP.md` & `pawpaw-1.0.0a9/docs/7. NLP.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # NLP
 
 # Instroduction
 
 Pawpaw is well suited for Natural Language Processing (NLP) software development.  NLP is a deep topic, and it can sometimes be difficult to select which state of the art (SoA) approaches are best suited for your particular data and needs.
 
-The intent of Pawpaw's ``nlp`` module is not serve as a replacement for all of the excellent work that has been done in this field.  Rather, ``nlp`` is available as a "quick and dirty" toolbox for trying out new ideas and approaches.  It offers a good combination of features and performance for lexcial English data.
+The intent of Pawpaw's ``nlp`` module is not serve as a replacement for all of the excellent work that has been done in this field.  Rather, ``nlp`` is available as a "quick and dirty" toolbox for trying out new ideas and approaches.  It offers a good combination of features and performance for lexical English data.
 
 *More coming soon...*
```

### Comparing `pawpaw-1.0.0a8/docs/8. Serialization.md` & `pawpaw-1.0.0a9/docs/8. Serialization.md`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/docs/Using Pawpaw with nltk.md` & `pawpaw-1.0.0a9/docs/Using Pawpaw with nltk.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 ## Tokenization
 
 ### Convert nlkt tokenizer output to Ito
 
 ```python
 >>> import nltk
->>> import pawpaw
 >>> from pawpaw import Ito
 >>> from nltk.tokenize import WhitespaceTokenizer
 >>> s = 'The quick brown fox.'
 >>> ws_tok = nltk.tokenize.WhitespaceTokenizer()
 >>> tokens = [Ito(s, *span, 'token') for span in ws_tok.span_tokenize(s)]
 >>> [str(i) for i in tokens]
 ['The', 'quick', 'brown', 'fox.']
@@ -21,33 +20,33 @@
 ```python
 >>> import nltk
 >>> import regex
 >>> from pawpaw import Ito, arborform
 >>> ws_tok = nltk.tokenize.WhitespaceTokenizer()
 >>> splitter = arborform.Split(regex.compile(ws_tok._pattern, ws_tok._flags))
 >>> i = Ito('The quick brown fox.')
->>> [str(i) for i in splitter.traverse(i)]
+>>> [str(i) for i in splitter(i)]
 ['The', 'quick', 'brown', 'fox.']
 ```
 
 ### Chaining NLP
 
 ```python
->>> from pawpaw import Ito, arborform
+>>> from pawpaw import Ito, arborform, visualization
 >>> s = 'Here is one sentence.  Here is another.'
 >>> i = Ito(s)
 >>>
 >>> nltk_tok = nltk.tokenize
->>> sent_itor = pawpaw.arborform.Itorator.wrap(lambda ito: ito.from_substrings(ito, *nltk_tok.sent_tokenize(str(ito))))
+>>> sent_itor = arborform.Itorator.wrap(lambda ito: ito.from_substrings(ito, *nltk_tok.sent_tokenize(str(ito))))
 >>>
->>> word_itor = pawpaw.arborform.Itorator.wrap(lambda ito: ito.from_substrings(ito, *nltk_tok.word_tokenize(str(ito))))
+>>> word_itor = arborform.Itorator.wrap(lambda ito: ito.from_substrings(ito, *nltk_tok.word_tokenize(str(ito))))
 >>> sent_itor.itor_children = word_itor
 >>>
->>> i.children.add(*sent_itor.traverse(i))
->>> vis_tree = pawpaw.visualization.pepo.Tree()
+>>> i.children.add(*sent_itor(i))
+>>> vis_tree = visualization.pepo.Tree()
 >>> print(vis_tree.dumps(i))
 (0, 39) 'None' : 'Here is one sentence.  Here is another.'
 ├──(0, 21) 'None' : 'Here is one sentence.'
 │  ├──(0, 4) 'None' : 'Here'
 │  ├──(5, 7) 'None' : 'is'
 │  ├──(8, 11) 'None' : 'one'
 │  ├──(12, 20) 'None' : 'sentence'
```

### Comparing `pawpaw-1.0.0a8/docs/demos/gettysburg_address/gettysburg_address.txt` & `pawpaw-1.0.0a9/docs/demos/gettysburg_address/gettysburg_address.txt`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/docs/demos/us_constitution/us_constitution.txt` & `pawpaw-1.0.0a9/docs/demos/us_constitution/us_constitution.txt`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/images/pawpaw.png` & `pawpaw-1.0.0a9/images/pawpaw.png`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/images/pawpaw2.png` & `pawpaw-1.0.0a9/images/pawpaw2.png`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/pawpaw/__init__.py` & `pawpaw-1.0.0a9/pawpaw/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from pawpaw.errors import Errors
 del errors
 
 import pawpaw._type_magic as type_magic
 del _type_magic
 
-from pawpaw._predicated_value import F_PREDICATE, PredicatedValue
+from pawpaw._predicated_value import P_A, PredicatedValue
 del _predicated_value
 
 from pawpaw._furcation import Furcation
 del _furcation
 
 from pawpaw.span import Span
 del span
```

### Comparing `pawpaw-1.0.0a8/pawpaw/_furcation.py` & `pawpaw-1.0.0a9/pawpaw/_furcation.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 from pawpaw import Errors, PredicatedValue, type_magic
 
 I = typing.TypeVar('I')  # Input to predicate
 R = typing.TypeVar('R')  # Return value type; should be "anything but None", but Python lacks this ability
 
 
 class Furcation(list[PredicatedValue], typing.Generic[I, R]):
-    C_ITEM = PredicatedValue | tuple[typing.Callable[[I], bool], R | None] | typing.Callable[[I], bool] | R
+    P_I = typing.Callable[[I], bool]
+    C_ITEM = PredicatedValue | tuple[P_I, R | None] | P_I | R
 
     @classmethod
     def tautology(cls, item: I) -> bool:
         return True
 
-    def evaluate(self, item: I) -> R | None:
+    def __call__(self, item: I) -> R | None:
         i_typ, r_typ = self.generic_types()
 
         if not type_magic.isinstance_ex(item, i_typ):
             raise Errors.parameter_invalid_type('item', item, i_typ)
 
         for pv in self:
             if pv.predicate(item):
@@ -30,28 +31,28 @@
 
     def generic_types(self) -> tuple[I, R]:
         return typing.get_args(self.__orig_class__)
 
     def _transform_insertion(self, item: C_ITEM) -> PredicatedValue:
         i_typ, r_typ = self.generic_types()
 
-        if type_magic.isinstance_ex(item, PredicatedValue):
-            return item
-
-        if type_magic.functoid_isinstance(item, typing.Callable[[i_typ], bool]):
-            return PredicatedValue(item, None)
+        if type_magic.isinstance_ex(item, r_typ):
+            return PredicatedValue(self.tautology, item)
 
         if type_magic.isinstance_ex(item, tuple) and \
             len(item) == 2 and \
             type_magic.functoid_isinstance(item[0], typing.Callable[[i_typ], bool]) and \
             type_magic.isinstance_ex(item[1], r_typ | None):
             return PredicatedValue(item[0], item[1])
 
-        if type_magic.isinstance_ex(item, r_typ):
-            return PredicatedValue(self.tautology, item)
+        if type_magic.isinstance_ex(item, PredicatedValue):
+            return item
+
+        if type_magic.functoid_isinstance(item, typing.Callable[[i_typ], bool]):
+            return PredicatedValue(item, None)
 
         raise Errors.parameter_invalid_type('item', item, PredicatedValue, tuple[typing.Callable[[i_typ], bool], r_typ | None], typing.Callable[[i_typ], bool], r_typ)
 
     def append(self, item: C_ITEM) -> None:
         super().append(self._transform_insertion(item))
 
     def insert(self, index: int, item: C_ITEM) -> None:
```

### Comparing `pawpaw-1.0.0a8/pawpaw/_predicated_value.py` & `pawpaw-1.0.0a9/pawpaw/_predicated_value.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from __future__ import annotations
 import typing
 
 from pawpaw import Errors, type_magic
 
-F_PREDICATE = typing.Callable[[typing.Any], bool]
+P_A = typing.Callable[[typing.Any], bool]
 
 
 class PredicatedValue:
-    def __init__(self, predicate: F_PREDICATE, value: typing.Any):
-        if not type_magic.functoid_isinstance(predicate, F_PREDICATE):
-            raise Errors.parameter_invalid_type('predicate', predicate, F_PREDICATE)
-        self._predicate: F_PREDICATE = predicate
+    def __init__(self, predicate: P_A, value: typing.Any):
+        if not type_magic.functoid_isinstance(predicate, P_A):
+            raise Errors.parameter_invalid_type('predicate', predicate, P_A)
+        self._predicate: P_A = predicate
         self._value: typing.Any = value
 
     @property
-    def predicate(self) -> F_PREDICATE:
+    def predicate(self) -> P_A:
         return self._predicate
 
     @property
     def value(self) -> typing.Any:
         return self._value
```

### Comparing `pawpaw-1.0.0a8/pawpaw/_type_magic.py` & `pawpaw-1.0.0a9/pawpaw/_type_magic.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/pawpaw/_version.py` & `pawpaw-1.0.0a9/pawpaw/_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import typing
 
-__version__ = '1.0.0.a8'
+__version__ = '1.0.0.a9'
 """The str literal that build, setup, documentation, and other tools typically want
 """
 
 
 class _PreRelease(typing.NamedTuple):
     kind: str  # 'a', 'b', or 'rc' : see https://peps.python.org/pep-0440/
     number: int
```

### Comparing `pawpaw-1.0.0a8/pawpaw/errors.py` & `pawpaw-1.0.0a9/pawpaw/errors.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,38 @@
 from __future__ import annotations
 import inspect
 import types
 import typing
+import enum
 
 
 class Errors:
     @classmethod
     def parameter_not_none(cls, name: str) -> ValueError:
         return ValueError(f'parameter \'{name}\' can not be None')
 
     @classmethod
     def parameter_neither_none_nor_empty(cls, name: str) -> ValueError:
         return ValueError(f'parameter \'{name}\' can be neither None nor empty')
 
     @classmethod
+    def parameter_enum_not_in(cls, name: str, value: typing.Any, enum_: enum.Enum) -> ValueError:
+        return ValueError(f'parameter \'{name}\' is not a valid {enum_.__name__}')
+
+    @classmethod
     def _get_type_strs(cls, *allowed) -> typing.Iterable[str]:
         for t in allowed:
             if hasattr(t, '__qualname__'):
-                if (qn := t.__qualname__) == 'Callable':
+                if t.__qualname__ == 'Callable':
                     yield str(t)
                 else:
                     yield t.__qualname__
             elif hasattr(t, '__bound__'):
                 yield from cls._get_type_strs(t.__bound__)
-            elif (origin := typing.get_origin(t)) is types.UnionType:
+            elif typing.get_origin(t) is types.UnionType:
                 args = typing.get_args(t)
                 yield from cls._get_type_strs(*args)
             elif t is None:
                 yield 'None'
             else:
                 yield repr(t)
```

### Comparing `pawpaw-1.0.0a8/pawpaw/infix.py` & `pawpaw-1.0.0a9/pawpaw/infix.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/pawpaw/ito.py` & `pawpaw-1.0.0a9/pawpaw/ito.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,11 @@
 from __future__ import annotations
 import bisect
 import collections.abc
-import dataclasses
-import inspect
-import itertools
 import json
-import pickle
 import types
 import typing
 
 import regex
 
 import pawpaw.query
 from pawpaw import Infix, Span, Errors, type_magic
@@ -77,15 +73,15 @@
         gn_spans |= {
             i: match.spans(i)
             for i in range(1, match.re.groups + 1)
             if i not in exclude_keys and i not in match.re.groupindex.values()
         }
 
         if isinstance(desc, str):
-            desc_func = lambda match, group: desc
+            desc_func = lambda m, gk: desc
         elif type_magic.functoid_isinstance(desc, Types.F_M_GK_2_DESC):
             desc_func = desc
         else:
             raise Errors.parameter_invalid_type('desc', desc, Types.F_M_GK_2_DESC)
 
         path_stack: typing.List[pawpaw.Ito] = []
         match_itos: typing.List[pawpaw.Ito] = []
@@ -305,18 +301,21 @@
 
     @property
     def value_func(self) -> Types.F_ITO_2_VAL | None:
         return self._value_func
 
     @value_func.setter
     def value_func(self, f: Types.F_ITO_2_VAL | None) -> None:
+        if not (f is None or type_magic.functoid_isinstance(f, Types.F_ITO_2_VAL)):
+            raise Errors.parameter_invalid_type('f', f, Types.F_ITO_2_VAL, None)
         if f is None:
-            delattr(self, 'value')
+            if self._value_func is not None:
+                delattr(self, 'value')
         else:
-            setattr(self, 'value', f.__get__(self))
+            setattr(self, 'value', lambda: f(self))
         self._value_func = f
 
     # endregion
 
     # region serialization
 
     # region pickling
@@ -542,15 +541,15 @@
                 else:  # 'stop'
                     sub = format(self.stop, fstr)
 
             elif directive in self._format_str_directives:
                 if directive == 'string':
                     sub = self._string
                 elif directive == 'desc':
-                    sub = str(self.desc)
+                    sub = self.desc
                 elif directive == 'substr':
                     sub = self.__str__()
                 else:  # 'value'
                     sub = str(self.value())
 
                 if (conv := m.group('conv')) is not None:
                     if conv == 'a':
@@ -1202,23 +1201,23 @@
 
     # endregion
 
     # region query
 
     def find_all(
             self,
-            path: pawpaw.Types.C_PATH,
+            path: pawpaw.Types.C_QPATH,
             values: typing.Dict[str, typing.Any] | None = None,
             predicates: typing.Dict[str, typing.Callable[[int, pawpaw.Ito], bool]] | None = None
     ) -> typing.Iterable[pawpaw.Ito]:
         yield from pawpaw.query.find_all(path, self, values, predicates)
 
     def find(
             self,
-            path: pawpaw.Types.C_PATH,
+            path: pawpaw.Types.C_QPATH,
             values: typing.Dict[str, typing.Any] | None = None,
             predicates: typing.Dict[str, typing.Callable[[int, pawpaw.Ito], bool]] | None = None
     ) -> pawpaw.Ito | None:
         return pawpaw.query.find(path, self, values, predicates)
 
     # endregion
 
@@ -1414,43 +1413,41 @@
                 self.__store.insert(i, ito)
                 ito._set_parent(self.__parent)
 
     # endregion
 
 
 class Types:
+    # Ito
     C_SQ_ITOS = typing.Sequence[Ito]
     C_IT_ITOS = typing.Iterable[Ito]
 
-    F_ITO_2_B = typing.Callable[[Ito], bool]
+    class C_EITO(typing.NamedTuple):
+        index: int
+        ito: Ito
+
+    C_IT_EITOS = typing.Iterable[C_EITO]
+
+    P_ITO = typing.Callable[[Ito], bool]
+    P_EITO = typing.Callable[[C_EITO], bool]
+
     F_ITO_2_VAL = typing.Callable[[Ito], typing.Any]
     F_ITO_2_DESC = typing.Callable[[Ito], str]
     F_ITO_2_SQ_ITOS = typing.Callable[[Ito], C_SQ_ITOS]
     F_ITO_2_IT_ITOS = typing.Callable[[Ito], C_IT_ITOS]
+    F_ITOS_2_ITOS = typing.Callable[[C_IT_ITOS], C_IT_ITOS]
 
+    # Regex
     C_GK = int | str
-    F_M_GK_2_DESC = typing.Callable[[regex.Match, C_GK], str]
-
-    F_ITO_M_GK_2_B = typing.Callable[[Ito | None, regex.Match, C_GK], bool]
-    F_ITO_M_GK_2_DESC = typing.Callable[[Ito | None, regex.Match, C_GK], str]
-    F_M_GK_2_B = typing.Callable[[regex.Match, C_GK], bool]
 
-    class C_BITO(typing.NamedTuple):
-        tf: bool
-        ito: Ito
-
-    C_IT_BITOS = typing.Iterable[C_BITO]
-    F_ITOS_2_BITOS = typing.Callable[[C_IT_ITOS], C_IT_BITOS]
-
-    class C_EITO(typing.NamedTuple):
-        index: int
-        ito: Ito
+    P_M_GK = typing.Callable[[regex.Match, C_GK], bool]
+    P_ITO_M_GK = typing.Callable[[Ito | None, regex.Match, C_GK], bool]
 
-    C_IT_EITOS = typing.Iterable[C_EITO]
+    F_M_GK_2_DESC = typing.Callable[[regex.Match, C_GK], str]
+    F_ITO_M_GK_2_DESC = typing.Callable[[Ito | None, regex.Match, C_GK], str]
 
+    # Query
     C_VALUES = typing.Dict[str, typing.Any] | None
-    C_PREDICATES = typing.Dict[str, typing.Callable[[C_EITO], bool]] | None
-    F_EITO_V_P_2_B = typing.Callable[[C_EITO, C_VALUES, C_PREDICATES], bool]
-
-    C_PATH = str | Ito
+    C_QPS = typing.Dict[str, P_EITO] | None
+    C_QPATH = str | Ito
 
-    C_TYPE_CHECK_T = typing.Type | types.UnionType
+    P_EITO_V_QPS = typing.Callable[[C_EITO, C_VALUES, C_QPS], bool]
```

### Comparing `pawpaw-1.0.0a8/pawpaw/span.py` & `pawpaw-1.0.0a9/pawpaw/span.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/pawpaw/util.py` & `pawpaw-1.0.0a9/pawpaw/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 import typing
 
 import pawpaw
 
 
-# Finds indeces of non-doubled escape chars
+# Finds indices of non-doubled escape chars
 def find_escapes(
     src: str | pawpaw.Ito,
     escape: str = '\\',
     start: int | None = None,
     stop: int | None = None
 ) -> typing.Iterable[int]:
     if isinstance(src, str):
```

### Comparing `pawpaw-1.0.0a8/pawpaw/arborform/itorator/desc.py` & `pawpaw-1.0.0a9/pawpaw/arborform/itorator/desc.py`

 * *Files 20% similar despite different names*

```diff
@@ -10,10 +10,10 @@
         if isinstance(desc, str):
             self._desc_func = lambda ito: desc
         elif type_magic.functoid_isinstance(desc, Types.F_ITO_2_DESC):
             self._desc_func = desc
         else:
             raise Errors.parameter_invalid_type('desc', desc, str | Types.F_ITO_2_DESC)
 
-    def _iter(self, ito: Ito) -> Types.C_SQ_ITOS:
+    def _transform(self, ito: Ito) -> Types.C_SQ_ITOS:
         ito.desc = self._desc_func(ito)
         return ito,
```

### Comparing `pawpaw-1.0.0a8/pawpaw/arborform/itorator/extract.py` & `pawpaw-1.0.0a9/pawpaw/arborform/itorator/extract.py`

 * *Files 24% similar despite different names*

```diff
@@ -8,69 +8,87 @@
 from pawpaw.arborform.itorator import Itorator
 
 
 class Extract(Itorator):
     def __init__(self,
                  re: regex.Pattern,
                  limit: int | None = None,
-                 desc_func: Types.F_ITO_M_GK_2_DESC = lambda ito, match, group: group,
-                 group_filter: collections.abc.Container[str] | Types.F_ITO_M_GK_2_B | None = None,
+                 desc_func: Types.F_ITO_M_GK_2_DESC = lambda ito, match, group_key: str(group_key),
+                 group_filter: collections.abc.Container[str] | Types.P_ITO_M_GK | None = lambda ito, m, gk: isinstance(gk, str),
                  tag: str | None = None):
         super().__init__(tag)
-        if not isinstance(re, regex.Pattern):
-            raise Errors.parameter_invalid_type('re', re, regex.Pattern)
-        self.re = re
+
+        self._group_keys: list[Types.C_GK]
+        self.re = re  # sets ._group_keys
+        
         if limit is not None and not isinstance(limit, int):
             raise Errors.parameter_invalid_type('limit', limit, int)
         self.limit = limit
-        if not type_magic.functoid_isinstance(desc_func, Types.F_ITO_M_GK_2_DESC):
-            raise Errors.parameter_invalid_type('desc_func', desc_func, Types.F_ITO_M_GK_2_DESC)
+
         self.desc_func = desc_func
-        self.group_filter = group_filter
+        self.group_filter = group_filter  
+
+    @classmethod
+    def _get_group_keys(cls, re: regex.Pattern) -> list[Types.C_GK]:
+        rv = [i for i in range(0, re.groups + 1)]
+        for n, i in re.groupindex.items():
+            rv[i] = n
+        return rv
 
     @property
-    def group_filter(self) -> typing.Callable[[Ito, regex.Match, str], bool]:
+    def re(self) -> regex.Pattern:
+        return self._re
+
+    @re.setter
+    def re(self, re: regex.Pattern) -> None:
+        if not isinstance(re, regex.Pattern):
+            raise Errors.parameter_invalid_type('re', re, regex.Pattern)
+        self._re = re
+        self._group_keys = self._get_group_keys(re)
+
+    @property
+    def group_filter(self) -> typing.Callable[[Ito, regex.Match, Types.C_GK], bool]:
         return self._group_filter
 
     @group_filter.setter
-    def group_filter(self, group_filter: collections.abc.Container[str] | Types.F_ITO_M_GK_2_B | None) -> None:
+    def group_filter(self, group_filter: collections.abc.Container[Types.C_GK] | Types.P_ITO_M_GK | None) -> None:
         if group_filter is None:
-            self._group_filter = lambda i, m_, g: True
+            self._group_filter = lambda i, m_, gk: True
 
-        elif type_magic.functoid_isinstance(group_filter, Types.F_ITO_M_GK_2_B):
+        elif type_magic.functoid_isinstance(group_filter, Types.P_ITO_M_GK):
             self._group_filter = group_filter
 
         elif isinstance(group_filter, collections.abc.Container):
-            self._group_filter = lambda i, m_, g: g in group_filter
+            self._group_filter = lambda i, m_, gk: gk in group_filter
 
         else:
             raise Errors.parameter_invalid_type(
                 'group_filter',
                 group_filter,
-                typing.Container[str],
-                Types.F_ITO_M_GK_2_B,
+                typing.Container[Types.C_GK],
+                Types.P_ITO_M_GK,
                 types.NoneType)
 
-    def _iter(self, ito: Ito) -> Types.C_SQ_ITOS:
+    def _transform(self, ito: Ito) -> Types.C_SQ_ITOS:
         rv: typing.List[Ito] = []
-        for count, m in enumerate(ito.regex_finditer(self.re), 1):
+        for count, m in enumerate(ito.regex_finditer(self._re), 1):
             path_stack: typing.List[Ito] = []
             match_itos: typing.List[Ito] = []
-            filtered_gns = (gn for gn in m.re.groupindex.keys() if self._group_filter(ito, m, gn))
-            span_gns = ((span, gn) for gn in filtered_gns for span in m.spans(gn))
-            for span, gn in sorted(span_gns, key=lambda val: (val[0][0], -val[0][1])):
-                ito = ito.clone(*span, desc=self.desc_func(ito, m, gn), clone_children=False)
+            filtered_gks = (gk for i, gk in enumerate(self._group_keys) if self.group_filter(ito, m, i) or self.group_filter(ito, m, gk))
+            span_gks = ((span, gk) for gk in filtered_gks for span in m.spans(gk))
+            for span, gk in sorted(span_gks, key=lambda val: (val[0][0], -val[0][1])):
+                ito = ito.clone(*span, desc=self.desc_func(ito, m, gk), clone_children=False)
                 while len(path_stack) > 0 and (ito.start < path_stack[-1].start or ito.stop > path_stack[-1].stop):
                     path_stack.pop()
                 if len(path_stack) == 0:
                     match_itos.append(ito)
                 else:
                     path_stack[-1].children.add(ito)
 
                 path_stack.append(ito)
 
             rv.extend(match_itos)
 
             if self.limit is not None and self.limit == count:
                 break
 
-        return rv
+        return rv
```

### Comparing `pawpaw-1.0.0a8/pawpaw/arborform/itorator/itorator.py` & `pawpaw-1.0.0a9/pawpaw/arborform/itorator/itorator.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,136 +1,145 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
-import itertools
 import types
 import typing
+import enum
 
 from pawpaw import Types, Errors, Ito, type_magic, PredicatedValue, Furcation
 from pawpaw.arborform.postorator.postorator import Postorator
 
 
 class Itorator(ABC):
-    # define Python user-defined exceptions
-    class SelfChainingError(ValueError):
-        """Raised when attempt is made to add self to the pipeline"""
-        def __init__(self, type: str):
-            self.message = f'can\t add self to {type} chain'
+    @classmethod
+    def wrap(cls, src: Types.F_ITO_2_SQ_ITOS, tag: str | None = None):
+        if type_magic.functoid_isinstance(src, Types.F_ITO_2_SQ_ITOS):
+            return _WrappedItorator(src, tag)
+
+        raise Errors.parameter_invalid_type('src', src, Types.F_ITO_2_SQ_ITOS)
+
+    class ItorChildrenMode(enum.Enum):
+        ADD = enum.auto()
+        REPLACE = enum.auto()
+        DEL = enum.auto()
 
     def __init__(self, tag: str | None = None):
         if tag is not None and not isinstance(tag, str):
             raise Errors.parameter_invalid_type('desc', tag, str)
         self.tag = tag
-        self._itor_next = Furcation[Ito, Itorator]()
+        self._itor_sub = Furcation[Ito, Itorator]()
         self._itor_children = Furcation[Ito, Itorator]()
-        self._postorator: Postorator | Types.F_ITOS_2_BITOS | None = None
-        self._post_func: Types.F_ITOS_2_BITOS | None = None
+        self._itor_children_mode = self.ItorChildrenMode.ADD
+        self._itor_next = Furcation[Ito, Itorator]()
+        self._postorator: Postorator | Types.F_ITOS_2_ITOS | None = None
 
     @property
-    def itor_next(self) -> Furcation[Ito, Itorator]():
-        return self._itor_next
+    def itor_sub(self) -> Furcation[Ito, Itorator]():
+        return self._itor_sub
 
-    @itor_next.setter
-    def itor_next(self, val: Itorator | PredicatedValue | tuple[typing.Callable[[Ito], bool], Itorator | None] | None) -> None:
-        if (val is self) or (isinstance(val, PredicatedValue) and val.value is self) or (isinstance(val, tuple) and val[1] is self):
-            raise Itorator.SelfChainingError('itor_next')
-
-        self._itor_next.clear()
+    @itor_sub.setter
+    def itor_sub(self, val: Itorator | PredicatedValue | tuple[typing.Callable[[Ito], bool], Itorator | None] | None) -> None:
+        self._itor_sub.clear()
         if val is not None:
-            self._itor_next.append(val)
+            self._itor_sub.append(val)
 
     @property
     def itor_children(self) -> Furcation[Ito, Itorator]():
         return self._itor_children
 
     @itor_children.setter
     def itor_children(self, val: Itorator | PredicatedValue | tuple[typing.Callable[[Ito], bool], Itorator | None] | None) -> None:
-        if (val is self) or (isinstance(val, PredicatedValue) and val.value is self) or (isinstance(val, tuple) and val[1] is self):
-            raise Itorator.SelfChainingError('itor_children')
-
         self._itor_children.clear()
         if val is not None:
             self._itor_children.append(val)
 
     @property
-    def postorator(self) -> Postorator | Types.F_ITOS_2_BITOS | None:
+    def itor_children_mode(self) -> ItorChildrenMode:
+        return self._itor_children_mode
+
+    @itor_children_mode.setter
+    def itor_children_mode(self, mode: Itorator.ItorChildrenMode) -> None:
+        if not isinstance(mode, self.ItorChildrenMode):
+            raise Errors.parameter_invalid_type('mode', mode, self.ItorChildrenMode)
+
+        if mode not in self.ItorChildrenMode:
+            raise Errors.parameter_enum_not_in('mode', mode, self.ItorChildrenMode)
+
+        self._itor_children_mode = mode
+
+    @property
+    def itor_next(self) -> Furcation[Ito, Itorator]():
+        return self._itor_next
+
+    @itor_next.setter
+    def itor_next(self, val: Itorator | PredicatedValue | tuple[typing.Callable[[Ito], bool], Itorator | None] | None) -> None:
+        self._itor_next.clear()
+        if val is not None:
+            self._itor_next.append(val)
+
+    @property
+    def postorator(self) -> Postorator | Types.F_ITOS_2_ITOS | None:
         return self._postorator
 
     @postorator.setter
-    def postorator(self, val: Postorator | Types.F_ITOS_2_BITOS | None):
-        if val is None or type_magic.functoid_isinstance(val, Types.F_ITOS_2_BITOS):
-            self._postorator = self._post_func = val
-        elif isinstance(val, Postorator):
+    def postorator(self, val: Postorator | Types.F_ITOS_2_ITOS | None):
+        if val is None or isinstance(val, Postorator):
             self._postorator = val
-            self._post_func = val.traverse
         else:
-            raise Errors.parameter_invalid_type('val', val, Postorator, Types.F_ITOS_2_BITOS, types.NoneType)
+            raise Errors.parameter_invalid_type('val', val, Postorator, Types.F_ITOS_2_ITOS, types.NoneType)
 
     @abstractmethod
-    def _iter(self, ito: Ito) -> Types.C_SQ_ITOS:
+    def _transform(self, ito: Ito) -> Types.C_SQ_ITOS:
         pass
 
-    def _do_children(self, ito: Ito) -> None:
-        if (itor_c := self._itor_children.evaluate(ito)) is not None:
-            for c in itor_c._traverse(ito, True):
-                pass  # force iter walk
+    def __do_sub(self, ito: Ito) -> Types.C_IT_ITOS:
+        if (itor_s := self._itor_sub(ito)) is None:
+            yield ito
+        else:
+            yield from itor_s._traverse(ito)
+
+    def __do_children(self, ito: Ito):
+        if (itor_c := self._itor_children(ito)) is not None:
+            children = [*itor_c._traverse(ito)]
+
+            if self._itor_children_mode == self.ItorChildrenMode.REPLACE:
+                ito.children.clear()
+
+            for c in children:
+                if self._itor_children_mode in (self.ItorChildrenMode.ADD, self.ItorChildrenMode.REPLACE):
+                    ito.children.add(c)
+                else:  # self.ItorChildrenMode.DEL
+                    ito.children.remove(c)
 
-    def _do_next(self, ito: Ito) -> Types.C_IT_ITOS:
-        if (itor_n := self._itor_next.evaluate(ito)) is None:
+    def __do_next(self, ito: Ito) -> Types.C_IT_ITOS:
+        if (itor_n := self._itor_next(ito)) is None:
             yield ito
         else:
             yield from itor_n._traverse(ito)
 
-    def _do_post(self, parent: Ito, itos: Types.C_IT_ITOS) -> Types.C_IT_ITOS:
-        if self._post_func is None:
+    def __do_prior_to_post(self, ito: Ito) -> Types.C_IT_ITOS:
+        for i in self._transform(ito):
+            for s in self.__do_sub(i):
+                self.__do_children(s)
+                yield from self.__do_next(s)
+
+    def __do_post(self, itos: Types.C_IT_ITOS) -> Types.C_IT_ITOS:
+        if self._postorator is None:
             yield from itos
         else:
-            for bito in self._post_func(itos):
-                if bito.tf:
-                    if parent is not None and bito.ito.parent is not parent:
-                        parent.children.add(bito.ito)
-                    yield bito.ito
-                elif (_parent := bito.ito.parent) is not None:
-                    _parent.children.remove(bito.ito)
-
-    def _traverse(self, ito: Ito, as_children: bool = False) -> Types.C_IT_ITOS:
-        # Process ._iter with parent in place
-        curs = self._iter(ito)
-        
-        if as_children:
-            parent = ito
-        elif (parent := ito.parent) is not None:
-            parent.children.remove(ito)  
-  
-        iters: typing.List[iter] = []
-        for cur in curs:
-            if parent is not None and cur.parent is not parent:
-                parent.children.add(cur)
-
-            self._do_children(cur)
-
-            iters.append(self._do_next(cur))
+            yield from self._postorator(itos)
 
-        yield from self._do_post(parent, itertools.chain(*iters))
+    def _traverse(self, ito: Ito) -> Types.C_IT_ITOS:
+        yield from self.__do_post(self.__do_prior_to_post(ito))
 
-    def traverse(self, ito: Ito) -> Types.C_IT_ITOS:
+    def __call__(self, ito: Ito) -> Types.C_IT_ITOS:
         if not isinstance(ito, Ito):
             raise Errors.parameter_invalid_type('ito', ito, Ito)
         yield from self._traverse(ito.clone())
 
-    @classmethod
-    def wrap(cls, src: Itorator | Types.F_ITO_2_SQ_ITOS, tag: str | None = None):
-        if isinstance(src, Itorator):
-            return _WrappedItorator(src.traverse, tag)
-        
-        if type_magic.functoid_isinstance(src, Types.F_ITO_2_SQ_ITOS):
-            return _WrappedItorator(src, tag)
-
-        raise Errors.parameter_invalid_type('src', src, Types.F_ITO_2_SQ_ITOS, Itorator)
-
 
 class _WrappedItorator(Itorator):
     def __init__(self, f: Types.F_ITO_2_SQ_ITOS, tag: str | None = None):
         super().__init__(tag)
         self.__f = f
 
-    def _iter(self, ito: Ito) -> Types.C_SQ_ITOS:
+    def _transform(self, ito: Ito) -> Types.C_SQ_ITOS:
         return self.__f(ito)
```

### Comparing `pawpaw-1.0.0a8/pawpaw/arborform/itorator/split.py` & `pawpaw-1.0.0a9/pawpaw/arborform/itorator/split.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 import enum
 import typing
+import itertools
 
 import regex
 from pawpaw import Span, Ito, Types
 from pawpaw.arborform.itorator import Itorator
 
 
 class Split(Itorator):
@@ -13,18 +14,20 @@
         NONE = 0
         LEADING = 1
         TRAILING = 2
 
     def __init__(
             self,
             re: regex.Pattern,
+            limit: int | None = None,
             group: int | str = 0,
             boundary_retention: BoundaryRetention = BoundaryRetention.NONE,
             return_zero_split: bool = True,
-            desc: str | None = None
+            desc: str | None = None,
+            tag: str | None = None
     ):
         """Given P-O-O-S where P is prefix, - is boundary, O is/are middle part(s), and S is suffix, the
         behavior is as follows:
 
           * BoundaryRetention.NONE -> P O O S : boundaries are discarded (this is an 'ordinary' split operation)
 
           * BoundaryRetention.LEADING -> -O -O -S : boundaries kept as prefixes, leading P is discarded
@@ -40,26 +43,31 @@
         boundary_retention: A rule used to determine if boundaries are discarded, or else how they are kept
         return_zero_split: Indicates how to handle the zero-split condition; when True and splits occur,
           returns a list containing a clone of the input Ito; when False and no splits occur, returns an
           empty list
         desc: Value used for the .desc of any returned Itos; note that a returned Ito can be surrounded by
           0, 1, or 2 boundaries, i.e., there is no clear mapping from a result to a boundary
         """
-        super().__init__()
+        super().__init__(tag)
         self.re = re
+        self.limit = limit
         self.group = group
         self.boundary_retention = boundary_retention
         self.return_zero_split = return_zero_split
         self.desc = desc
-        tag: str | None = None
 
-    def _iter(self, ito: Ito) -> Types.C_SQ_ITOS:
+    def _transform(self, ito: Ito) -> Types.C_SQ_ITOS:
+        if self.limit == 0:
+            return ito,
+
         rv: typing.List[Ito] = []
+        
+        count = 0
         prior: Span | None = None
-        for m in ito.regex_finditer(self.re):
+        for m in itertools.takewhile(lambda i: self.limit is None or count < self.limit, ito.regex_finditer(self.re)):
             cur = Span(*m.span(self.group))
             if prior is None:
                 if self.boundary_retention == self.BoundaryRetention.LEADING:
                     start = stop = 0
                 else:
                     start = ito.start
                     if self.boundary_retention == self.BoundaryRetention.NONE:
@@ -73,14 +81,16 @@
                 elif self.boundary_retention == self.BoundaryRetention.LEADING:
                     start = prior.start
                     stop = cur.start
                 else:  # TRAILING
                     start = prior.stop
                     stop = cur.stop
 
+            count += 1
+
             if start != stop:
                 rv.append(ito.clone(start, stop, self.desc))
 
             prior = cur
 
         if prior is not None and self.boundary_retention != self.BoundaryRetention.TRAILING:
             if self.boundary_retention == self.BoundaryRetention.NONE:
@@ -88,10 +98,10 @@
             else:  # LEADING
                 start = prior.start
             stop = ito.stop
             if start != stop:
                 rv.append(ito.clone(start, stop, self.desc))
 
         if len(rv) == 0 and self.return_zero_split:
-            rv.append(ito.clone(desc=self.desc))
+            rv.append(ito.clone(desc=self.desc))  # TODO : Don't clone this!
 
         return rv
```

### Comparing `pawpaw-1.0.0a8/pawpaw/arborform/postorator/postorator.py` & `pawpaw-1.0.0a9/pawpaw/arborform/postorator/postorator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 from abc import ABC, abstractmethod
-import typing
 
-from pawpaw import Types, Errors
+from pawpaw import Types, type_magic, Errors
 
 
 class Postorator(ABC):
-    @abstractmethod
-    def traverse(self, itos: Types.C_IT_ITOS) -> Types.C_IT_BITOS:
-        ...
-
     @classmethod
-    def wrap(cls, func: Types.F_ITOS_2_BITOS, tag: str | None = None):
-        return _WrappedPostorator(func, tag)
+    def wrap(cls, func: Types.F_ITOS_2_ITOS, tag: str | None = None):
+        if type_magic.functoid_isinstance(func, Types.F_ITOS_2_ITOS):
+            return _WrappedPostorator(func, tag)
+
+        raise Errors.parameter_invalid_type('func', func, Types.F_ITOS_2_ITOS)        
 
     def __init__(self, tag: str | None = None):
         if tag is not None and not isinstance(tag, str):
             raise Errors.parameter_invalid_type('desc', tag, str)
         self.tag = tag
 
+    @abstractmethod
+    def _transform(self, itos: Types.C_IT_ITOS) -> Types.C_IT_ITOS:
+        ...
+
+    def __call__(self, itos: Types.C_IT_ITOS) -> Types.C_IT_ITOS:
+        yield from self._transform(itos)
+
 
 class _WrappedPostorator(Postorator):
-    def __init__(self, f: Types.F_ITOS_2_BITOS, tag: str | None = None):
+    def __init__(self, f: Types.F_ITOS_2_ITOS, tag: str | None = None):
         super().__init__(tag)
         self.__f = f
 
-    def traverse(self, itos: Types.C_IT_ITOS) -> Types.C_IT_BITOS:
-        yield from self.__f(itos)
+    def _transform(self, itos: Types.C_IT_ITOS) -> Types.C_IT_ITOS:
+        yield from self.__f(itos)
```

### Comparing `pawpaw-1.0.0a8/pawpaw/arborform/postorator/stacked_reduce.py` & `pawpaw-1.0.0a9/pawpaw/arborform/postorator/stacked_reduce.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,40 +1,39 @@
-from abc import ABC, abstractmethod
 import typing
 
 from pawpaw import Ito, Types, Errors, type_magic
 from pawpaw.arborform.postorator import Postorator
 
        
 class StackedReduce(Postorator):
     F_SQ_ITOS_2_ITO = typing.Callable[[Types.C_SQ_ITOS], Ito]
-    F_SQ_ITOS_ITO_2_B = typing.Callable[[Types.C_SQ_ITOS, Ito], bool]
+    P_SQ_ITOS_ITO = typing.Callable[[Types.C_SQ_ITOS, Ito], bool]
     
     def __init__(
             self,
             reduce_func: F_SQ_ITOS_2_ITO,
-            push_predicate: Types.F_ITO_2_B,
-            pop_predicate: F_SQ_ITOS_ITO_2_B | None = None,
+            push_predicate: Types.P_ITO,
+            pop_predicate: P_SQ_ITOS_ITO | None = None,
             tag: str | None = None
     ):
         super().__init__(tag)
         if not type_magic.functoid_isinstance(reduce_func, self.F_SQ_ITOS_2_ITO):
             raise Errors.parameter_invalid_type('reduce_func', reduce_func, self.F_SQ_ITOS_2_ITO)
         self.reduce_func = reduce_func
 
-        if not type_magic.functoid_isinstance(push_predicate, Types.F_ITO_2_B):
-            raise Errors.parameter_invalid_type('push_predicate', push_predicate, Types.F_ITO_2_B)
+        if not type_magic.functoid_isinstance(push_predicate, Types.P_ITO):
+            raise Errors.parameter_invalid_type('push_predicate', push_predicate, Types.P_ITO)
         self.push_predicate = push_predicate
 
-        if pop_predicate is None or type_magic.functoid_isinstance(pop_predicate, self.F_SQ_ITOS_ITO_2_B):
+        if pop_predicate is None or type_magic.functoid_isinstance(pop_predicate, self.P_SQ_ITOS_ITO):
             self.pop_predicate = pop_predicate
         else:
-            raise Errors.parameter_invalid_type('pop_predicate', pop_predicate, self.F_SQ_ITOS_ITO_2_B, None)
+            raise Errors.parameter_invalid_type('pop_predicate', pop_predicate, self.P_SQ_ITOS_ITO, None)
 
-    def traverse(self, itos: Types.C_IT_ITOS) -> Types.C_IT_BITOS:
+    def _transform(self, itos: Types.C_IT_ITOS) -> Types.C_IT_ITOS:
         stack: typing.List[Ito] = []
         for ito in itos:
             if stack:
                 if self.pop_predicate is not None and self.pop_predicate(stack, ito):
                     yield self.reduce_func(stack)
                     stack.clear()
                 else:
@@ -44,26 +43,7 @@
                 if self.push_predicate(ito):
                     stack.append(ito)
                 else:
                     yield ito
 
         if stack:
             yield self.reduce_func(stack)
-
-
-# class PromoteChildren(Consolidator):
-#     def __init__(self, predicate: Types.F_ITO_2_B):
-#         super().__init__()
-#         if not type_magic.functoid_isinstance(predicate, Types.F_ITO_2_B):
-#             raise Errors.parameter_invalid_type('predicate', predicate, Types.F_ITO_2_B)
-#         self.predicate = predicate
-
-#     def traverse(self, itos: Types.C_IT_ITOS) -> Types.C_IT_ITOS:
-#         stack: typing.List[pawpaw.Ito] = []
-
-#         for ito in itos:
-#             if self.predicate(ito):
-#                 stack.extend(ito.children)
-#             else:
-#                 stack.append(ito)
-
-#         yield from stack
```

### Comparing `pawpaw-1.0.0a8/pawpaw/arborform/postorator/windowed_join.py` & `pawpaw-1.0.0a9/pawpaw/arborform/postorator/windowed_join.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from abc import ABC, abstractmethod
 import typing
 
 from pawpaw import Ito, Types, Errors, type_magic
 from pawpaw.arborform.postorator import Postorator
 
 
 class WindowedJoin(Postorator):
@@ -30,21 +29,19 @@
 
         if not issubclass(ito_class, Ito):
             raise ValueError('parameter \'ito_class\' ({ito_class}) is not an \'{Ito}\' or subclass.')
         self.ito_class = ito_class
 
         self.desc = desc
 
-    def traverse(self, itos: Types.C_IT_ITOS) -> Types.C_IT_BITOS:
+    def _transform(self, itos: Types.C_IT_ITOS) -> Types.C_IT_ITOS:
         window: typing.List[Ito] = []
         for ito in itos:
             window.append(ito)
             if len(window) == self.window_size:
                 if self.predicate(window):
-                    joined = self.ito_class.join(*window, desc=self.desc)
-                    yield from (Types.C_BITO(False, i) for i in window)
+                    yield self.ito_class.join(*window, desc=self.desc)
                     window.clear()
-                    yield Types.C_BITO(True, joined)
                 else:
-                    yield Types.C_BITO(True, window.pop(0))
+                    yield window.pop(0)
 
-        yield from (Types.C_BITO(True, i) for i in window)
+        yield from window
```

### Comparing `pawpaw-1.0.0a8/pawpaw/nlp/nlp.py` & `pawpaw-1.0.0a9/pawpaw/nlp/nlp.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-import itertools
 import locale
-import typing
 
 import regex
 import pawpaw
 from pawpaw import nuco
 
 # See https://www.unicode.org/Public/UNIDATA/NamesList.txt
 
@@ -452,24 +450,32 @@
 
     _trimmable_ws = list(byte_order_controls.values())
     _trimmable_ws.extend(unicode_white_space_LF_FF.values())
     _trimmable_ws.extend(unicode_white_space_other.values())
 
     _word_pat = r'\w(?:(?:\L<sqs>|-\s*)?\w)*'
 
+    def get_paragraph(self) -> pawpaw.arborform.Itorator:
+        rv = pawpaw.arborform.Split(self._paragraph_re, desc='paragraph', tag='para splitter')
+
+        trimmer = pawpaw.arborform.Itorator.wrap(lambda ito: [ito.str_strip(''.join(self._trimmable_ws))], tag='para trimmer')
+        rv.itor_sub.append(trimmer)
+
+        return rv
+
+    def get_sentence(self) -> pawpaw.arborform.Itorator:
+        return pawpaw.arborform.Split(Sentence().re, desc='sentence', tag='sentence')
+
     def __init__(self, number: Number | None = None, chars: bool = False):
         super().__init__()
 
-        paragraph = pawpaw.arborform.Split(self._paragraph_re, desc='paragraph')
-
-        para_trimmer = pawpaw.arborform.Itorator.wrap(lambda ito: [ito.str_strip(''.join(self._trimmable_ws))])
-        paragraph.itor_next = para_trimmer
+        paragraph = self.get_paragraph()
 
-        sentence = pawpaw.arborform.Split(Sentence().re, desc='sentence')
-        para_trimmer.itor_children = sentence
+        sentence = self.get_sentence()
+        paragraph.itor_children = sentence
 
         self._number = number |nuco| Number()
         word_num_re = regex.compile(self._number.num_pat + r'|(?P<word>' + self._word_pat + r')', regex.DOTALL, sqs=list(unicode_single_quote_marks.values()))
 
         word_number = pawpaw.arborform.Extract(word_num_re)
         sentence.itor_children = word_number
 
@@ -481,9 +487,9 @@
 
     @property
     def number(self) -> Number:
         return self._number
 
     def from_text(self, text: str) -> pawpaw.Ito:
         doc = pawpaw.Ito(text, desc='Document')
-        doc.children.add(*self.itor.traverse(doc))
+        doc.children.add(*self.itor(doc))
         return doc
```

### Comparing `pawpaw-1.0.0a8/pawpaw/query/query.py` & `pawpaw-1.0.0a9/pawpaw/query/_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,27 +39,27 @@
             expression: pawpaw.Ito | str,
             sub_region: pawpaw.Ito | str | int = None) -> ValueError:
         msg = f'unbalanced parentheses in \'{expression}\''
         if isinstance(sub_region, int):
             msg += f' at location {sub_region}'
         elif isinstance(sub_region, (pawpaw.Ito, str)):
             msg += f' in sub-region \'{sub_region}\''
-        raise ValueError(msg)
+        return ValueError(msg)
 
     @classmethod
     def empty_parentheses(
             cls,
             expression: pawpaw.Ito | str,
             sub_region: pawpaw.Ito | str | int = None) -> ValueError:
         msg = f'empty parentheses in \'{expression}\''
         if isinstance(sub_region, int):
             msg += f' at location {sub_region}'
         elif isinstance(sub_region, (pawpaw.Ito, str)):
             msg += f' in sub-region \'{sub_region}\''
-        raise ValueError(msg)
+        return ValueError(msg)
 
 
 def escape(value: str) -> str:
     rv = value.replace('\\', '\\\\')  # Must do backslash before other chars
     for c in filter(lambda e: e != '\\',  MUST_ESCAPE_CHARS):
         rv = rv.replace(c, f'\\{c}')
     return rv
@@ -273,38 +273,38 @@
     @classmethod
     def validate_values(cls, values: pawpaw.Types.C_VALUES) -> pawpaw.Types.C_VALUES:
         if values is None:
             raise ValueError('value expression found, however, no values dictionary supplied')
         return values
     
     @classmethod
-    def validate_predicates(cls, predicates: pawpaw.Types.C_PREDICATES) -> pawpaw.Types.C_PREDICATES:
+    def validate_predicates(cls, predicates: pawpaw.Types.C_QPS) -> pawpaw.Types.C_QPS:
         if predicates is None:
             raise ValueError('predicate expression found, however, no predicates dictionary supplied')
         return predicates
     
     @abstractmethod
-    def func(self, ec: pawpaw.Types.C_EITO, values: pawpaw.Types.C_VALUES, predicates: pawpaw.Types.C_PREDICATES) -> bool:
+    def func(self, ec: pawpaw.Types.C_EITO, values: pawpaw.Types.C_VALUES, predicates: pawpaw.Types.C_QPS) -> bool:
         pass
     
     
 class EcfTautology(Ecf):
-    def func(self, ec: pawpaw.Types.C_EITO, values: pawpaw.Types.C_VALUES, predicates: pawpaw.Types.C_PREDICATES) -> bool:
+    def func(self, ec: pawpaw.Types.C_EITO, values: pawpaw.Types.C_VALUES, predicates: pawpaw.Types.C_QPS) -> bool:
         return True
     
 
 class EcfCombined(Ecf):
     _obs_pat_1 = r'(?<!\\)(?:(?:\\{2})*)'  # Odd number of backslashes ver 1
     _obs_pat_2 = r'\\(\\\\)*'  # Odd number of backslashes ver 2
 
     def __init__(
             self,
             ito: pawpaw.Ito,
-            filters: typing.Sequence[pawpaw.Types.F_EITO_V_P_2_B],
-            operands: typing.Sequence[pawpaw.Ito]
+            filters: list[pawpaw.Types.P_EITO_V_QPS],
+            operands: list[pawpaw.Ito]
     ):
         self.ito = ito
         
         if len(filters) == 0:
             raise ValueError(f'empty filters list')
 
         if len(operands) != len(filters) + 1:
@@ -341,15 +341,15 @@
                 filters[last_open_i:next_closed_i] = [subf]
                 del operands[last_open_i + 1:next_closed_i]
 
         self.filters = filters
         self.operands = operands
 
     @classmethod
-    def _eval(cls, operand: pawpaw.Ito, filter_: pawpaw.Types.F_EITO_V_P_2_B, ec, values, predicates):
+    def _eval(cls, operand: pawpaw.Ito, filter_: pawpaw.Types.P_EITO_V_QPS, ec, values, predicates):
         rv = filter_(ec, values, predicates)
 
         if operand.str_count('~') & 1 == 1:  # bitwise op to determine if n is odd
             rv = not rv
         
         return rv
 
@@ -359,15 +359,15 @@
             if k == '~':
                 continue
 
             for i, op in enumerate(ops):
                 if k in str(op):
                     return i, f
 
-    def func(self, ec: pawpaw.Types.C_EITO, values: pawpaw.Types.C_VALUES, predicates: pawpaw.Types.C_PREDICATES) -> bool:
+    def func(self, ec: pawpaw.Types.C_EITO, values: pawpaw.Types.C_VALUES, predicates: pawpaw.Types.C_QPS) -> bool:
         vals = [self._eval(self.operands[i], f, ec, values, predicates) for i, f in enumerate(self.filters)]
         ops = self.operands[1:-1]
 
         while len(vals) > 1:
             i, op = self._highest_precedence_diadic(ops)
             combined = op(vals[i], vals[i + 1])
             vals[i:i + 2] = [combined]
@@ -383,15 +383,15 @@
     _re = regex.compile(r'\[(?P<not>\~)?(?P<k>[a-z\-]+):\s*(?P<v>.+?)\]', regex.DOTALL)
     _re_balanced_splitter = regex.compile(
         r'(?P<bra>(?<!' + EcfCombined._obs_pat_2 + r')\[(?:(?:' + EcfCombined._obs_pat_2 + r'[\[\]]|[^\[\]])++|(?&bra))*(?<!' + EcfCombined._obs_pat_2 + r')\])',
         regex.DOTALL
     )
 
     @classmethod
-    def _func(cls, not_: str, key: str, value: str) -> pawpaw.Types.F_EITO_V_P_2_B:
+    def _func(cls, not_: str, key: str, value: str) -> pawpaw.Types.P_EITO_V_QPS:
         if key in FILTER_KEYS['desc']:
             if not_ == '~':
                 return lambda ec, values, predicates: ec.ito.desc not in [descape(s) for s in pawpaw.split_unescaped(value, ',')]
             else:
                 return lambda ec, values, predicates: ec.ito.desc in [descape(s) for s in pawpaw.split_unescaped(value, ',')]
 
         if key in FILTER_KEYS['str']:
@@ -469,16 +469,16 @@
                 return lambda ec, values, predicates: ec.ito.value() not in [v for k, v in cls.validate_values(values).items() if k in keys]
             else:
                 return lambda ec, values, predicates: ec.ito.value() in [v for k, v in cls.validate_values(values).items() if k in keys]
 
         raise ValueError(f'unknown filter key \'{key}\'')
 
     def __init__(self, ito: pawpaw.Ito):
-        filters: typing.List[pawpaw.Types.F_EITO_V_P_2_B] = []
-        operands: typing.List[pawpaw.Types.F_EITO_V_P_2_B] = []
+        filters: typing.List[pawpaw.Types.P_EITO_V_QPS] = []
+        operands: typing.List[pawpaw.Types.P_EITO_V_QPS] = []
 
         if len([*ito.regex_finditer(self._re_open_bracket)]) != len([*ito.regex_finditer(self._re_close_bracket)]):
             raise ValueError(f'unbalanced brackets in filter(s) \'{ito}\'')
 
         last = None
         for i, f in enumerate(ito.regex_finditer(self._re_balanced_splitter)):
             start = ito.start if last is None else last.span(0)[1]
@@ -509,31 +509,31 @@
     _re = regex.compile(EcfFilter._obs_pat_1 + r'(?P<sq>\{.*)', regex.DOTALL)
     _re_balanced_splitter = regex.compile(
         r'(?P<cur>(?<!' + EcfCombined._obs_pat_2 + r')\{(?:(?:' + EcfCombined._obs_pat_2 + r'[{}]|[^{}])++|(?&cur))*(?<!' + EcfCombined._obs_pat_2 + r')\})',
         regex.DOTALL
     )
     
     @classmethod
-    def _func(cls, sq: pawpaw.Ito) -> pawpaw.Types.F_EITO_V_P_2_B:
+    def _func(cls, sq: pawpaw.Ito) -> pawpaw.Types.P_EITO_V_QPS:
         query = Query(sq)
         return lambda e, v, p: next(query.find_all(e.ito, v, p), None) is not None
     
     def __init__(self, ito: pawpaw.Ito):
-        subqueries: typing.List[pawpaw.Types.F_EITO_V_P_2_B] = []
+        subqueries: typing.List[pawpaw.Types.P_EITO_V_QPS] = []
         operands: typing.List[pawpaw.Ito] = []
 
         m = ito.regex_search(self._re)
         if m is None:
             raise ValueError(f'Invalid parameter \'subquery\' value: {ito}')
 
         sqm = pawpaw.Ito.from_match_group(m, 'sq')
         if sum(1 for i in sqm.regex_finditer(self._re_open_cur)) != sum(1 for i in sqm.regex_finditer(self._re_close_cur)):
             raise ValueError(f'unbalanced curly braces in sub-query(ies) \'{sqm}\'')
 
-        last: regex.Match = None
+        last: regex.Match | None = None
         for i, sq in enumerate(sqm.regex_finditer(self._re_balanced_splitter)):
             start = ito.start if last is None else last.span(0)[1]
             stop = sq.span(0)[0]
 
             op = pawpaw.Ito(ito.string, start, stop).str_strip()
             if i > 0 and len(op) == 0:
                 raise ValueError(f'missing operator between subqueries \'{last}\' and \'{sq}\'')
@@ -567,22 +567,22 @@
 
         filt_ito = phrase[len(self.axis.ito):unesc_curl].str_strip()
         if len(filt_ito) == 0:
             self.filter = EcfTautology()
         else:
             self.filter = EcfFilter(filt_ito)
 
-    def combined(self, ec: pawpaw.Types.C_EITO, values: pawpaw.Types.C_VALUES, predicates: pawpaw.Types.C_PREDICATES) -> bool:
+    def combined(self, ec: pawpaw.Types.C_EITO, values: pawpaw.Types.C_VALUES, predicates: pawpaw.Types.C_QPS) -> bool:
         return self.filter.func(ec, values, predicates) and self.subquery.func(ec, values, predicates)
 
     def find_all(
             self,
             itos: pawpaw.Types.C_IT_ITOS,
             values: pawpaw.Types.C_VALUES,
-            predicates: pawpaw.Types.C_PREDICATES
+            predicates: pawpaw.Types.C_QPS
     ) -> pawpaw.Types.C_IT_ITOS:
         func = lambda ec: self.combined(ec, values, predicates)
         yield from (ec.ito for ec in filter(func, self.axis.find_all(itos)))
 
 
 class Query:
     @classmethod
@@ -611,15 +611,15 @@
 
         if esc:
             raise ValueError('found escape with no succeeding character in \'{ito_path}\'')
         else:
             i += 1
             yield ito_path[i-ls:i]
 
-    def __init__(self, path: pawpaw.Types.C_PATH):
+    def __init__(self, path: pawpaw.Types.C_QPATH):
         """Creates a compiled query that can be used to search an Ito hierarchy
 
         Args:
             path: one or more phrases, separated by foreslashes:
 
                 path := {phrase}[/phrase][/phrase]...
 
@@ -650,54 +650,54 @@
                 https://www.tutorialspoint.com/xpath/xpath_axes.htm
 
         """
         if isinstance(path, str):
             path = pawpaw.Ito(path)
             
         if not isinstance(path, pawpaw.Ito):
-            raise pawpaw.Errors.parameter_invalid_type('path', path, pawpaw.Types.C_PATH)
+            raise pawpaw.Errors.parameter_invalid_type('path', path, pawpaw.Types.C_QPATH)
             
         if len(path) == 0 or not path.str_isprintable():
             raise pawpaw.Errors.parameter_neither_none_nor_empty('path')
 
         self.phrases = [Phrase(p) for p in self._split_phrases(path)]
 
     def find_all(
         self,
         ito: pawpaw.Ito,
         values: pawpaw.Types.C_VALUES = None,
-        predicates: pawpaw.Types.C_PREDICATES = None
+        predicates: pawpaw.Types.C_QPS = None
     ) -> pawpaw.Types.C_IT_ITOS:
         cur = [ito]
         for phrase in self.phrases:
             cur = phrase.find_all(cur, values, predicates)
         yield from cur
 
     def find(
         self,
         ito: pawpaw.Ito,
         values: pawpaw.Types.C_VALUES = None,
-        predicates: pawpaw.Types.C_PREDICATES = None
+        predicates: pawpaw.Types.C_QPS = None
     ) -> pawpaw.Ito | None:
         return next(self.find_all(ito, values, predicates), None)
 
 
-def compile(path: pawpaw.Types.C_PATH) -> Query:
+def compile(path: pawpaw.Types.C_QPATH) -> Query:
     return Query(path)
 
 
 def find_all(
-        path: pawpaw.Types.C_PATH,
+        path: pawpaw.Types.C_QPATH,
         ito: pawpaw.Ito,
         values: pawpaw.Types.C_VALUES = None,
-        predicates: pawpaw.Types.C_PREDICATES = None
+        predicates: pawpaw.Types.C_QPS = None
 ) -> pawpaw.Types.C_IT_ITOS:
     yield from Query(path).find_all(ito, values, predicates)
 
 
 def find(
-        path: pawpaw.Types.C_PATH,
+        path: pawpaw.Types.C_QPATH,
         ito: pawpaw.Ito,
         values: pawpaw.Types.C_VALUES = None,
-        predicates: pawpaw.Types.C_PREDICATES = None
+        predicates: pawpaw.Types.C_QPS = None
 ) -> pawpaw.Ito | None:
     return next(find_all(path, ito, values, predicates), None)
```

### Comparing `pawpaw-1.0.0a8/pawpaw/visualization/ascii_box.py` & `pawpaw-1.0.0a9/pawpaw/visualization/ascii_box.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/pawpaw/visualization/highlighter.py` & `pawpaw-1.0.0a9/pawpaw/visualization/highlighter.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/pawpaw/visualization/pepo/pepo.py` & `pawpaw-1.0.0a9/pawpaw/visualization/pepo/pepo.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     def __init__(self, indent: str = '    ', children: bool = True, fstr: str = '%desc'):
         super().__init__(indent, children)
         self.fstr = fstr
 
 
 class Compact(_PepoFstr):
     def __init__(self, indent: str = '    ', children: bool = True):
-        super().__init__(indent, children, '%span \'%desc\' : \'%substr!1r1:40…% \'')
+        super().__init__(indent, children, '%span %desc!r : \'%substr!1r1:40…% \'')
         self.children = children
 
     def _dump(self, fs: typing.IO, ei: pawpaw.Types.C_EITO, level: int = 0) -> None:
         fs.write(f'{self.indent * level}{ei.index:,}: {ei.ito:{self.fstr}}{self.linesep}')
 
         if self.children:
             level += 1
@@ -59,15 +59,15 @@
 class Tree(_PepoFstr):
     HORZ = ascii_box.BoxDrawingChar.from_char('─')
     VERT = ascii_box.BoxDrawingChar.from_char('│')
     TEE = ascii_box.BoxDrawingChar.from_char('├')
     ELBOW = ascii_box.BoxDrawingChar.from_char('└')
 
     def __init__(self, indent: str = '  ', children: bool = True):
-        super().__init__(indent, children, '%span \'%desc\' : \'%substr!1r1:^40…% \'')
+        super().__init__(indent, children, '%span %desc!r : \'%substr!1r1:^40…% \'')
         self.children = False
 
     def _dump_children(self, fs: typing.IO, ito: pawpaw.Ito, prefix: str = '') -> None:
         for child in ito.children[:-1]:
             fs.write(f'{prefix}'
                      f'{self.TEE}'
                      f'{self.HORZ.char * len(self.indent)}'
```

### Comparing `pawpaw-1.0.0a8/pawpaw/visualization/sgr/sgr.py` & `pawpaw-1.0.0a9/pawpaw/visualization/sgr/sgr.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/pawpaw/xml/xml_helper.py` & `pawpaw-1.0.0a9/pawpaw/xml/xml_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 # Force Python XML parser, not faster C version so that we can hook methods
 sys.modules['_elementtree'] = None
 import xml.etree.ElementTree as ET
 import typing
 
 import regex
-from pawpaw import Ito, Types, query, xml
+from pawpaw import Ito, query, xml
 from pawpaw.errors import Errors
 from pawpaw.arborform import Extract
 
 
 # See 4 Qualified Names in https://www.w3.org/TR/xml-names/
 class QualifiedName(typing.NamedTuple):
     prefix: Ito | None
@@ -51,15 +51,15 @@
         if isinstance(item, str):
             item = Ito(item)
         elif isinstance(item, ET.Element):
             item = item.ito if hasattr(item, 'ito') else Ito(item.tag)
         elif not isinstance(item, Ito):
             raise Errors.parameter_invalid_type('item', item, str, Ito, ET.Element)
 
-        vals = [*cls._extractor.traverse(item)]
+        vals = [*cls._extractor(item)]
         if len(vals) == 1:
             vals.insert(0, None)
         return cls(*vals)
 
     def __str__(self):
         start = self.namespace.start if self.namespace is not None else self.name.start
         stop = self.name.stop
@@ -86,27 +86,39 @@
         ns = ito.find(f'**[d:{xml.descriptors.NAMESPACE}]')
         name = ito.find(f'**[d:{xml.descriptors.NAME}]')
 
         return QualifiedName(ns, name)
 
     _re_xmlns = regex.compile(r'xmlns(?:\:.+)?', regex.DOTALL)
     _query_xmlns_predicates = {'is_xmlns': lambda ei: ei.ito.regex_fullmatch(XmlHelper._re_xmlns) is not None}
-    _query_xmlns = query.compile(f'*[d:{xml.descriptors.START_TAG}]/*[d:{xml.descriptors.ATTRIBUTES}]/*[d:{xml.descriptors.ATTRIBUTE}]' + '{*[p:is_xmlns]}')
+    __query_xmlns: query.Query = None
+
+    # Lazily instantiate to avoid some circular dependencies
+    @classmethod
+    @property
+    def _query_xmlns(cls) -> query.Query:
+        if cls.__query_xmlns is None:
+            cls.__query_xmlns = query.compile(f'*[d:{xml.descriptors.START_TAG}]/*[d:{xml.descriptors.ATTRIBUTES}]/*[d:{xml.descriptors.ATTRIBUTE}]' + '{*[p:is_xmlns]}')
+
+        return cls.__query_xmlns
 
     @classmethod
     def get_xmlns(cls, element: ET.Element) -> typing.Dict[QualifiedName, Ito]:
+        if cls._query_xmlns is None:
+            cls.__query_xmlns = query.compile(f'*[d:{xml.descriptors.START_TAG}]/*[d:{xml.descriptors.ATTRIBUTES}]/*[d:{xml.descriptors.ATTRIBUTE}]' + '{*[p:is_xmlns]}')
+
         if not isinstance(element, ET.Element):
             raise Errors.parameter_invalid_type('element', element, ET.Element)
         elif not hasattr(element, 'ito'):
             raise XmlErrors.element_lacks_ito_attr('element', element)
         
         return {
             cls.get_qualified_name(xmlns): xmlns.find(f'*[d:{xml.descriptors.VALUE}]')
             for xmlns
-            in cls._query_xmlns.find_all(element.ito, predicates=cls._query_xmlns_predicates)
+            in cls.__query_xmlns.find_all(element.ito, predicates=cls._query_xmlns_predicates)
         }
 
     @classmethod
     def get_prefix_map(cls, element: ET.ElementTree) -> typing.Dict[str, str]:
         """Builds a prefix dict suitable for passing to ET methods such as Element.find('foo:goo', prefix_map);
         keys & values are suitable for passing to xml.etree.ElementTree.register_namespace
```

### Comparing `pawpaw-1.0.0a8/pawpaw/xml/xml_parser.py` & `pawpaw-1.0.0a9/pawpaw/xml/xml_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import sys
 # Force Python XML parser, not faster C version so that we can hook methods
 sys.modules['_elementtree'] = None
 import xml.etree.ElementTree as ET
 import xml.parsers.expat as expat
-import itertools
 
 import regex
-from pawpaw import Span, Ito, xml, Types
+from pawpaw import Span, Ito, xml
 from pawpaw.arborform import Extract
 
         
 class XmlParser(ET.XMLParser):
     _NAMESPACE = r'(?P<' + xml.descriptors.NAMESPACE + r'>[^ :]+):'
     _NAME = r'(?P<' + xml.descriptors.NAME + r'>[^ />=]+)'
     _TAG = r'(?P<' + xml.descriptors.TAG + r'>(?:' + _NAMESPACE + r')?' + _NAME + r')'
@@ -107,27 +106,27 @@
         super().feed(data)
 
     text_comments = Extract
 
     def _find_text(self, start: int, stop: int) -> Ito | None:
         rv = Ito(self._text, start, stop, xml.descriptors.TEXT)
         if len(rv) > 0 and not (self.ignore_empties and rv.str_isspace()):
-            rv.children.add(*self._itor_extract_pi_comments.traverse(rv))
+            rv.children.add(*self._itor_extract_pi_comments(rv))
             return rv
 
     def _extract_itos(self, element: ET.Element) -> None:
         start_tag = Ito(
             self._text,
             element._spans.char.start,
             self._text.index('>', element._spans.char.start + 1) + 1,
             xml.descriptors.START_TAG)
         
-        start_tag.children.add(*self._itor_extract_tag.traverse(start_tag))
+        start_tag.children.add(*self._itor_extract_tag(start_tag))
 
-        attrs = [*self._itor_extract_attributes.traverse(start_tag)]
+        attrs = [*self._itor_extract_attributes(start_tag)]
         if len(attrs) > 0:
             attrs_parent = Ito.join(*attrs, desc=xml.descriptors.ATTRIBUTES)
             attrs_parent.value_func = lambda ito: element.attrib
             attrs_parent.children.add(*attrs)
             start_tag.children.add(attrs_parent)
 
         for tag in start_tag.find_all('**[d:' + xml.descriptors.TAG + ']'):
@@ -136,15 +135,15 @@
 
         if (element._spans.char.stop + 2) < len(self._text) and self._text[element._spans.char.stop:element._spans.char.stop + 2] == '</':
             end_tag = Ito(
                 self._text,
                 element._spans.char.stop,
                 self._text.index('>', element._spans.char.stop + 1) + 1,
                 xml.descriptors.END_TAG)
-            for c in self._itor_extract_tag.traverse(end_tag):
+            for c in self._itor_extract_tag(end_tag):
                 c.value_func = lambda i: xml.QualifiedName.from_src(c)
                 end_tag.children.add(c)
             end_index = end_tag.stop
         else:
             end_tag = None
             end_index = element._spans.char.stop
 
@@ -155,15 +154,15 @@
         
         # Note: Don't use element.text or element.tail here because these values:
         #   a) are absent for whitespace-only strs
         #   b) get html-decoded (to change entity references) and resulting offsets may not match original string
         #   c) could contain pi and comments
         # See https://docs.python.org/3/library/xml.etree.elementtree.html for definition of .text and .tail
 
-        last_child: ET.Element = None        
+        last_child: ET.Element | None = None
         for child in element:
             self._extract_itos(child)
             ito.children.add(child.ito)
 
             if last_child is not None:
                 if (t := self._find_text(last_child.ito.stop, child.ito.start)) is not None:
                     ito.children.add(t)
```

### Comparing `pawpaw-1.0.0a8/tests/test_child_itos.py` & `pawpaw-1.0.0a9/tests/test_child_itos.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/test_furcation.py` & `pawpaw-1.0.0a9/tests/test_furcation.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/test_invoke_func.py` & `pawpaw-1.0.0a9/tests/test_invoke_func.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/test_ito.py` & `pawpaw-1.0.0a9/tests/test_ito.py`

 * *Files 4% similar despite different names*

```diff
@@ -57,29 +57,64 @@
             with self.assertRaises(ValueError):
                 i2._set_parent(i1)
 
         with self.subTest(scenario='parent as self'):
             with self.assertRaises(ValueError):
                 i1._set_parent(i1)
 
-    def test_value_func(self):
+    def test_value_None(self):
         s = 'abc'
         ito = Ito(s)
 
+        # Verify initial state        
         self.assertIsNone(ito.value_func)
-        self.assertEqual(s, ito.value())
 
-        f = lambda i: str(i) * 2
-        ito.value_func = f
-        self.assertEqual(f, ito.value_func)
-        self.assertEqual(s * 2, ito.value())
+        # Ensure setting to None when already None doesn't throw
+        ito.value_func = None
+
+        ito.value_func = lambda ito: len(ito)
+        self.assertIsNotNone(ito.value_func)
 
         ito.value_func = None
         self.assertIsNone(ito.value_func)
-        self.assertEqual(s, ito.value())
+
+    @classmethod
+    def upper_static_method(cls, ito: Ito) -> str:
+        return str(ito).upper()
+
+    def upper_instance_method(self, ito: Ito) -> str:
+        return str(ito).upper()
+
+    def test_value_func(self):
+        def upper_inline_method(ito: Ito) -> str:
+            return str(ito).upper()
+
+        upper_lambda_method = lambda ito: str(ito).upper()
+
+        tests = {
+            'static': self.upper_static_method,
+            'instance': self.upper_instance_method,
+            'inline': upper_inline_method,
+            'lambda': upper_lambda_method,
+        }
+
+        s = 'abc'
+        ito = Ito(s)
+        for t, f in tests.items():
+            with self.subTest(method_type=t):
+                self.assertIsNone(ito.value_func)
+                self.assertEqual(str(ito), ito.value())
+
+                ito.value_func = f
+                self.assertIs(f, ito.value_func)
+                self.assertEqual(f(ito), ito.value())
+
+                ito.value_func = None
+                self.assertIsNone(ito.value_func)
+                self.assertEqual(str(ito), ito.value())
 
     def test_children(self):
         i = Ito('abc')
         self.assertIsNotNone(i.children)
 
     # endregion
```

### Comparing `pawpaw-1.0.0a8/tests/test_ito_ctor.py` & `pawpaw-1.0.0a9/tests/test_ito_ctor.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/test_ito_regex_equivalence_methods.py` & `pawpaw-1.0.0a9/tests/test_ito_regex_equivalence_methods.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/test_ito_serialization.py` & `pawpaw-1.0.0a9/tests/test_ito_serialization.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/test_ito_str_equivalence_methods.py` & `pawpaw-1.0.0a9/tests/test_ito_str_equivalence_methods.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/test_itorator_extract.py` & `pawpaw-1.0.0a9/tests/test_itorator_extract.py`

 * *Files 25% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 class TestExtract(_TestIto):
     def test_iter(self):
         s = 'ten 10 eleven 11 twelve 12 '
         root = Ito(s)
         re = regex.compile(r'(?P<phrase>(?P<word>(?P<char>\w)+) (?P<number>(?P<digit>\d)+) )+')
         itor = Extract(re)
-        rv = itor._iter(root)
+        rv = itor._transform(root)
         itos = rv + [*itertools.chain(*(i.walk_descendants() for i in rv))]
         grouped = {k: [v for v in itos if v.desc == k] for k, val in itertools.groupby(itos, lambda x: x.desc)}
 
         self.assertEqual(3, len(grouped['phrase']))
         for phrase in grouped['phrase']:
             self.assertEqual('phrase', phrase.desc)
             self.assertEqual(2, len(phrase.children))
@@ -29,21 +29,65 @@
 
         self.assertEqual(len('teneleventwelve'), len(grouped['char']))
         self.assertTrue(all(c.parent.desc == 'word' for c in grouped['char']))
 
         self.assertEqual(6, len(grouped['digit']))
         self.assertTrue(all(d.parent.desc == 'number' for d in grouped['digit']))
 
+    def test_group_filter_default(self):
+        s = 'abc'
+        root = Ito(s)
+        name = 'X'
+        re = regex.compile(r'.(.).')
+
+        extract = Extract(re)
+        rv = [*extract(root)]
+        self.assertEqual(0, len(rv))
+
+    def test_group_filter_none(self):
+        s = 'abc'
+        root = Ito(s)
+        name = 'X'
+        re = regex.compile(r'.(.).')
+
+        extract = Extract(re, group_filter=None)
+        expected = root.clone(desc='0')
+        expected.children.add(root.clone(1, 2, desc='1'))
+        rv = [*extract(root)]
+        self.assertEqual(1, len(rv))
+        self.assertEqual(expected, rv[0])
+        self.assertSequenceEqual([*expected.children], [*rv[0].children])
+
+    def test_group_filter_inverse_tautology(self):
+        s = 'abc'
+        root = Ito(s)
+        name = 'X'
+        re = regex.compile(r'.(.).')
+
+        extract = Extract(re, group_filter=lambda ito, match, gk: False)
+        rv = [*extract(root)]
+        self.assertEqual(0, len(rv))
+
+    def test_named_and_unnamed_groups_present_in_match(self):
+        s = 'AB'
+        root = Ito(s)
+        re = regex.compile(r'(.)(?<foo>.)')
+        d = lambda ito, match, group: match.group(1)  # Used first (unnamed) group as descriptor for 'foo'
+        extract = Extract(re, desc_func=d)
+        rv = [*extract(Ito(s))]
+        self.assertEqual(1, len(rv))
+        self.assertEqual(root.clone(1, desc=s[0]), rv[0])
+
     def test_desc_func(self):
         s = 'ten 10 eleven 11 twelve 12 '
         root = Ito(s)
         re = regex.compile(r'(?P<phrase>(?P<word>(?P<char>\w)+) (?P<number>(?P<digit>\d)+) )+')
-        df = lambda i, m, g: g + 'x' if g == 'char' else g
+        df = lambda i, m, gk: str(gk) + 'x' if str(gk) == 'char' else str(gk)
         itor = Extract(re, desc_func=df)
-        rv = itor._iter(root)
+        rv = itor._transform(root)
         itos = rv + [*itertools.chain(*(i.walk_descendants() for i in rv))]
         grouped = {k: [v for v in itos if v.desc == k] for k, val in itertools.groupby(itos, lambda x: x.desc)}
 
         self.assertEqual(3, len(grouped['phrase']))
         for phrase in grouped['phrase']:
             self.assertEqual('phrase', phrase.desc)
             self.assertEqual(2, len(phrase.children))
@@ -62,15 +106,15 @@
 
     def test_limit(self):
         s = 'ten 10 eleven 11 twelve 12 '
         root = Ito(s)
         re = regex.compile(r'(?P<phrase>(?P<word>(?P<char>\w)+) (?P<number>(?P<digit>\d)+) )')
         limit = 2
         itor = Extract(re, limit=2)
-        rv = itor._iter(root)
+        rv = itor._transform(root)
 
         itos = rv + [*itertools.chain(*(i.walk_descendants() for i in rv))]
         grouped = {k: [v for v in itos if v.desc == k] for k, val in itertools.groupby(itos, lambda x: x.desc)}
 
         self.assertEqual(limit, len(grouped['phrase']))
         for phrase in grouped['phrase']:
             self.assertEqual('phrase', phrase.desc)
@@ -90,15 +134,15 @@
 
     def test_group_filter_list(self):
         s = 'ten 10 eleven 11 twelve 12 '
         root = Ito(s)
         re = regex.compile(r'(?P<phrase>(?P<word>(?P<char>\w)+) (?P<number>(?P<digit>\d)+) )+')
         gf = ('phrase', 'word')
         itor = Extract(re, group_filter=gf)
-        rv = itor._iter(root)
+        rv = itor._transform(root)
         itos = rv + [*itertools.chain(*(i.walk_descendants() for i in rv))]
         grouped = {k: [v for v in itos if v.desc == k] for k, val in itertools.groupby(itos, lambda x: x.desc)}
 
         self.assertEqual(3, len(grouped['phrase']))
         for phrase in grouped['phrase']:
             self.assertEqual('phrase', phrase.desc)
             self.assertEqual(1, len(phrase.children))
@@ -112,15 +156,15 @@
 
     def test_group_filter_lambda(self):
         s = 'ten 10 eleven 11 twelve 12 '
         root = Ito(s)
         re = regex.compile(r'(?P<phrase>(?P<word>(?P<char>\w)+) (?P<number>(?P<digit>\d)+) )+')
         gf = lambda i, m, g: g in ('phrase', 'number')
         itor = Extract(re, group_filter=gf)
-        rv = itor._iter(root)
+        rv = itor._transform(root)
         itos = rv + [*itertools.chain(*(i.walk_descendants() for i in rv))]
         grouped = {k: [v for v in itos if v.desc == k] for k, val in itertools.groupby(itos, lambda x: x.desc)}
 
         self.assertEqual(3, len(grouped['phrase']))
         for phrase in grouped['phrase']:
             self.assertEqual('phrase', phrase.desc)
             self.assertEqual(1, len(phrase.children))
```

### Comparing `pawpaw-1.0.0a8/tests/test_itorator_split.py` & `pawpaw-1.0.0a9/tests/test_itorator_split.py`

 * *Files 25% similar despite different names*

```diff
@@ -42,30 +42,30 @@
             ito = Ito(s, desc='root')
             re = self.re_from(sep)
             for brt in Split.BoundaryRetention:
                 with self.subTest(string=s, separator=sep, boundary_retention=brt):
                     expected = self.expected_from(s, sep, brt)
                     desc = 'split'
                     split = Split(re, boundary_retention=brt, desc=desc)
-                    actual = [*split._iter(ito)]
+                    actual = [*split._transform(ito)]
                     self.assertListEqual(expected, [str(i) for i in actual])
                     self.assertTrue(all(i.desc == desc for i in actual))
 
     def test_iter_sep_not_present(self):
         sep = 'XXX'
         s = self.str_from(' ')
         ito = Ito(s)
         re = regex.compile(regex.escape(sep))
         desc='post-split'
         for brt in Split.BoundaryRetention:
             for return_zero_split in True, False:
                 with self.subTest(string=s, separator=sep, boundary_retention=brt, return_zero_split=return_zero_split, desc=desc):
                     expected = [ito.clone(desc=desc)] if return_zero_split else []
                     split = Split(re, boundary_retention=brt, return_zero_split=return_zero_split, desc=desc)
-                    actual = [*split._iter(ito)]
+                    actual = [*split._transform(ito)]
                     self.assertListEqual(expected, actual)
 
     @classmethod
     def zero_width_patterns(cls, sep: str) -> typing.Iterable[regex.Pattern]:
         esc_sep = regex.escape(sep)
         yield r'(?<=' + esc_sep + r')'  # look behind
         yield r'(?=' + esc_sep + r')'  # look ahead
@@ -81,10 +81,57 @@
                     expected = re.split(s)
                     if brt == Split.BoundaryRetention.LEADING:
                         del expected[0]
                     elif brt == Split.BoundaryRetention.TRAILING:
                         del expected[-1]
                     desc = 'split'
                     split = Split(re, boundary_retention=brt, desc=desc)
-                    actual = [*split._iter(ito)]
+                    actual = [*split._transform(ito)]
                     self.assertListEqual(expected, [str(i) for i in actual])
                     self.assertTrue(all(i.desc == desc for i in actual))
+
+    def test_limit(self):
+        s = 'abc'
+        root = Ito(s)
+        
+        re = regex.compile('(?=.)')
+        for limit in None, *range(0, len(s)):
+            with self.subTest(re=re.pattern, limit=limit):
+                splitter = Split(re, limit=limit)
+                rv = [*splitter(root)]
+                expected = []
+                if limit is None:
+                    expected.extend(root)
+                elif limit == 0:
+                    expected.append(root)
+                else:
+                    expected.extend(i for i in root[:limit-1] if len(i) > 0)  # split parts
+                    expected.append(root.clone(limit-1))  # remaining part
+                self.assertSequenceEqual(expected, rv)
+
+        re = regex.compile('(?<=.)')
+        for limit in None, *range(0, len(s)):
+            with self.subTest(re=re.pattern, limit=limit):
+                splitter = Split(re, limit=limit)
+                rv = [*splitter(root)]
+                expected = []
+                if limit is None:
+                    expected.extend(root)
+                elif limit == 0:
+                    expected.append(root)
+                else:
+                    expected.extend(i for i in root[:limit] if len(i) > 0)  # split parts
+                    expected.append(root.clone(limit))  # remaining part
+                self.assertSequenceEqual(expected, rv)
+
+        re = regex.compile('b')
+        for limit in None, *range(0, len(s)):
+            with self.subTest(re=re.pattern, limit=limit):
+                splitter = Split(re, limit=limit)
+                rv = [*splitter(root)]
+                expected = []
+                if limit is None or limit > 0:
+                    expected.extend(root.str_split('b'))
+                else:
+                    expected.append(root)
+                self.assertSequenceEqual(expected, rv)
+
```

### Comparing `pawpaw-1.0.0a8/tests/test_nlp.py` & `pawpaw-1.0.0a9/tests/test_nlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,15 +176,15 @@
     def test_all(self):
         sbd = pawpaw.arborform.Split(pawpaw.nlp.Sentence().re, desc='sentence')
 
         for td in self.test_data:
             with self.subTest(description=td.description, text=td.text):
                 text = pawpaw.Ito(td.text)
                 expected = [*pawpaw.Ito.from_substrings(text, *td.expected, desc='sentence')]
-                actual = [*sbd.traverse(text)]
+                actual = [*sbd(text)]
                 self.assertListEqual(expected, actual)
 
 
 class TestSimpleNlp(_TestIto):
     def test_from_text(self):
         nlp = pawpaw.nlp.SimpleNlp()
         for name, data in {
```

### Comparing `pawpaw-1.0.0a8/tests/test_postorator.py` & `pawpaw-1.0.0a9/tests/test_postorator.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,35 +7,31 @@
 from tests.util import _TestIto
 
 
 class TestPostorator(_TestIto):
     post_desc = 'joined'
 
     @classmethod
-    def simple(cls, itos: Types.C_IT_ITOS) -> Types.C_IT_BITOS:
-        iter_1, iter_2 = tee(itos, 2)
-        joined = Ito.join(*iter_1, desc=cls.post_desc)
-        yield from (Types.C_BITO(False, i) for i in iter_2)
-        yield Types.C_BITO(True, joined)
+    def simple(cls, itos: Types.C_IT_ITOS) -> Types.C_IT_ITOS:
+        yield Ito.join(*itos)
 
     def test_traverse(self):
         for s in 'One', 'One Two', 'One Two Three', 'One Two Three Four':
             itos = Ito(s).str_split()
             with self.subTest(string=s, itos=itos, desc=self.post_desc):
                 wrapped = Postorator.wrap(self.simple)
-                expected = [Types.C_BITO(False, i) for i in itos]
-                expected.append(Types.C_BITO(True, Ito(s, desc=self.post_desc)))
-                actual = [*wrapped.traverse(itos)]
+                expected = [*self.simple(itos)]
+                actual = [*wrapped(itos)]
                 self.assertListEqual(expected, actual)
 
     def test_post(self):
         for s in 'One', 'One Two', 'One Two Three', 'One Two Three Four':
             root = Ito(s, desc='root')
             splitter = Split(regex.compile(r'\s+'))
 
-            rv = [*splitter.traverse(root)]
+            rv = [*splitter(root)]
             self.assertListEqual(root.str_split(), rv)
 
             splitter.postorator = Postorator.wrap(self.simple)
-            expected = [Ito(s, desc=self.post_desc)]
-            actual = [*splitter.traverse(root)]
+            expected = [Ito(s)]
+            actual = [*splitter(root)]
             self.assertListEqual(expected, actual)
```

### Comparing `pawpaw-1.0.0a8/tests/test_postorator_windowed_join.py` & `pawpaw-1.0.0a9/tests/test_postorator_windowed_join.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,30 +11,48 @@
           with self.subTest(window_size=window_size):
               if window_size < 2:
                   with self.assertRaises(ValueError):
                       WindowedJoin(window_size, func)
               else:
                   WindowedJoin(window_size, func)
 
-    def test_traverse(self):
+    def test_traverse_tautology(self):
         func = lambda itos: True
         re = regex.compile(r'\s')
         for s in '', 'One', 'One Two', 'One Two Three', 'One Two Three Four':
             root = Ito(s, desc='root')
             itos = root.split(re)
             desc = 'merged'
             for window_size in 2, 3, 4:
-                with self.subTest(string=s, itos=itos, window_size=window_size, desc=desc):
+                with self.subTest(string=s, window_size=window_size, desc=desc):
                     wj = WindowedJoin(window_size, func, desc=desc)
-                    itos_iter = root.split_iter(re)
-                    actual = [*wj.traverse(itos_iter)]
+                    actual = [*wj(itos)]
                     if len(itos) < window_size:
-                        self.assertListEqual([Types.C_BITO(True, i) for i in itos], actual)
+                        self.assertListEqual(itos, actual)
                     else:
-                        while len(actual) >= window_size:
-                            self.assertTrue(all(not bi.tf for bi in actual[:window_size]))
-                            del actual[:window_size]
-                            if len(actual) > 0:
-                                self.assertTrue(actual[0].tf)
-                                del actual[0]
+                        joined_count = len(itos) // window_size
+                        unjoined_count = len(itos) % window_size
+                        self.assertEqual(joined_count + unjoined_count, len(actual))
 
-                        self.assertTrue(all(bi.tf for bi in actual))
+                        for i in range(0, joined_count):
+                            expected = Ito.join(*itos[i * window_size:i * window_size + window_size], desc=desc)
+                            self.assertEqual(expected, actual[i])
+
+                        if unjoined_count > 0:
+                            tail = itos[-unjoined_count:]
+                            self.assertListEqual(tail, actual[-unjoined_count:])
+
+    def test_traverse_non_tautology(self):
+        s = 'One Two Three Four'
+        root = Ito(s, desc='root')
+        itos = root.str_split()
+
+        window_size = 2
+        func = lambda itos: all(i.str_startswith('T') for i in itos)
+        desc = 'merged'
+
+        wj = WindowedJoin(window_size, func, desc=desc)
+        actual = [*wj(itos)]
+        self.assertEqual(3, len(actual))
+        self.assertEqual(itos[0], actual[0])
+        self.assertEqual(itos[-1], actual[-1])
+        self.assertEqual('Two Three', str(actual[1]))
```

### Comparing `pawpaw-1.0.0a8/tests/test_predicated_value.py` & `pawpaw-1.0.0a9/tests/test_predicated_value.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/test_query_and_traversal.py` & `pawpaw-1.0.0a9/tests/test_query_and_traversal.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/test_sgr.py` & `pawpaw-1.0.0a9/tests/test_sgr.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/test_span.py` & `pawpaw-1.0.0a9/tests/test_span.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/test_type_magic.py` & `pawpaw-1.0.0a9/tests/test_type_magic.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/test_util.py` & `pawpaw-1.0.0a9/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/test_visualization_ascii_box.py` & `pawpaw-1.0.0a9/tests/test_visualization_ascii_box.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/test_xml_helper.py` & `pawpaw-1.0.0a9/tests/test_xml_helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,16 +81,16 @@
             invalid_path = path + '/.[tag=""]'  # ensures path returns nothing
             with self.subTest(xml_sample_index=sample_index, path=invalid_path):
                 actual = xml.XmlHelper.get_element_text_if_found(root, invalid_path)
                 self.assertIsNone(actual)
 
     def test_reverse_find(self):
         for sample_index, sample in enumerate(XML_TEST_SAMPLES):
-            desc_path, anc_pred = sample.descendant_path_with_ancestor_predicate
-            with self.subTest(xml_sample_index=sample_index, descendant_path=desc_path, ancestor_predicate=anc_pred):
+            desC_QPATH, anc_pred = sample.descendant_path_with_ancestor_predicate
+            with self.subTest(xml_sample_index=sample_index, descendant_path=desC_QPATH, ancestor_predicate=anc_pred):
                 root = ET.fromstring(sample.xml, xml.XmlParser())
 
-                desc = root.find(desc_path)
+                desc = root.find(desC_QPATH)
                 self.assertIsNotNone(desc)
 
                 actual = xml.XmlHelper.reverse_find(desc, anc_pred)
                 self.assertIsNotNone(actual)
```

### Comparing `pawpaw-1.0.0a8/tests/test_xml_parser.py` & `pawpaw-1.0.0a9/tests/test_xml_parser.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/tests/util.py` & `pawpaw-1.0.0a9/tests/util.py`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/LICENSE` & `pawpaw-1.0.0a9/LICENSE`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/README.md` & `pawpaw-1.0.0a9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,19 @@
 [![Stargazers][stars-social]][stars-url]
 <br />
 
 <!-- ![Pawpaw](svg/title.svg) -->
 
 # Pawpaw  [![High Performance Text Segmentation, Parsing, & Query][byline-img]][repo]
 
-Pawpaw is a high performance text segmentation framework.  Segments are organized into tree graphs that can be serialized, traversed, and searched using a powerful structured query language.  Pawpaw also features a framework for quickly and easily building complex, pipelined parsers.
+Pawpaw is a high performance parsing & text segmentation framework that allows you to quickly and easily build complex, pipelined parsers.  Segments are automatically organized into tree graphs that can be serialized, traversed, and searched using a powerful structured query language called *plumule*.
 
 <img align="right" width="30%" height="30%" alt="Botanical Drawing: Asimina triloba: the American papaw" src="https://raw.githubusercontent.com/rlayers/pawpaw/master/images/pawpaw.png"> 
 
-- Indexed str and substr representation
+- Indexed string and substring representation
   - Efficient memory utilization
   - Fast processing
   - Pythonic relative indexing and slicing
   - Runtime & polymorphic value extraction
   - Tree graphs for all indexed text
 - Search and Query
   - Search trees using plumule: a powerful structured query language similar to XPATH
@@ -39,15 +39,15 @@
   - Extract *both* ElementTree and Pawpaw datastructures in one go; with cross-linked nodes between trees
 - NLP Support:
   - Pawpaw is ideal for both a) *preprocessing* unstructured text for downstream NLP consumption and b) *storing and searching* NLP generated content
   - Works with other libraries, such as [NLTK](https://www.nltk.org/)
 - Efficient pickling and JSON persistence
   - Security option enables persistence of index-only data, with reference strings re-injected during de-serialization 
 - Stable & Defect Free
-  - Over 4,000 unit tests and counting!
+  - Over 4,100 unit tests and counting!
 
 <div align="center">
   <a href="https://github.com/rlayers/pawpaw/tree/master/docs">Explore the docs</a>
   &nbsp;&nbsp;•&nbsp;&nbsp;
   <a href="https://github.com/rlayers/pawpaw/issues">Request a feature or report a bug</a>
   &nbsp;&nbsp;•&nbsp;&nbsp;
   <a href="https://github.com/rlayers/pawpaw/tree/master/pawpaw">Explore the code</a>
@@ -277,27 +277,30 @@
 <!-- HISTORY & ROADMAP -->
 ## History & Roadmap
 
 Pawpaw is a rewrite of *desponia*, a now-deprecated Python 2.x segmentation framework that was itself based on a prior framework called *Ito*.  Currently in alpha, many components and features are production ready.  However, documentation is still being written and some newer features are still undergoing work.  A rough outline of which components are finalized is as follows:
 
 - [x] arborform
   - [x] itorator
-    - [x] desc
-    - [x] extract
-    - [x] reflect
-    - [x] split
+    - [x] Desc
+    - [x] Extract
+    - [x] Reflect
+    - [x] Split
+    - [x] ValueFunc
   - [x] postorator
-    - [x] stacked_reduce
-    - [x] windowed_join
+    - [ ] StackedReduce
+    - [x] WindowedJoin
 - [x] core
   - [x] Errors
+  - [x] Furcation
   - [x] Infix
   - [x] Ito
   - [x] ItoChildren
   - [x] nuco
+  - [x] PredicatedValue
   - [x] Span
   - [x] Types
 - [ ] documentation & examples
 - [x] query
   - [x] radicle query engine
   - [x] plumule
 - [ ] nlp
```

#### html2text {}

```diff
@@ -1,36 +1,36 @@
    [![Python][Python-shield]][Python-url] [![Contributors][contributors-
 shield]][contributors-url] [![Watchers][watchers-shield]][watchers-url] [!
 [Forks][forks-shield]][forks-url] [![MIT License][license-shield]][license-url]
 [![Stargazers][stars-social]][stars-url]
  # Pawpaw [![High Performance Text Segmentation, Parsing, & Query][byline-img]]
-[repo] Pawpaw is a high performance text segmentation framework. Segments are
-organized into tree graphs that can be serialized, traversed, and searched
-using a powerful structured query language. Pawpaw also features a framework
-for quickly and easily building complex, pipelined parsers. [Botanical Drawing:
-Asimina triloba: the American papaw] - Indexed str and substr representation -
-Efficient memory utilization - Fast processing - Pythonic relative indexing and
-slicing - Runtime & polymorphic value extraction - Tree graphs for all indexed
-text - Search and Query - Search trees using plumule: a powerful structured
-query language similar to XPATH - Combined multiple axes, filters, and
-subqueries sequentially and recursively to any depth - Optionally pre-compile
-queries for increased performance - Rules Pipelining Engine - Develop complex
-lexical parsers with just a few lines of code - Quickly and easily convert
-unstructured text into structured, indexed, & searchable tree graphs - Pre-
-process text for downstream NLP/AI/ML consumers - XML Processing - Features a
-drop-in replacement for ElementTree.XmlParser - Full text indices for all
-elements, attributes, tags, text, etc. - Search the resulting XML using either
-XPATH and/or plumule - Extract *both* ElementTree and Pawpaw datastructures in
-one go; with cross-linked nodes between trees - NLP Support: - Pawpaw is ideal
-for both a) *preprocessing* unstructured text for downstream NLP consumption
-and b) *storing and searching* NLP generated content - Works with other
-libraries, such as [NLTK](https://www.nltk.org/) - Efficient pickling and JSON
-persistence - Security option enables persistence of index-only data, with
-reference strings re-injected during de-serialization - Stable & Defect Free -
-Over 4,000 unit tests and counting!
+[repo] Pawpaw is a high performance parsing & text segmentation framework that
+allows you to quickly and easily build complex, pipelined parsers. Segments are
+automatically organized into tree graphs that can be serialized, traversed, and
+searched using a powerful structured query language called *plumule*.
+[Botanical Drawing: Asimina triloba: the American papaw] - Indexed string and
+substring representation - Efficient memory utilization - Fast processing -
+Pythonic relative indexing and slicing - Runtime & polymorphic value extraction
+- Tree graphs for all indexed text - Search and Query - Search trees using
+plumule: a powerful structured query language similar to XPATH - Combined
+multiple axes, filters, and subqueries sequentially and recursively to any
+depth - Optionally pre-compile queries for increased performance - Rules
+Pipelining Engine - Develop complex lexical parsers with just a few lines of
+code - Quickly and easily convert unstructured text into structured, indexed, &
+searchable tree graphs - Pre-process text for downstream NLP/AI/ML consumers -
+XML Processing - Features a drop-in replacement for ElementTree.XmlParser -
+Full text indices for all elements, attributes, tags, text, etc. - Search the
+resulting XML using either XPATH and/or plumule - Extract *both* ElementTree
+and Pawpaw datastructures in one go; with cross-linked nodes between trees -
+NLP Support: - Pawpaw is ideal for both a) *preprocessing* unstructured text
+for downstream NLP consumption and b) *storing and searching* NLP generated
+content - Works with other libraries, such as [NLTK](https://www.nltk.org/) -
+Efficient pickling and JSON persistence - Security option enables persistence
+of index-only data, with reference strings re-injected during de-serialization
+- Stable & Defect Free - Over 4,100 unit tests and counting!
 Explore_the_docs   â¢   Request_a_feature_or_report_a_bug   â¢   Explore_the
                                      code
  ## Example With Pawpaw, you can start with flattened text like this: ```
 ARTICLE I Section 1: Congress All legislative Powers herein granted shall be
 vested in a Congress of the United States, which shall consist of a Senate and
 House of Representatives. Section 2: The House of Representatives The House of
 Representatives shall be composed of Members chosen every second Year by the
@@ -141,20 +141,21 @@
 are up and running with Pawpaw!
                                                                   (back_to_top)
  ## History & Roadmap Pawpaw is a rewrite of *desponia*, a now-deprecated
 Python 2.x segmentation framework that was itself based on a prior framework
 called *Ito*. Currently in alpha, many components and features are production
 ready. However, documentation is still being written and some newer features
 are still undergoing work. A rough outline of which components are finalized is
-as follows: - [x] arborform - [x] itorator - [x] desc - [x] extract - [x]
-reflect - [x] split - [x] postorator - [x] stacked_reduce - [x] windowed_join -
-[x] core - [x] Errors - [x] Infix - [x] Ito - [x] ItoChildren - [x] nuco - [x]
-Span - [x] Types - [ ] documentation & examples - [x] query - [x] radicle query
-engine - [x] plumule - [ ] nlp - [ ] visualization - [x] ascibox - [x]
-highlighter - [ ] pepo - [x] sgr - [x] xml - [x] XmlHelper - [x] XmlParser
+as follows: - [x] arborform - [x] itorator - [x] Desc - [x] Extract - [x]
+Reflect - [x] Split - [x] ValueFunc - [x] postorator - [ ] StackedReduce - [x]
+WindowedJoin - [x] core - [x] Errors - [x] Furcation - [x] Infix - [x] Ito -
+[x] ItoChildren - [x] nuco - [x] PredicatedValue - [x] Span - [x] Types - [ ]
+documentation & examples - [x] query - [x] radicle query engine - [x] plumule -
+[ ] nlp - [ ] visualization - [x] ascibox - [x] highlighter - [ ] pepo - [x]
+sgr - [x] xml - [x] XmlHelper - [x] XmlParser
                                                                   (back_to_top)
  ## Contributing Contributions to Pawpaw are **greatly appreciated** - please
 refer to the [contributing guildelines](/contributing.md) for details.
                                                                   (back_to_top)
  ## License Distributed under the MIT License. See [LICENSE](LICENSE) for more
 information.
                                                                   (back_to_top)
```

### Comparing `pawpaw-1.0.0a8/pyproject.toml` & `pawpaw-1.0.0a9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pawpaw-1.0.0a8/PKG-INFO` & `pawpaw-1.0.0a9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pawpaw
-Version: 1.0.0a8
+Version: 1.0.0a9
 Summary: High Performance Text Processing & Segmentation Framework
 Project-URL: Homepage, https://github.com/rlayers/pawpaw
 Project-URL: Bug Tracker, https://github.com/rlayers/pawpaw/issues
 Author-email: "Robert L. Ayers" <rlayers@yahoo.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: extract-text,hierarchical-text-segmentation,information-extraction,knowledge-graph,nlp,python,text-processing,text-segmentation,xml-parser
@@ -32,19 +32,19 @@
 [![Stargazers][stars-social]][stars-url]
 <br />
 
 <!-- ![Pawpaw](svg/title.svg) -->
 
 # Pawpaw  [![High Performance Text Segmentation, Parsing, & Query][byline-img]][repo]
 
-Pawpaw is a high performance text segmentation framework.  Segments are organized into tree graphs that can be serialized, traversed, and searched using a powerful structured query language.  Pawpaw also features a framework for quickly and easily building complex, pipelined parsers.
+Pawpaw is a high performance parsing & text segmentation framework that allows you to quickly and easily build complex, pipelined parsers.  Segments are automatically organized into tree graphs that can be serialized, traversed, and searched using a powerful structured query language called *plumule*.
 
 <img align="right" width="30%" height="30%" alt="Botanical Drawing: Asimina triloba: the American papaw" src="https://raw.githubusercontent.com/rlayers/pawpaw/master/images/pawpaw.png"> 
 
-- Indexed str and substr representation
+- Indexed string and substring representation
   - Efficient memory utilization
   - Fast processing
   - Pythonic relative indexing and slicing
   - Runtime & polymorphic value extraction
   - Tree graphs for all indexed text
 - Search and Query
   - Search trees using plumule: a powerful structured query language similar to XPATH
@@ -61,15 +61,15 @@
   - Extract *both* ElementTree and Pawpaw datastructures in one go; with cross-linked nodes between trees
 - NLP Support:
   - Pawpaw is ideal for both a) *preprocessing* unstructured text for downstream NLP consumption and b) *storing and searching* NLP generated content
   - Works with other libraries, such as [NLTK](https://www.nltk.org/)
 - Efficient pickling and JSON persistence
   - Security option enables persistence of index-only data, with reference strings re-injected during de-serialization 
 - Stable & Defect Free
-  - Over 4,000 unit tests and counting!
+  - Over 4,100 unit tests and counting!
 
 <div align="center">
   <a href="https://github.com/rlayers/pawpaw/tree/master/docs">Explore the docs</a>
   &nbsp;&nbsp;•&nbsp;&nbsp;
   <a href="https://github.com/rlayers/pawpaw/issues">Request a feature or report a bug</a>
   &nbsp;&nbsp;•&nbsp;&nbsp;
   <a href="https://github.com/rlayers/pawpaw/tree/master/pawpaw">Explore the code</a>
@@ -299,27 +299,30 @@
 <!-- HISTORY & ROADMAP -->
 ## History & Roadmap
 
 Pawpaw is a rewrite of *desponia*, a now-deprecated Python 2.x segmentation framework that was itself based on a prior framework called *Ito*.  Currently in alpha, many components and features are production ready.  However, documentation is still being written and some newer features are still undergoing work.  A rough outline of which components are finalized is as follows:
 
 - [x] arborform
   - [x] itorator
-    - [x] desc
-    - [x] extract
-    - [x] reflect
-    - [x] split
+    - [x] Desc
+    - [x] Extract
+    - [x] Reflect
+    - [x] Split
+    - [x] ValueFunc
   - [x] postorator
-    - [x] stacked_reduce
-    - [x] windowed_join
+    - [ ] StackedReduce
+    - [x] WindowedJoin
 - [x] core
   - [x] Errors
+  - [x] Furcation
   - [x] Infix
   - [x] Ito
   - [x] ItoChildren
   - [x] nuco
+  - [x] PredicatedValue
   - [x] Span
   - [x] Types
 - [ ] documentation & examples
 - [x] query
   - [x] radicle query engine
   - [x] plumule
 - [ ] nlp
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pawpaw Version: 1.0.0a8 Summary: High Performance
+Metadata-Version: 2.1 Name: pawpaw Version: 1.0.0a9 Summary: High Performance
 Text Processing & Segmentation Framework Project-URL: Homepage, https://
 github.com/rlayers/pawpaw Project-URL: Bug Tracker, https://github.com/rlayers/
 pawpaw/issues Author-email: "Robert L. Ayers"
 yahoo.com> License-Expression: MIT License-File: LICENSE Keywords: extract-
 text,hierarchical-text-segmentation,information-extraction,knowledge-
 graph,nlp,python,text-processing,text-segmentation,xml-parser Classifier:
 Development Status :: 3 - Alpha Classifier: Intended Audience :: Developers
@@ -12,38 +12,38 @@
 Software Development :: Libraries :: Python Modules Classifier: Topic :: Text
 Processing Requires-Python: >=3.10 Requires-Dist: regex>=2022.7.9 Description-
 Content-Type: text/markdown    [![Python][Python-shield]][Python-url] [!
 [Contributors][contributors-shield]][contributors-url] [![Watchers][watchers-
 shield]][watchers-url] [![Forks][forks-shield]][forks-url] [![MIT License]
 [license-shield]][license-url] [![Stargazers][stars-social]][stars-url]
  # Pawpaw [![High Performance Text Segmentation, Parsing, & Query][byline-img]]
-[repo] Pawpaw is a high performance text segmentation framework. Segments are
-organized into tree graphs that can be serialized, traversed, and searched
-using a powerful structured query language. Pawpaw also features a framework
-for quickly and easily building complex, pipelined parsers. [Botanical Drawing:
-Asimina triloba: the American papaw] - Indexed str and substr representation -
-Efficient memory utilization - Fast processing - Pythonic relative indexing and
-slicing - Runtime & polymorphic value extraction - Tree graphs for all indexed
-text - Search and Query - Search trees using plumule: a powerful structured
-query language similar to XPATH - Combined multiple axes, filters, and
-subqueries sequentially and recursively to any depth - Optionally pre-compile
-queries for increased performance - Rules Pipelining Engine - Develop complex
-lexical parsers with just a few lines of code - Quickly and easily convert
-unstructured text into structured, indexed, & searchable tree graphs - Pre-
-process text for downstream NLP/AI/ML consumers - XML Processing - Features a
-drop-in replacement for ElementTree.XmlParser - Full text indices for all
-elements, attributes, tags, text, etc. - Search the resulting XML using either
-XPATH and/or plumule - Extract *both* ElementTree and Pawpaw datastructures in
-one go; with cross-linked nodes between trees - NLP Support: - Pawpaw is ideal
-for both a) *preprocessing* unstructured text for downstream NLP consumption
-and b) *storing and searching* NLP generated content - Works with other
-libraries, such as [NLTK](https://www.nltk.org/) - Efficient pickling and JSON
-persistence - Security option enables persistence of index-only data, with
-reference strings re-injected during de-serialization - Stable & Defect Free -
-Over 4,000 unit tests and counting!
+[repo] Pawpaw is a high performance parsing & text segmentation framework that
+allows you to quickly and easily build complex, pipelined parsers. Segments are
+automatically organized into tree graphs that can be serialized, traversed, and
+searched using a powerful structured query language called *plumule*.
+[Botanical Drawing: Asimina triloba: the American papaw] - Indexed string and
+substring representation - Efficient memory utilization - Fast processing -
+Pythonic relative indexing and slicing - Runtime & polymorphic value extraction
+- Tree graphs for all indexed text - Search and Query - Search trees using
+plumule: a powerful structured query language similar to XPATH - Combined
+multiple axes, filters, and subqueries sequentially and recursively to any
+depth - Optionally pre-compile queries for increased performance - Rules
+Pipelining Engine - Develop complex lexical parsers with just a few lines of
+code - Quickly and easily convert unstructured text into structured, indexed, &
+searchable tree graphs - Pre-process text for downstream NLP/AI/ML consumers -
+XML Processing - Features a drop-in replacement for ElementTree.XmlParser -
+Full text indices for all elements, attributes, tags, text, etc. - Search the
+resulting XML using either XPATH and/or plumule - Extract *both* ElementTree
+and Pawpaw datastructures in one go; with cross-linked nodes between trees -
+NLP Support: - Pawpaw is ideal for both a) *preprocessing* unstructured text
+for downstream NLP consumption and b) *storing and searching* NLP generated
+content - Works with other libraries, such as [NLTK](https://www.nltk.org/) -
+Efficient pickling and JSON persistence - Security option enables persistence
+of index-only data, with reference strings re-injected during de-serialization
+- Stable & Defect Free - Over 4,100 unit tests and counting!
 Explore_the_docs   â¢   Request_a_feature_or_report_a_bug   â¢   Explore_the
                                      code
  ## Example With Pawpaw, you can start with flattened text like this: ```
 ARTICLE I Section 1: Congress All legislative Powers herein granted shall be
 vested in a Congress of the United States, which shall consist of a Senate and
 House of Representatives. Section 2: The House of Representatives The House of
 Representatives shall be composed of Members chosen every second Year by the
@@ -154,20 +154,21 @@
 are up and running with Pawpaw!
                                                                   (back_to_top)
  ## History & Roadmap Pawpaw is a rewrite of *desponia*, a now-deprecated
 Python 2.x segmentation framework that was itself based on a prior framework
 called *Ito*. Currently in alpha, many components and features are production
 ready. However, documentation is still being written and some newer features
 are still undergoing work. A rough outline of which components are finalized is
-as follows: - [x] arborform - [x] itorator - [x] desc - [x] extract - [x]
-reflect - [x] split - [x] postorator - [x] stacked_reduce - [x] windowed_join -
-[x] core - [x] Errors - [x] Infix - [x] Ito - [x] ItoChildren - [x] nuco - [x]
-Span - [x] Types - [ ] documentation & examples - [x] query - [x] radicle query
-engine - [x] plumule - [ ] nlp - [ ] visualization - [x] ascibox - [x]
-highlighter - [ ] pepo - [x] sgr - [x] xml - [x] XmlHelper - [x] XmlParser
+as follows: - [x] arborform - [x] itorator - [x] Desc - [x] Extract - [x]
+Reflect - [x] Split - [x] ValueFunc - [x] postorator - [ ] StackedReduce - [x]
+WindowedJoin - [x] core - [x] Errors - [x] Furcation - [x] Infix - [x] Ito -
+[x] ItoChildren - [x] nuco - [x] PredicatedValue - [x] Span - [x] Types - [ ]
+documentation & examples - [x] query - [x] radicle query engine - [x] plumule -
+[ ] nlp - [ ] visualization - [x] ascibox - [x] highlighter - [ ] pepo - [x]
+sgr - [x] xml - [x] XmlHelper - [x] XmlParser
                                                                   (back_to_top)
  ## Contributing Contributions to Pawpaw are **greatly appreciated** - please
 refer to the [contributing guildelines](/contributing.md) for details.
                                                                   (back_to_top)
  ## License Distributed under the MIT License. See [LICENSE](LICENSE) for more
 information.
                                                                   (back_to_top)
```

