# Comparing `tmp/mmda-0.3.0.tar.gz` & `tmp/mmda-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mmda-0.3.0.tar", last modified: Tue Mar 14 19:18:16 2023, max compression
+gzip compressed data, was "mmda-0.3.6.tar", last modified: Mon Apr 10 18:29:08 2023, max compression
```

## Comparing `mmda-0.3.0.tar` & `mmda-0.3.6.tar`

### file list

```diff
@@ -1,153 +1,152 @@
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.443675 mmda-0.3.0/
--rw-r--r--   0 kylel      (502) staff       (20)    10764 2021-06-29 23:30:11.000000 mmda-0.3.0/LICENSE
--rw-r--r--   0 kylel      (502) staff       (20)     8842 2023-03-14 19:18:16.442878 mmda-0.3.0/PKG-INFO
--rw-r--r--   0 kylel      (502) staff       (20)     7785 2023-03-13 17:31:20.000000 mmda-0.3.0/README.md
--rw-r--r--   0 kylel      (502) staff       (20)     3114 2023-03-14 04:16:03.000000 mmda-0.3.0/pyproject.toml
--rw-r--r--   0 kylel      (502) staff       (20)       38 2023-03-14 19:18:16.444018 mmda-0.3.0/setup.cfg
--rw-r--r--   0 kylel      (502) staff       (20)       38 2022-12-07 01:58:14.000000 mmda-0.3.0/setup.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.268431 mmda-0.3.0/src/
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.274027 mmda-0.3.0/src/ai2_internal/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     4799 2023-03-09 01:33:11.000000 mmda-0.3.0/src/ai2_internal/api.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.276390 mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/__init__.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.285979 mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/data/
--rw-r--r--   0 kylel      (502) staff       (20)   334931 2023-03-07 05:52:23.000000 mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/data/000026bab3c52aa8ff37dc3e155ffbcb506aa1f6.pdf
--rw-r--r--   0 kylel      (502) staff       (20)    96377 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/data/no_bibs.pdf
--rw-r--r--   0 kylel      (502) staff       (20)      185 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/data/no_bibs_vila_span_groups.json
--rw-r--r--   0 kylel      (502) staff       (20)   501454 2023-03-07 05:52:23.000000 mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/data/spanless_bibs_3cf45514384bbb7d083ae53e19bdc22300e648ab.pdf
--rw-r--r--   0 kylel      (502) staff       (20)    59603 2023-03-07 05:52:23.000000 mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/data/spanless_bibs_vila_span_groups.json
--rw-r--r--   0 kylel      (502) staff       (20)     3558 2023-03-07 05:52:23.000000 mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/data/vila_span_groups.json
--rw-r--r--   0 kylel      (502) staff       (20)     5708 2023-03-07 05:52:24.000000 mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/integration_test.py
--rw-r--r--   0 kylel      (502) staff       (20)     5132 2023-03-07 05:52:24.000000 mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/interface.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.286987 mmda-0.3.0/src/ai2_internal/bibentry_predictor/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/bibentry_predictor/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     2269 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/bibentry_predictor/integration_test.py
--rw-r--r--   0 kylel      (502) staff       (20)     3109 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/bibentry_predictor/interface.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.288413 mmda-0.3.0/src/ai2_internal/bibentry_predictor_mmda/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/bibentry_predictor_mmda/__init__.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.290607 mmda-0.3.0/src/ai2_internal/bibentry_predictor_mmda/data/
--rw-r--r--   0 kylel      (502) staff       (20)   285777 2023-03-07 05:52:24.000000 mmda-0.3.0/src/ai2_internal/bibentry_predictor_mmda/data/test_data.json.gz
--rw-r--r--   0 kylel      (502) staff       (20)  1595942 2023-03-07 05:52:24.000000 mmda-0.3.0/src/ai2_internal/bibentry_predictor_mmda/data/test_data_v2_boxes_turn_into_empty_span_groups.json.gz
--rw-r--r--   0 kylel      (502) staff       (20)     5328 2023-03-07 05:52:24.000000 mmda-0.3.0/src/ai2_internal/bibentry_predictor_mmda/integration_test.py
--rw-r--r--   0 kylel      (502) staff       (20)     4941 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/bibentry_predictor_mmda/interface.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.295833 mmda-0.3.0/src/ai2_internal/citation_links/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/citation_links/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     4538 2023-03-09 22:35:11.000000 mmda-0.3.0/src/ai2_internal/citation_links/integration_test.py
--rw-r--r--   0 kylel      (502) staff       (20)     3221 2023-03-09 01:33:11.000000 mmda-0.3.0/src/ai2_internal/citation_links/interface.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.297327 mmda-0.3.0/src/ai2_internal/citation_mentions/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/citation_mentions/__init__.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.298859 mmda-0.3.0/src/ai2_internal/citation_mentions/data/
--rw-r--r--   0 kylel      (502) staff       (20)    96377 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/citation_mentions/data/arxiv-1906.08632-page0.pdf
--rw-r--r--   0 kylel      (502) staff       (20)   129229 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/citation_mentions/data/arxiv-1906.08632-pages1-2.pdf
--rw-r--r--   0 kylel      (502) staff       (20)     3249 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/citation_mentions/integration_test.py
--rw-r--r--   0 kylel      (502) staff       (20)     2780 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/citation_mentions/interface.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.300703 mmda-0.3.0/src/ai2_internal/figure_table_predictors/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/figure_table_predictors/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     2956 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/figure_table_predictors/integration_test.py
--rw-r--r--   0 kylel      (502) staff       (20)     3964 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/figure_table_predictors/interface.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.319665 mmda-0.3.0/src/ai2_internal/figure_table_predictors/test_fixtures/
--rw-r--r--   0 kylel      (502) staff       (20)  1159226 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/figure_table_predictors/test_fixtures/test_doc.json
--rw-r--r--   0 kylel      (502) staff       (20)  5381024 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/figure_table_predictors/test_fixtures/test_doc_sha_d0450478c38dda61f9943f417ab9fcdb2ebeae0a.json
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.331401 mmda-0.3.0/src/ai2_internal/layout_parser/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/layout_parser/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     1513 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/layout_parser/integration_test.py
--rw-r--r--   0 kylel      (502) staff       (20)     3946 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/layout_parser/interface.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.332131 mmda-0.3.0/src/ai2_internal/shared_test_fixtures/
--rw-r--r--   0 kylel      (502) staff       (20)   166624 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/shared_test_fixtures/page0.png
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.335284 mmda-0.3.0/src/ai2_internal/vila/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/vila/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     2676 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/vila/integration_test.py
--rw-r--r--   0 kylel      (502) staff       (20)     3399 2023-03-06 18:54:21.000000 mmda-0.3.0/src/ai2_internal/vila/interface.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.336605 mmda-0.3.0/src/ai2_internal/vila/test_fixtures/
--rw-r--r--   0 kylel      (502) staff       (20)     1121 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/vila/test_fixtures/test_blocks.json
--rw-r--r--   0 kylel      (502) staff       (20)    47588 2022-12-07 01:58:14.000000 mmda-0.3.0/src/ai2_internal/vila/test_fixtures/test_doc.json
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.337366 mmda-0.3.0/src/mmda/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/__init__.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.342308 mmda-0.3.0/src/mmda/eval/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/eval/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     2829 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/eval/metrics.py
--rw-r--r--   0 kylel      (502) staff       (20)      743 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/eval/s2.py
--rw-r--r--   0 kylel      (502) staff       (20)     2577 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/eval/vlue.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.343698 mmda-0.3.0/src/mmda/featurizers/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/featurizers/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     5868 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/featurizers/citation_link_featurizers.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.351615 mmda-0.3.0/src/mmda/parsers/
--rw-r--r--   0 kylel      (502) staff       (20)       97 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/parsers/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     4064 2023-03-09 22:35:11.000000 mmda-0.3.0/src/mmda/parsers/grobid_augment_existing_document_parser.py
--rw-r--r--   0 kylel      (502) staff       (20)     3770 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/parsers/grobid_parser.py
--rw-r--r--   0 kylel      (502) staff       (20)      552 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/parsers/parser.py
--rw-r--r--   0 kylel      (502) staff       (20)    18328 2023-03-08 00:06:03.000000 mmda-0.3.0/src/mmda/parsers/pdfplumber_parser.py
--rw-r--r--   0 kylel      (502) staff       (20)    13725 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/parsers/symbol_scraper_parser.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.353407 mmda-0.3.0/src/mmda/predictors/
--rw-r--r--   0 kylel      (502) staff       (20)      934 2023-03-07 05:52:24.000000 mmda-0.3.0/src/mmda/predictors/__init__.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.354886 mmda-0.3.0/src/mmda/predictors/base_predictors/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/predictors/base_predictors/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)      146 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/predictors/base_predictors/base_heuristic_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)     2192 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/predictors/base_predictors/base_predictor.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.382619 mmda-0.3.0/src/mmda/predictors/d2_predictors/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/predictors/d2_predictors/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     6988 2023-03-07 05:52:24.000000 mmda-0.3.0/src/mmda/predictors/d2_predictors/bibentry_detection_predictor.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.387372 mmda-0.3.0/src/mmda/predictors/heuristic_predictors/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/predictors/heuristic_predictors/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)    24983 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/predictors/heuristic_predictors/dictionary_word_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)     8500 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/predictors/heuristic_predictors/figure_table_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)      912 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/predictors/heuristic_predictors/grobid_citation_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)     8439 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/predictors/heuristic_predictors/section_header_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)     2861 2023-02-21 03:07:15.000000 mmda-0.3.0/src/mmda/predictors/heuristic_predictors/section_paragraph_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)     5096 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/predictors/heuristic_predictors/sentence_boundary_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)     1840 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/predictors/heuristic_predictors/whitespace_predictor.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.391774 mmda-0.3.0/src/mmda/predictors/hf_predictors/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/predictors/hf_predictors/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     1206 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/predictors/hf_predictors/base_hf_predictor.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.396737 mmda-0.3.0/src/mmda/predictors/hf_predictors/bibentry_predictor/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/predictors/hf_predictors/bibentry_predictor/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     9646 2023-03-07 05:52:24.000000 mmda-0.3.0/src/mmda/predictors/hf_predictors/bibentry_predictor/predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)     1474 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/predictors/hf_predictors/bibentry_predictor/types.py
--rw-r--r--   0 kylel      (502) staff       (20)     3302 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/predictors/hf_predictors/bibentry_predictor/utils.py
--rw-r--r--   0 kylel      (502) staff       (20)     7193 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/predictors/hf_predictors/mention_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)    14554 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/predictors/hf_predictors/span_group_classification_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)     5137 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/predictors/hf_predictors/token_classification_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)     3926 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/predictors/hf_predictors/utils.py
--rw-r--r--   0 kylel      (502) staff       (20)    11250 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/predictors/hf_predictors/vila_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)     3464 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/predictors/lp_predictors.py
--rw-r--r--   0 kylel      (502) staff       (20)     3199 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/predictors/tesseract_predictors.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.399161 mmda-0.3.0/src/mmda/predictors/xgb_predictors/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/predictors/xgb_predictors/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     1473 2023-03-09 22:35:11.000000 mmda-0.3.0/src/mmda/predictors/xgb_predictors/citation_link_predictor.py
--rw-r--r--   0 kylel      (502) staff       (20)    13683 2023-03-07 05:52:24.000000 mmda-0.3.0/src/mmda/predictors/xgb_predictors/section_nesting_predictor.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.400226 mmda-0.3.0/src/mmda/rasterizers/
--rw-r--r--   0 kylel      (502) staff       (20)      100 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/rasterizers/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)      978 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/rasterizers/rasterizer.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.401985 mmda-0.3.0/src/mmda/recipes/
--rw-r--r--   0 kylel      (502) staff       (20)       79 2023-03-13 17:17:12.000000 mmda-0.3.0/src/mmda/recipes/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     2287 2023-03-13 17:17:12.000000 mmda-0.3.0/src/mmda/recipes/core_recipe.py
--rw-r--r--   0 kylel      (502) staff       (20)      303 2023-03-13 17:17:12.000000 mmda-0.3.0/src/mmda/recipes/recipe.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.435876 mmda-0.3.0/src/mmda/types/
--rw-r--r--   0 kylel      (502) staff       (20)      355 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/types/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)     8389 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/types/annotation.py
--rw-r--r--   0 kylel      (502) staff       (20)     4392 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/types/box.py
--rw-r--r--   0 kylel      (502) staff       (20)    10285 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/types/document.py
--rw-r--r--   0 kylel      (502) staff       (20)      832 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/types/image.py
--rw-r--r--   0 kylel      (502) staff       (20)     3109 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/types/indexers.py
--rw-r--r--   0 kylel      (502) staff       (20)    15513 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/types/metadata.py
--rw-r--r--   0 kylel      (502) staff       (20)      305 2023-03-08 00:24:47.000000 mmda-0.3.0/src/mmda/types/names.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.439436 mmda-0.3.0/src/mmda/types/old/
--rw-r--r--   0 kylel      (502) staff       (20)     1928 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/types/old/annotations.old.py
--rw-r--r--   0 kylel      (502) staff       (20)     2270 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/types/old/boundingbox.old.py
--rw-r--r--   0 kylel      (502) staff       (20)     9084 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/types/old/document.old.py
--rw-r--r--   0 kylel      (502) staff       (20)     1889 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/types/old/document_elements.py
--rw-r--r--   0 kylel      (502) staff       (20)      798 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/types/old/image.old.py
--rw-r--r--   0 kylel      (502) staff       (20)     2121 2023-03-06 18:54:21.000000 mmda-0.3.0/src/mmda/types/old/span.old.py
--rw-r--r--   0 kylel      (502) staff       (20)     1437 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/types/span.py
--rw-r--r--   0 kylel      (502) staff       (20)     1376 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/types/user_data.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.441913 mmda-0.3.0/src/mmda/utils/
--rw-r--r--   0 kylel      (502) staff       (20)        0 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/utils/__init__.py
--rw-r--r--   0 kylel      (502) staff       (20)    10257 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/utils/outline_metadata.py
--rw-r--r--   0 kylel      (502) staff       (20)     5694 2022-12-07 01:58:14.000000 mmda-0.3.0/src/mmda/utils/tools.py
-drwxr-xr-x   0 kylel      (502) staff       (20)        0 2023-03-14 19:18:16.339671 mmda-0.3.0/src/mmda.egg-info/
--rw-r--r--   0 kylel      (502) staff       (20)     8842 2023-03-14 19:18:16.000000 mmda-0.3.0/src/mmda.egg-info/PKG-INFO
--rw-r--r--   0 kylel      (502) staff       (20)     5502 2023-03-14 19:18:16.000000 mmda-0.3.0/src/mmda.egg-info/SOURCES.txt
--rw-r--r--   0 kylel      (502) staff       (20)        1 2023-03-14 19:18:16.000000 mmda-0.3.0/src/mmda.egg-info/dependency_links.txt
--rw-r--r--   0 kylel      (502) staff       (20)     1030 2023-03-14 19:18:16.000000 mmda-0.3.0/src/mmda.egg-info/requires.txt
--rw-r--r--   0 kylel      (502) staff       (20)       18 2023-03-14 19:18:16.000000 mmda-0.3.0/src/mmda.egg-info/top_level.txt
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.132230 mmda-0.3.6/
+-rw-r--r--   0 lucas      (502) staff       (20)    10764 2022-04-21 21:28:24.000000 mmda-0.3.6/LICENSE
+-rw-r--r--   0 lucas      (502) staff       (20)     8842 2023-04-10 18:29:08.131958 mmda-0.3.6/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     7785 2023-03-14 17:05:00.000000 mmda-0.3.6/README.md
+-rw-r--r--   0 lucas      (502) staff       (20)     3122 2023-04-10 18:28:54.000000 mmda-0.3.6/pyproject.toml
+-rw-r--r--   0 lucas      (502) staff       (20)       38 2023-04-10 18:29:08.132304 mmda-0.3.6/setup.cfg
+-rw-r--r--   0 lucas      (502) staff       (20)       38 2023-01-06 17:32:53.000000 mmda-0.3.6/setup.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.084282 mmda-0.3.6/src/
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.092422 mmda-0.3.6/src/ai2_internal/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4799 2023-03-14 17:05:00.000000 mmda-0.3.6/src/ai2_internal/api.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.093066 mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.096408 mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/data/
+-rw-r--r--   0 lucas      (502) staff       (20)   334931 2023-02-22 22:35:17.000000 mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/data/000026bab3c52aa8ff37dc3e155ffbcb506aa1f6.pdf
+-rw-r--r--   0 lucas      (502) staff       (20)    96377 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/data/no_bibs.pdf
+-rw-r--r--   0 lucas      (502) staff       (20)      185 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/data/no_bibs_vila_span_groups.json
+-rw-r--r--   0 lucas      (502) staff       (20)   501454 2023-02-22 22:35:17.000000 mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/data/spanless_bibs_3cf45514384bbb7d083ae53e19bdc22300e648ab.pdf
+-rw-r--r--   0 lucas      (502) staff       (20)    59603 2023-02-22 22:35:17.000000 mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/data/spanless_bibs_vila_span_groups.json
+-rw-r--r--   0 lucas      (502) staff       (20)     3558 2023-02-22 22:35:17.000000 mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/data/vila_span_groups.json
+-rw-r--r--   0 lucas      (502) staff       (20)     5708 2023-02-22 22:35:17.000000 mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/integration_test.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5132 2023-02-22 22:35:17.000000 mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/interface.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.096828 mmda-0.3.6/src/ai2_internal/bibentry_predictor/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/bibentry_predictor/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2269 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/bibentry_predictor/integration_test.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3109 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/bibentry_predictor/interface.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.097360 mmda-0.3.6/src/ai2_internal/bibentry_predictor_mmda/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/bibentry_predictor_mmda/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.098123 mmda-0.3.6/src/ai2_internal/bibentry_predictor_mmda/data/
+-rw-r--r--   0 lucas      (502) staff       (20)   285777 2023-02-22 22:35:17.000000 mmda-0.3.6/src/ai2_internal/bibentry_predictor_mmda/data/test_data.json.gz
+-rw-r--r--   0 lucas      (502) staff       (20)  1595942 2023-02-22 22:35:17.000000 mmda-0.3.6/src/ai2_internal/bibentry_predictor_mmda/data/test_data_v2_boxes_turn_into_empty_span_groups.json.gz
+-rw-r--r--   0 lucas      (502) staff       (20)     6109 2023-04-10 16:18:25.000000 mmda-0.3.6/src/ai2_internal/bibentry_predictor_mmda/integration_test.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4941 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/bibentry_predictor_mmda/interface.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.100555 mmda-0.3.6/src/ai2_internal/citation_links/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/citation_links/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4538 2023-03-14 17:05:00.000000 mmda-0.3.6/src/ai2_internal/citation_links/integration_test.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3221 2023-03-14 17:05:00.000000 mmda-0.3.6/src/ai2_internal/citation_links/interface.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.101194 mmda-0.3.6/src/ai2_internal/citation_mentions/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/citation_mentions/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.101725 mmda-0.3.6/src/ai2_internal/citation_mentions/data/
+-rw-r--r--   0 lucas      (502) staff       (20)    96377 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/citation_mentions/data/arxiv-1906.08632-page0.pdf
+-rw-r--r--   0 lucas      (502) staff       (20)   129229 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/citation_mentions/data/arxiv-1906.08632-pages1-2.pdf
+-rw-r--r--   0 lucas      (502) staff       (20)     3249 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/citation_mentions/integration_test.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2780 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/citation_mentions/interface.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.102319 mmda-0.3.6/src/ai2_internal/figure_table_predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/figure_table_predictors/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2956 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/figure_table_predictors/integration_test.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3964 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/figure_table_predictors/interface.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.104190 mmda-0.3.6/src/ai2_internal/figure_table_predictors/test_fixtures/
+-rw-r--r--   0 lucas      (502) staff       (20)  1159226 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/figure_table_predictors/test_fixtures/test_doc.json
+-rw-r--r--   0 lucas      (502) staff       (20)  5381024 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/figure_table_predictors/test_fixtures/test_doc_sha_d0450478c38dda61f9943f417ab9fcdb2ebeae0a.json
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.112341 mmda-0.3.6/src/ai2_internal/layout_parser/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/layout_parser/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1513 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/layout_parser/integration_test.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3946 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/layout_parser/interface.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.115340 mmda-0.3.6/src/ai2_internal/shared_test_fixtures/
+-rw-r--r--   0 lucas      (502) staff       (20)   166624 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/shared_test_fixtures/page0.png
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.116094 mmda-0.3.6/src/ai2_internal/vila/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/vila/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2676 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/vila/integration_test.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3399 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/vila/interface.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.116604 mmda-0.3.6/src/ai2_internal/vila/test_fixtures/
+-rw-r--r--   0 lucas      (502) staff       (20)     1121 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/vila/test_fixtures/test_blocks.json
+-rw-r--r--   0 lucas      (502) staff       (20)    47588 2023-01-06 17:32:53.000000 mmda-0.3.6/src/ai2_internal/vila/test_fixtures/test_doc.json
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.117229 mmda-0.3.6/src/mmda/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.118610 mmda-0.3.6/src/mmda/eval/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/eval/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2829 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/eval/metrics.py
+-rw-r--r--   0 lucas      (502) staff       (20)      743 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/eval/s2.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2577 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/eval/vlue.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.118916 mmda-0.3.6/src/mmda/featurizers/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/featurizers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5868 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/featurizers/citation_link_featurizers.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.120655 mmda-0.3.6/src/mmda/parsers/
+-rw-r--r--   0 lucas      (502) staff       (20)       97 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/parsers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4113 2023-04-10 16:18:25.000000 mmda-0.3.6/src/mmda/parsers/grobid_augment_existing_document_parser.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3770 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/parsers/grobid_parser.py
+-rw-r--r--   0 lucas      (502) staff       (20)      552 2023-03-15 00:02:51.000000 mmda-0.3.6/src/mmda/parsers/parser.py
+-rw-r--r--   0 lucas      (502) staff       (20)    18328 2023-04-10 16:18:20.000000 mmda-0.3.6/src/mmda/parsers/pdfplumber_parser.py
+-rw-r--r--   0 lucas      (502) staff       (20)    13725 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/parsers/symbol_scraper_parser.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.121351 mmda-0.3.6/src/mmda/predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)      934 2023-02-22 22:35:17.000000 mmda-0.3.6/src/mmda/predictors/__init__.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.121885 mmda-0.3.6/src/mmda/predictors/base_predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/base_predictors/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)      146 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/base_predictors/base_heuristic_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2192 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/base_predictors/base_predictor.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.122249 mmda-0.3.6/src/mmda/predictors/d2_predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/d2_predictors/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     6988 2023-02-22 22:35:17.000000 mmda-0.3.6/src/mmda/predictors/d2_predictors/bibentry_detection_predictor.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.123657 mmda-0.3.6/src/mmda/predictors/heuristic_predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/heuristic_predictors/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)    24983 2023-04-10 16:18:20.000000 mmda-0.3.6/src/mmda/predictors/heuristic_predictors/dictionary_word_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8500 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/heuristic_predictors/figure_table_predictors.py
+-rw-r--r--   0 lucas      (502) staff       (20)      912 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/heuristic_predictors/grobid_citation_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8439 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/heuristic_predictors/section_header_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5096 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/heuristic_predictors/sentence_boundary_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1840 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/heuristic_predictors/whitespace_predictor.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.124959 mmda-0.3.6/src/mmda/predictors/hf_predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/hf_predictors/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1206 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/hf_predictors/base_hf_predictor.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.125768 mmda-0.3.6/src/mmda/predictors/hf_predictors/bibentry_predictor/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/hf_predictors/bibentry_predictor/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     9697 2023-04-10 16:18:25.000000 mmda-0.3.6/src/mmda/predictors/hf_predictors/bibentry_predictor/predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1474 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/hf_predictors/bibentry_predictor/types.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3302 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/hf_predictors/bibentry_predictor/utils.py
+-rw-r--r--   0 lucas      (502) staff       (20)     7193 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/hf_predictors/mention_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)    14554 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/hf_predictors/span_group_classification_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     5137 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/hf_predictors/token_classification_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3926 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/hf_predictors/utils.py
+-rw-r--r--   0 lucas      (502) staff       (20)    11250 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/hf_predictors/vila_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3464 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/lp_predictors.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3199 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/tesseract_predictors.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.126356 mmda-0.3.6/src/mmda/predictors/xgb_predictors/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/predictors/xgb_predictors/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1473 2023-03-14 17:05:00.000000 mmda-0.3.6/src/mmda/predictors/xgb_predictors/citation_link_predictor.py
+-rw-r--r--   0 lucas      (502) staff       (20)    13683 2023-02-22 22:35:17.000000 mmda-0.3.6/src/mmda/predictors/xgb_predictors/section_nesting_predictor.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.126701 mmda-0.3.6/src/mmda/rasterizers/
+-rw-r--r--   0 lucas      (502) staff       (20)      100 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/rasterizers/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)      978 2023-03-14 23:32:49.000000 mmda-0.3.6/src/mmda/rasterizers/rasterizer.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.127713 mmda-0.3.6/src/mmda/recipes/
+-rw-r--r--   0 lucas      (502) staff       (20)       79 2023-03-14 17:05:00.000000 mmda-0.3.6/src/mmda/recipes/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2528 2023-04-10 18:28:54.000000 mmda-0.3.6/src/mmda/recipes/core_recipe.py
+-rw-r--r--   0 lucas      (502) staff       (20)      303 2023-03-15 03:22:15.000000 mmda-0.3.6/src/mmda/recipes/recipe.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.129899 mmda-0.3.6/src/mmda/types/
+-rw-r--r--   0 lucas      (502) staff       (20)      355 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/types/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)     8389 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/types/annotation.py
+-rw-r--r--   0 lucas      (502) staff       (20)     4392 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/types/box.py
+-rw-r--r--   0 lucas      (502) staff       (20)    11700 2023-04-10 16:18:25.000000 mmda-0.3.6/src/mmda/types/document.py
+-rw-r--r--   0 lucas      (502) staff       (20)      832 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/types/image.py
+-rw-r--r--   0 lucas      (502) staff       (20)     3109 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/types/indexers.py
+-rw-r--r--   0 lucas      (502) staff       (20)    15513 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/types/metadata.py
+-rw-r--r--   0 lucas      (502) staff       (20)      305 2023-02-22 22:35:17.000000 mmda-0.3.6/src/mmda/types/names.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.131080 mmda-0.3.6/src/mmda/types/old/
+-rw-r--r--   0 lucas      (502) staff       (20)     1928 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/types/old/annotations.old.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2270 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/types/old/boundingbox.old.py
+-rw-r--r--   0 lucas      (502) staff       (20)     9084 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/types/old/document.old.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1889 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/types/old/document_elements.py
+-rw-r--r--   0 lucas      (502) staff       (20)      798 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/types/old/image.old.py
+-rw-r--r--   0 lucas      (502) staff       (20)     2121 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/types/old/span.old.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1437 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/types/span.py
+-rw-r--r--   0 lucas      (502) staff       (20)     1376 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/types/user_data.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.131595 mmda-0.3.6/src/mmda/utils/
+-rw-r--r--   0 lucas      (502) staff       (20)        0 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/utils/__init__.py
+-rw-r--r--   0 lucas      (502) staff       (20)    10257 2023-01-06 17:32:53.000000 mmda-0.3.6/src/mmda/utils/outline_metadata.py
+-rw-r--r--   0 lucas      (502) staff       (20)     7543 2023-04-10 16:18:25.000000 mmda-0.3.6/src/mmda/utils/tools.py
+drwxr-xr-x   0 lucas      (502) staff       (20)        0 2023-04-10 18:29:08.117923 mmda-0.3.6/src/mmda.egg-info/
+-rw-r--r--   0 lucas      (502) staff       (20)     8842 2023-04-10 18:29:08.000000 mmda-0.3.6/src/mmda.egg-info/PKG-INFO
+-rw-r--r--   0 lucas      (502) staff       (20)     5430 2023-04-10 18:29:08.000000 mmda-0.3.6/src/mmda.egg-info/SOURCES.txt
+-rw-r--r--   0 lucas      (502) staff       (20)        1 2023-04-10 18:29:08.000000 mmda-0.3.6/src/mmda.egg-info/dependency_links.txt
+-rw-r--r--   0 lucas      (502) staff       (20)     1038 2023-04-10 18:29:08.000000 mmda-0.3.6/src/mmda.egg-info/requires.txt
+-rw-r--r--   0 lucas      (502) staff       (20)       18 2023-04-10 18:29:08.000000 mmda-0.3.6/src/mmda.egg-info/top_level.txt
```

### Comparing `mmda-0.3.0/LICENSE` & `mmda-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/PKG-INFO` & `mmda-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmda
-Version: 0.3.0
+Version: 0.3.6
 Summary: MMDA - multimodal document analysis
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>
 License: Apache-2.0
 Project-URL: Homepage, https://www.github.com/allenai/mmda
 Project-URL: Repository, https://www.github.com/allenai/mmda
 Project-URL: Bug Tracker, https://www.github.com/allenai/mmda/issues
 Requires-Python: >=3.7
```

### Comparing `mmda-0.3.0/README.md` & `mmda-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/pyproject.toml` & `mmda-0.3.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = 'mmda'
-version = '0.3.0'
+version = '0.3.6'
 description = 'MMDA - multimodal document analysis'
 authors = [
     {name = 'Allen Institute for Artificial Intelligence', email = 'contact@allenai.org'},
 ]
 license = {text = 'Apache-2.0'}
 readme = 'README.md'
 requires-python = '>=3.7'
 dependencies = [
         'tqdm',
         'pdf2image',
         'pdfplumber==0.7.4',
         'requests',
         'pandas',
         'pydantic',
-        'ncls',
+        'ncls==0.0.66',
         'necessary>=0.3.2',
 ]
 
 [project.urls]
 'Homepage' = 'https://www.github.com/allenai/mmda'
 'Repository' = 'https://www.github.com/allenai/mmda'
 'Bug Tracker' = 'https://www.github.com/allenai/mmda/issues'
```

### Comparing `mmda-0.3.0/src/ai2_internal/api.py` & `mmda-0.3.6/src/ai2_internal/api.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/data/000026bab3c52aa8ff37dc3e155ffbcb506aa1f6.pdf` & `mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/data/000026bab3c52aa8ff37dc3e155ffbcb506aa1f6.pdf`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/data/no_bibs.pdf` & `mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/data/no_bibs.pdf`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/data/spanless_bibs_3cf45514384bbb7d083ae53e19bdc22300e648ab.pdf` & `mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/data/spanless_bibs_3cf45514384bbb7d083ae53e19bdc22300e648ab.pdf`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/data/spanless_bibs_vila_span_groups.json` & `mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/data/spanless_bibs_vila_span_groups.json`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/data/vila_span_groups.json` & `mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/data/vila_span_groups.json`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/integration_test.py` & `mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/integration_test.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/bibentry_detection_predictor/interface.py` & `mmda-0.3.6/src/ai2_internal/bibentry_detection_predictor/interface.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/bibentry_predictor/integration_test.py` & `mmda-0.3.6/src/ai2_internal/bibentry_predictor/integration_test.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/bibentry_predictor/interface.py` & `mmda-0.3.6/src/ai2_internal/bibentry_predictor/interface.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/bibentry_predictor_mmda/data/test_data.json.gz` & `mmda-0.3.6/src/ai2_internal/bibentry_predictor_mmda/data/test_data.json.gz`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/bibentry_predictor_mmda/data/test_data_v2_boxes_turn_into_empty_span_groups.json.gz` & `mmda-0.3.6/src/ai2_internal/bibentry_predictor_mmda/data/test_data_v2_boxes_turn_into_empty_span_groups.json.gz`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/bibentry_predictor_mmda/integration_test.py` & `mmda-0.3.6/src/ai2_internal/bibentry_predictor_mmda/integration_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 import os
 import pathlib
 import sys
 import unittest
 
 from .. import api
 from mmda.types.document import Document
-from .interface import Instance
+from .interface import Instance, Prediction
 
 try:
     from timo_interface import with_timo_container
 except ImportError as e:
     logging.warning("""
     This test can only be run by a TIMO test runner. No tests will run. 
     You may need to add this file to your project's pytest exclusions.
@@ -63,14 +63,35 @@
     bib_entry_boxes = raw["bib_entry_boxes"]
 
     return doc, bib_entry_boxes
 
 
 @with_timo_container
 class TestInterfaceIntegration(unittest.TestCase):
+    def test__handles_no_bib_entries(self, container):
+        filename = "test_data.json.gz"
+        doc, bib_entry_boxes = read_fixture_doc_and_entries(filename)
+        instance = Instance(
+            symbols=doc.symbols,
+            tokens=[api.SpanGroup.from_mmda(token) for token in doc.tokens],
+            pages=[api.SpanGroup.from_mmda(page) for page in doc.pages],
+            bib_entry_boxes=[]
+        )
+        prediction = container.predict_batch([instance])[0]
+
+        self.assertEqual(prediction, Prediction(
+            bib_entry_number=[],
+            bib_entry_authors=[],
+            bib_entry_title=[],
+            bib_entry_venue_or_event=[],
+            bib_entry_year=[],
+            bib_entry_doi=[],
+            bib_entry_url=[]
+        ))
+
     def test__predictions(self, container):
         # Produced from running upstream models on example paper
         # (000026bab3c52aa8ff37dc3e155ffbcb506aa1f6.pdf)
         filename = "test_data.json.gz"
         doc, bib_entry_boxes = read_fixture_doc_and_entries(filename)
         instance = Instance(
             symbols=doc.symbols,
```

### Comparing `mmda-0.3.0/src/ai2_internal/bibentry_predictor_mmda/interface.py` & `mmda-0.3.6/src/ai2_internal/bibentry_predictor_mmda/interface.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/citation_links/integration_test.py` & `mmda-0.3.6/src/ai2_internal/citation_links/integration_test.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/citation_links/interface.py` & `mmda-0.3.6/src/ai2_internal/citation_links/interface.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/citation_mentions/data/arxiv-1906.08632-page0.pdf` & `mmda-0.3.6/src/ai2_internal/citation_mentions/data/arxiv-1906.08632-page0.pdf`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/citation_mentions/data/arxiv-1906.08632-pages1-2.pdf` & `mmda-0.3.6/src/ai2_internal/citation_mentions/data/arxiv-1906.08632-pages1-2.pdf`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/citation_mentions/integration_test.py` & `mmda-0.3.6/src/ai2_internal/citation_mentions/integration_test.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/citation_mentions/interface.py` & `mmda-0.3.6/src/ai2_internal/citation_mentions/interface.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/figure_table_predictors/integration_test.py` & `mmda-0.3.6/src/ai2_internal/figure_table_predictors/integration_test.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/figure_table_predictors/interface.py` & `mmda-0.3.6/src/ai2_internal/figure_table_predictors/interface.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/figure_table_predictors/test_fixtures/test_doc.json` & `mmda-0.3.6/src/ai2_internal/figure_table_predictors/test_fixtures/test_doc.json`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/figure_table_predictors/test_fixtures/test_doc_sha_d0450478c38dda61f9943f417ab9fcdb2ebeae0a.json` & `mmda-0.3.6/src/ai2_internal/figure_table_predictors/test_fixtures/test_doc_sha_d0450478c38dda61f9943f417ab9fcdb2ebeae0a.json`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/layout_parser/integration_test.py` & `mmda-0.3.6/src/ai2_internal/layout_parser/integration_test.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/layout_parser/interface.py` & `mmda-0.3.6/src/ai2_internal/layout_parser/interface.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/shared_test_fixtures/page0.png` & `mmda-0.3.6/src/ai2_internal/shared_test_fixtures/page0.png`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/vila/integration_test.py` & `mmda-0.3.6/src/ai2_internal/vila/integration_test.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/vila/interface.py` & `mmda-0.3.6/src/ai2_internal/vila/interface.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/vila/test_fixtures/test_blocks.json` & `mmda-0.3.6/src/ai2_internal/vila/test_fixtures/test_blocks.json`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/ai2_internal/vila/test_fixtures/test_doc.json` & `mmda-0.3.6/src/ai2_internal/vila/test_fixtures/test_doc.json`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/eval/metrics.py` & `mmda-0.3.6/src/mmda/eval/metrics.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/eval/s2.py` & `mmda-0.3.6/src/mmda/eval/s2.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/eval/vlue.py` & `mmda-0.3.6/src/mmda/eval/vlue.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/featurizers/citation_link_featurizers.py` & `mmda-0.3.6/src/mmda/featurizers/citation_link_featurizers.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/parsers/grobid_augment_existing_document_parser.py` & `mmda-0.3.6/src/mmda/parsers/grobid_augment_existing_document_parser.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 
 @geli-gel
 
 """
 from grobid_client.grobid_client import GrobidClient
 from typing import Optional, List
 
-import io
 import os
 import xml.etree.ElementTree as et
 
 from mmda.parsers.parser import Parser
+from mmda.types import Metadata
 from mmda.types.annotation import BoxGroup, Box
 from mmda.types.document import Document
 from mmda.types.names import PagesField, RowsField, TokensField
 
 REQUIRED_DOCUMENT_FIELDS = [PagesField, RowsField, TokensField]
 NS = {"tei": "http://www.tei-c.org/ns/1.0"}
 
@@ -61,16 +61,16 @@
         return doc
 
     def _parse_xml_onto_doc(self, xml: str, doc: Document) -> Document:
         xml_root = et.fromstring(xml)
 
         bib_entries = self._get_grobid_bib_box_groups(xml_root)
         
-        # if/when adding in relations between mention sources and bib targets, we'll have to 
-        #  re-map the source and target IDs onto their new MMDA SpanGroup IDs
+        # note for if/when adding in relations between mention sources and bib targets:
+        # big_entries metadata contains original grobid id attached to the BoxGroup.
         doc.annotate(
             bib_entries=bib_entries
             )
 
         return doc
 
     def _xml_coords_to_boxes(self, coords_attribute: str, page_sizes: dict):
@@ -105,13 +105,13 @@
             coords_string = bib.attrib["coords"]
             boxes = self._xml_coords_to_boxes(coords_string, page_sizes)
             grobid_id = bib.attrib["{http://www.w3.org/XML/1998/namespace}id"]
 
             grobid_bibs.append(
                 BoxGroup(
                 boxes=boxes, 
-                id=grobid_id
+                metadata=Metadata(grobid_id=grobid_id)
                 )
             )
 
         return grobid_bibs
```

### Comparing `mmda-0.3.0/src/mmda/parsers/grobid_parser.py` & `mmda-0.3.6/src/mmda/parsers/grobid_parser.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/parsers/parser.py` & `mmda-0.3.6/src/mmda/parsers/parser.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/parsers/pdfplumber_parser.py` & `mmda-0.3.6/src/mmda/parsers/pdfplumber_parser.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/parsers/symbol_scraper_parser.py` & `mmda-0.3.6/src/mmda/parsers/symbol_scraper_parser.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/__init__.py` & `mmda-0.3.6/src/mmda/predictors/__init__.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/base_predictors/base_predictor.py` & `mmda-0.3.6/src/mmda/predictors/base_predictors/base_predictor.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/d2_predictors/bibentry_detection_predictor.py` & `mmda-0.3.6/src/mmda/predictors/d2_predictors/bibentry_detection_predictor.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/heuristic_predictors/dictionary_word_predictor.py` & `mmda-0.3.6/src/mmda/predictors/heuristic_predictors/dictionary_word_predictor.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/heuristic_predictors/figure_table_predictors.py` & `mmda-0.3.6/src/mmda/predictors/heuristic_predictors/figure_table_predictors.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/heuristic_predictors/grobid_citation_predictor.py` & `mmda-0.3.6/src/mmda/predictors/heuristic_predictors/grobid_citation_predictor.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/heuristic_predictors/section_header_predictor.py` & `mmda-0.3.6/src/mmda/predictors/heuristic_predictors/section_header_predictor.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/heuristic_predictors/sentence_boundary_predictor.py` & `mmda-0.3.6/src/mmda/predictors/heuristic_predictors/sentence_boundary_predictor.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/heuristic_predictors/whitespace_predictor.py` & `mmda-0.3.6/src/mmda/predictors/heuristic_predictors/whitespace_predictor.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/hf_predictors/base_hf_predictor.py` & `mmda-0.3.6/src/mmda/predictors/hf_predictors/base_hf_predictor.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/hf_predictors/bibentry_predictor/predictor.py` & `mmda-0.3.6/src/mmda/predictors/hf_predictors/bibentry_predictor/predictor.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
 
         # Map raw predictions back into valid annotations for passed document
         prediction = utils.map_raw_predictions_to_mmda(document.bib_entry_boxes, raw_predictions)
 
         return prediction
 
     def predict_raw(self, bib_entries: List[str]) -> List[BibEntryPredictionWithSpan]:
+        if not bib_entries:
+            return []
+
         res = []
 
         tokenized_inputs = self.tokenizer(bib_entries, padding=True, truncation=True, return_tensors="pt")
         # put the data on the same device of the model.
         tokenized_inputs = tokenized_inputs.to(self.model.device)
 
         predictions = self.model(**tokenized_inputs)
```

### Comparing `mmda-0.3.0/src/mmda/predictors/hf_predictors/bibentry_predictor/types.py` & `mmda-0.3.6/src/mmda/predictors/hf_predictors/bibentry_predictor/types.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/hf_predictors/bibentry_predictor/utils.py` & `mmda-0.3.6/src/mmda/predictors/hf_predictors/bibentry_predictor/utils.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/hf_predictors/mention_predictor.py` & `mmda-0.3.6/src/mmda/predictors/hf_predictors/mention_predictor.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/hf_predictors/span_group_classification_predictor.py` & `mmda-0.3.6/src/mmda/predictors/hf_predictors/span_group_classification_predictor.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/hf_predictors/token_classification_predictor.py` & `mmda-0.3.6/src/mmda/predictors/hf_predictors/token_classification_predictor.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/hf_predictors/utils.py` & `mmda-0.3.6/src/mmda/predictors/hf_predictors/utils.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/hf_predictors/vila_predictor.py` & `mmda-0.3.6/src/mmda/predictors/hf_predictors/vila_predictor.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/lp_predictors.py` & `mmda-0.3.6/src/mmda/predictors/lp_predictors.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/tesseract_predictors.py` & `mmda-0.3.6/src/mmda/predictors/tesseract_predictors.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/xgb_predictors/citation_link_predictor.py` & `mmda-0.3.6/src/mmda/predictors/xgb_predictors/citation_link_predictor.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/predictors/xgb_predictors/section_nesting_predictor.py` & `mmda-0.3.6/src/mmda/predictors/xgb_predictors/section_nesting_predictor.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/rasterizers/rasterizer.py` & `mmda-0.3.6/src/mmda/rasterizers/rasterizer.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/recipes/core_recipe.py` & `mmda-0.3.6/src/mmda/recipes/core_recipe.py`

 * *Files 5% similar despite different names*

```diff
@@ -45,16 +45,24 @@
         doc.annotate_images(images=images)
 
         logger.info("Predicting words...")
         words = self.word_predictor.predict(document=doc)
         doc.annotate(words=words)
 
         logger.info("Predicting blocks...")
-        blocks = self.effdet_publaynet_predictor.predict(document=doc)
+        layout = self.effdet_publaynet_predictor.predict(document=doc)
         equations = self.effdet_mfd_predictor.predict(document=doc)
-        doc.annotate(blocks=blocks + equations)
+
+        # we annotate layout info in the document
+        doc.annotate(layout=layout)
+
+        # list annotations separately
+        doc.annotate(equations=equations)
+
+        # blocks are used by IVILA, so we need to annotate them as well
+        doc.annotate(blocks=layout + equations)
 
         logger.info("Predicting vila...")
         vila_span_groups = self.vila_predictor.predict(document=doc)
         doc.annotate(vila_span_groups=vila_span_groups)
 
         return doc
```

### Comparing `mmda-0.3.0/src/mmda/types/annotation.py` & `mmda-0.3.6/src/mmda/types/annotation.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/types/box.py` & `mmda-0.3.6/src/mmda/types/box.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/types/document.py` & `mmda-0.3.6/src/mmda/types/document.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 """
 
 
 
 """
 
 import itertools
+import logging
 import warnings
 from typing import Dict, Iterable, List, Optional
 
 from mmda.types.annotation import Annotation, BoxGroup, SpanGroup
 from mmda.types.image import PILImage
 from mmda.types.indexers import Indexer, SpanGroupIndexer
 from mmda.types.metadata import Metadata
 from mmda.types.names import ImagesField, MetadataField, SymbolsField
 from mmda.utils.tools import MergeSpans, allocate_overlapping_tokens_for_box
 
 
 class Document:
-
     SPECIAL_FIELDS = [SymbolsField, ImagesField, MetadataField]
     UNALLOWED_FIELD_NAMES = ["fields"]
 
     def __init__(self, symbols: str, metadata: Optional[Metadata] = None):
         self.symbols = symbols
         self.images = []
         self.__fields = []
@@ -42,23 +42,23 @@
 
     def add_metadata(self, **kwargs):
         """Copy kwargs into the document metadata"""
         for k, value in kwargs.items():
             self.metadata.set(k, value)
 
     def annotate(
-        self, is_overwrite: bool = False, **kwargs: Iterable[Annotation]
+            self, is_overwrite: bool = False, **kwargs: Iterable[Annotation]
     ) -> None:
         """Annotate the fields for document symbols (correlating the annotations with the
         symbols) and store them into the papers.
         """
         # 1) check validity of field names
         for field_name in kwargs.keys():
             assert (
-                field_name not in self.SPECIAL_FIELDS
+                    field_name not in self.SPECIAL_FIELDS
             ), f"The field_name {field_name} should not be in {self.SPECIAL_FIELDS}."
 
             if field_name in self.fields:
                 # already existing field, check if ok overriding
                 if not is_overwrite:
                     raise AssertionError(
                         f"This field name {field_name} already exists. To override, set `is_overwrite=True`"
@@ -79,15 +79,15 @@
                 warnings.warn(f"The annotations is empty for the field {field_name}")
                 setattr(self, field_name, [])
                 self.__fields.append(field_name)
                 continue
 
             annotation_types = {type(a) for a in annotations}
             assert (
-                len(annotation_types) == 1
+                    len(annotation_types) == 1
             ), f"Annotations in field_name {field_name} more than 1 type: {annotation_types}"
             annotation_type = annotation_types.pop()
 
             if annotation_type == SpanGroup:
                 span_groups = self._annotate_span_group(
                     span_groups=annotations, field_name=field_name
                 )
@@ -106,17 +106,16 @@
             self.__fields.append(field_name)
 
     def remove(self, field_name: str):
         delattr(self, field_name)
         self.__fields = [f for f in self.__fields if f != field_name]
         del self.__indexers[field_name]
 
-
     def annotate_images(
-        self, images: Iterable[PILImage], is_overwrite: bool = False
+            self, images: Iterable[PILImage], is_overwrite: bool = False
     ) -> None:
         if not is_overwrite and len(self.images) > 0:
             raise AssertionError(
                 "This field name {Images} already exists. To override, set `is_overwrite=True`"
             )
 
         if len(images) == 0:
@@ -130,15 +129,15 @@
             raise NotImplementedError(
                 f"Unsupported image type {image_type} for {ImagesField}"
             )
 
         self.images = images
 
     def _annotate_span_group(
-        self, span_groups: List[SpanGroup], field_name: str
+            self, span_groups: List[SpanGroup], field_name: str
     ) -> List[SpanGroup]:
         """Annotate the Document using a bunch of span groups.
         It will associate the annotations with the document symbols.
         """
         assert all([isinstance(group, SpanGroup) for group in span_groups])
 
         # 1) add Document to each SpanGroup
@@ -147,61 +146,90 @@
 
         # 2) Build fast overlap lookup index
         self.__indexers[field_name] = SpanGroupIndexer(span_groups)
 
         return span_groups
 
     def _annotate_box_group(
-        self, box_groups: List[BoxGroup], field_name: str
+            self, box_groups: List[BoxGroup], field_name: str
     ) -> List[SpanGroup]:
         """Annotate the Document using a bunch of box groups.
         It will associate the annotations with the document symbols.
         """
         assert all([isinstance(group, BoxGroup) for group in box_groups])
 
         all_page_tokens = dict()
         derived_span_groups = []
+        token_box_in_box_group = None
 
         for box_id, box_group in enumerate(box_groups):
 
-            all_token_spans_with_box_group = []
+            all_tokens_overlapping_box_group = []
 
             for box in box_group.boxes:
 
                 # Caching the page tokens to avoid duplicated search
                 if box.page not in all_page_tokens:
-                    cur_page_tokens = all_page_tokens[box.page] = list(
-                        itertools.chain.from_iterable(
-                            span_group.spans
-                            for span_group in self.pages[box.page].tokens
+                    cur_page_tokens = all_page_tokens[box.page] = self.pages[
+                        box.page
+                    ].tokens
+                    if token_box_in_box_group is None:
+                        # Determine whether box is stored on token SpanGroup span.box or in the box_group
+                        token_box_in_box_group = all(
+                            [
+                                (
+                                        (hasattr(token.box_group, "boxes") and len(token.box_group.boxes) == 1)
+                                        and token.spans[0].box is None
+                                )
+                                for token in cur_page_tokens
+                            ]
                         )
-                    )
                 else:
                     cur_page_tokens = all_page_tokens[box.page]
 
                 # Find all the tokens within the box
                 tokens_in_box, remaining_tokens = allocate_overlapping_tokens_for_box(
-                    token_spans=cur_page_tokens, box=box
+                    tokens=cur_page_tokens,
+                    box=box,
+                    token_box_in_box_group=token_box_in_box_group,
                 )
                 all_page_tokens[box.page] = remaining_tokens
 
-                all_token_spans_with_box_group.extend(tokens_in_box)
+                all_tokens_overlapping_box_group.extend(tokens_in_box)
+
+            merge_spans = (
+                MergeSpans.from_span_groups_with_box_groups(
+                    span_groups=all_tokens_overlapping_box_group, index_distance=1
+                )
+                if token_box_in_box_group
+                else MergeSpans(
+                    list_of_spans=list(
+                        itertools.chain.from_iterable(
+                            span_group.spans for span_group in all_tokens_overlapping_box_group
+                        )
+                    ),
+                    index_distance=1,
+                )
+            )
 
             derived_span_groups.append(
                 SpanGroup(
-                    spans=MergeSpans(
-                        list_of_spans=all_token_spans_with_box_group, index_distance=1
-                    ).merge_neighbor_spans_by_symbol_distance(),
+                    spans=merge_spans.merge_neighbor_spans_by_symbol_distance(),
                     box_group=box_group,
                     # id = box_id,
                 )
                 # TODO Right now we cannot assign the box id, or otherwise running doc.blocks will
                 # generate blocks out-of-the-specified order.
             )
 
+        if not token_box_in_box_group:
+            logging.warning("tokens with box stored in SpanGroup span.box will be deprecated (that is, "
+                            "future Spans wont contain box). Ensure Document is annotated with tokens "
+                            "having box stored in SpanGroup box_group.boxes")
+
         del all_page_tokens
 
         derived_span_groups = sorted(
             derived_span_groups, key=lambda span_group: span_group.start
         )
         # ensure they are ordered based on span indices
```

### Comparing `mmda-0.3.0/src/mmda/types/image.py` & `mmda-0.3.6/src/mmda/types/image.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/types/indexers.py` & `mmda-0.3.6/src/mmda/types/indexers.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/types/metadata.py` & `mmda-0.3.6/src/mmda/types/metadata.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/types/old/annotations.old.py` & `mmda-0.3.6/src/mmda/types/old/annotations.old.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/types/old/boundingbox.old.py` & `mmda-0.3.6/src/mmda/types/old/boundingbox.old.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/types/old/document.old.py` & `mmda-0.3.6/src/mmda/types/old/document.old.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/types/old/document_elements.py` & `mmda-0.3.6/src/mmda/types/old/document_elements.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/types/old/image.old.py` & `mmda-0.3.6/src/mmda/types/old/image.old.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/types/old/span.old.py` & `mmda-0.3.6/src/mmda/types/old/span.old.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/types/span.py` & `mmda-0.3.6/src/mmda/types/span.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/types/user_data.py` & `mmda-0.3.6/src/mmda/types/user_data.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/utils/outline_metadata.py` & `mmda-0.3.6/src/mmda/utils/outline_metadata.py`

 * *Files identical despite different names*

### Comparing `mmda-0.3.0/src/mmda/utils/tools.py` & `mmda-0.3.6/src/mmda/utils/tools.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,80 +1,118 @@
-from typing import List, Union, Dict, Any, Tuple, Optional
+from __future__ import annotations
 from collections import defaultdict
+from itertools import groupby
+from typing import List, Dict, Tuple
 
 from mmda.types.span import Span
 from mmda.types.box import Box
 
 
 def allocate_overlapping_tokens_for_box(
-    token_spans: List[Span], box
+    tokens: List["SpanGroup"], box, token_box_in_box_group: bool = False
 ) -> Tuple[List[Span], List[Span]]:
     """Different from `find_overlapping_tokens_for_box`, it will return a tuple
     (allocate_tokens, remaining_tokens):
-    `allocated_tokens` is a list of spans where their boxes overlap with the input box,
-    `remaining_tokens` is a list of spans where they don't overlap with the input box.
+    `allocated_tokens` is a list of token SpanGroups where their boxes overlap with the input box,
+    `remaining_tokens` is a list of token SpanGroups where they don't overlap with the input box.
     """
 
     allocated_tokens, remaining_tokens = [], []
-    for token in token_spans:
-        if token.box is not None and token.box.is_overlap(box):
+    for token in tokens:
+        if token_box_in_box_group and token.box_group.boxes[0].is_overlap(box):
+            # The token "box" is stored within the SpanGroup's .box_group
+            allocated_tokens.append(token)
+        elif token.spans[0].box is not None and token.spans[0].box.is_overlap(box):
+            # default to assuming the token "box" is stored in the SpanGroup .box
             allocated_tokens.append(token)
         else:
             remaining_tokens.append(token)
     return allocated_tokens, remaining_tokens
 
 
 class MergeSpans:
     """
     Given w=width and h=height merge neighboring spans which are w, h or less apart or by merging neighboring spans
     which are index distance apart
     Inspired by https://leetcode.com/problems/merge-intervals/
     """
-    def __init__(self, list_of_spans: List["Span"], w: float = 0, h: float = 0, index_distance: int = 1) -> None:
+
+    def __init__(
+        self,
+        list_of_spans: List["Span"],
+        w: float = 0,
+        h: float = 0,
+        index_distance: int = 1,
+    ) -> None:
         """
         Args
             w (float): The input width between boxes to merge
             h (float): The input height between the boxes to merge
             index_distance (int): Distance between the spans
         """
         self.list_of_spans = list_of_spans
         self.w = w
         self.h = h
         self.graph = defaultdict(list)
         self.index_distance = index_distance
 
+    @classmethod
+    def from_span_groups_with_box_groups(
+        cls,
+        span_groups: List["SpanGroup"],
+        w: float = 0,
+        h: float = 0,
+        index_distance: int = 1,
+    ) -> MergeSpans:
+        # Convert SpanGroups with single box_group box into SpanGroups with span.box
+        spans_with_boxes = []
+        for sg in span_groups:
+            assert len(sg.spans) == len(
+                sg.box_group.boxes
+            ), "Unequal number of spans and boxes for SpanGroup"
+            for span, box in zip(sg.spans, sg.box_group.boxes):
+                spans_with_boxes.append(Span(start=span.start, end=span.end, box=box))
+        return cls(spans_with_boxes, w, h, index_distance)
+
     def build_graph_index_overlap(self):
         """
         Build graph, each node is represented by (start, end) of tuple, with the list of spans. Spans are considered
         overlapping if they are index_distance apart
         """
         is_neighboring_spans = (
             lambda span1, span2: min(
                 abs(span1.start - span2.end), abs(span1.end - span2.start)
-            ) <= self.index_distance
+            )
+            <= self.index_distance
         )
 
         for i, span_i in enumerate(self.list_of_spans):
             for j in range(i + 1, len(self.list_of_spans)):
                 if is_neighboring_spans(span_i, self.list_of_spans[j]):
                     self.graph[span_i.start, span_i.end].append(self.list_of_spans[j])
-                    self.graph[self.list_of_spans[j].start, self.list_of_spans[j].end].append(span_i)
+                    self.graph[
+                        self.list_of_spans[j].start, self.list_of_spans[j].end
+                    ].append(span_i)
 
     def build_graph_box_overlap(self):
         """
         Build graph, each node is represented by (start, end) of tuple, with the list of spans with overlapping
         boxes given, w, h
         """
         for i, span_i in enumerate(self.list_of_spans):
-            assert hasattr(span_i, 'box'), 'Missing attribute box in a span'
+            assert hasattr(span_i, "box"), "Missing attribute box in a span"
             for j in range(i + 1, len(self.list_of_spans)):
-                assert hasattr(self.list_of_spans[j], 'box'), 'Missing attribute box in a span'
+                assert hasattr(
+                    self.list_of_spans[j], "box"
+                ), "Missing attribute box in a span"
                 if span_i.box.is_overlap(self.list_of_spans[j].box, self.w, self.h):
                     self.graph[span_i.start, span_i.end].append(self.list_of_spans[j])
-                    self.graph[self.list_of_spans[j].start, self.list_of_spans[j].end].append(span_i)
+                    self.graph[
+                        self.list_of_spans[j].start, self.list_of_spans[j].end
+                    ].append(span_i)
 
     # gets the connected components of the boxes overlap graph.
     def get_components(self):
         """
         Groups connected graph nodes into dictionary list
         """
         visited = set()
@@ -126,12 +164,26 @@
 
         nodes_in_comp, number_of_comps = self.get_components()
 
         # all intervals in each connected component must be merged.
         merged_spans = []
         for comp in range(number_of_comps):
             if nodes_in_comp[comp]:
-                merged_box = Box.small_boxes_to_big_box([span.box for span in nodes_in_comp[comp]])
-                merged_spans.append(Span(start=min([span.start for span in nodes_in_comp[comp]]),
-                                         end=max([span.end for span in nodes_in_comp[comp]]), box=merged_box))
+                spans_by_page: Dict[any, List[Span]] = defaultdict(list)
+                for pg, page_spans in groupby(
+                    nodes_in_comp[comp],
+                    lambda s: s.box.page if s.box is not None else None,
+                ):
+                    for span in page_spans:
+                        spans_by_page[pg].append(span)
+                for page_spans in spans_by_page.values():
+                    merged_box = Box.small_boxes_to_big_box(
+                        [span.box for span in page_spans]
+                    )
+                    merged_spans.append(
+                        Span(
+                            start=min([span.start for span in page_spans]),
+                            end=max([span.end for span in page_spans]),
+                            box=merged_box,
+                        )
+                    )
         return merged_spans
-
```

### Comparing `mmda-0.3.0/src/mmda.egg-info/PKG-INFO` & `mmda-0.3.6/src/mmda.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mmda
-Version: 0.3.0
+Version: 0.3.6
 Summary: MMDA - multimodal document analysis
 Author-email: Allen Institute for Artificial Intelligence <contact@allenai.org>
 License: Apache-2.0
 Project-URL: Homepage, https://www.github.com/allenai/mmda
 Project-URL: Repository, https://www.github.com/allenai/mmda
 Project-URL: Bug Tracker, https://www.github.com/allenai/mmda/issues
 Requires-Python: >=3.7
```

### Comparing `mmda-0.3.0/src/mmda.egg-info/SOURCES.txt` & `mmda-0.3.6/src/mmda.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,14 @@
 src/mmda/predictors/d2_predictors/__init__.py
 src/mmda/predictors/d2_predictors/bibentry_detection_predictor.py
 src/mmda/predictors/heuristic_predictors/__init__.py
 src/mmda/predictors/heuristic_predictors/dictionary_word_predictor.py
 src/mmda/predictors/heuristic_predictors/figure_table_predictors.py
 src/mmda/predictors/heuristic_predictors/grobid_citation_predictor.py
 src/mmda/predictors/heuristic_predictors/section_header_predictor.py
-src/mmda/predictors/heuristic_predictors/section_paragraph_predictor.py
 src/mmda/predictors/heuristic_predictors/sentence_boundary_predictor.py
 src/mmda/predictors/heuristic_predictors/whitespace_predictor.py
 src/mmda/predictors/hf_predictors/__init__.py
 src/mmda/predictors/hf_predictors/base_hf_predictor.py
 src/mmda/predictors/hf_predictors/mention_predictor.py
 src/mmda/predictors/hf_predictors/span_group_classification_predictor.py
 src/mmda/predictors/hf_predictors/token_classification_predictor.py
```

### Comparing `mmda-0.3.0/src/mmda.egg-info/requires.txt` & `mmda-0.3.6/src/mmda.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 tqdm
 pdf2image
 pdfplumber==0.7.4
 requests
 pandas
 pydantic
-ncls
+ncls==0.0.66
 necessary>=0.3.2
 
 [bibentry_detection_predictor]
 layoutparser
 torch==1.8.0+cu111
 torchvision==0.9.0+cu111
```

