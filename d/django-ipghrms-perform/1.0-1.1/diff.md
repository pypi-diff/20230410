# Comparing `tmp/django-ipghrms-perform-1.0.tar.gz` & `tmp/django-ipghrms-perform-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-ipghrms-perform-1.0.tar", last modified: Mon Mar 27 15:12:21 2023, max compression
+gzip compressed data, was "django-ipghrms-perform-1.1.tar", last modified: Mon Apr 10 06:04:43 2023, max compression
```

## Comparing `django-ipghrms-perform-1.0.tar` & `django-ipghrms-perform-1.1.tar`

### file list

```diff
@@ -1,210 +1,210 @@
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:21.121091 django-ipghrms-perform-1.0/
--rw-rw-rw-   0        0        0     1067 2023-03-27 15:12:01.000000 django-ipghrms-perform-1.0/LICENSE
--rw-rw-rw-   0        0        0      149 2023-03-27 14:30:27.000000 django-ipghrms-perform-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0      942 2023-03-27 15:12:21.122511 django-ipghrms-perform-1.0/PKG-INFO
--rw-rw-rw-   0        0        0      496 2023-03-27 14:30:34.000000 django-ipghrms-perform-1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.283917 django-ipghrms-perform-1.0/django_ipghrms_perform.egg-info/
--rw-rw-rw-   0        0        0      942 2023-03-27 15:12:20.000000 django-ipghrms-perform-1.0/django_ipghrms_perform.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     9462 2023-03-27 15:12:20.000000 django-ipghrms-perform-1.0/django_ipghrms_perform.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-27 15:12:20.000000 django-ipghrms-perform-1.0/django_ipghrms_perform.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-03-27 15:12:20.000000 django-ipghrms-perform-1.0/django_ipghrms_perform.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.305382 django-ipghrms-perform-1.0/perform/
--rw-rw-rw-   0        0        0        0 2022-12-03 02:55:42.000000 django-ipghrms-perform-1.0/perform/__init__.py
--rw-rw-rw-   0        0        0      778 2023-02-17 02:17:55.000000 django-ipghrms-perform-1.0/perform/admin.py
--rw-rw-rw-   0        0        0      193 2022-12-11 11:53:49.000000 django-ipghrms-perform-1.0/perform/apps.py
--rw-rw-rw-   0        0        0    27965 2023-03-13 01:29:17.000000 django-ipghrms-perform-1.0/perform/forms.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.363638 django-ipghrms-perform-1.0/perform/migrations/
--rw-rw-rw-   0        0        0    14355 2022-12-11 11:44:08.000000 django-ipghrms-perform-1.0/perform/migrations/0001_initial.py
--rw-rw-rw-   0        0        0     3623 2023-02-16 09:42:24.000000 django-ipghrms-perform-1.0/perform/migrations/0002_evalchoiceplanning_evalplanning.py
--rw-rw-rw-   0        0        0     2872 2023-02-16 09:58:15.000000 django-ipghrms-perform-1.0/perform/migrations/0003_evalplanninga_evalplanningb.py
--rw-rw-rw-   0        0        0      427 2023-02-16 13:38:20.000000 django-ipghrms-perform-1.0/perform/migrations/0004_evalplanninga_eval_date.py
--rw-rw-rw-   0        0        0      424 2023-02-16 14:00:50.000000 django-ipghrms-perform-1.0/perform/migrations/0005_evalplanninga_enter_date.py
--rw-rw-rw-   0        0        0      668 2023-02-16 14:05:52.000000 django-ipghrms-perform-1.0/perform/migrations/0006_evalplanninga_usereval.py
--rw-rw-rw-   0        0        0     1016 2023-02-16 15:14:43.000000 django-ipghrms-perform-1.0/perform/migrations/0007_auto_20230217_0014.py
--rw-rw-rw-   0        0        0     5984 2023-02-17 02:16:59.000000 django-ipghrms-perform-1.0/perform/migrations/0008_evalpreassessment_evalpreassessmenta_evalpreassessmentb.py
--rw-rw-rw-   0        0        0     1183 2023-02-17 09:13:31.000000 django-ipghrms-perform-1.0/perform/migrations/0009_auto_20230217_1813.py
--rw-rw-rw-   0        0        0     1707 2023-02-17 14:02:49.000000 django-ipghrms-perform-1.0/perform/migrations/0010_auto_20230217_2302.py
--rw-rw-rw-   0        0        0      412 2023-02-18 06:01:20.000000 django-ipghrms-perform-1.0/perform/migrations/0011_evalplanning_date.py
--rw-rw-rw-   0        0        0      564 2023-02-18 06:38:04.000000 django-ipghrms-perform-1.0/perform/migrations/0012_auto_20230218_1538.py
--rw-rw-rw-   0        0        0      580 2023-02-18 06:57:46.000000 django-ipghrms-perform-1.0/perform/migrations/0013_auto_20230218_1557.py
--rw-rw-rw-   0        0        0      767 2023-02-18 07:45:49.000000 django-ipghrms-perform-1.0/perform/migrations/0014_auto_20230218_1645.py
--rw-rw-rw-   0        0        0      404 2023-02-18 07:49:55.000000 django-ipghrms-perform-1.0/perform/migrations/0015_rename_eval_obj_date_evalpreassessment_eval_beh_date.py
--rw-rw-rw-   0        0        0      606 2023-02-18 08:18:38.000000 django-ipghrms-perform-1.0/perform/migrations/0016_auto_20230218_1718.py
--rw-rw-rw-   0        0        0      544 2023-02-18 08:19:19.000000 django-ipghrms-perform-1.0/perform/migrations/0017_auto_20230218_1719.py
--rw-rw-rw-   0        0        0      924 2023-02-18 09:27:15.000000 django-ipghrms-perform-1.0/perform/migrations/0018_auto_20230218_1827.py
--rw-rw-rw-   0        0        0     1792 2023-03-07 00:50:41.000000 django-ipghrms-perform-1.0/perform/migrations/0019_auto_20230307_0950.py
--rw-rw-rw-   0        0        0      999 2023-03-07 01:26:39.000000 django-ipghrms-perform-1.0/perform/migrations/0020_auto_20230307_1026.py
--rw-rw-rw-   0        0        0     1744 2023-03-07 01:27:04.000000 django-ipghrms-perform-1.0/perform/migrations/0021_auto_20230307_1027.py
--rw-rw-rw-   0        0        0      830 2023-03-10 00:23:54.000000 django-ipghrms-perform-1.0/perform/migrations/0022_auto_20230310_0923.py
--rw-rw-rw-   0        0        0      379 2023-03-10 00:25:11.000000 django-ipghrms-perform-1.0/perform/migrations/0023_rename_year_evalmonth_month.py
--rw-rw-rw-   0        0        0      353 2023-03-10 00:28:06.000000 django-ipghrms-perform-1.0/perform/migrations/0024_remove_evaltype_month.py
--rw-rw-rw-   0        0        0      432 2023-03-10 10:15:51.000000 django-ipghrms-perform-1.0/perform/migrations/0025_evalplanning_month.py
--rw-rw-rw-   0        0        0        0 2022-12-03 02:55:42.000000 django-ipghrms-perform-1.0/perform/migrations/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.544497 django-ipghrms-perform-1.0/perform/migrations/__pycache__/
--rw-rw-rw-   0        0        0     4808 2022-12-11 11:44:16.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0001_initial.cpython-310.pyc
--rw-rw-rw-   0        0        0     2131 2023-02-16 09:42:31.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0002_evalchoiceplanning_evalplanning.cpython-310.pyc
--rw-rw-rw-   0        0        0     1824 2023-02-16 09:58:23.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0003_evalplanninga_evalplanningb.cpython-310.pyc
--rw-rw-rw-   0        0        0      607 2023-02-16 13:38:28.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0004_evalplanninga_eval_date.cpython-310.pyc
--rw-rw-rw-   0        0        0      605 2023-02-16 14:00:56.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0005_evalplanninga_enter_date.cpython-310.pyc
--rw-rw-rw-   0        0        0      840 2023-02-16 14:05:57.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0006_evalplanninga_usereval.cpython-310.pyc
--rw-rw-rw-   0        0        0      949 2023-02-16 15:14:47.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0007_auto_20230217_0014.cpython-310.pyc
--rw-rw-rw-   0        0        0     3069 2023-02-17 02:17:07.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0008_evalpreassessment_evalpreassessmenta_evalpreassessmentb.cpython-310.pyc
--rw-rw-rw-   0        0        0     1073 2023-02-17 09:13:48.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0009_auto_20230217_1813.cpython-310.pyc
--rw-rw-rw-   0        0        0     1146 2023-02-17 14:02:59.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0010_auto_20230217_2302.cpython-310.pyc
--rw-rw-rw-   0        0        0      586 2023-02-18 06:01:26.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0011_evalplanning_date.cpython-310.pyc
--rw-rw-rw-   0        0        0      670 2023-02-18 06:38:11.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0012_auto_20230218_1538.cpython-310.pyc
--rw-rw-rw-   0        0        0      686 2023-02-18 06:57:51.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0013_auto_20230218_1557.cpython-310.pyc
--rw-rw-rw-   0        0        0      746 2023-02-18 07:45:52.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0014_auto_20230218_1645.cpython-310.pyc
--rw-rw-rw-   0        0        0      601 2023-02-18 07:49:59.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0015_rename_eval_obj_date_evalpreassessment_eval_beh_date.cpython-310.pyc
--rw-rw-rw-   0        0        0      716 2023-02-18 08:18:42.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0016_auto_20230218_1718.cpython-310.pyc
--rw-rw-rw-   0        0        0      602 2023-02-18 08:19:23.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0017_auto_20230218_1719.cpython-310.pyc
--rw-rw-rw-   0        0        0      739 2023-02-18 09:27:22.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0018_auto_20230218_1827.cpython-310.pyc
--rw-rw-rw-   0        0        0     1263 2023-03-07 00:50:47.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0019_auto_20230307_0950.cpython-310.pyc
--rw-rw-rw-   0        0        0      747 2023-03-07 01:26:44.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0020_auto_20230307_1026.cpython-310.pyc
--rw-rw-rw-   0        0        0     1255 2023-03-07 01:27:09.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0021_auto_20230307_1027.cpython-310.pyc
--rw-rw-rw-   0        0        0      928 2023-03-10 00:24:06.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0022_auto_20230310_0923.cpython-310.pyc
--rw-rw-rw-   0        0        0      551 2023-03-10 00:25:17.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0023_rename_year_evalmonth_month.cpython-310.pyc
--rw-rw-rw-   0        0        0      529 2023-03-10 00:28:13.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0024_remove_evaltype_month.cpython-310.pyc
--rw-rw-rw-   0        0        0      610 2023-03-10 10:16:01.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/0025_evalplanning_month.cpython-310.pyc
--rw-rw-rw-   0        0        0      145 2022-12-11 11:33:18.000000 django-ipghrms-perform-1.0/perform/migrations/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0    19371 2023-03-10 00:37:17.000000 django-ipghrms-perform-1.0/perform/models.py
--rw-rw-rw-   0        0        0      482 2022-12-03 11:32:52.000000 django-ipghrms-perform-1.0/perform/signals.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.254019 django-ipghrms-perform-1.0/perform/templates/
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.689476 django-ipghrms-perform-1.0/perform/templates/perform2/
--rw-rw-rw-   0        0        0     2836 2022-12-04 12:33:14.000000 django-ipghrms-perform-1.0/perform/templates/perform2/all_eval_cat_list.html
--rw-rw-rw-   0        0        0    10269 2023-02-21 00:18:24.000000 django-ipghrms-perform-1.0/perform/templates/perform2/all_eval_dash.html
--rw-rw-rw-   0        0        0    10359 2022-12-04 12:42:08.000000 django-ipghrms-perform-1.0/perform/templates/perform2/all_eval_detail.html
--rw-rw-rw-   0        0        0     2934 2022-12-10 23:58:14.000000 django-ipghrms-perform-1.0/perform/templates/perform2/all_eval_list.html
--rw-rw-rw-   0        0        0     2854 2022-12-04 12:43:18.000000 django-ipghrms-perform-1.0/perform/templates/perform2/all_eval_year_list.html
--rw-rw-rw-   0        0        0     2264 2023-02-16 15:03:53.000000 django-ipghrms-perform-1.0/perform/templates/perform2/behavior_list.html
--rw-rw-rw-   0        0        0     2836 2022-12-04 12:33:08.000000 django-ipghrms-perform-1.0/perform/templates/perform2/c_eval_cat_list.html
--rw-rw-rw-   0        0        0     2610 2023-02-13 01:58:26.000000 django-ipghrms-perform-1.0/perform/templates/perform2/c_eval_dash.html
--rw-rw-rw-   0        0        0    16809 2023-02-13 02:08:55.000000 django-ipghrms-perform-1.0/perform/templates/perform2/c_eval_detail.html
--rw-rw-rw-   0        0        0     3302 2023-02-13 02:08:12.000000 django-ipghrms-perform-1.0/perform/templates/perform2/c_eval_list.html
--rw-rw-rw-   0        0        0     2971 2023-02-13 02:06:53.000000 django-ipghrms-perform-1.0/perform/templates/perform2/c_eval_year_list.html
--rw-rw-rw-   0        0        0    17224 2023-02-18 10:04:19.000000 django-ipghrms-perform-1.0/perform/templates/perform2/eval_detail.html
--rw-rw-rw-   0        0        0    26459 2023-03-07 06:23:09.000000 django-ipghrms-perform-1.0/perform/templates/perform2/evaluator_eval_detail.html
--rw-rw-rw-   0        0        0     4541 2023-02-18 06:55:36.000000 django-ipghrms-perform-1.0/perform/templates/perform2/evaluator_plan_detail.html
--rw-rw-rw-   0        0        0    13328 2023-02-19 08:54:21.000000 django-ipghrms-perform-1.0/perform/templates/perform2/evaluator_preass_detail.html
--rw-rw-rw-   0        0        0    11081 2023-02-19 08:54:32.000000 django-ipghrms-perform-1.0/perform/templates/perform2/evaluator_self_detail.html
--rw-rw-rw-   0        0        0     3176 2023-02-19 07:15:16.000000 django-ipghrms-perform-1.0/perform/templates/perform2/form.html
--rw-rw-rw-   0        0        0     2861 2023-03-07 05:46:32.000000 django-ipghrms-perform-1.0/perform/templates/perform2/form_det.html
--rw-rw-rw-   0        0        0      968 2023-02-13 02:04:37.000000 django-ipghrms-perform-1.0/perform/templates/perform2/form_eval.html
--rw-rw-rw-   0        0        0    12727 2023-02-18 06:46:32.000000 django-ipghrms-perform-1.0/perform/templates/perform2/plan_detail.html
--rw-rw-rw-   0        0        0    10412 2023-02-18 10:06:55.000000 django-ipghrms-perform-1.0/perform/templates/perform2/pre_ass_detail.html
--rw-rw-rw-   0        0        0    14352 2023-02-19 07:38:10.000000 django-ipghrms-perform-1.0/perform/templates/perform2/self_detail.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.713999 django-ipghrms-perform-1.0/perform/templates/perform2_conf/
--rw-rw-rw-   0        0        0     2714 2022-09-28 15:51:12.000000 django-ipghrms-perform-1.0/perform/templates/perform2_conf/cat_score.html
--rw-rw-rw-   0        0        0    10473 2023-02-18 06:25:42.000000 django-ipghrms-perform-1.0/perform/templates/perform2_conf/conf_dash.html
--rw-rw-rw-   0        0        0      779 2022-12-04 04:10:24.000000 django-ipghrms-perform-1.0/perform/templates/perform2_conf/form.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.763083 django-ipghrms-perform-1.0/perform/templates/perform2_self/
--rw-rw-rw-   0        0        0     8049 2022-12-04 14:16:10.000000 django-ipghrms-perform-1.0/perform/templates/perform2_self/all_eval_detail.html
--rw-rw-rw-   0        0        0     3224 2023-02-09 04:43:42.000000 django-ipghrms-perform-1.0/perform/templates/perform2_self/all_eval_list.html
--rw-rw-rw-   0        0        0    10721 2023-02-09 04:49:07.000000 django-ipghrms-perform-1.0/perform/templates/perform2_self/eval_detail.html
--rw-rw-rw-   0        0        0     2725 2023-02-09 04:47:23.000000 django-ipghrms-perform-1.0/perform/templates/perform2_self/eval_list.html
--rw-rw-rw-   0        0        0     3415 2023-02-13 02:03:37.000000 django-ipghrms-perform-1.0/perform/templates/perform2_self/eval_unit_list.html
--rw-rw-rw-   0        0        0      947 2023-02-09 04:48:40.000000 django-ipghrms-perform-1.0/perform/templates/perform2_self/form.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.783500 django-ipghrms-perform-1.0/perform/templates/perform_eval_components/
--rw-rw-rw-   0        0        0     4617 2023-02-17 00:21:22.000000 django-ipghrms-perform-1.0/perform/templates/perform_eval_components/behavior.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.802369 django-ipghrms-perform-1.0/perform/templates/perform_eval_components/evaluator/
--rw-rw-rw-   0        0        0     4053 2023-02-17 01:03:16.000000 django-ipghrms-perform-1.0/perform/templates/perform_eval_components/evaluator/behavior.html
--rw-rw-rw-   0        0        0      841 2023-02-16 13:35:38.000000 django-ipghrms-perform-1.0/perform/templates/perform_eval_components/evaluator/header.html
--rw-rw-rw-   0        0        0     5699 2023-02-19 07:08:40.000000 django-ipghrms-perform-1.0/perform/templates/perform_eval_components/evaluator/individual.html
--rw-rw-rw-   0        0        0      549 2023-02-17 15:06:43.000000 django-ipghrms-perform-1.0/perform/templates/perform_eval_components/evaluator/objectives.html
--rw-rw-rw-   0        0        0      841 2023-02-16 13:35:38.000000 django-ipghrms-perform-1.0/perform/templates/perform_eval_components/header.html
--rw-rw-rw-   0        0        0     5498 2023-02-18 09:36:29.000000 django-ipghrms-perform-1.0/perform/templates/perform_eval_components/individual.html
--rw-rw-rw-   0        0        0      549 2023-02-17 14:35:48.000000 django-ipghrms-perform-1.0/perform/templates/perform_eval_components/objectives.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.819970 django-ipghrms-perform-1.0/perform/templates/perform_plan_components/
--rw-rw-rw-   0        0        0     4617 2023-02-17 00:21:22.000000 django-ipghrms-perform-1.0/perform/templates/perform_plan_components/behavior.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.837602 django-ipghrms-perform-1.0/perform/templates/perform_plan_components/evaluator/
--rw-rw-rw-   0        0        0     4960 2023-02-19 07:18:34.000000 django-ipghrms-perform-1.0/perform/templates/perform_plan_components/evaluator/behavior.html
--rw-rw-rw-   0        0        0      841 2023-02-16 13:35:38.000000 django-ipghrms-perform-1.0/perform/templates/perform_plan_components/evaluator/header.html
--rw-rw-rw-   0        0        0     4569 2023-02-19 08:51:00.000000 django-ipghrms-perform-1.0/perform/templates/perform_plan_components/evaluator/individual.html
--rw-rw-rw-   0        0        0      567 2023-02-17 00:48:26.000000 django-ipghrms-perform-1.0/perform/templates/perform_plan_components/evaluator/objectives.html
--rw-rw-rw-   0        0        0      841 2023-02-16 13:35:38.000000 django-ipghrms-perform-1.0/perform/templates/perform_plan_components/header.html
--rw-rw-rw-   0        0        0     3781 2023-02-17 02:58:02.000000 django-ipghrms-perform-1.0/perform/templates/perform_plan_components/individual.html
--rw-rw-rw-   0        0        0     1504 2023-02-16 16:46:35.000000 django-ipghrms-perform-1.0/perform/templates/perform_plan_components/objectives.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.855170 django-ipghrms-perform-1.0/perform/templates/perform_pre_ass_components/
--rw-rw-rw-   0        0        0     4617 2023-03-01 00:53:07.000000 django-ipghrms-perform-1.0/perform/templates/perform_pre_ass_components/behavior.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.863282 django-ipghrms-perform-1.0/perform/templates/perform_pre_ass_components/evaluator/
--rw-rw-rw-   0        0        0      458 2023-02-17 13:50:00.000000 django-ipghrms-perform-1.0/perform/templates/perform_pre_ass_components/evaluator/header.html
--rw-rw-rw-   0        0        0     4795 2023-02-18 07:58:17.000000 django-ipghrms-perform-1.0/perform/templates/perform_pre_ass_components/evaluator/individual.html
--rw-rw-rw-   0        0        0      458 2023-02-17 02:52:56.000000 django-ipghrms-perform-1.0/perform/templates/perform_pre_ass_components/header.html
--rw-rw-rw-   0        0        0     3650 2023-02-18 10:06:01.000000 django-ipghrms-perform-1.0/perform/templates/perform_pre_ass_components/individual.html
--rw-rw-rw-   0        0        0     1504 2023-02-17 07:51:20.000000 django-ipghrms-perform-1.0/perform/templates/perform_pre_ass_components/objectives.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.883535 django-ipghrms-perform-1.0/perform/templates/perform_self_eval/
--rw-rw-rw-   0        0        0     4617 2023-02-17 00:21:22.000000 django-ipghrms-perform-1.0/perform/templates/perform_self_eval/behavior.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.889586 django-ipghrms-perform-1.0/perform/templates/perform_self_eval/evaluator/
--rw-rw-rw-   0        0        0      458 2023-02-18 08:36:46.000000 django-ipghrms-perform-1.0/perform/templates/perform_self_eval/evaluator/header.html
--rw-rw-rw-   0        0        0     3754 2023-02-19 08:49:18.000000 django-ipghrms-perform-1.0/perform/templates/perform_self_eval/evaluator/individual.html
--rw-rw-rw-   0        0        0      458 2023-02-17 12:33:37.000000 django-ipghrms-perform-1.0/perform/templates/perform_self_eval/header.html
--rw-rw-rw-   0        0        0     3783 2023-02-19 07:36:13.000000 django-ipghrms-perform-1.0/perform/templates/perform_self_eval/individual.html
--rw-rw-rw-   0        0        0     1518 2023-02-19 07:36:43.000000 django-ipghrms-perform-1.0/perform/templates/perform_self_eval/objectives.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.920738 django-ipghrms-perform-1.0/perform/templates/perform_staff/
--rw-rw-rw-   0        0        0    17143 2023-03-01 01:07:34.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff/eval_detail.html
--rw-rw-rw-   0        0        0     5308 2023-03-01 04:46:25.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff/list.html
--rw-rw-rw-   0        0        0    12658 2023-02-19 05:40:13.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff/plan_detail.html
--rw-rw-rw-   0        0        0    10322 2023-03-01 01:11:43.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff/preass_detail.html
--rw-rw-rw-   0        0        0    13547 2023-03-01 01:07:51.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff/self_detail.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.255018 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.933703 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/eval/
--rw-rw-rw-   0        0        0      841 2023-02-16 13:35:38.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/eval/header.html
--rw-rw-rw-   0        0        0     5498 2023-02-18 09:36:29.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/eval/individual.html
--rw-rw-rw-   0        0        0      549 2023-02-17 14:35:48.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/eval/objectives.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.947147 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/planning/
--rw-rw-rw-   0        0        0      841 2023-02-16 13:35:38.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/planning/header.html
--rw-rw-rw-   0        0        0     3793 2023-02-19 07:31:16.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/planning/individual.html
--rw-rw-rw-   0        0        0     1504 2023-02-16 16:46:35.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/planning/objectives.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.953314 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/preass/
--rw-rw-rw-   0        0        0      458 2023-02-17 02:52:56.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/preass/header.html
--rw-rw-rw-   0        0        0     3650 2023-02-19 06:26:40.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/preass/individual.html
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.959812 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/self/
--rw-rw-rw-   0        0        0      458 2023-02-17 12:33:37.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/self/header.html
--rw-rw-rw-   0        0        0     3664 2023-03-01 01:08:26.000000 django-ipghrms-perform-1.0/perform/templates/perform_staff_components/self/individual.html
--rw-rw-rw-   0        0        0       63 2022-12-03 02:55:42.000000 django-ipghrms-perform-1.0/perform/tests.py
--rw-rw-rw-   0        0        0    10691 2023-03-07 06:00:15.000000 django-ipghrms-perform-1.0/perform/urls.py
--rw-rw-rw-   0        0        0      325 2022-10-18 10:39:31.000000 django-ipghrms-perform-1.0/perform/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:20.993355 django-ipghrms-perform-1.0/perform/views/
--rw-rw-rw-   0        0        0      348 2023-02-19 05:20:47.000000 django-ipghrms-perform-1.0/perform/views/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-27 15:12:21.119091 django-ipghrms-perform-1.0/perform/views/__pycache__/
--rw-rw-rw-   0        0        0      435 2023-02-19 05:21:06.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      339 2022-12-04 12:46:06.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     5705 2023-03-12 11:09:36.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/all_perform_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     3924 2022-12-06 12:02:56.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/all_perform_v.cpython-39.pyc
--rw-rw-rw-   0        0        0     8085 2023-02-19 07:03:35.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/c_perform_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     5773 2022-12-04 12:44:38.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/c_perform_m.cpython-39.pyc
--rw-rw-rw-   0        0        0     4314 2023-02-16 12:19:25.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/c_perform_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     4287 2022-12-06 01:41:52.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/c_perform_v.cpython-39.pyc
--rw-rw-rw-   0        0        0     3794 2022-12-04 06:02:42.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/emp_perform_m.cpython-39.pyc
--rw-rw-rw-   0        0        0     1764 2022-12-04 05:57:38.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/emp_perform_v.cpython-39.pyc
--rw-rw-rw-   0        0        0     4188 2022-12-04 12:30:40.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/hr_perform_v.cpython-39.pyc
--rw-rw-rw-   0        0        0      145 2023-02-16 10:07:51.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/perfom_conf_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     8380 2023-02-27 01:22:43.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/perfom_plan.cpython-310.pyc
--rw-rw-rw-   0        0        0     4923 2023-02-19 05:55:59.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/perform_conf.cpython-310.pyc
--rw-rw-rw-   0        0        0     3628 2022-12-04 04:13:52.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/perform_conf.cpython-39.pyc
--rw-rw-rw-   0        0        0     2307 2023-02-16 14:53:48.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/perform_conf_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     6535 2023-03-07 05:57:39.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/perform_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     5048 2022-12-04 12:59:04.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/perform_m.cpython-39.pyc
--rw-rw-rw-   0        0        0     7332 2023-03-01 00:56:06.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/perform_pre_ass.cpython-310.pyc
--rw-rw-rw-   0        0        0      141 2022-12-11 11:32:30.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/perform_r.cpython-310.pyc
--rw-rw-rw-   0        0        0      146 2022-12-03 10:56:26.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/perform_r.cpython-39.pyc
--rw-rw-rw-   0        0        0     3421 2023-03-01 01:11:28.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/perform_staff.cpython-310.pyc
--rw-rw-rw-   0        0        0     7887 2023-02-27 01:13:02.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/self_perform_m.cpython-310.pyc
--rw-rw-rw-   0        0        0     4329 2022-12-10 23:47:32.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/self_perform_m.cpython-39.pyc
--rw-rw-rw-   0        0        0     4398 2023-02-18 08:39:27.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/self_perform_v.cpython-310.pyc
--rw-rw-rw-   0        0        0     3881 2022-12-11 00:15:20.000000 django-ipghrms-perform-1.0/perform/views/__pycache__/self_perform_v.cpython-39.pyc
--rw-rw-rw-   0        0        0     6864 2023-03-12 11:09:33.000000 django-ipghrms-perform-1.0/perform/views/all_perform_v.py
--rw-rw-rw-   0        0        0    11254 2023-02-19 07:03:31.000000 django-ipghrms-perform-1.0/perform/views/c_perform_m.py
--rw-rw-rw-   0        0        0     4935 2023-02-16 12:19:21.000000 django-ipghrms-perform-1.0/perform/views/c_perform_v.py
--rw-rw-rw-   0        0        0    14059 2023-02-27 01:22:40.000000 django-ipghrms-perform-1.0/perform/views/perfom_plan.py
--rw-rw-rw-   0        0        0     5927 2023-02-19 05:55:55.000000 django-ipghrms-perform-1.0/perform/views/perform_conf.py
--rw-rw-rw-   0        0        0     2686 2023-02-16 14:53:45.000000 django-ipghrms-perform-1.0/perform/views/perform_conf_m.py
--rw-rw-rw-   0        0        0    12285 2023-03-07 05:57:36.000000 django-ipghrms-perform-1.0/perform/views/perform_m.py
--rw-rw-rw-   0        0        0    16284 2023-03-01 00:56:01.000000 django-ipghrms-perform-1.0/perform/views/perform_pre_ass.py
--rw-rw-rw-   0        0        0        0 2022-12-03 02:58:48.000000 django-ipghrms-perform-1.0/perform/views/perform_r.py
--rw-rw-rw-   0        0        0     4403 2023-03-01 01:11:24.000000 django-ipghrms-perform-1.0/perform/views/perform_staff.py
--rw-rw-rw-   0        0        0    11451 2023-02-27 01:13:00.000000 django-ipghrms-perform-1.0/perform/views/self_perform_m.py
--rw-rw-rw-   0        0        0     6075 2023-02-18 08:39:26.000000 django-ipghrms-perform-1.0/perform/views/self_perform_v.py
--rw-rw-rw-   0        0        0       66 2022-12-03 02:55:42.000000 django-ipghrms-perform-1.0/perform/views.py
--rw-rw-rw-   0        0        0      509 2023-03-27 15:12:21.125511 django-ipghrms-perform-1.0/setup.cfg
--rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-perform-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.934226 django-ipghrms-perform-1.1/
+-rw-rw-rw-   0        0        0     1067 2023-03-27 15:12:01.000000 django-ipghrms-perform-1.1/LICENSE
+-rw-rw-rw-   0        0        0      149 2023-03-27 14:30:27.000000 django-ipghrms-perform-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      942 2023-04-10 06:04:43.934900 django-ipghrms-perform-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      496 2023-03-27 14:30:34.000000 django-ipghrms-perform-1.1/README.rst
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:41.644208 django-ipghrms-perform-1.1/django_ipghrms_perform.egg-info/
+-rw-rw-rw-   0        0        0      942 2023-04-10 06:04:41.000000 django-ipghrms-perform-1.1/django_ipghrms_perform.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     9462 2023-04-10 06:04:41.000000 django-ipghrms-perform-1.1/django_ipghrms_perform.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-10 06:04:41.000000 django-ipghrms-perform-1.1/django_ipghrms_perform.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-04-10 06:04:41.000000 django-ipghrms-perform-1.1/django_ipghrms_perform.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:41.709829 django-ipghrms-perform-1.1/perform/
+-rw-rw-rw-   0        0        0        0 2022-12-03 02:55:42.000000 django-ipghrms-perform-1.1/perform/__init__.py
+-rw-rw-rw-   0        0        0      778 2023-02-17 02:17:55.000000 django-ipghrms-perform-1.1/perform/admin.py
+-rw-rw-rw-   0        0        0      193 2022-12-11 11:53:49.000000 django-ipghrms-perform-1.1/perform/apps.py
+-rw-rw-rw-   0        0        0    27965 2023-03-13 01:29:17.000000 django-ipghrms-perform-1.1/perform/forms.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:41.912391 django-ipghrms-perform-1.1/perform/migrations/
+-rw-rw-rw-   0        0        0    14355 2022-12-11 11:44:08.000000 django-ipghrms-perform-1.1/perform/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0     3623 2023-02-16 09:42:24.000000 django-ipghrms-perform-1.1/perform/migrations/0002_evalchoiceplanning_evalplanning.py
+-rw-rw-rw-   0        0        0     2872 2023-02-16 09:58:15.000000 django-ipghrms-perform-1.1/perform/migrations/0003_evalplanninga_evalplanningb.py
+-rw-rw-rw-   0        0        0      427 2023-02-16 13:38:20.000000 django-ipghrms-perform-1.1/perform/migrations/0004_evalplanninga_eval_date.py
+-rw-rw-rw-   0        0        0      424 2023-02-16 14:00:50.000000 django-ipghrms-perform-1.1/perform/migrations/0005_evalplanninga_enter_date.py
+-rw-rw-rw-   0        0        0      668 2023-02-16 14:05:52.000000 django-ipghrms-perform-1.1/perform/migrations/0006_evalplanninga_usereval.py
+-rw-rw-rw-   0        0        0     1016 2023-02-16 15:14:43.000000 django-ipghrms-perform-1.1/perform/migrations/0007_auto_20230217_0014.py
+-rw-rw-rw-   0        0        0     5984 2023-02-17 02:16:59.000000 django-ipghrms-perform-1.1/perform/migrations/0008_evalpreassessment_evalpreassessmenta_evalpreassessmentb.py
+-rw-rw-rw-   0        0        0     1183 2023-02-17 09:13:31.000000 django-ipghrms-perform-1.1/perform/migrations/0009_auto_20230217_1813.py
+-rw-rw-rw-   0        0        0     1707 2023-02-17 14:02:49.000000 django-ipghrms-perform-1.1/perform/migrations/0010_auto_20230217_2302.py
+-rw-rw-rw-   0        0        0      412 2023-02-18 06:01:20.000000 django-ipghrms-perform-1.1/perform/migrations/0011_evalplanning_date.py
+-rw-rw-rw-   0        0        0      564 2023-02-18 06:38:04.000000 django-ipghrms-perform-1.1/perform/migrations/0012_auto_20230218_1538.py
+-rw-rw-rw-   0        0        0      580 2023-02-18 06:57:46.000000 django-ipghrms-perform-1.1/perform/migrations/0013_auto_20230218_1557.py
+-rw-rw-rw-   0        0        0      767 2023-02-18 07:45:49.000000 django-ipghrms-perform-1.1/perform/migrations/0014_auto_20230218_1645.py
+-rw-rw-rw-   0        0        0      404 2023-02-18 07:49:55.000000 django-ipghrms-perform-1.1/perform/migrations/0015_rename_eval_obj_date_evalpreassessment_eval_beh_date.py
+-rw-rw-rw-   0        0        0      606 2023-02-18 08:18:38.000000 django-ipghrms-perform-1.1/perform/migrations/0016_auto_20230218_1718.py
+-rw-rw-rw-   0        0        0      544 2023-02-18 08:19:19.000000 django-ipghrms-perform-1.1/perform/migrations/0017_auto_20230218_1719.py
+-rw-rw-rw-   0        0        0      924 2023-02-18 09:27:15.000000 django-ipghrms-perform-1.1/perform/migrations/0018_auto_20230218_1827.py
+-rw-rw-rw-   0        0        0     1792 2023-03-07 00:50:41.000000 django-ipghrms-perform-1.1/perform/migrations/0019_auto_20230307_0950.py
+-rw-rw-rw-   0        0        0      999 2023-03-07 01:26:39.000000 django-ipghrms-perform-1.1/perform/migrations/0020_auto_20230307_1026.py
+-rw-rw-rw-   0        0        0     1744 2023-03-07 01:27:04.000000 django-ipghrms-perform-1.1/perform/migrations/0021_auto_20230307_1027.py
+-rw-rw-rw-   0        0        0      830 2023-03-10 00:23:54.000000 django-ipghrms-perform-1.1/perform/migrations/0022_auto_20230310_0923.py
+-rw-rw-rw-   0        0        0      379 2023-03-10 00:25:11.000000 django-ipghrms-perform-1.1/perform/migrations/0023_rename_year_evalmonth_month.py
+-rw-rw-rw-   0        0        0      353 2023-03-10 00:28:06.000000 django-ipghrms-perform-1.1/perform/migrations/0024_remove_evaltype_month.py
+-rw-rw-rw-   0        0        0      432 2023-03-10 10:15:51.000000 django-ipghrms-perform-1.1/perform/migrations/0025_evalplanning_month.py
+-rw-rw-rw-   0        0        0        0 2022-12-03 02:55:42.000000 django-ipghrms-perform-1.1/perform/migrations/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:42.370921 django-ipghrms-perform-1.1/perform/migrations/__pycache__/
+-rw-rw-rw-   0        0        0     4808 2022-12-11 11:44:16.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0001_initial.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2131 2023-02-16 09:42:31.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0002_evalchoiceplanning_evalplanning.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1824 2023-02-16 09:58:23.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0003_evalplanninga_evalplanningb.cpython-310.pyc
+-rw-rw-rw-   0        0        0      607 2023-02-16 13:38:28.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0004_evalplanninga_eval_date.cpython-310.pyc
+-rw-rw-rw-   0        0        0      605 2023-02-16 14:00:56.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0005_evalplanninga_enter_date.cpython-310.pyc
+-rw-rw-rw-   0        0        0      840 2023-02-16 14:05:57.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0006_evalplanninga_usereval.cpython-310.pyc
+-rw-rw-rw-   0        0        0      949 2023-02-16 15:14:47.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0007_auto_20230217_0014.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3069 2023-02-17 02:17:07.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0008_evalpreassessment_evalpreassessmenta_evalpreassessmentb.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1073 2023-02-17 09:13:48.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0009_auto_20230217_1813.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1146 2023-02-17 14:02:59.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0010_auto_20230217_2302.cpython-310.pyc
+-rw-rw-rw-   0        0        0      586 2023-02-18 06:01:26.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0011_evalplanning_date.cpython-310.pyc
+-rw-rw-rw-   0        0        0      670 2023-02-18 06:38:11.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0012_auto_20230218_1538.cpython-310.pyc
+-rw-rw-rw-   0        0        0      686 2023-02-18 06:57:51.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0013_auto_20230218_1557.cpython-310.pyc
+-rw-rw-rw-   0        0        0      746 2023-02-18 07:45:52.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0014_auto_20230218_1645.cpython-310.pyc
+-rw-rw-rw-   0        0        0      601 2023-02-18 07:49:59.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0015_rename_eval_obj_date_evalpreassessment_eval_beh_date.cpython-310.pyc
+-rw-rw-rw-   0        0        0      716 2023-02-18 08:18:42.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0016_auto_20230218_1718.cpython-310.pyc
+-rw-rw-rw-   0        0        0      602 2023-02-18 08:19:23.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0017_auto_20230218_1719.cpython-310.pyc
+-rw-rw-rw-   0        0        0      739 2023-02-18 09:27:22.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0018_auto_20230218_1827.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1263 2023-03-07 00:50:47.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0019_auto_20230307_0950.cpython-310.pyc
+-rw-rw-rw-   0        0        0      747 2023-03-07 01:26:44.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0020_auto_20230307_1026.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1255 2023-03-07 01:27:09.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0021_auto_20230307_1027.cpython-310.pyc
+-rw-rw-rw-   0        0        0      928 2023-03-10 00:24:06.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0022_auto_20230310_0923.cpython-310.pyc
+-rw-rw-rw-   0        0        0      551 2023-03-10 00:25:17.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0023_rename_year_evalmonth_month.cpython-310.pyc
+-rw-rw-rw-   0        0        0      529 2023-03-10 00:28:13.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0024_remove_evaltype_month.cpython-310.pyc
+-rw-rw-rw-   0        0        0      610 2023-03-10 10:16:01.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/0025_evalplanning_month.cpython-310.pyc
+-rw-rw-rw-   0        0        0      145 2022-12-11 11:33:18.000000 django-ipghrms-perform-1.1/perform/migrations/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0    19371 2023-03-10 00:37:17.000000 django-ipghrms-perform-1.1/perform/models.py
+-rw-rw-rw-   0        0        0      482 2022-12-03 11:32:52.000000 django-ipghrms-perform-1.1/perform/signals.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:41.550783 django-ipghrms-perform-1.1/perform/templates/
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:42.793002 django-ipghrms-perform-1.1/perform/templates/perform2/
+-rw-rw-rw-   0        0        0     2836 2022-12-04 12:33:14.000000 django-ipghrms-perform-1.1/perform/templates/perform2/all_eval_cat_list.html
+-rw-rw-rw-   0        0        0    10269 2023-02-21 00:18:24.000000 django-ipghrms-perform-1.1/perform/templates/perform2/all_eval_dash.html
+-rw-rw-rw-   0        0        0    10359 2022-12-04 12:42:08.000000 django-ipghrms-perform-1.1/perform/templates/perform2/all_eval_detail.html
+-rw-rw-rw-   0        0        0     2934 2022-12-10 23:58:14.000000 django-ipghrms-perform-1.1/perform/templates/perform2/all_eval_list.html
+-rw-rw-rw-   0        0        0     2854 2022-12-04 12:43:18.000000 django-ipghrms-perform-1.1/perform/templates/perform2/all_eval_year_list.html
+-rw-rw-rw-   0        0        0     2264 2023-02-16 15:03:53.000000 django-ipghrms-perform-1.1/perform/templates/perform2/behavior_list.html
+-rw-rw-rw-   0        0        0     2836 2022-12-04 12:33:08.000000 django-ipghrms-perform-1.1/perform/templates/perform2/c_eval_cat_list.html
+-rw-rw-rw-   0        0        0     2610 2023-02-13 01:58:26.000000 django-ipghrms-perform-1.1/perform/templates/perform2/c_eval_dash.html
+-rw-rw-rw-   0        0        0    16809 2023-02-13 02:08:55.000000 django-ipghrms-perform-1.1/perform/templates/perform2/c_eval_detail.html
+-rw-rw-rw-   0        0        0     3302 2023-02-13 02:08:12.000000 django-ipghrms-perform-1.1/perform/templates/perform2/c_eval_list.html
+-rw-rw-rw-   0        0        0     2971 2023-02-13 02:06:53.000000 django-ipghrms-perform-1.1/perform/templates/perform2/c_eval_year_list.html
+-rw-rw-rw-   0        0        0    17224 2023-02-18 10:04:19.000000 django-ipghrms-perform-1.1/perform/templates/perform2/eval_detail.html
+-rw-rw-rw-   0        0        0    26459 2023-03-07 06:23:09.000000 django-ipghrms-perform-1.1/perform/templates/perform2/evaluator_eval_detail.html
+-rw-rw-rw-   0        0        0     4541 2023-02-18 06:55:36.000000 django-ipghrms-perform-1.1/perform/templates/perform2/evaluator_plan_detail.html
+-rw-rw-rw-   0        0        0    13328 2023-02-19 08:54:21.000000 django-ipghrms-perform-1.1/perform/templates/perform2/evaluator_preass_detail.html
+-rw-rw-rw-   0        0        0    11081 2023-02-19 08:54:32.000000 django-ipghrms-perform-1.1/perform/templates/perform2/evaluator_self_detail.html
+-rw-rw-rw-   0        0        0     3176 2023-02-19 07:15:16.000000 django-ipghrms-perform-1.1/perform/templates/perform2/form.html
+-rw-rw-rw-   0        0        0     2861 2023-03-07 05:46:32.000000 django-ipghrms-perform-1.1/perform/templates/perform2/form_det.html
+-rw-rw-rw-   0        0        0      968 2023-02-13 02:04:37.000000 django-ipghrms-perform-1.1/perform/templates/perform2/form_eval.html
+-rw-rw-rw-   0        0        0    12727 2023-02-18 06:46:32.000000 django-ipghrms-perform-1.1/perform/templates/perform2/plan_detail.html
+-rw-rw-rw-   0        0        0    10412 2023-02-18 10:06:55.000000 django-ipghrms-perform-1.1/perform/templates/perform2/pre_ass_detail.html
+-rw-rw-rw-   0        0        0    14352 2023-02-19 07:38:10.000000 django-ipghrms-perform-1.1/perform/templates/perform2/self_detail.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:42.828239 django-ipghrms-perform-1.1/perform/templates/perform2_conf/
+-rw-rw-rw-   0        0        0     2714 2022-09-28 15:51:12.000000 django-ipghrms-perform-1.1/perform/templates/perform2_conf/cat_score.html
+-rw-rw-rw-   0        0        0    10482 2023-04-10 05:01:43.000000 django-ipghrms-perform-1.1/perform/templates/perform2_conf/conf_dash.html
+-rw-rw-rw-   0        0        0      779 2022-12-04 04:10:24.000000 django-ipghrms-perform-1.1/perform/templates/perform2_conf/form.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:42.928122 django-ipghrms-perform-1.1/perform/templates/perform2_self/
+-rw-rw-rw-   0        0        0     8049 2022-12-04 14:16:10.000000 django-ipghrms-perform-1.1/perform/templates/perform2_self/all_eval_detail.html
+-rw-rw-rw-   0        0        0     3224 2023-02-09 04:43:42.000000 django-ipghrms-perform-1.1/perform/templates/perform2_self/all_eval_list.html
+-rw-rw-rw-   0        0        0    10721 2023-02-09 04:49:07.000000 django-ipghrms-perform-1.1/perform/templates/perform2_self/eval_detail.html
+-rw-rw-rw-   0        0        0     2725 2023-02-09 04:47:23.000000 django-ipghrms-perform-1.1/perform/templates/perform2_self/eval_list.html
+-rw-rw-rw-   0        0        0     3415 2023-02-13 02:03:37.000000 django-ipghrms-perform-1.1/perform/templates/perform2_self/eval_unit_list.html
+-rw-rw-rw-   0        0        0      947 2023-02-09 04:48:40.000000 django-ipghrms-perform-1.1/perform/templates/perform2_self/form.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:42.989880 django-ipghrms-perform-1.1/perform/templates/perform_eval_components/
+-rw-rw-rw-   0        0        0     4617 2023-02-17 00:21:22.000000 django-ipghrms-perform-1.1/perform/templates/perform_eval_components/behavior.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.073240 django-ipghrms-perform-1.1/perform/templates/perform_eval_components/evaluator/
+-rw-rw-rw-   0        0        0     4053 2023-02-17 01:03:16.000000 django-ipghrms-perform-1.1/perform/templates/perform_eval_components/evaluator/behavior.html
+-rw-rw-rw-   0        0        0      841 2023-02-16 13:35:38.000000 django-ipghrms-perform-1.1/perform/templates/perform_eval_components/evaluator/header.html
+-rw-rw-rw-   0        0        0     5699 2023-02-19 07:08:40.000000 django-ipghrms-perform-1.1/perform/templates/perform_eval_components/evaluator/individual.html
+-rw-rw-rw-   0        0        0      549 2023-02-17 15:06:43.000000 django-ipghrms-perform-1.1/perform/templates/perform_eval_components/evaluator/objectives.html
+-rw-rw-rw-   0        0        0      841 2023-02-16 13:35:38.000000 django-ipghrms-perform-1.1/perform/templates/perform_eval_components/header.html
+-rw-rw-rw-   0        0        0     5498 2023-02-18 09:36:29.000000 django-ipghrms-perform-1.1/perform/templates/perform_eval_components/individual.html
+-rw-rw-rw-   0        0        0      549 2023-02-17 14:35:48.000000 django-ipghrms-perform-1.1/perform/templates/perform_eval_components/objectives.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.126955 django-ipghrms-perform-1.1/perform/templates/perform_plan_components/
+-rw-rw-rw-   0        0        0     4617 2023-02-17 00:21:22.000000 django-ipghrms-perform-1.1/perform/templates/perform_plan_components/behavior.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.179581 django-ipghrms-perform-1.1/perform/templates/perform_plan_components/evaluator/
+-rw-rw-rw-   0        0        0     4960 2023-02-19 07:18:34.000000 django-ipghrms-perform-1.1/perform/templates/perform_plan_components/evaluator/behavior.html
+-rw-rw-rw-   0        0        0      841 2023-02-16 13:35:38.000000 django-ipghrms-perform-1.1/perform/templates/perform_plan_components/evaluator/header.html
+-rw-rw-rw-   0        0        0     4569 2023-02-19 08:51:00.000000 django-ipghrms-perform-1.1/perform/templates/perform_plan_components/evaluator/individual.html
+-rw-rw-rw-   0        0        0      567 2023-02-17 00:48:26.000000 django-ipghrms-perform-1.1/perform/templates/perform_plan_components/evaluator/objectives.html
+-rw-rw-rw-   0        0        0      841 2023-02-16 13:35:38.000000 django-ipghrms-perform-1.1/perform/templates/perform_plan_components/header.html
+-rw-rw-rw-   0        0        0     3781 2023-02-17 02:58:02.000000 django-ipghrms-perform-1.1/perform/templates/perform_plan_components/individual.html
+-rw-rw-rw-   0        0        0     1504 2023-02-16 16:46:35.000000 django-ipghrms-perform-1.1/perform/templates/perform_plan_components/objectives.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.225214 django-ipghrms-perform-1.1/perform/templates/perform_pre_ass_components/
+-rw-rw-rw-   0        0        0     4617 2023-03-01 00:53:07.000000 django-ipghrms-perform-1.1/perform/templates/perform_pre_ass_components/behavior.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.251060 django-ipghrms-perform-1.1/perform/templates/perform_pre_ass_components/evaluator/
+-rw-rw-rw-   0        0        0      458 2023-02-17 13:50:00.000000 django-ipghrms-perform-1.1/perform/templates/perform_pre_ass_components/evaluator/header.html
+-rw-rw-rw-   0        0        0     4795 2023-02-18 07:58:17.000000 django-ipghrms-perform-1.1/perform/templates/perform_pre_ass_components/evaluator/individual.html
+-rw-rw-rw-   0        0        0      458 2023-02-17 02:52:56.000000 django-ipghrms-perform-1.1/perform/templates/perform_pre_ass_components/header.html
+-rw-rw-rw-   0        0        0     3650 2023-02-18 10:06:01.000000 django-ipghrms-perform-1.1/perform/templates/perform_pre_ass_components/individual.html
+-rw-rw-rw-   0        0        0     1504 2023-02-17 07:51:20.000000 django-ipghrms-perform-1.1/perform/templates/perform_pre_ass_components/objectives.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.297250 django-ipghrms-perform-1.1/perform/templates/perform_self_eval/
+-rw-rw-rw-   0        0        0     4617 2023-02-17 00:21:22.000000 django-ipghrms-perform-1.1/perform/templates/perform_self_eval/behavior.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.313602 django-ipghrms-perform-1.1/perform/templates/perform_self_eval/evaluator/
+-rw-rw-rw-   0        0        0      458 2023-02-18 08:36:46.000000 django-ipghrms-perform-1.1/perform/templates/perform_self_eval/evaluator/header.html
+-rw-rw-rw-   0        0        0     3754 2023-02-19 08:49:18.000000 django-ipghrms-perform-1.1/perform/templates/perform_self_eval/evaluator/individual.html
+-rw-rw-rw-   0        0        0      458 2023-02-17 12:33:37.000000 django-ipghrms-perform-1.1/perform/templates/perform_self_eval/header.html
+-rw-rw-rw-   0        0        0     3783 2023-02-19 07:36:13.000000 django-ipghrms-perform-1.1/perform/templates/perform_self_eval/individual.html
+-rw-rw-rw-   0        0        0     1518 2023-02-19 07:36:43.000000 django-ipghrms-perform-1.1/perform/templates/perform_self_eval/objectives.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.393093 django-ipghrms-perform-1.1/perform/templates/perform_staff/
+-rw-rw-rw-   0        0        0    17143 2023-03-01 01:07:34.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff/eval_detail.html
+-rw-rw-rw-   0        0        0     5308 2023-03-01 04:46:25.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff/list.html
+-rw-rw-rw-   0        0        0    12658 2023-02-19 05:40:13.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff/plan_detail.html
+-rw-rw-rw-   0        0        0    10322 2023-03-01 01:11:43.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff/preass_detail.html
+-rw-rw-rw-   0        0        0    13547 2023-03-01 01:07:51.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff/self_detail.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:41.550783 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.423840 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/eval/
+-rw-rw-rw-   0        0        0      841 2023-02-16 13:35:38.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/eval/header.html
+-rw-rw-rw-   0        0        0     5498 2023-02-18 09:36:29.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/eval/individual.html
+-rw-rw-rw-   0        0        0      549 2023-02-17 14:35:48.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/eval/objectives.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.454675 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/planning/
+-rw-rw-rw-   0        0        0      841 2023-02-16 13:35:38.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/planning/header.html
+-rw-rw-rw-   0        0        0     3793 2023-02-19 07:31:16.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/planning/individual.html
+-rw-rw-rw-   0        0        0     1504 2023-02-16 16:46:35.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/planning/objectives.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.472776 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/preass/
+-rw-rw-rw-   0        0        0      458 2023-02-17 02:52:56.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/preass/header.html
+-rw-rw-rw-   0        0        0     3650 2023-02-19 06:26:40.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/preass/individual.html
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.492896 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/self/
+-rw-rw-rw-   0        0        0      458 2023-02-17 12:33:37.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/self/header.html
+-rw-rw-rw-   0        0        0     3664 2023-03-01 01:08:26.000000 django-ipghrms-perform-1.1/perform/templates/perform_staff_components/self/individual.html
+-rw-rw-rw-   0        0        0       63 2022-12-03 02:55:42.000000 django-ipghrms-perform-1.1/perform/tests.py
+-rw-rw-rw-   0        0        0    10691 2023-03-07 06:00:15.000000 django-ipghrms-perform-1.1/perform/urls.py
+-rw-rw-rw-   0        0        0      325 2022-10-18 10:39:31.000000 django-ipghrms-perform-1.1/perform/utils.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.610532 django-ipghrms-perform-1.1/perform/views/
+-rw-rw-rw-   0        0        0      348 2023-02-19 05:20:47.000000 django-ipghrms-perform-1.1/perform/views/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-10 06:04:43.928374 django-ipghrms-perform-1.1/perform/views/__pycache__/
+-rw-rw-rw-   0        0        0      435 2023-02-19 05:21:06.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      339 2022-12-04 12:46:06.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     5705 2023-03-12 11:09:36.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/all_perform_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3924 2022-12-06 12:02:56.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/all_perform_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0     8085 2023-02-19 07:03:35.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/c_perform_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5773 2022-12-04 12:44:38.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/c_perform_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4314 2023-02-16 12:19:25.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/c_perform_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4287 2022-12-06 01:41:52.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/c_perform_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3794 2022-12-04 06:02:42.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/emp_perform_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1764 2022-12-04 05:57:38.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/emp_perform_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4188 2022-12-04 12:30:40.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/hr_perform_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0      145 2023-02-16 10:07:51.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/perfom_conf_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     8380 2023-02-27 01:22:43.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/perfom_plan.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4923 2023-02-19 05:55:59.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/perform_conf.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3628 2022-12-04 04:13:52.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/perform_conf.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2307 2023-02-16 14:53:48.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/perform_conf_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6535 2023-03-07 05:57:39.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/perform_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5048 2022-12-04 12:59:04.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/perform_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0     7332 2023-03-01 00:56:06.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/perform_pre_ass.cpython-310.pyc
+-rw-rw-rw-   0        0        0      141 2022-12-11 11:32:30.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/perform_r.cpython-310.pyc
+-rw-rw-rw-   0        0        0      146 2022-12-03 10:56:26.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/perform_r.cpython-39.pyc
+-rw-rw-rw-   0        0        0     3421 2023-03-01 01:11:28.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/perform_staff.cpython-310.pyc
+-rw-rw-rw-   0        0        0     7887 2023-02-27 01:13:02.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/self_perform_m.cpython-310.pyc
+-rw-rw-rw-   0        0        0     4329 2022-12-10 23:47:32.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/self_perform_m.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4398 2023-02-18 08:39:27.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/self_perform_v.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3881 2022-12-11 00:15:20.000000 django-ipghrms-perform-1.1/perform/views/__pycache__/self_perform_v.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6864 2023-03-12 11:09:33.000000 django-ipghrms-perform-1.1/perform/views/all_perform_v.py
+-rw-rw-rw-   0        0        0    11254 2023-02-19 07:03:31.000000 django-ipghrms-perform-1.1/perform/views/c_perform_m.py
+-rw-rw-rw-   0        0        0     4935 2023-02-16 12:19:21.000000 django-ipghrms-perform-1.1/perform/views/c_perform_v.py
+-rw-rw-rw-   0        0        0    14059 2023-02-27 01:22:40.000000 django-ipghrms-perform-1.1/perform/views/perfom_plan.py
+-rw-rw-rw-   0        0        0     5927 2023-02-19 05:55:55.000000 django-ipghrms-perform-1.1/perform/views/perform_conf.py
+-rw-rw-rw-   0        0        0     3173 2023-04-10 03:02:36.000000 django-ipghrms-perform-1.1/perform/views/perform_conf_m.py
+-rw-rw-rw-   0        0        0    12285 2023-03-07 05:57:36.000000 django-ipghrms-perform-1.1/perform/views/perform_m.py
+-rw-rw-rw-   0        0        0    16284 2023-03-01 00:56:01.000000 django-ipghrms-perform-1.1/perform/views/perform_pre_ass.py
+-rw-rw-rw-   0        0        0        0 2022-12-03 02:58:48.000000 django-ipghrms-perform-1.1/perform/views/perform_r.py
+-rw-rw-rw-   0        0        0     4403 2023-03-01 01:11:24.000000 django-ipghrms-perform-1.1/perform/views/perform_staff.py
+-rw-rw-rw-   0        0        0    11451 2023-02-27 01:13:00.000000 django-ipghrms-perform-1.1/perform/views/self_perform_m.py
+-rw-rw-rw-   0        0        0     6075 2023-02-18 08:39:26.000000 django-ipghrms-perform-1.1/perform/views/self_perform_v.py
+-rw-rw-rw-   0        0        0       66 2022-12-03 02:55:42.000000 django-ipghrms-perform-1.1/perform/views.py
+-rw-rw-rw-   0        0        0      509 2023-04-10 06:04:43.941057 django-ipghrms-perform-1.1/setup.cfg
+-rw-rw-rw-   0        0        0       39 2023-03-22 07:44:49.000000 django-ipghrms-perform-1.1/setup.py
```

### Comparing `django-ipghrms-perform-1.0/LICENSE` & `django-ipghrms-perform-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/PKG-INFO` & `django-ipghrms-perform-1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-perform
-Version: 1.0
+Version: 1.1
 Summary: Django IPG HRMS APP PERFORM
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-perform-1.0/django_ipghrms_perform.egg-info/PKG-INFO` & `django-ipghrms-perform-1.1/django_ipghrms_perform.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ipghrms-perform
-Version: 1.0
+Version: 1.1
 Summary: Django IPG HRMS APP PERFORM
 Home-page: http://ipg.tl/
 Author: Kinos
 Author-email: info@kinos.tl
 Maintainer: kinos
 Maintainer-email: info@kinos.tl
 License: MIT
```

### Comparing `django-ipghrms-perform-1.0/django_ipghrms_perform.egg-info/SOURCES.txt` & `django-ipghrms-perform-1.1/django_ipghrms_perform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/admin.py` & `django-ipghrms-perform-1.1/perform/admin.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/forms.py` & `django-ipghrms-perform-1.1/perform/forms.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0001_initial.py` & `django-ipghrms-perform-1.1/perform/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0002_evalchoiceplanning_evalplanning.py` & `django-ipghrms-perform-1.1/perform/migrations/0002_evalchoiceplanning_evalplanning.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0003_evalplanninga_evalplanningb.py` & `django-ipghrms-perform-1.1/perform/migrations/0003_evalplanninga_evalplanningb.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0006_evalplanninga_usereval.py` & `django-ipghrms-perform-1.1/perform/migrations/0006_evalplanninga_usereval.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0007_auto_20230217_0014.py` & `django-ipghrms-perform-1.1/perform/migrations/0007_auto_20230217_0014.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0008_evalpreassessment_evalpreassessmenta_evalpreassessmentb.py` & `django-ipghrms-perform-1.1/perform/migrations/0008_evalpreassessment_evalpreassessmenta_evalpreassessmentb.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0009_auto_20230217_1813.py` & `django-ipghrms-perform-1.1/perform/migrations/0009_auto_20230217_1813.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0010_auto_20230217_2302.py` & `django-ipghrms-perform-1.1/perform/migrations/0010_auto_20230217_2302.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0012_auto_20230218_1538.py` & `django-ipghrms-perform-1.1/perform/migrations/0012_auto_20230218_1538.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0013_auto_20230218_1557.py` & `django-ipghrms-perform-1.1/perform/migrations/0013_auto_20230218_1557.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0014_auto_20230218_1645.py` & `django-ipghrms-perform-1.1/perform/migrations/0014_auto_20230218_1645.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0016_auto_20230218_1718.py` & `django-ipghrms-perform-1.1/perform/migrations/0016_auto_20230218_1718.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0017_auto_20230218_1719.py` & `django-ipghrms-perform-1.1/perform/migrations/0017_auto_20230218_1719.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0018_auto_20230218_1827.py` & `django-ipghrms-perform-1.1/perform/migrations/0018_auto_20230218_1827.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0019_auto_20230307_0950.py` & `django-ipghrms-perform-1.1/perform/migrations/0019_auto_20230307_0950.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0020_auto_20230307_1026.py` & `django-ipghrms-perform-1.1/perform/migrations/0020_auto_20230307_1026.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0021_auto_20230307_1027.py` & `django-ipghrms-perform-1.1/perform/migrations/0021_auto_20230307_1027.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/0022_auto_20230310_0923.py` & `django-ipghrms-perform-1.1/perform/migrations/0022_auto_20230310_0923.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0001_initial.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0001_initial.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0002_evalchoiceplanning_evalplanning.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0002_evalchoiceplanning_evalplanning.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0003_evalplanninga_evalplanningb.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0003_evalplanninga_evalplanningb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0004_evalplanninga_eval_date.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0004_evalplanninga_eval_date.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0005_evalplanninga_enter_date.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0005_evalplanninga_enter_date.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0006_evalplanninga_usereval.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0006_evalplanninga_usereval.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0007_auto_20230217_0014.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0007_auto_20230217_0014.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0008_evalpreassessment_evalpreassessmenta_evalpreassessmentb.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0008_evalpreassessment_evalpreassessmenta_evalpreassessmentb.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0009_auto_20230217_1813.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0009_auto_20230217_1813.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0010_auto_20230217_2302.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0010_auto_20230217_2302.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0011_evalplanning_date.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0011_evalplanning_date.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0012_auto_20230218_1538.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0012_auto_20230218_1538.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0013_auto_20230218_1557.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0013_auto_20230218_1557.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0014_auto_20230218_1645.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0014_auto_20230218_1645.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0015_rename_eval_obj_date_evalpreassessment_eval_beh_date.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0015_rename_eval_obj_date_evalpreassessment_eval_beh_date.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0016_auto_20230218_1718.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0016_auto_20230218_1718.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0017_auto_20230218_1719.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0017_auto_20230218_1719.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0018_auto_20230218_1827.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0018_auto_20230218_1827.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0019_auto_20230307_0950.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0019_auto_20230307_0950.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0020_auto_20230307_1026.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0020_auto_20230307_1026.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0021_auto_20230307_1027.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0021_auto_20230307_1027.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0022_auto_20230310_0923.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0022_auto_20230310_0923.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0023_rename_year_evalmonth_month.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0023_rename_year_evalmonth_month.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0024_remove_evaltype_month.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0024_remove_evaltype_month.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/migrations/__pycache__/0025_evalplanning_month.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/migrations/__pycache__/0025_evalplanning_month.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/models.py` & `django-ipghrms-perform-1.1/perform/models.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/all_eval_cat_list.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/all_eval_cat_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/all_eval_dash.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/all_eval_dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/all_eval_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/all_eval_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/all_eval_list.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/all_eval_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/all_eval_year_list.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/all_eval_year_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/behavior_list.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/behavior_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/c_eval_cat_list.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/c_eval_cat_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/c_eval_dash.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/c_eval_dash.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/c_eval_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/c_eval_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/c_eval_list.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/c_eval_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/c_eval_year_list.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/c_eval_year_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/eval_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/eval_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/evaluator_eval_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/evaluator_eval_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/evaluator_plan_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/evaluator_plan_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/evaluator_preass_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/evaluator_preass_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/evaluator_self_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/evaluator_self_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/form.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/form_det.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/form_det.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/form_eval.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/form_eval.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/plan_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/plan_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/pre_ass_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/pre_ass_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2/self_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform2/self_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2_conf/cat_score.html` & `django-ipghrms-perform-1.1/perform/templates/perform2_conf/cat_score.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2_conf/conf_dash.html` & `django-ipghrms-perform-1.1/perform/templates/perform2_conf/conf_dash.html`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                                         <tr align="center">
                                             <td>{{forloop.counter}}</td>
                                             <td class="text-left">{{obj.0}}</td>
                                             <td>
                                                 {% if obj.1 %}
                                                   <a href="{% url 'eval-conf-plan-detail' obj.1.hashed %}" class="btn btn-sm btn-info">Hare <i class="fa fa-eye"></i></a>
                                                   {% if obj.1.is_lock == False %}                                                
-                                                      <a href="{% url 'eval-conf-plan-detail' obj.1.hashed %}" class="btn btn-sm btn-warning">Delete <i class="fa fa-trash"></i></a>
+                                                      <!-- <a href="{% url 'eval-conf-plan-detail' obj.1.hashed %}" class="btn btn-sm btn-warning">Delete <i class="fa fa-trash"></i></a> -->
                                                   {% endif %}
                                                 {% else %}
                                                   <a href="{% url 'eval-conf-add-plan' obj.0.hashed ayear %}" class="btn btn-sm btn-danger">Kria <i class="fa fa-plus"></i></a>
                                                 {% endif %}
                                             </td>
                                             <td>
                                                 {% if obj.3 and not obj.2 %}
```

#### html2text {}

```diff
@@ -10,22 +10,22 @@
                                                 All_Behaviors
                                         LISTA FUNSIONARIO & AVALIASAUN
                              Planning &        Pre-          Self-
            Nu.       Staff  Monitoring      Assessment    Evaluation    Evaluation
                               Add_All
                                            {% if obj.3   {% if obj.3   {% if obj.3
                                           and not obj.2 and not obj.4 and not obj.5
-                             {% if obj.1       %}            %}            %}
-                                 %}           Kria          Kria          Kria
-                                Hare         {% elif       {% elif       {% elif
-                                {% if       obj.3 and     obj.3 and     obj.3 and
-                            obj.1.is_lock   obj.2 %}      obj.4 %}      obj.5 %}
-        {             {     == False %}       Hare          Hare          Hare
-{forloop.counter}} {obj.0}}    Delete         {% if         {% if         {% if
-                             {% endif %}  obj.2.is_lock obj.4.is_lock obj.5.is_lock
+                                               %}            %}            %}
+                             {% if obj.1      Kria          Kria          Kria
+                                 %}          {% elif       {% elif       {% elif
+                                Hare        obj.3 and     obj.3 and     obj.3 and
+                                {% if       obj.2 %}      obj.4 %}      obj.5 %}
+        {             {     obj.1.is_lock     Hare          Hare          Hare
+{forloop.counter}} {obj.0}} == False %}       {% if         {% if         {% if
+                            {% endif %}   obj.2.is_lock obj.4.is_lock obj.5.is_lock
                              {% else %}   == False %}   == False %}   == False %}
                                 Kria      {% endif %}   {% endif %}   {% endif %}
                              {% endif %}   {% else %}    {% else %}    {% else %}
                                           Plano Seidauk Plano Seidauk Plano Seidauk
                                             kria  {%      kria  {%      kria  {%
                                             endif %}      endif %}      endif %}
 {% endblock %} {% block scripts %}
```

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2_conf/form.html` & `django-ipghrms-perform-1.1/perform/templates/perform2_conf/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2_self/all_eval_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform2_self/all_eval_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2_self/all_eval_list.html` & `django-ipghrms-perform-1.1/perform/templates/perform2_self/all_eval_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2_self/eval_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform2_self/eval_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2_self/eval_list.html` & `django-ipghrms-perform-1.1/perform/templates/perform2_self/eval_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2_self/eval_unit_list.html` & `django-ipghrms-perform-1.1/perform/templates/perform2_self/eval_unit_list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform2_self/form.html` & `django-ipghrms-perform-1.1/perform/templates/perform2_self/form.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_eval_components/behavior.html` & `django-ipghrms-perform-1.1/perform/templates/perform_eval_components/behavior.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_eval_components/evaluator/behavior.html` & `django-ipghrms-perform-1.1/perform/templates/perform_eval_components/evaluator/behavior.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_eval_components/evaluator/header.html` & `django-ipghrms-perform-1.1/perform/templates/perform_eval_components/evaluator/header.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_eval_components/evaluator/individual.html` & `django-ipghrms-perform-1.1/perform/templates/perform_eval_components/evaluator/individual.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_eval_components/evaluator/objectives.html` & `django-ipghrms-perform-1.1/perform/templates/perform_eval_components/evaluator/objectives.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_eval_components/header.html` & `django-ipghrms-perform-1.1/perform/templates/perform_eval_components/header.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_eval_components/individual.html` & `django-ipghrms-perform-1.1/perform/templates/perform_eval_components/individual.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_eval_components/objectives.html` & `django-ipghrms-perform-1.1/perform/templates/perform_eval_components/objectives.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_plan_components/behavior.html` & `django-ipghrms-perform-1.1/perform/templates/perform_plan_components/behavior.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_plan_components/evaluator/behavior.html` & `django-ipghrms-perform-1.1/perform/templates/perform_plan_components/evaluator/behavior.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_plan_components/evaluator/header.html` & `django-ipghrms-perform-1.1/perform/templates/perform_plan_components/evaluator/header.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_plan_components/evaluator/individual.html` & `django-ipghrms-perform-1.1/perform/templates/perform_plan_components/evaluator/individual.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_plan_components/evaluator/objectives.html` & `django-ipghrms-perform-1.1/perform/templates/perform_plan_components/evaluator/objectives.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_plan_components/header.html` & `django-ipghrms-perform-1.1/perform/templates/perform_plan_components/header.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_plan_components/individual.html` & `django-ipghrms-perform-1.1/perform/templates/perform_plan_components/individual.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_plan_components/objectives.html` & `django-ipghrms-perform-1.1/perform/templates/perform_plan_components/objectives.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_pre_ass_components/behavior.html` & `django-ipghrms-perform-1.1/perform/templates/perform_pre_ass_components/behavior.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_pre_ass_components/evaluator/individual.html` & `django-ipghrms-perform-1.1/perform/templates/perform_pre_ass_components/evaluator/individual.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_pre_ass_components/individual.html` & `django-ipghrms-perform-1.1/perform/templates/perform_pre_ass_components/individual.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_pre_ass_components/objectives.html` & `django-ipghrms-perform-1.1/perform/templates/perform_pre_ass_components/objectives.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_self_eval/behavior.html` & `django-ipghrms-perform-1.1/perform/templates/perform_self_eval/behavior.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_self_eval/evaluator/individual.html` & `django-ipghrms-perform-1.1/perform/templates/perform_self_eval/evaluator/individual.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_self_eval/individual.html` & `django-ipghrms-perform-1.1/perform/templates/perform_self_eval/individual.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_self_eval/objectives.html` & `django-ipghrms-perform-1.1/perform/templates/perform_self_eval/objectives.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_staff/eval_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform_staff/eval_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_staff/list.html` & `django-ipghrms-perform-1.1/perform/templates/perform_staff/list.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_staff/plan_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform_staff/plan_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_staff/preass_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform_staff/preass_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_staff/self_detail.html` & `django-ipghrms-perform-1.1/perform/templates/perform_staff/self_detail.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_staff_components/eval/header.html` & `django-ipghrms-perform-1.1/perform/templates/perform_staff_components/eval/header.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_staff_components/eval/individual.html` & `django-ipghrms-perform-1.1/perform/templates/perform_staff_components/eval/individual.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_staff_components/eval/objectives.html` & `django-ipghrms-perform-1.1/perform/templates/perform_staff_components/eval/objectives.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_staff_components/planning/header.html` & `django-ipghrms-perform-1.1/perform/templates/perform_staff_components/planning/header.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_staff_components/planning/individual.html` & `django-ipghrms-perform-1.1/perform/templates/perform_staff_components/planning/individual.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_staff_components/planning/objectives.html` & `django-ipghrms-perform-1.1/perform/templates/perform_staff_components/planning/objectives.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_staff_components/preass/individual.html` & `django-ipghrms-perform-1.1/perform/templates/perform_staff_components/preass/individual.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/templates/perform_staff_components/self/individual.html` & `django-ipghrms-perform-1.1/perform/templates/perform_staff_components/self/individual.html`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/urls.py` & `django-ipghrms-perform-1.1/perform/urls.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/all_perform_v.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/all_perform_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/all_perform_v.cpython-39.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/all_perform_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/c_perform_m.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/c_perform_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/c_perform_m.cpython-39.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/c_perform_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/c_perform_v.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/c_perform_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/c_perform_v.cpython-39.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/c_perform_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/emp_perform_m.cpython-39.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/emp_perform_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/emp_perform_v.cpython-39.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/emp_perform_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/hr_perform_v.cpython-39.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/hr_perform_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/perfom_plan.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/perfom_plan.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/perform_conf.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/perform_conf.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/perform_conf.cpython-39.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/perform_conf.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/perform_conf_m.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/perform_conf_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/perform_m.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/perform_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/perform_m.cpython-39.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/perform_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/perform_pre_ass.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/perform_pre_ass.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/perform_staff.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/perform_staff.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/self_perform_m.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/self_perform_m.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/self_perform_m.cpython-39.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/self_perform_m.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/self_perform_v.cpython-310.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/self_perform_v.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/__pycache__/self_perform_v.cpython-39.pyc` & `django-ipghrms-perform-1.1/perform/views/__pycache__/self_perform_v.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/all_perform_v.py` & `django-ipghrms-perform-1.1/perform/views/all_perform_v.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/c_perform_m.py` & `django-ipghrms-perform-1.1/perform/views/c_perform_m.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/c_perform_v.py` & `django-ipghrms-perform-1.1/perform/views/c_perform_v.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/perfom_plan.py` & `django-ipghrms-perform-1.1/perform/views/perfom_plan.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/perform_conf.py` & `django-ipghrms-perform-1.1/perform/views/perform_conf.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/perform_conf_m.py` & `django-ipghrms-perform-1.1/perform/views/perform_conf_m.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,51 +16,62 @@
 @login_required
 @allowed_users(allowed_roles=['admin','hr'])
 def PerfomConfAddPlan(request, hashid, year):
     employee = get_object_or_404(Employee, hashed=hashid)
     pyear = get_object_or_404(EvalYear, year=year)
     ptype = get_object_or_404(EvalType, pk=1)
     contract = Contract.objects.filter(employee=employee, is_active=True).last()
-    empdiv = CurEmpDivision.objects.filter(employee=employee).last()
-    newid, new_hashid = getnewid(EvalPlanning)
-    obj = EvalPlanning(
-        id = newid,
-        hashed= new_hashid,
-        year = pyear,
-        type = ptype,
-        employee = employee,
-        category = contract.category,
-        position = contract.position,
-        department = empdiv.department,
-        unit = empdiv.unit
-    )
-    obj.save()
-    messages.success(request, 'Susesu Kria Planning and Monitoring Sheet')
-    return redirect('eval-conf-dash')
+    if contract:
+        empdiv = CurEmpDivision.objects.filter(employee=employee).last()
+        newid, new_hashid = getnewid(EvalPlanning)
+        obj = EvalPlanning(
+            id = newid,
+            hashed= new_hashid,
+            year = pyear,
+            type = ptype,
+            employee = employee,
+            category = contract.category,
+            position = contract.position,
+            department = empdiv.department,
+            unit = empdiv.unit
+        )
+        obj.save()
+        messages.success(request, 'Susesu Kria Planning and Monitoring Sheet')
+        return redirect('eval-conf-dash')
+    else:
+        messages.error(request, 'Funsionario Seidauk Iha Kontrato')
+        return redirect('eval-conf-dash')
+
 
 @login_required
 @allowed_users(allowed_roles=['admin','hr'])
 def PerfomConfAddPlanAll(request, year):
     pyear = get_object_or_404(EvalYear, year=year)
     ptype = get_object_or_404(EvalType, pk=1)
     employees = Employee.objects.filter(status_id=1).exclude(curempdivision__de__pk=1)
     for emp in employees:
         check_emp_plan = EvalPlanning.objects.filter(employee=emp, year=pyear).last()
         if not check_emp_plan:
             contract = Contract.objects.filter(employee=emp, is_active=True).last()
-            empdiv = CurEmpDivision.objects.filter(employee=emp).last()
-            newid, new_hashid = getnewid(EvalPlanning)
-            obj = EvalPlanning(
-                id = newid,
-                hashed= new_hashid,
-                year = pyear,
-                type = ptype,
-                employee = emp,
-                category = contract.category,
-                position = contract.position,
-                department = empdiv.department,
-                unit = empdiv.unit
-            )
-            obj.save()
-    messages.success(request, 'Susesu Kria Planning and Monitoring Sheet')
-    return redirect('eval-conf-dash')
+            if contract:
+                empdiv = CurEmpDivision.objects.filter(employee=emp).last()
+                newid, new_hashid = getnewid(EvalPlanning)
+                obj = EvalPlanning(
+                    id = newid,
+                    hashed= new_hashid,
+                    year = pyear,
+                    type = ptype,
+                    employee = emp,
+                    category = contract.category,
+                    position = contract.position,
+                    department = empdiv.department,
+                    unit = empdiv.unit
+                )
+                obj.save()
+                messages.success(request, 'Susesu Kria Planning and Monitoring Sheet')
+                return redirect('eval-conf-dash')
+            else:
+                messages.error(request, f'Funsionario {emp} Seidauk Iha Kontrato')
+                return redirect('eval-conf-dash')
+
+
```

### Comparing `django-ipghrms-perform-1.0/perform/views/perform_m.py` & `django-ipghrms-perform-1.1/perform/views/perform_m.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/perform_pre_ass.py` & `django-ipghrms-perform-1.1/perform/views/perform_pre_ass.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/perform_staff.py` & `django-ipghrms-perform-1.1/perform/views/perform_staff.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/self_perform_m.py` & `django-ipghrms-perform-1.1/perform/views/self_perform_m.py`

 * *Files identical despite different names*

### Comparing `django-ipghrms-perform-1.0/perform/views/self_perform_v.py` & `django-ipghrms-perform-1.1/perform/views/self_perform_v.py`

 * *Files identical despite different names*

