# Comparing `tmp/pyecharts-2.0.2.tar.gz` & `tmp/pyecharts-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyecharts-2.0.2.tar", last modified: Tue Feb 28 01:49:49 2023, max compression
+gzip compressed data, was "dist/pyecharts-2.0.3.tar", last modified: Mon Apr 10 01:17:02 2023, max compression
```

## Comparing `pyecharts-2.0.2.tar` & `pyecharts-2.0.3.tar`

### file list

```diff
@@ -1,163 +1,164 @@
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/
--rw-r--r--   0 sunhailin   (501) staff       (20)      114 2019-07-16 15:15:19.000000 pyecharts-2.0.2/MANIFEST.in
--rw-r--r--   0 sunhailin   (501) staff       (20)     1030 2023-02-28 01:49:49.000000 pyecharts-2.0.2/PKG-INFO
--rw-r--r--   0 sunhailin   (501) staff       (20)    12418 2023-01-05 07:14:05.000000 pyecharts-2.0.2/README.md
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/pyecharts/
--rw-r--r--   0 sunhailin   (501) staff       (20)      142 2019-07-16 15:15:19.000000 pyecharts-2.0.2/pyecharts/__init__.py
--rw-r--r--   0 sunhailin   (501) staff       (20)       53 2023-02-28 01:49:20.000000 pyecharts-2.0.2/pyecharts/_version.py
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/pyecharts/charts/
--rw-r--r--   0 sunhailin   (501) staff       (20)     2027 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/__init__.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     4178 2023-02-20 06:20:33.000000 pyecharts-2.0.2/pyecharts/charts/base.py
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/
--rw-r--r--   0 sunhailin   (501) staff       (20)        0 2019-07-16 15:15:19.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/__init__.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     3780 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/bar.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     3043 2021-02-08 05:10:57.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/bmap.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2845 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/boxplot.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1933 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/calendar.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2350 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/custom.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1965 2020-10-29 15:11:51.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/effectscatter.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1865 2020-10-29 15:11:51.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/funnel.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2544 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/gauge.py
--rw-r--r--   0 sunhailin   (501) staff       (20)    10481 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/geo.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     3279 2023-02-28 01:49:20.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/graph.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1797 2020-10-29 15:11:51.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/heatmap.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1905 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/kline.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     3364 2023-02-28 01:49:20.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/line.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2129 2020-07-06 08:57:41.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/liquid.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     3360 2023-01-05 06:35:40.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/map.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1942 2020-10-29 15:11:51.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/parallel.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2800 2020-06-07 15:18:09.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/pictorialbar.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     3736 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/pie.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     4390 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/polar.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     3183 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/radar.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2453 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/sankey.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2914 2020-07-06 08:57:41.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/scatter.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1628 2019-07-16 15:15:19.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/sunburst.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1307 2020-06-07 15:18:09.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/themeriver.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     3080 2020-06-07 15:18:09.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/tree.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     3323 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/treemap.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     4940 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/basic_charts/wordcloud.py
--rw-r--r--   0 sunhailin   (501) staff       (20)    15099 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/chart.py
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/pyecharts/charts/composite_charts/
--rw-r--r--   0 sunhailin   (501) staff       (20)        0 2019-07-16 15:15:19.000000 pyecharts-2.0.2/pyecharts/charts/composite_charts/__init__.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     3560 2023-02-28 01:49:20.000000 pyecharts-2.0.2/pyecharts/charts/composite_charts/grid.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     7099 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/composite_charts/page.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     4926 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/composite_charts/tab.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     5085 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/composite_charts/timeline.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      415 2019-10-10 01:57:06.000000 pyecharts-2.0.2/pyecharts/charts/mixins.py
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/pyecharts/charts/three_axis_charts/
--rw-r--r--   0 sunhailin   (501) staff       (20)        0 2019-10-10 01:57:06.000000 pyecharts-2.0.2/pyecharts/charts/three_axis_charts/__init__.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      345 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/three_axis_charts/bar3D.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1507 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/three_axis_charts/graph_gl.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      348 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/three_axis_charts/line3D.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2215 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/three_axis_charts/lines3D.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     9944 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/three_axis_charts/map3D.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1535 2019-10-10 01:57:06.000000 pyecharts-2.0.2/pyecharts/charts/three_axis_charts/map_globe.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      357 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/three_axis_charts/scatter3D.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      387 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/charts/three_axis_charts/surface3D.py
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/pyecharts/commons/
--rw-r--r--   0 sunhailin   (501) staff       (20)        0 2019-07-16 15:15:19.000000 pyecharts-2.0.2/pyecharts/commons/__init__.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2914 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/commons/utils.py
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/pyecharts/components/
--rw-r--r--   0 sunhailin   (501) staff       (20)       50 2019-07-16 15:15:19.000000 pyecharts-2.0.2/pyecharts/components/__init__.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1963 2019-10-10 01:57:06.000000 pyecharts-2.0.2/pyecharts/components/image.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2010 2020-03-11 07:42:19.000000 pyecharts-2.0.2/pyecharts/components/table.py
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/pyecharts/datasets/
--rw-r--r--   0 sunhailin   (501) staff       (20)     4643 2019-10-10 01:57:06.000000 pyecharts-2.0.2/pyecharts/datasets/__init__.py
--rw-r--r--   0 sunhailin   (501) staff       (20)   179739 2019-10-10 01:57:06.000000 pyecharts-2.0.2/pyecharts/datasets/city_coordinates.json
--rw-r--r--   0 sunhailin   (501) staff       (20)     5627 2019-07-16 15:15:19.000000 pyecharts-2.0.2/pyecharts/datasets/countries_regions_db.json
--rw-r--r--   0 sunhailin   (501) staff       (20)    32648 2020-07-06 08:57:41.000000 pyecharts-2.0.2/pyecharts/datasets/map_filename.json
--rw-r--r--   0 sunhailin   (501) staff       (20)      529 2020-02-28 05:16:31.000000 pyecharts-2.0.2/pyecharts/exceptions.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     9935 2023-01-05 07:14:05.000000 pyecharts-2.0.2/pyecharts/faker.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     3875 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/globals.py
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/pyecharts/options/
--rw-r--r--   0 sunhailin   (501) staff       (20)     2687 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/options/__init__.py
--rw-r--r--   0 sunhailin   (501) staff       (20)    47198 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/options/charts_options.py
--rw-r--r--   0 sunhailin   (501) staff       (20)    51292 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/options/global_options.py
--rw-r--r--   0 sunhailin   (501) staff       (20)    14324 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/options/series_options.py
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/pyecharts/render/
--rw-r--r--   0 sunhailin   (501) staff       (20)       36 2019-07-16 15:15:19.000000 pyecharts-2.0.2/pyecharts/render/__init__.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1476 2020-06-07 15:18:09.000000 pyecharts-2.0.2/pyecharts/render/display.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     4136 2022-12-24 03:11:40.000000 pyecharts-2.0.2/pyecharts/render/engine.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2654 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/render/snapshot.py
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/pyecharts/render/templates/
--rw-r--r--   0 sunhailin   (501) staff       (20)      217 2019-10-10 01:57:06.000000 pyecharts-2.0.2/pyecharts/render/templates/components.html
--rw-r--r--   0 sunhailin   (501) staff       (20)     8211 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/render/templates/macro
--rw-r--r--   0 sunhailin   (501) staff       (20)      121 2019-10-10 01:57:06.000000 pyecharts-2.0.2/pyecharts/render/templates/nb_components.html
--rw-r--r--   0 sunhailin   (501) staff       (20)     1436 2019-10-10 01:57:06.000000 pyecharts-2.0.2/pyecharts/render/templates/nb_jupyter_globe.html
--rw-r--r--   0 sunhailin   (501) staff       (20)      359 2019-10-10 01:57:06.000000 pyecharts-2.0.2/pyecharts/render/templates/nb_jupyter_lab.html
--rw-r--r--   0 sunhailin   (501) staff       (20)      458 2019-10-10 01:57:06.000000 pyecharts-2.0.2/pyecharts/render/templates/nb_jupyter_lab_tab.html
--rw-r--r--   0 sunhailin   (501) staff       (20)      489 2019-10-10 01:57:06.000000 pyecharts-2.0.2/pyecharts/render/templates/nb_jupyter_notebook.html
--rw-r--r--   0 sunhailin   (501) staff       (20)      608 2019-10-10 01:57:06.000000 pyecharts-2.0.2/pyecharts/render/templates/nb_jupyter_notebook_tab.html
--rw-r--r--   0 sunhailin   (501) staff       (20)      253 2019-10-10 01:57:06.000000 pyecharts-2.0.2/pyecharts/render/templates/nb_nteract.html
--rw-r--r--   0 sunhailin   (501) staff       (20)      333 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/render/templates/simple_chart.html
--rw-r--r--   0 sunhailin   (501) staff       (20)     1438 2019-07-16 15:15:19.000000 pyecharts-2.0.2/pyecharts/render/templates/simple_globe.html
--rw-r--r--   0 sunhailin   (501) staff       (20)     1074 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/render/templates/simple_page.html
--rw-r--r--   0 sunhailin   (501) staff       (20)      993 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/render/templates/simple_tab.html
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/pyecharts/scaffold/
--rw-r--r--   0 sunhailin   (501) staff       (20)        0 2019-07-16 15:15:19.000000 pyecharts-2.0.2/pyecharts/scaffold/__init__.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     4585 2023-01-03 07:51:04.000000 pyecharts-2.0.2/pyecharts/types.py
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/pyecharts.egg-info/
--rw-r--r--   0 sunhailin   (501) staff       (20)     1030 2023-02-28 01:49:48.000000 pyecharts-2.0.2/pyecharts.egg-info/PKG-INFO
--rw-r--r--   0 sunhailin   (501) staff       (20)     4533 2023-02-28 01:49:48.000000 pyecharts-2.0.2/pyecharts.egg-info/SOURCES.txt
--rw-r--r--   0 sunhailin   (501) staff       (20)        1 2023-02-28 01:49:48.000000 pyecharts-2.0.2/pyecharts.egg-info/dependency_links.txt
--rw-r--r--   0 sunhailin   (501) staff       (20)        1 2023-02-28 01:49:48.000000 pyecharts-2.0.2/pyecharts.egg-info/not-zip-safe
--rw-r--r--   0 sunhailin   (501) staff       (20)      138 2023-02-28 01:49:48.000000 pyecharts-2.0.2/pyecharts.egg-info/requires.txt
--rw-r--r--   0 sunhailin   (501) staff       (20)       10 2023-02-28 01:49:48.000000 pyecharts-2.0.2/pyecharts.egg-info/top_level.txt
--rw-r--r--   0 sunhailin   (501) staff       (20)       38 2023-02-28 01:49:49.000000 pyecharts-2.0.2/setup.cfg
--rw-r--r--   0 sunhailin   (501) staff       (20)     2976 2023-01-05 07:14:05.000000 pyecharts-2.0.2/setup.py
-drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-02-28 01:49:49.000000 pyecharts-2.0.2/test/
--rw-r--r--   0 sunhailin   (501) staff       (20)    11042 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_bar.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1980 2019-11-13 01:12:20.000000 pyecharts-2.0.2/test/test_bar3d.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1210 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_base.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     4885 2020-02-28 05:16:31.000000 pyecharts-2.0.2/test/test_bmap.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2293 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_boxplot.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2201 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_calendar.py
--rw-r--r--   0 sunhailin   (501) staff       (20)    10075 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_chart.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2723 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_chart_options.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1473 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_custom.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1473 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_datasets.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      689 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_display.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      957 2020-10-29 15:11:51.000000 pyecharts-2.0.2/test/test_effectscatter.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1882 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_exception.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      299 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_faker.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      998 2020-10-29 15:11:51.000000 pyecharts-2.0.2/test/test_funnel.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1165 2020-06-07 15:18:09.000000 pyecharts-2.0.2/test/test_gauge.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     5350 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_geo.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     9362 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_global_options.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     4575 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_graph.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1552 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_graphic.py
--rw-r--r--   0 sunhailin   (501) staff       (20)    11234 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_grid.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      675 2019-10-10 01:57:06.000000 pyecharts-2.0.2/test/test_heatmap.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1219 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_image.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      207 2019-10-10 01:57:06.000000 pyecharts-2.0.2/test/test_item_style_options.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2416 2020-10-29 15:11:51.000000 pyecharts-2.0.2/test/test_kline.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2691 2020-10-29 15:11:51.000000 pyecharts-2.0.2/test/test_line.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1136 2019-10-10 01:57:06.000000 pyecharts-2.0.2/test/test_line3d.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1647 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_lines3d.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1400 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_liquid.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1590 2020-10-29 15:11:51.000000 pyecharts-2.0.2/test/test_map.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     9702 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_map3d.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1483 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_map_globe.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      593 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_mixins.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     4882 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_page.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2887 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_parallel.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      734 2019-10-10 01:57:06.000000 pyecharts-2.0.2/test/test_pictorialbar.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2864 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_pie.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1744 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_polar.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     3381 2020-10-29 15:11:51.000000 pyecharts-2.0.2/test/test_radar.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2204 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_sankey.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     6474 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_scatter.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      721 2019-10-10 01:57:06.000000 pyecharts-2.0.2/test/test_scatter3d.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     3634 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_series_options.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2889 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_snapshot.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1837 2019-10-10 01:57:06.000000 pyecharts-2.0.2/test/test_sunburst.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1252 2019-10-10 01:57:06.000000 pyecharts-2.0.2/test/test_surface3d.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     2665 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_tab.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1540 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_table.py
--rw-r--r--   0 sunhailin   (501) staff       (20)      803 2019-10-10 01:57:06.000000 pyecharts-2.0.2/test/test_themeriver.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     5891 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_timeline.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1676 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_tree.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1709 2020-03-12 08:02:05.000000 pyecharts-2.0.2/test/test_treemap.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1250 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_utils.py
--rw-r--r--   0 sunhailin   (501) staff       (20)     1765 2023-01-03 07:51:04.000000 pyecharts-2.0.2/test/test_wordcloud.py
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/
+-rw-r--r--   0 sunhailin   (501) staff       (20)      114 2019-07-16 15:15:19.000000 pyecharts-2.0.3/MANIFEST.in
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1030 2023-04-10 01:17:02.000000 pyecharts-2.0.3/PKG-INFO
+-rw-r--r--   0 sunhailin   (501) staff       (20)    12418 2023-01-05 07:14:05.000000 pyecharts-2.0.3/README.md
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts/
+-rw-r--r--   0 sunhailin   (501) staff       (20)      142 2019-07-16 15:15:19.000000 pyecharts-2.0.3/pyecharts/__init__.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)       53 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/_version.py
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts/charts/
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2027 2023-01-03 07:51:04.000000 pyecharts-2.0.3/pyecharts/charts/__init__.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     4775 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/base.py
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/
+-rw-r--r--   0 sunhailin   (501) staff       (20)        0 2019-07-16 15:15:19.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/__init__.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3732 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/bar.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3127 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/bmap.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2918 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/boxplot.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1996 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/calendar.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2335 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/custom.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1917 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/effectscatter.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1804 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/funnel.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2496 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/gauge.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)    10629 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/geo.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3231 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/graph.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1857 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/heatmap.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1968 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/kline.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3711 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/line.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2240 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/liquid.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     4188 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/map.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2005 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/parallel.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2752 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/pictorialbar.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3736 2023-01-03 07:51:04.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/pie.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     4429 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/polar.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3120 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/radar.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2405 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/sankey.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2866 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/scatter.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1628 2019-07-16 15:15:19.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/sunburst.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1259 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/themeriver.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3080 2020-06-07 15:18:09.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/tree.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3276 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/treemap.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     5019 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/basic_charts/wordcloud.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)    15311 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/chart.py
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts/charts/composite_charts/
+-rw-r--r--   0 sunhailin   (501) staff       (20)        0 2019-07-16 15:15:19.000000 pyecharts-2.0.3/pyecharts/charts/composite_charts/__init__.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3824 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/composite_charts/grid.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     7099 2023-01-03 07:51:04.000000 pyecharts-2.0.3/pyecharts/charts/composite_charts/page.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     4927 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/composite_charts/tab.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     5164 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/composite_charts/timeline.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      415 2019-10-10 01:57:06.000000 pyecharts-2.0.3/pyecharts/charts/mixins.py
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts/charts/three_axis_charts/
+-rw-r--r--   0 sunhailin   (501) staff       (20)        0 2019-10-10 01:57:06.000000 pyecharts-2.0.3/pyecharts/charts/three_axis_charts/__init__.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      447 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/three_axis_charts/bar3D.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1609 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/three_axis_charts/graph_gl.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      450 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/three_axis_charts/line3D.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2317 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/three_axis_charts/lines3D.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     9999 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/three_axis_charts/map3D.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1637 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/three_axis_charts/map_globe.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      459 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/three_axis_charts/scatter3D.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      489 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/charts/three_axis_charts/surface3D.py
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts/commons/
+-rw-r--r--   0 sunhailin   (501) staff       (20)        0 2019-07-16 15:15:19.000000 pyecharts-2.0.3/pyecharts/commons/__init__.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2914 2023-03-16 06:15:14.000000 pyecharts-2.0.3/pyecharts/commons/utils.py
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts/components/
+-rw-r--r--   0 sunhailin   (501) staff       (20)       50 2019-07-16 15:15:19.000000 pyecharts-2.0.3/pyecharts/components/__init__.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1963 2019-10-10 01:57:06.000000 pyecharts-2.0.3/pyecharts/components/image.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2010 2020-03-11 07:42:19.000000 pyecharts-2.0.3/pyecharts/components/table.py
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts/datasets/
+-rw-r--r--   0 sunhailin   (501) staff       (20)     4643 2023-03-16 07:45:29.000000 pyecharts-2.0.3/pyecharts/datasets/__init__.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)   179739 2019-10-10 01:57:06.000000 pyecharts-2.0.3/pyecharts/datasets/city_coordinates.json
+-rw-r--r--   0 sunhailin   (501) staff       (20)     5627 2019-07-16 15:15:19.000000 pyecharts-2.0.3/pyecharts/datasets/countries_regions_db.json
+-rw-r--r--   0 sunhailin   (501) staff       (20)    32648 2020-07-06 08:57:41.000000 pyecharts-2.0.3/pyecharts/datasets/map_filename.json
+-rw-r--r--   0 sunhailin   (501) staff       (20)      529 2020-02-28 05:16:31.000000 pyecharts-2.0.3/pyecharts/exceptions.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     9935 2023-01-05 07:14:05.000000 pyecharts-2.0.3/pyecharts/faker.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3875 2023-01-03 07:51:04.000000 pyecharts-2.0.3/pyecharts/globals.py
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts/options/
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2704 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/options/__init__.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)    47198 2023-01-03 07:51:04.000000 pyecharts-2.0.3/pyecharts/options/charts_options.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)    51471 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/options/global_options.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)    14324 2023-01-03 07:51:04.000000 pyecharts-2.0.3/pyecharts/options/series_options.py
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts/render/
+-rw-r--r--   0 sunhailin   (501) staff       (20)       36 2019-07-16 15:15:19.000000 pyecharts-2.0.3/pyecharts/render/__init__.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2364 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/render/display.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     4137 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/render/engine.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2654 2023-01-03 07:51:04.000000 pyecharts-2.0.3/pyecharts/render/snapshot.py
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts/render/templates/
+-rw-r--r--   0 sunhailin   (501) staff       (20)      217 2019-10-10 01:57:06.000000 pyecharts-2.0.3/pyecharts/render/templates/components.html
+-rw-r--r--   0 sunhailin   (501) staff       (20)     8622 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/render/templates/macro
+-rw-r--r--   0 sunhailin   (501) staff       (20)      121 2019-10-10 01:57:06.000000 pyecharts-2.0.3/pyecharts/render/templates/nb_components.html
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1436 2019-10-10 01:57:06.000000 pyecharts-2.0.3/pyecharts/render/templates/nb_jupyter_globe.html
+-rw-r--r--   0 sunhailin   (501) staff       (20)      359 2019-10-10 01:57:06.000000 pyecharts-2.0.3/pyecharts/render/templates/nb_jupyter_lab.html
+-rw-r--r--   0 sunhailin   (501) staff       (20)      458 2019-10-10 01:57:06.000000 pyecharts-2.0.3/pyecharts/render/templates/nb_jupyter_lab_tab.html
+-rw-r--r--   0 sunhailin   (501) staff       (20)      489 2019-10-10 01:57:06.000000 pyecharts-2.0.3/pyecharts/render/templates/nb_jupyter_notebook.html
+-rw-r--r--   0 sunhailin   (501) staff       (20)      608 2019-10-10 01:57:06.000000 pyecharts-2.0.3/pyecharts/render/templates/nb_jupyter_notebook_tab.html
+-rw-r--r--   0 sunhailin   (501) staff       (20)      274 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/render/templates/nb_nteract.html
+-rw-r--r--   0 sunhailin   (501) staff       (20)      333 2023-01-03 07:51:04.000000 pyecharts-2.0.3/pyecharts/render/templates/simple_chart.html
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1438 2019-07-16 15:15:19.000000 pyecharts-2.0.3/pyecharts/render/templates/simple_globe.html
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1074 2023-01-03 07:51:04.000000 pyecharts-2.0.3/pyecharts/render/templates/simple_page.html
+-rw-r--r--   0 sunhailin   (501) staff       (20)      993 2023-01-03 07:51:04.000000 pyecharts-2.0.3/pyecharts/render/templates/simple_tab.html
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts/scaffold/
+-rw-r--r--   0 sunhailin   (501) staff       (20)        0 2019-07-16 15:15:19.000000 pyecharts-2.0.3/pyecharts/scaffold/__init__.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     4628 2023-04-10 01:13:00.000000 pyecharts-2.0.3/pyecharts/types.py
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts.egg-info/
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1030 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts.egg-info/PKG-INFO
+-rw-r--r--   0 sunhailin   (501) staff       (20)     4555 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts.egg-info/SOURCES.txt
+-rw-r--r--   0 sunhailin   (501) staff       (20)        1 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts.egg-info/dependency_links.txt
+-rw-r--r--   0 sunhailin   (501) staff       (20)        1 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts.egg-info/not-zip-safe
+-rw-r--r--   0 sunhailin   (501) staff       (20)      138 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts.egg-info/requires.txt
+-rw-r--r--   0 sunhailin   (501) staff       (20)       10 2023-04-10 01:17:02.000000 pyecharts-2.0.3/pyecharts.egg-info/top_level.txt
+-rw-r--r--   0 sunhailin   (501) staff       (20)       38 2023-04-10 01:17:02.000000 pyecharts-2.0.3/setup.cfg
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2976 2023-01-05 07:14:05.000000 pyecharts-2.0.3/setup.py
+drwxr-xr-x   0 sunhailin   (501) staff       (20)        0 2023-04-10 01:17:02.000000 pyecharts-2.0.3/test/
+-rw-r--r--   0 sunhailin   (501) staff       (20)    11042 2023-01-03 07:51:04.000000 pyecharts-2.0.3/test/test_bar.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1980 2019-11-13 01:12:20.000000 pyecharts-2.0.3/test/test_bar3d.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2960 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_base.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     4885 2020-02-28 05:16:31.000000 pyecharts-2.0.3/test/test_bmap.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2833 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_boxplot.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2109 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_calendar.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)    10076 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_chart.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3716 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_chart_options.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1444 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_custom.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2038 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_datasets.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      918 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_display.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      957 2020-10-29 15:11:51.000000 pyecharts-2.0.3/test/test_effectscatter.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1882 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_exception.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      444 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_faker.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      998 2020-10-29 15:11:51.000000 pyecharts-2.0.3/test/test_funnel.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1165 2020-06-07 15:18:09.000000 pyecharts-2.0.3/test/test_gauge.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)    15534 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_geo.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     9941 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_global_options.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     4580 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_graph.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1772 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_graph_gl.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1539 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_graphic.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)    13618 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_grid.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      675 2019-10-10 01:57:06.000000 pyecharts-2.0.3/test/test_heatmap.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1219 2023-01-03 07:51:04.000000 pyecharts-2.0.3/test/test_image.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      207 2019-10-10 01:57:06.000000 pyecharts-2.0.3/test/test_item_style_options.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2408 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_kline.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2691 2020-10-29 15:11:51.000000 pyecharts-2.0.3/test/test_line.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1136 2019-10-10 01:57:06.000000 pyecharts-2.0.3/test/test_line3d.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1663 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_lines3d.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1400 2023-01-03 07:51:04.000000 pyecharts-2.0.3/test/test_liquid.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)    10059 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_map.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)    11604 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_map3d.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1483 2023-01-03 07:51:04.000000 pyecharts-2.0.3/test/test_map_globe.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      592 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_mixins.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     5001 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_page.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2888 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_parallel.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      734 2019-10-10 01:57:06.000000 pyecharts-2.0.3/test/test_pictorialbar.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2864 2023-01-03 07:51:04.000000 pyecharts-2.0.3/test/test_pie.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1744 2023-01-03 07:51:04.000000 pyecharts-2.0.3/test/test_polar.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3381 2020-10-29 15:11:51.000000 pyecharts-2.0.3/test/test_radar.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     2204 2023-01-03 07:51:04.000000 pyecharts-2.0.3/test/test_sankey.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     6851 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_scatter.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      721 2019-10-10 01:57:06.000000 pyecharts-2.0.3/test/test_scatter3d.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3715 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_series_options.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3280 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_snapshot.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1837 2019-10-10 01:57:06.000000 pyecharts-2.0.3/test/test_sunburst.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1252 2019-10-10 01:57:06.000000 pyecharts-2.0.3/test/test_surface3d.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     3034 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_tab.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1540 2023-01-03 07:51:04.000000 pyecharts-2.0.3/test/test_table.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)      803 2019-10-10 01:57:06.000000 pyecharts-2.0.3/test/test_themeriver.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     5891 2023-01-03 07:51:04.000000 pyecharts-2.0.3/test/test_timeline.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1676 2023-01-03 07:51:04.000000 pyecharts-2.0.3/test/test_tree.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1709 2020-03-12 08:02:05.000000 pyecharts-2.0.3/test/test_treemap.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1744 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_utils.py
+-rw-r--r--   0 sunhailin   (501) staff       (20)     1781 2023-04-10 01:13:00.000000 pyecharts-2.0.3/test/test_wordcloud.py
```

### Comparing `pyecharts-2.0.2/PKG-INFO` & `pyecharts-2.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecharts
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python options, make charting easier
 Home-page: https://github.com/pyecharts/pyecharts
 Author: chenjiandongx
 Author-email: chenjiandongx@qq.com
 License: MIT
 Description: UNKNOWN
 Keywords: Echarts,charts,plotting-tool
```

### Comparing `pyecharts-2.0.2/README.md` & `pyecharts-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/charts/__init__.py` & `pyecharts-2.0.3/pyecharts/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/charts/base.py` & `pyecharts-2.0.3/pyecharts/charts/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,33 +2,41 @@
 import uuid
 
 import simplejson as json
 from jinja2 import Environment
 
 from ..commons import utils
 from ..globals import CurrentConfig, RenderType, ThemeType
-from ..options import InitOpts
+from ..options import InitOpts, RenderOpts
 from ..options.global_options import AnimationOpts
 from ..options.series_options import BasicOpts
 from ..render import engine
 from ..types import Optional, Sequence, Union
 from .mixins import ChartMixin
 
 
 class Base(ChartMixin):
     """
     `Base` is the root class for all graphical class, it provides
     part of the initialization parameters and common methods
     """
 
-    def __init__(self, init_opts: Union[InitOpts, dict] = InitOpts()):
+    def __init__(
+        self,
+        init_opts: Union[InitOpts, dict] = InitOpts(),
+        render_opts: Union[RenderOpts, dict] = RenderOpts(),
+    ):
         _opts = init_opts
         if isinstance(init_opts, InitOpts):
             _opts = init_opts.opts
 
+        _render_opts = render_opts
+        if isinstance(render_opts, RenderOpts):
+            _render_opts = render_opts.opts
+
         self.width = _opts.get("width", "900px")
         self.height = _opts.get("height", "500px")
         self.horizontal_center = (
             "text-align:center; margin: auto"
             if _opts.get("is_horizontal_center", False)
             else ""
         )
@@ -36,28 +44,32 @@
         self.page_title = _opts.get("page_title", CurrentConfig.PAGE_TITLE)
         self.theme = _opts.get("theme", ThemeType.WHITE)
         self.chart_id = _opts.get("chart_id") or uuid.uuid4().hex
         self.fill_bg = _opts.get("fill_bg", False)
         self.bg_color = _opts.get("bg_color")
 
         self.options: dict = {}
+        self.render_options: dict = {}
         self.js_host: str = _opts.get("js_host") or CurrentConfig.ONLINE_HOST
         self.js_functions: utils.OrderedSet = utils.OrderedSet()
         self.js_dependencies: utils.OrderedSet = utils.OrderedSet("echarts")
         self.options.update(backgroundColor=self.bg_color)
         if isinstance(_opts.get("animationOpts", AnimationOpts()), dict):
             self.options.update(_opts.get("animationOpts", AnimationOpts().opts))
         else:
             self.options.update(_opts.get("animationOpts", AnimationOpts()).opts)
         self.options.update(aria=_opts.get("ariaOpts"))
 
         self._is_geo_chart: bool = False
         self._geo_json_name: Optional[str] = None
         self._geo_json: Optional[dict] = None
 
+        self.render_options.update(embed_js=bool(_render_opts.get("embed_js")))
+        self._render_cache: dict = dict()
+
     def get_chart_id(self) -> str:
         return self.chart_id
 
     def get_options(self) -> dict:
         return utils.remove_key_with_none_value(self.options)
 
     def dump_options(self) -> str:
@@ -100,14 +112,20 @@
         if self.theme not in ThemeType.BUILTIN_THEMES:
             self.js_dependencies.add(self.theme)
 
     def _prepare_render(self):
         self.json_contents = self.dump_options()
         self._use_theme()
 
+        self._render_cache.clear()
+        if self.render_options.get("embed_js"):
+            self._render_cache[
+                "javascript"
+            ] = self.load_javascript().load_javascript_contents()
+
 
 def default(o):
     if isinstance(o, (datetime.date, datetime.datetime)):
         return o.isoformat()
     if isinstance(o, utils.JsCode):
         return (
             o.replace("\\n|\\t", "").replace(r"\\n", "\n").replace(r"\\t", "\t").js_code
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/bar.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/bar.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     """
 
     def add_yaxis(
         self,
         series_name: str,
         y_axis: types.Sequence[types.Union[types.Numeric, opts.BarItem, dict]],
         *,
-        is_selected: bool = True,
         xaxis_index: types.Optional[types.Numeric] = None,
         yaxis_index: types.Optional[types.Numeric] = None,
         is_legend_hover_link: bool = True,
         color: types.Optional[str] = None,
         is_realtime_sort: bool = False,
         is_show_background: bool = False,
         background_style: types.Union[types.BarBackground, dict, None] = None,
@@ -47,15 +46,15 @@
         markpoint_opts: types.MarkPoint = None,
         markline_opts: types.MarkLine = None,
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
         encode: types.Union[types.JSFunc, dict, None] = None,
     ):
         self._append_color(color)
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
 
         if self.options.get("dataset") is not None:
             y_axis = None
 
         self.options.get("series").append(
             {
                 "type": ChartType.BAR,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/bmap.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/bmap.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,16 +16,17 @@
     Support scatter plot, line
     """
 
     def __init__(
         self,
         init_opts: types.Init = opts.InitOpts(),
         is_ignore_nonexistent_coord: bool = False,
+        render_opts: types.RenderInit = opts.RenderOpts(),
     ):
-        super().__init__(init_opts=init_opts)
+        super().__init__(init_opts=init_opts, render_opts=render_opts)
         self.js_dependencies.add("bmap")
         self._is_geo_chart = True
         self._coordinate_system: types.Optional[str] = "bmap"
         self.bmap_js_functions: OrderedSet = OrderedSet()
         self._is_ignore_nonexistent_coord = is_ignore_nonexistent_coord
 
     def _feed_data(self, data_pair: types.Sequence, type_: str) -> types.Sequence:
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/boxplot.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/kline.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,80 +1,58 @@
 from ... import options as opts
 from ... import types
 from ...charts.chart import RectChart
 from ...globals import ChartType
 
 
-class Boxplot(RectChart):
+class Kline(RectChart):
     """
-    <<< Boxplot >>>
+    <<< K-line >>>
 
-    A box-plot is a statistical chart used to show a set of data dispersion data.
-    It displays the maximum, minimum, median, lower quartile, and upper quartile
-    of a set of data.
+    K-line shows the highest value, the lowest value,
+    the starting value and the ending value of the data on the day,
+    which is used to show the daily fluctuation of the data or
+    the fluctuation of a certain period.
     """
 
+    def __init__(
+        self,
+        init_opts: types.Init = opts.InitOpts(),
+        render_opts: types.RenderInit = opts.RenderOpts(),
+    ):
+        super().__init__(init_opts=init_opts, render_opts=render_opts)
+        self.set_global_opts(
+            xaxis_opts=opts.AxisOpts(is_scale=True),
+            yaxis_opts=opts.AxisOpts(is_scale=True),
+        )
+
     def add_yaxis(
         self,
         series_name: str,
-        y_axis: types.Optional[
-            types.Sequence[types.Union[opts.BoxplotItem, dict]]
-        ] = None,
+        y_axis: types.Sequence[types.Union[opts.CandleStickItem, dict]],
         *,
-        chart_type: str = ChartType.BOXPLOT,
-        is_selected: bool = True,
+        color_by: types.Optional[str] = "series",
+        layout: types.Optional[str] = None,
         xaxis_index: types.Optional[types.Numeric] = None,
         yaxis_index: types.Optional[types.Numeric] = None,
-        dataset_index: types.Optional[types.Numeric] = None,
-        box_width: types.Optional[types.Sequence] = None,
-        selected_mode: types.Union[bool, str] = False,
-        label_opts: types.Label = opts.LabelOpts(),
-        markpoint_opts: types.MarkPoint = opts.MarkPointOpts(),
-        markline_opts: types.MarkLine = opts.MarkLineOpts(),
+        markline_opts: types.MarkLine = None,
+        markpoint_opts: types.MarkPoint = None,
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
     ):
-        if box_width is None:
-            box_width = [7, 50]
-
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
         self.options.get("series").append(
             {
-                "type": chart_type,
+                "type": ChartType.KLINE,
                 "name": series_name,
+                "colorBy": color_by,
+                "layout": layout,
                 "xAxisIndex": xaxis_index,
                 "yAxisIndex": yaxis_index,
-                "datasetIndex": dataset_index,
-                "boxWidth": box_width,
-                "selected_mode": selected_mode,
                 "data": y_axis,
-                "label": label_opts,
                 "markPoint": markpoint_opts,
                 "markLine": markline_opts,
                 "tooltip": tooltip_opts,
                 "itemStyle": itemstyle_opts,
             }
         )
         return self
-
-    @staticmethod
-    def prepare_data(items):
-        data = []
-        for item in items:
-            try:
-                d, res = sorted(item), []
-                for i in range(1, 4):
-                    n = i * (len(d) + 1) / 4
-                    k = int(n)
-                    m = n - k
-                    if m == 0:
-                        res.append(d[k - 1])
-                    elif m == 1 / 4:
-                        res.append(d[k - 1] * 0.75 + d[k] * 0.25)
-                    elif m == 1 / 2:
-                        res.append(d[k - 1] * 0.50 + d[k] * 0.50)
-                    elif m == 3 / 4:
-                        res.append(d[k - 1] * 0.25 + d[k] * 0.75)
-                data.append([d[0]] + res + [d[-1]])
-            except Exception:
-                pass
-        return data
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/calendar.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/calendar.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,39 +9,42 @@
     <<< Calendar Diagram >>>
 
     The calendar diagram is mainly used to represent the size of a value by
     color and must be used in conjunction with the visualMap component.
     Two categories of axes must be used in rectangular coordinates.
     """
 
-    def __init__(self, init_opts: types.Init = opts.InitOpts()):
-        super().__init__(init_opts=init_opts)
+    def __init__(
+        self,
+        init_opts: types.Init = opts.InitOpts(),
+        render_opts: types.RenderInit = opts.RenderOpts(),
+    ):
+        super().__init__(init_opts=init_opts, render_opts=render_opts)
         self.options.update(calendar=opts.CalendarOpts().opts)
 
     def add(
         self,
         series_name: str,
         yaxis_data: types.Sequence,
         *,
         type_: types.Union[str, ChartType] = ChartType.HEATMAP,
-        is_selected: bool = True,
         calendar_index: types.Optional[types.Numeric] = None,
         label_opts: types.Label = opts.LabelOpts(is_show=False, position="inside"),
         calendar_opts: types.Union[types.Calendar, types.List[types.Calendar]] = None,
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
         visualmap_opts: types.VisualMap = None,
         **other_calendar_opts,
     ):
         if calendar_opts:
             self.options.update(calendar=calendar_opts)
         if visualmap_opts:
             self.options.update(visualMap=visualmap_opts)
 
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
         self.options.get("series").append(
             {
                 "type": type_,
                 "coordinateSystem": "calendar",
                 "calendarIndex": calendar_index,
                 "name": series_name,
                 "data": yaxis_data,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/custom.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/custom.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         data: types.Optional[types.Sequence] = None,
         is_clip: bool = True,
         z_level: types.Numeric = 0,
         z: types.Numeric = 2,
         itemstyle_opts: types.ItemStyle = None,
         tooltip_opts: types.Tooltip = None,
     ):
-        self._append_legend(series_name, selected_mode)
+        self._append_legend(series_name)
 
         self.options.get("series").append(
             {
                 "type": ChartType.CUSTOM,
                 "name": series_name,
                 "renderItem": render_item,
                 "colorBy": color_by,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/effectscatter.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/effectscatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,28 +12,27 @@
     """
 
     def add_yaxis(
         self,
         series_name: str,
         y_axis: types.Sequence[types.Union[opts.EffectScatterItem, dict]],
         *,
-        is_selected: bool = True,
         xaxis_index: types.Optional[types.Numeric] = None,
         yaxis_index: types.Optional[types.Numeric] = None,
         color: types.Optional[str] = None,
         symbol: types.Optional[str] = None,
         symbol_size: types.Numeric = 10,
         symbol_rotate: types.Optional[types.Numeric] = None,
         label_opts: types.Label = opts.LabelOpts(),
         effect_opts: types.Effect = opts.EffectOpts(),
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
     ):
         self._append_color(color)
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
 
         if all([isinstance(d, opts.EffectScatterItem) for d in y_axis]):
             y_axis = y_axis
         else:
             y_axis = [list(z) for z in zip(self._xaxis_data, y_axis)]
 
         self.options.get("series").append(
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/funnel.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/funnel.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,31 +16,30 @@
     """
 
     def add(
         self,
         series_name: str,
         data_pair: types.Sequence,
         *,
-        is_selected: bool = True,
         color: types.Optional[str] = None,
         sort_: str = "descending",
         gap: types.Numeric = 0,
         label_opts: types.Label = opts.LabelOpts(),
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
     ):
         self._append_color(color)
         if all([isinstance(d, opts.FunnelItem) for d in data_pair]):
             data = data_pair
             for a in data_pair:
-                self._append_legend(a.opts.get("name"), is_selected)
+                self._append_legend(a.opts.get("name"))
         else:
             data = [{"name": n, "value": v} for n, v in data_pair]
             for a, _ in data_pair:
-                self._append_legend(a, is_selected)
+                self._append_legend(a)
 
         _dset = set(self.options.get("legend")[0].get("data"))
         self.options.get("legend")[0].update(data=list(_dset))
 
         self.options.get("series").append(
             {
                 "type": ChartType.FUNNEL,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/gauge.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/gauge.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     """
 
     def add(
         self,
         series_name: str,
         data_pair: types.Sequence,
         *,
-        is_selected: bool = True,
         min_: types.Numeric = 0,
         max_: types.Numeric = 100,
         split_number: types.Numeric = 10,
         center: types.Sequence = None,
         radius: types.Union[types.Numeric, str] = "75%",
         start_angle: types.Numeric = 225,
         end_angle: types.Numeric = -45,
@@ -40,15 +39,15 @@
         axistick_opts: types.AxisTick = None,
         axislabel_opts: types.AxisLabel = None,
         itemstyle_opts: types.ItemStyle = None,
     ):
         if center is None:
             center = ["50%", "50%"]
 
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
         self.options.get("series").append(
             {
                 "type": ChartType.GAUGE,
                 "title": title_label_opts,
                 "detail": detail_label_opts,
                 "name": series_name,
                 "min": min_,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/geo.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/geo.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,16 +5,20 @@
 from ...charts.chart import Chart
 from ...datasets import COORDINATES
 from ...exceptions import NonexistentCoordinatesException
 from ...globals import ChartType
 
 
 class GeoChartBase(Chart):
-    def __init__(self, init_opts: types.Init = opts.InitOpts()):
-        super().__init__(init_opts=init_opts)
+    def __init__(
+        self,
+        init_opts: types.Init = opts.InitOpts(),
+        render_opts: types.RenderInit = opts.RenderOpts(),
+    ):
+        super().__init__(init_opts=init_opts, render_opts=render_opts)
         self.set_global_opts()
         self._coordinates = COORDINATES
         self._zlevel = 1
         self._coordinate_system: types.Optional[str] = None
         self._chart_type = ChartType.GEO
 
     def add_geo_json(self, geo_json: dict):
@@ -40,15 +44,14 @@
 
     def add(
         self,
         series_name: str,
         data_pair: types.Sequence,
         type_: str = "scatter",
         *,
-        is_selected: bool = True,
         symbol: types.Optional[str] = None,
         symbol_size: types.Numeric = 12,
         blur_size: types.Numeric = 20,
         point_size: types.Numeric = 20,
         color: types.Optional[str] = None,
         is_polyline: bool = False,
         is_large: bool = False,
@@ -63,15 +66,15 @@
         render_item: types.JsCode = None,
         encode: types.Union[types.JsCode, dict] = None,
     ):
         self._zlevel += 1
         data = self._feed_data(data_pair, type_)
 
         self._append_color(color)
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
 
         if type_ == ChartType.SCATTER:
             self.options.get("series").append(
                 {
                     "type": type_,
                     "name": series_name,
                     "coordinateSystem": self._coordinate_system,
@@ -193,16 +196,17 @@
     support scatter plot and line
     """
 
     def __init__(
         self,
         init_opts: types.Init = opts.InitOpts(),
         is_ignore_nonexistent_coord: bool = False,
+        render_opts: types.RenderInit = opts.RenderOpts(),
     ):
-        super().__init__(init_opts=init_opts)
+        super().__init__(init_opts=init_opts, render_opts=render_opts)
         self._coordinate_system: types.Optional[str] = "geo"
         self._is_ignore_nonexistent_coord = is_ignore_nonexistent_coord
 
     def _feed_data(self, data_pair: types.Sequence, type_: str) -> types.Sequence:
         result = []
         for n, v in data_pair:
             try:
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/graph.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/graph.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,14 @@
     def add(
         self,
         series_name: str,
         nodes: types.Sequence[types.GraphNode],
         links: types.Sequence[types.GraphLink],
         categories: types.Union[types.Sequence[types.GraphCategory], None] = None,
         *,
-        is_selected: bool = True,
         is_focusnode: bool = True,
         is_roam: bool = True,
         is_draggable: bool = False,
         is_rotate_label: bool = False,
         layout: str = "force",
         symbol: types.Optional[str] = None,
         symbol_size: types.Numeric = 10,
@@ -51,15 +50,15 @@
                 link = link.opts
             _links.append(link)
 
         if categories:
             for c in categories:
                 if isinstance(c, opts.GraphCategory):
                     c = c.opts
-                self._append_legend(c.get("name", ""), is_selected)
+                self._append_legend(c.get("name", ""))
 
         if edge_label is None:
             edge_label = opts.LabelOpts(is_show=False)
 
         if edge_symbol is None:
             edge_symbol = [None, None]
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/heatmap.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/heatmap.py`

 * *Files 7% similar despite different names*

```diff
@@ -9,34 +9,37 @@
     <<< HeatMap >>>
 
     The heat map is mainly used to represent the size of the value by color,
     which must be used in conjunction with the visualMap component.
     Two categories of axes must be used in rectangular coordinates.
     """
 
-    def __init__(self, init_opts: types.Init = opts.InitOpts()):
-        super().__init__(init_opts=init_opts)
+    def __init__(
+        self,
+        init_opts: types.Init = opts.InitOpts(),
+        render_opts: types.RenderInit = opts.RenderOpts(),
+    ):
+        super().__init__(init_opts=init_opts, render_opts=render_opts)
         self.set_global_opts(visualmap_opts=opts.VisualMapOpts(orient="horizontal"))
 
     def add_yaxis(
         self,
         series_name: str,
         yaxis_data: types.Sequence[types.Union[dict]],
         value: types.Sequence[types.Union[dict]],
         *,
-        is_selected: bool = True,
         xaxis_index: types.Optional[types.Numeric] = None,
         yaxis_index: types.Optional[types.Numeric] = None,
         label_opts: types.Label = opts.LabelOpts(),
         markpoint_opts: types.MarkPoint = None,
         markline_opts: types.MarkLine = None,
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
     ):
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
         self.options.get("yAxis")[0].update(data=yaxis_data)
         self.options.get("series").append(
             {
                 "type": ChartType.HEATMAP,
                 "name": series_name,
                 "xAxisIndex": xaxis_index,
                 "yAxisIndex": yaxis_index,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/kline.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/boxplot.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,82 @@
 from ... import options as opts
 from ... import types
 from ...charts.chart import RectChart
 from ...globals import ChartType
 
 
-class Kline(RectChart):
+class Boxplot(RectChart):
     """
-    <<< K-line >>>
+    <<< Boxplot >>>
 
-    K-line shows the highest value, the lowest value,
-    the starting value and the ending value of the data on the day,
-    which is used to show the daily fluctuation of the data or
-    the fluctuation of a certain period.
+    A box-plot is a statistical chart used to show a set of data dispersion data.
+    It displays the maximum, minimum, median, lower quartile, and upper quartile
+    of a set of data.
     """
 
-    def __init__(self, init_opts: types.Init = opts.InitOpts()):
-        super().__init__(init_opts=init_opts)
-        self.set_global_opts(
-            xaxis_opts=opts.AxisOpts(is_scale=True),
-            yaxis_opts=opts.AxisOpts(is_scale=True),
-        )
-
     def add_yaxis(
         self,
         series_name: str,
-        y_axis: types.Sequence[types.Union[opts.CandleStickItem, dict]],
+        y_axis: types.Optional[
+            types.Sequence[types.Union[opts.BoxplotItem, dict]]
+        ] = None,
         *,
-        is_selected: bool = True,
-        color_by: types.Optional[str] = "series",
-        layout: types.Optional[str] = None,
+        chart_type: str = ChartType.BOXPLOT,
         xaxis_index: types.Optional[types.Numeric] = None,
         yaxis_index: types.Optional[types.Numeric] = None,
-        markline_opts: types.MarkLine = None,
-        markpoint_opts: types.MarkPoint = None,
+        dataset_index: types.Optional[types.Numeric] = None,
+        box_width: types.Optional[types.Sequence] = None,
+        selected_mode: types.Union[bool, str] = False,
+        label_opts: types.Label = opts.LabelOpts(),
+        markpoint_opts: types.MarkPoint = opts.MarkPointOpts(),
+        markline_opts: types.MarkLine = opts.MarkLineOpts(),
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
     ):
-        self._append_legend(series_name, is_selected)
+        if box_width is None:
+            box_width = [7, 50]
+
+        self._append_legend(series_name)
         self.options.get("series").append(
             {
-                "type": ChartType.KLINE,
+                "type": chart_type,
                 "name": series_name,
-                "colorBy": color_by,
-                "layout": layout,
                 "xAxisIndex": xaxis_index,
                 "yAxisIndex": yaxis_index,
+                "datasetIndex": dataset_index,
+                "boxWidth": box_width,
+                "selected_mode": selected_mode,
                 "data": y_axis,
+                "label": label_opts,
                 "markPoint": markpoint_opts,
                 "markLine": markline_opts,
                 "tooltip": tooltip_opts,
                 "itemStyle": itemstyle_opts,
             }
         )
         return self
+
+    @staticmethod
+    def prepare_data(items):
+        data = []
+        for item in items:
+            if not item:
+                data.append([])
+            try:
+                d, res = sorted(item), []
+                for i in range(1, 4):
+                    n = i * (len(d) + 1) / 4
+                    k = int(n)
+                    m = n - k
+                    if m == 0:
+                        res.append(d[k - 1])
+                    elif m == 1 / 4:
+                        res.append(d[k - 1] * 0.75 + d[k] * 0.25)
+                    elif m == 1 / 2:
+                        res.append(d[k - 1] * 0.50 + d[k] * 0.50)
+                    elif m == 3 / 4:
+                        res.append(d[k - 1] * 0.25 + d[k] * 0.75)
+                data.append([d[0]] + res + [d[-1]])
+            except TypeError:
+                # one of the item element is None
+                data.append([])
+        return data
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/line.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/line.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     """
 
     def add_yaxis(
         self,
         series_name: str,
         y_axis: types.Sequence[types.Union[opts.LineItem, dict]],
         *,
-        is_selected: bool = True,
         is_connect_nones: bool = False,
         xaxis_index: types.Optional[types.Numeric] = None,
         yaxis_index: types.Optional[types.Numeric] = None,
         color: types.Optional[str] = None,
         is_symbol_show: bool = True,
         symbol: types.Optional[str] = None,
         symbol_size: types.Union[types.Numeric, types.Sequence] = 4,
@@ -30,24 +29,27 @@
         is_clip: bool = True,
         is_step: bool = False,
         is_hover_animation: bool = True,
         z_level: types.Numeric = 0,
         z: types.Numeric = 0,
         log_base: types.Numeric = 10,
         sampling: types.Optional[str] = None,
+        dimensions: types.Union[types.Sequence, None] = None,
+        series_layout_by: str = "column",
         markpoint_opts: types.MarkPoint = None,
         markline_opts: types.MarkLine = None,
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
         label_opts: types.Label = opts.LabelOpts(),
         linestyle_opts: types.LineStyle = opts.LineStyleOpts(),
         areastyle_opts: types.AreaStyle = opts.AreaStyleOpts(),
+        encode: types.Union[types.JSFunc, dict, None] = None,
     ):
         self._append_color(color)
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
 
         if all([isinstance(d, opts.LineItem) for d in y_axis]):
             data = y_axis
         else:
             # 合并 x 和 y 轴数据，避免当 X 轴的类型设置为 'value' 的时候，
             # X、Y 轴均显示 Y 轴数据
             try:
@@ -55,14 +57,17 @@
                 data = [
                     list(z)
                     for z in zip(self.options["xAxis"][xaxis_index]["data"], y_axis)
                 ]
             except IndexError:
                 data = [list(z) for z in zip(self._xaxis_data, y_axis)]
 
+        if self.options.get("dataset") is not None and not y_axis:
+            data = None
+
         self.options.get("series").append(
             {
                 "type": ChartType.LINE,
                 "name": series_name,
                 "connectNulls": is_connect_nones,
                 "xAxisIndex": xaxis_index,
                 "yAxisIndex": yaxis_index,
@@ -74,14 +79,17 @@
                 "step": is_step,
                 "stack": stack,
                 "data": data,
                 "hoverAnimation": is_hover_animation,
                 "label": label_opts,
                 "logBase": log_base,
                 "sampling": sampling,
+                "dimensions": dimensions,
+                "encode": encode,
+                "seriesLayoutBy": series_layout_by,
                 "lineStyle": linestyle_opts,
                 "areaStyle": areastyle_opts,
                 "markPoint": markpoint_opts,
                 "markLine": markline_opts,
                 "tooltip": tooltip_opts,
                 "itemStyle": itemstyle_opts,
                 "zlevel": z_level,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/liquid.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/liquid.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,16 +7,20 @@
 class Liquid(Chart):
     """
     <<< Liquid >>>
 
     The liquid chart is mainly used to highlight the percentage of data.
     """
 
-    def __init__(self, init_opts: types.Init = opts.InitOpts()):
-        super().__init__(init_opts=init_opts)
+    def __init__(
+        self,
+        init_opts: types.Init = opts.InitOpts(),
+        render_opts: types.RenderInit = opts.RenderOpts(),
+    ):
+        super().__init__(init_opts=init_opts, render_opts=render_opts)
         self.js_dependencies.add("echarts-liquidfill")
 
     def add(
         self,
         series_name: str,
         data: types.Sequence,
         *,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/map.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/map.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,28 +13,36 @@
 
     def add(
         self,
         series_name: str,
         data_pair: types.Sequence[types.Union[types.Sequence, opts.MapItem, dict]],
         maptype: str = "china",
         *,
-        is_selected: bool = True,
         is_roam: bool = True,
         center: types.Optional[types.Sequence] = None,
         aspect_scale: types.Numeric = 0.75,
         bounding_coords: types.Optional[types.Sequence[types.Numeric]] = None,
         min_scale_limit: types.Optional[types.Numeric] = None,
         max_scale_limit: types.Optional[types.Numeric] = None,
         name_property: str = "name",
         selected_mode: types.Union[bool, str] = False,
         zoom: types.Optional[types.Numeric] = 1,
         name_map: types.Optional[dict] = None,
         symbol: types.Optional[str] = None,
         map_value_calculation: str = "sum",
         is_map_symbol_show: bool = True,
+        z_level: types.Numeric = 0,
+        z: types.Numeric = 2,
+        pos_left: types.Optional[types.Union[str, types.Numeric]] = None,
+        pos_top: types.Optional[types.Union[str, types.Numeric]] = None,
+        pos_right: types.Optional[types.Union[str, types.Numeric]] = None,
+        pos_bottom: types.Optional[types.Union[str, types.Numeric]] = None,
+        geo_index: types.Optional[types.Numeric] = None,
+        series_layout_by: str = "column",
+        dataset_index: types.Optional[types.Numeric] = 0,
         layout_center: types.Optional[types.Sequence[str]] = None,
         layout_size: types.Union[str, types.Numeric] = None,
         label_opts: types.Label = opts.LabelOpts(),
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
         emphasis_label_opts: types.Label = None,
         emphasis_itemstyle_opts: types.ItemStyle = None,
@@ -50,15 +58,15 @@
         scale_limit: types.Optional[dict] = {
             "min": min_scale_limit,
             "max": max_scale_limit,
         }
         if min_scale_limit is None and max_scale_limit is None:
             scale_limit = None
 
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
         self.options.get("series").append(
             {
                 "type": ChartType.MAP,
                 "name": series_name,
                 "symbol": symbol,
                 "label": label_opts,
                 "map": maptype,
@@ -68,14 +76,23 @@
                 "boundingCoords": bounding_coords,
                 "scaleLimit": scale_limit,
                 "nameProperty": name_property,
                 "selectedMode": selected_mode,
                 "center": center,
                 "zoom": zoom,
                 "nameMap": name_map,
+                "zlevel": z_level,
+                "z": z,
+                "left": pos_left,
+                "top": pos_top,
+                "right": pos_right,
+                "bottom": pos_bottom,
+                "geoIndex": geo_index,
+                "seriesLayoutBy": series_layout_by,
+                "datasetIndex": dataset_index,
                 "mapValueCalculation": map_value_calculation,
                 "showLegendSymbol": is_map_symbol_show,
                 "layoutCenter": layout_center,
                 "layoutSize": layout_size,
                 "tooltip": tooltip_opts,
                 "itemStyle": itemstyle_opts,
                 "emphasis": {
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/parallel.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/parallel.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,20 @@
     """
     <<< Parallel >>>
 
     Parallel coordinate systems are commonly used to visualize graphs of
     high dimensional data.
     """
 
-    def __init__(self, init_opts: types.Init = opts.InitOpts()):
-        super().__init__(init_opts=init_opts)
+    def __init__(
+        self,
+        init_opts: types.Init = opts.InitOpts(),
+        render_opts: types.RenderInit = opts.RenderOpts(),
+    ):
+        super().__init__(init_opts=init_opts, render_opts=render_opts)
         self.options.update(parallel=opts.ParallelOpts().opts)
 
     def add_schema(
         self,
         schema: types.Sequence[types.Union[opts.ParallelAxisOpts, dict]],
         parallel_opts: types.Union[opts.ParallelOpts, dict, None] = None,
     ):
@@ -36,20 +40,19 @@
 
     def add(
         self,
         series_name: str,
         data: types.Sequence[types.Union[dict]],
         *,
         is_smooth: bool = False,
-        is_selected: bool = True,
         linestyle_opts: types.LineStyle = opts.LineStyleOpts(),
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
     ):
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
         self.options.get("series").append(
             {
                 "type": ChartType.PARALLEL,
                 "coordinateSystem": "parallel",
                 "lineStyle": linestyle_opts,
                 "name": series_name,
                 "data": data,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/pictorialbar.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/pictorialbar.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,29 +22,28 @@
         symbol_pos: types.Optional[str] = None,
         symbol_offset: types.Optional[types.Sequence] = None,
         symbol_rotate: types.Optional[types.Numeric] = None,
         symbol_repeat: types.Optional[str] = None,
         symbol_repeat_direction: types.Optional[str] = None,
         symbol_margin: types.Union[types.Numeric, str, None] = None,
         is_symbol_clip: bool = False,
-        is_selected: bool = True,
         xaxis_index: types.Optional[types.Numeric] = None,
         yaxis_index: types.Optional[types.Numeric] = None,
         color: types.Optional[str] = None,
         category_gap: types.Union[types.Numeric, str] = "20%",
         gap: types.Optional[str] = None,
         label_opts: types.Label = opts.LabelOpts(),
         markpoint_opts: types.MarkPoint = None,
         markline_opts: types.MarkLine = None,
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
         encode: types.Union[types.JsCode, dict] = None,
     ):
         self._append_color(color)
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
         self.options.get("series").append(
             {
                 "type": ChartType.PICTORIALBAR,
                 "symbol": symbol,
                 "symbolSize": symbol_size,
                 "symbolPosition": symbol_pos,
                 "symbolOffset": symbol_offset,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/pie.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/pie.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/polar.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/polar.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,16 +8,20 @@
 class Polar(Chart):
     """
     <<< Polar >>>
 
     Polar coordinates can be used for scatter and polyline graphs.
     """
 
-    def __init__(self, init_opts: types.Init = opts.InitOpts()):
-        super().__init__(init_opts=init_opts)
+    def __init__(
+        self,
+        init_opts: types.Init = opts.InitOpts(),
+        render_opts: types.RenderInit = opts.RenderOpts(),
+    ):
+        super().__init__(init_opts=init_opts, render_opts=render_opts)
         self.add_schema()
 
     def add_schema(
         self,
         radiusaxis_opts: types.RadiusAxis = opts.RadiusAxisOpts(),
         angleaxis_opts: types.AngleAxis = opts.AngleAxisOpts(),
     ):
@@ -29,30 +33,27 @@
         return self
 
     def add(
         self,
         series_name: str,
         data: types.Sequence,
         *,
-        is_selected: bool = True,
         type_: str = "line",
         symbol: types.Optional[str] = None,
         symbol_size: types.Numeric = 4,
         stack: types.Optional[str] = None,
         center: types.Optional[types.Sequence] = None,
         label_opts: types.Label = opts.LabelOpts(is_show=False),
         areastyle_opts: types.AreaStyle = opts.AreaStyleOpts(),
         effect_opts: types.Effect = opts.EffectOpts(),
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
     ):
-        self._append_legend(series_name, is_selected)
-        self.options.update(polar={
-            "center": center if center else ["50%", "50%"]
-        })
+        self._append_legend(series_name)
+        self.options.update(polar={"center": center if center else ["50%", "50%"]})
 
         if type_ in (ChartType.SCATTER, ChartType.LINE, ChartType.BAR):
             self.options.get("series").append(
                 {
                     "type": type_,
                     "name": series_name,
                     "coordinateSystem": "polar",
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/radar.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/radar.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,14 @@
         splitline_opt: types.SplitLine = opts.SplitLineOpts(is_show=True),
         splitarea_opt: types.SplitArea = opts.SplitAreaOpts(),
         axisline_opt: types.AxisLine = opts.AxisLineOpts(),
         radiusaxis_opts: types.RadiusAxis = None,
         angleaxis_opts: types.AngleAxis = None,
         polar_opts: types.Polar = None,
     ):
-
         self.options.update(
             radiusAxis=radiusaxis_opts, angleAxis=angleaxis_opts, polar=polar_opts
         )
 
         indicators = []
         for s in schema:
             if isinstance(s, opts.RadarIndicatorItem):
@@ -56,28 +55,27 @@
         return self
 
     def add(
         self,
         series_name: str,
         data: types.Sequence[types.Union[opts.RadarItem, dict]],
         *,
-        is_selected: bool = True,
         symbol: types.Optional[str] = None,
         color: types.Optional[str] = None,
         label_opts: opts.LabelOpts = opts.LabelOpts(),
         radar_index: types.Numeric = None,
         linestyle_opts: opts.LineStyleOpts = opts.LineStyleOpts(),
         areastyle_opts: opts.AreaStyleOpts = opts.AreaStyleOpts(),
         tooltip_opts: types.Tooltip = None,
     ):
         if all([isinstance(d, opts.RadarItem) for d in data]):
             for a in data:
-                self._append_legend(a.get("name"), is_selected)
+                self._append_legend(a.get("name"))
         else:
-            self._append_legend(series_name, is_selected)
+            self._append_legend(series_name)
         self.options.get("series").append(
             {
                 "type": ChartType.RADAR,
                 "name": series_name,
                 "data": data,
                 "symbol": symbol,
                 "label": label_opts,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/sankey.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/sankey.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,36 +15,35 @@
 
     def add(
         self,
         series_name: str,
         nodes: types.Sequence,
         links: types.Sequence,
         *,
-        is_selected: bool = True,
         pos_left: types.Union[str, types.Numeric] = "5%",
         pos_top: types.Union[str, types.Numeric] = "5%",
         pos_right: types.Union[str, types.Numeric] = "20%",
         pos_bottom: types.Union[str, types.Numeric] = "5%",
         node_width: types.Numeric = 20,
         node_gap: types.Numeric = 8,
         node_align: str = "justify",
         layout_iterations: types.Numeric = 32,
         orient: str = "horizontal",
         is_draggable: bool = True,
-        focus_node_mode: str = 'none',
+        focus_node_mode: str = "none",
         levels: types.SankeyLevel = None,
         label_opts: types.Label = opts.LabelOpts(),
         linestyle_opt: types.LineStyle = opts.LineStyleOpts(),
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
     ):
         if layout_iterations < 32:
             layout_iterations = 32
 
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
         self.options.get("series").append(
             {
                 "type": ChartType.SANKEY,
                 "name": series_name,
                 "data": nodes,
                 "links": links,
                 "left": pos_left,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/scatter.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/scatter.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,15 +34,14 @@
             return [list(z) for z in zip(self._xaxis_data, y_axis)]
 
     def add_yaxis(
         self,
         series_name: str,
         y_axis: types.Sequence[types.Union[opts.ScatterItem, dict]],
         *,
-        is_selected: bool = True,
         xaxis_index: types.Optional[types.Numeric] = None,
         yaxis_index: types.Optional[types.Numeric] = None,
         color: types.Optional[str] = None,
         symbol: types.Optional[str] = None,
         symbol_size: types.Union[types.Numeric, types.Sequence] = 10,
         symbol_rotate: types.Optional[types.Numeric] = None,
         label_opts: types.Label = opts.LabelOpts(position="right"),
@@ -50,15 +49,15 @@
         markline_opts: types.MarkLine = None,
         markarea_opts: types.MarkArea = None,
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
         encode: types.Union[types.JSFunc, dict, None] = None,
     ):
         self._append_color(color)
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
 
         data = self._parse_data(y_axis=y_axis)
 
         self.options.get("series").append(
             {
                 "type": ChartType.SCATTER,
                 "name": series_name,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/sunburst.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/sunburst.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/themeriver.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/themeriver.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,22 +14,21 @@
     """
 
     def add(
         self,
         series_name: types.Sequence,
         data: types.Sequence[types.Union[opts.ThemeRiverItem, dict]],
         *,
-        is_selected: bool = True,
         label_opts: types.Label = opts.LabelOpts(),
         singleaxis_opts: types.SingleAxis = opts.SingleAxisOpts(),
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
     ):
         for n in series_name:
-            self._append_legend(n, is_selected)
+            self._append_legend(n)
 
         self.options.get("series").append(
             {
                 "type": ChartType.THEMERIVER,
                 "name": series_name,
                 "data": data,
                 "label": label_opts,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/tree.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/tree.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/treemap.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/treemap.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     """
 
     def add(
         self,
         series_name: str,
         data: types.Sequence[types.Union[opts.TreeItem, dict]],
         *,
-        is_selected: bool = True,
         leaf_depth: types.Optional[types.Numeric] = None,
         pos_left: types.Optional[str] = None,
         pos_right: types.Optional[str] = None,
         pos_top: types.Optional[str] = None,
         pos_bottom: types.Optional[str] = None,
         width: types.Union[str, types.Numeric] = "80%",
         height: types.Union[str, types.Numeric] = "80%",
@@ -41,15 +40,15 @@
         children_visible_min: types.Optional[types.Numeric] = None,
         label_opts: types.Label = opts.LabelOpts(position="inside"),
         upper_label_opts: types.Label = opts.LabelOpts(position="inside"),
         tooltip_opts: types.Tooltip = None,
         itemstyle_opts: types.ItemStyle = None,
         breadcrumb_opts: types.TreeMapBreadcrumb = None,
     ):
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
         self.options.get("series").append(
             {
                 "type": ChartType.TREEMAP,
                 "name": series_name,
                 "data": data,
                 "left": pos_left,
                 "right": pos_right,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/basic_charts/wordcloud.py` & `pyecharts-2.0.3/pyecharts/charts/basic_charts/wordcloud.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,16 +27,20 @@
     """
     <<< WordCloud >>>
 
     Word cloud is to visually highlight the keywords that
     appear frequently in the text.
     """
 
-    def __init__(self, init_opts: types.Init = opts.InitOpts()):
-        super().__init__(init_opts=init_opts)
+    def __init__(
+        self,
+        init_opts: types.Init = opts.InitOpts(),
+        render_opts: types.RenderInit = opts.RenderOpts(),
+    ):
+        super().__init__(init_opts=init_opts, render_opts=render_opts)
         self.js_dependencies.add("echarts-wordcloud")
         self._mask_image_suffix: types.Sequence = ["jpg", "jpeg", "png", "ico"]
 
     def _create_mask_image_variable(self, data: str) -> JsCode:
         image_str = self._encode_image_to_base64(image_or_path=data)
         if image_str is None:
             raise WordCloudMaskImageException(data=data)
@@ -85,17 +89,15 @@
         itemstyle_opts: types.ItemStyle = None,
         textstyle_opts: types.TextStyle = None,
         emphasis_shadow_blur: types.Optional[types.Numeric] = None,
         emphasis_shadow_color: types.Optional[str] = None,
     ):
         data = []
         for n, v in data_pair:
-            data.append(
-                {"name": n, "value": v, "textStyle": {"color": gen_color()}}
-            )
+            data.append({"name": n, "value": v, "textStyle": {"color": gen_color()}})
 
         word_size_range = word_size_range or (12, 60)
 
         _rmin, _rmax = -90, 90
         # 确保设置的形状有效，单词的旋转角度应该设置在 [-90, 90]
         if shape in SHAPES:
             _rmin = _rmax = 0
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/chart.py` & `pyecharts-2.0.3/pyecharts/charts/chart.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,39 +2,42 @@
 from .. import types
 from ..charts.base import Base
 from ..globals import RenderType, ThemeType, ToolTipFormatterType
 from ..types import Optional, Sequence
 
 
 class Chart(Base):
-    def __init__(self, init_opts: types.Init = opts.InitOpts()):
+    def __init__(
+        self,
+        init_opts: types.Init = opts.InitOpts(),
+        render_opts: types.RenderInit = opts.RenderOpts(),
+    ):
         if isinstance(init_opts, dict):
             temp_opts = opts.InitOpts()
             temp_opts.update(**init_opts)
             init_opts = temp_opts
-        super().__init__(init_opts=init_opts)
+        super().__init__(init_opts=init_opts, render_opts=render_opts)
         # Change to Echarts V5 default color list
         self.colors = (
-            "#5470c6 #91cc75 #fac858 #ee6666 #73c0de #3ba272 #fc8452 #9a60b4 "
-            "#ea7ccc"
+            "#5470c6 #91cc75 #fac858 #ee6666 #73c0de #3ba272 #fc8452 #9a60b4 " "#ea7ccc"
         ).split()
         self.default_color_n = len(self.colors)
         if init_opts.opts.get("theme") == ThemeType.WHITE:
             self.options.update(color=self.colors)
         self.options.update(
             series=[],
             legend=[{"data": [], "selected": dict()}],
             tooltip=opts.TooltipOpts().opts,
         )
         self._chart_type: Optional[str] = None
 
     def set_dark_mode(
         self,
         dark_mode_colors: Optional[Sequence[str]] = None,
-        dark_mode_bg_color: str = "#100C2A"
+        dark_mode_bg_color: str = "#100C2A",
     ):
         # [Hard Code Here] The Echarts default Dark Mode Configurations
         if dark_mode_colors is None:
             dark_mode_colors = (
                 "#4992ff #7cffb2 #fddd60 #ff6e76 #58d9f9 #05c091 #ff8a45 "
                 "#8d48e3 #dd79ff"
             ).split()
@@ -100,18 +103,16 @@
                 s.update(itemStyle=itemstyle_opts)
 
             if len(kwargs) > 0:
                 s.update(kwargs)
 
         return self
 
-    def _append_legend(self, name, is_selected):
+    def _append_legend(self, name):
         self.options.get("legend")[0].get("data").append(name)
-        if self.options.get("legend")[0].get("selected") is not None:
-            self.options.get("legend")[0].get("selected").update({name: is_selected})
 
     def _append_color(self, color: Optional[str]):
         if color:
             # 这是一个bug
             # 添加轴（执行add_yaxis操作）的顺序与新添加的color值（设置color属性）未一一对应，正好颠倒
             self.colors.insert(-self.default_color_n, color)
             # self.colors = [color] + self.colors
@@ -187,30 +188,36 @@
                     "fromDatasetIndex": from_dataset_index,
                     "fromDatasetId": from_dataset_id,
                     "fromTransformResult": from_transform_result,
                 }
             )
         else:
             self.options.update(
-                dataset=[{
-                    "source": source,
-                    "dimensions": dimensions,
-                    "sourceHeader": source_header,
-                    "transform": transform,
-                    "fromDatasetIndex": from_dataset_index,
-                    "fromDatasetId": from_dataset_id,
-                    "fromTransformResult": from_transform_result,
-                }]
+                dataset=[
+                    {
+                        "source": source,
+                        "dimensions": dimensions,
+                        "sourceHeader": source_header,
+                        "transform": transform,
+                        "fromDatasetIndex": from_dataset_index,
+                        "fromDatasetId": from_dataset_id,
+                        "fromTransformResult": from_transform_result,
+                    }
+                ]
             )
         return self
 
 
 class RectChart(Chart):
-    def __init__(self, init_opts: types.Init = opts.InitOpts()):
-        super().__init__(init_opts=init_opts)
+    def __init__(
+        self,
+        init_opts: types.Init = opts.InitOpts(),
+        render_opts: types.RenderInit = opts.RenderOpts(),
+    ):
+        super().__init__(init_opts=init_opts, render_opts=render_opts)
         self.options.update(xAxis=[opts.AxisOpts().opts], yAxis=[opts.AxisOpts().opts])
 
     def extend_axis(
         self,
         xaxis_data: Sequence = None,
         xaxis: types.Axis = None,
         yaxis: types.Axis = None,
@@ -242,27 +249,31 @@
         )
         if self.options.get("legend")[0].get("selected") is not None:
             self.options.get("legend")[0].get("selected").update(
                 chart.options.get("legend")[0].get("selected")
             )
         self.options.get("series").extend(chart.options.get("series"))
         # to merge colors of chart
-        for c in chart.colors[:len(chart.colors) - self.default_color_n]:
+        for c in chart.colors[: len(chart.colors) - self.default_color_n]:
             self.colors.insert(len(self.colors) - self.default_color_n, c)
         return self
 
 
 class Chart3D(Chart):
     """
     `Chart3D`类是所有 3D 类图表的基类，继承自 `Chart` 类
     """
 
-    def __init__(self, init_opts: types.Init = opts.InitOpts()):
+    def __init__(
+        self,
+        init_opts: types.Init = opts.InitOpts(),
+        render_opts: types.RenderInit = opts.RenderOpts(),
+    ):
         init_opts.renderer = RenderType.CANVAS
-        super().__init__(init_opts)
+        super().__init__(init_opts, render_opts)
         self.js_dependencies.add("echarts-gl")
         self._3d_chart_type: Optional[str] = None  # 3d chart type,don't use it directly
 
     def add_globe(
         self,
         is_show: bool = True,
         globe_radius: types.Numeric = 100,
@@ -362,15 +373,15 @@
                     "itemStyle": itemstyle_opts,
                     "parametric": is_parametric,
                     "wireframe": {
                         "show": is_show_wire_frame,
                         "lineStyle": wire_frame_line_style_opts,
                     },
                     "equation": equation,
-                    "parametricEquation": parametric_equation
+                    "parametricEquation": parametric_equation,
                 }
             )
         else:
             self.options.get("series").append(
                 {
                     "type": self._3d_chart_type,
                     "name": series_name,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/composite_charts/grid.py` & `pyecharts-2.0.3/pyecharts/charts/composite_charts/grid.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,16 +10,20 @@
 class Grid(Base):
     """
     `Gird` Drawing grid in rectangular coordinate. In a single grid,
     at most two X and Y axes each is allowed. Line chart, bar chart,
     and scatter chart (bubble chart) can be drawn in grid.
     """
 
-    def __init__(self, init_opts: types.Init = opts.InitOpts()):
-        super().__init__(init_opts=init_opts)
+    def __init__(
+        self,
+        init_opts: types.Init = opts.InitOpts(),
+        render_opts: types.RenderInit = opts.RenderOpts(),
+    ):
+        super().__init__(init_opts=init_opts, render_opts=render_opts)
         self.options: types.Optional[dict] = None
         self._axis_index: int = 0
         self._grow_grid_index: int = 0
         self.bg_color = init_opts.opts.get("bg_color")
 
     def add(
         self,
@@ -45,15 +49,18 @@
 
         # visualMap 配置添加
         visual_map = chart.options.get("visualMap")
         if visual_map is not None:
             if isinstance(self.options.get("visualMap"), opts.VisualMapOpts):
                 self.options.update(visualMap=[self.options.get("visualMap")])
             else:
-                self.options.get("visualMap").extend(visual_map)
+                if self.options.get("visualMap") is None:
+                    self.options.update(visualMap=[visual_map])
+                else:
+                    self.options.get("visualMap").extend([visual_map])
 
         # title 配置添加
         title = chart.options.get("title", opts.TitleOpts().opts)
         if isinstance(title, opts.TitleOpts):
             title = title.opts
         if not isinstance(title, types.Sequence):
             title = (title,)
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/composite_charts/page.py` & `pyecharts-2.0.3/pyecharts/charts/composite_charts/page.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/charts/composite_charts/tab.py` & `pyecharts-2.0.3/pyecharts/charts/composite_charts/tab.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
             opts=css_opts, key="button_active", css_selector=".tab button.active"
         )
         result += (
             tab_button_active
             if tab_button_active != ""
             else DEFAULT_TAB_BUTTON_ACTIVE_CSS
         )
-        if "chart-container" not in result:
+        if ".chart-container" not in result:
             result += """
             .chart-container { display: block; }
 
             .chart-container:nth-child(n+2) { display: none; }
             """
         return result
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/composite_charts/timeline.py` & `pyecharts-2.0.3/pyecharts/charts/composite_charts/timeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,20 @@
 
 
 class Timeline(Base):
     """
     `Timeline` provides functions like switching and playing between multiple charts.
     """
 
-    def __init__(self, init_opts: types.Init = opts.InitOpts()):
-        super().__init__(init_opts=init_opts)
+    def __init__(
+        self,
+        init_opts: types.Init = opts.InitOpts(),
+        render_opts: types.RenderInit = opts.RenderOpts(),
+    ):
+        super().__init__(init_opts=init_opts, render_opts=render_opts)
         self.options = {"baseOption": {"series": [], "timeline": {}}, "options": []}
         self.add_schema()
         self._time_points: types.Sequence = []
 
     def add_schema(
         self,
         axis_type: str = "category",
@@ -70,29 +74,28 @@
                 "graphic": graphic_opts,
                 "checkpointStyle": checkpointstyle_opts,
                 "controlStyle": controlstyle_opts,
                 "progress": {
                     "lineStyle": progress_linestyle_opts,
                     "itemStyle": progress_itemstyle_opts,
                     "label": progress_label_opts,
-                }
+                },
             }
         )
         return self
 
     def add(self, chart: Base, time_point: str):
         for dep in chart.js_dependencies.items:
             self.js_dependencies.add(dep)
         self._time_points.append(time_point)
 
         self.options.get("baseOption").get("timeline").update(data=self._time_points)
         self.options.get("options").append(
             {
                 "backgroundColor": chart.options.get("backgroundColor"),
-                "legend": chart.options.get("legend"),
                 "series": chart.options.get("series"),
                 "xAxis": chart.options.get("xAxis"),
                 "yAxis": chart.options.get("yAxis"),
                 "title": chart.options.get("title"),
                 "tooltip": chart.options.get("tooltip"),
                 "visualMap": chart.options.get("visualMap"),
                 "color": chart.options.get("color"),
@@ -117,13 +120,14 @@
             "radiusAxis",
             "geo",
             "angleAxis",
             "radar",
             "visualMap",
             "dataZoom",
             "parallelAxis",
+            "legend",
         ]
 
         for component in components:
             c = chart.options.get(component, None)
             if c is not None:
                 self.options.get("baseOption").update({component: c})
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/three_axis_charts/graph_gl.py` & `pyecharts-2.0.3/pyecharts/charts/three_axis_charts/graph_gl.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from ... import options as opts
 from ... import types
 from ...charts.chart import Chart3D
 from ...globals import ChartType
-from ...options import InitOpts
+from ...options import InitOpts, RenderOpts
 
 
 class GraphGL(Chart3D):
     """
     <<< GraphGL Relational graphs using WebGL to support the layout and
     drawing of large-scale network/relational data. >>>
     """
 
-    def __init__(self, init_opts: types.Init = InitOpts()):
-        super().__init__(init_opts)
+    def __init__(
+        self,
+        init_opts: types.Init = InitOpts(),
+        render_opts: types.RenderInit = RenderOpts(),
+    ):
+        super().__init__(init_opts, render_opts)
         self._3d_chart_type = ChartType.GRAPHGL
 
     def add(
         self,
         series_name: str,
         nodes: types.Sequence[types.GraphGLNode],
         links: types.Sequence[types.GraphGLLink],
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/three_axis_charts/lines3D.py` & `pyecharts-2.0.3/pyecharts/charts/three_axis_charts/lines3D.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from ... import options as opts
 from ... import types
 from ...charts.chart import Chart3D
 from ...globals import ChartType
-from ...options import InitOpts
+from ...options import InitOpts, RenderOpts
 
 
 class Lines3D(Chart3D):
     """
     Lines 3D
     """
 
-    def __init__(self, init_opts: types.Init = InitOpts()):
-        super().__init__(init_opts)
+    def __init__(
+        self,
+        init_opts: types.Init = InitOpts(),
+        render_opts: types.RenderInit = RenderOpts(),
+    ):
+        super().__init__(init_opts, render_opts)
         self._3d_chart_type = ChartType.LINES3D
 
     def add(
         self,
         series_name: str,
         data_pair: types.Sequence,
         coordinate_system: str,
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/three_axis_charts/map3D.py` & `pyecharts-2.0.3/pyecharts/charts/three_axis_charts/map3D.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from ... import options as opts
 from ... import types
 from ...charts.chart import Chart3D
 from ...globals import ChartType
-from ...options import InitOpts
+from ...options import InitOpts, RenderOpts
 
 
 class Map3D(Chart3D):
     """
     3D map
     """
 
-    def __init__(self, init_opts: types.Init = InitOpts()):
-        super().__init__(init_opts)
+    def __init__(
+        self,
+        init_opts: types.Init = InitOpts(),
+        render_opts: types.RenderInit = RenderOpts(),
+    ):
+        super().__init__(init_opts, render_opts)
         self._3d_chart_type = ChartType.MAP3D
 
     def add(
         self,
         series_name: str,
         data_pair: types.Sequence,
         *,
         type_: ChartType = None,
         maptype: str = "china",
-        is_selected: bool = True,
         is_map_symbol_show: bool = True,
         grid_3d_index: types.Numeric = 0,
         geo_3d_index: types.Numeric = 0,
         globe_index: types.Numeric = 0,
         bar_size: types.Optional[types.Numeric] = None,
         bevel_size: types.Numeric = 0,
         bevel_smoothness: types.Numeric = 2,
@@ -52,15 +55,15 @@
         animation_duration_update: types.Numeric = 100,
         animation_easing_update: types.Numeric = "cubicOut",
     ):
         if type_ != ChartType.LINES3D:
             data = [{"name": n, "value": v} for n, v in data_pair]
         else:
             data = data_pair
-        self._append_legend(series_name, is_selected)
+        self._append_legend(series_name)
         if type_ is None or type_ == ChartType.MAP3D:
             self.options.get("series").append(
                 {
                     "type": ChartType.MAP3D,
                     "name": series_name,
                     "map": maptype,
                     "coordinateSystem": "geo3D",
```

### Comparing `pyecharts-2.0.2/pyecharts/charts/three_axis_charts/map_globe.py` & `pyecharts-2.0.3/pyecharts/charts/three_axis_charts/map_globe.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,26 +3,30 @@
 from jinja2 import Environment
 
 from ... import types
 from ...charts.basic_charts.map import MapMixin
 from ...charts.chart import Chart3D
 from ...commons import utils
 from ...globals import CurrentConfig, NotebookType
-from ...options import InitOpts
+from ...options import InitOpts, RenderOpts
 from ...render.display import HTML
 from ...render.engine import RenderEngine
 
 
 class MapGlobe(Chart3D, MapMixin):
     """
     Globe Map
     """
 
-    def __init__(self, init_opts: types.Init = InitOpts()):
-        super().__init__(init_opts)
+    def __init__(
+        self,
+        init_opts: types.Init = InitOpts(),
+        render_opts: types.RenderInit = RenderOpts(),
+    ):
+        super().__init__(init_opts, render_opts)
 
     def add_schema(self, maptype: str = "china"):
         self.js_dependencies.add(maptype)
         return self
 
     def render(
         self,
```

### Comparing `pyecharts-2.0.2/pyecharts/commons/utils.py` & `pyecharts-2.0.3/pyecharts/commons/utils.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/components/image.py` & `pyecharts-2.0.3/pyecharts/components/image.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/components/table.py` & `pyecharts-2.0.3/pyecharts/components/table.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/datasets/__init__.py` & `pyecharts-2.0.3/pyecharts/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/datasets/city_coordinates.json` & `pyecharts-2.0.3/pyecharts/datasets/city_coordinates.json`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/datasets/countries_regions_db.json` & `pyecharts-2.0.3/pyecharts/datasets/countries_regions_db.json`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/datasets/map_filename.json` & `pyecharts-2.0.3/pyecharts/datasets/map_filename.json`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/exceptions.py` & `pyecharts-2.0.3/pyecharts/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/faker.py` & `pyecharts-2.0.3/pyecharts/faker.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/globals.py` & `pyecharts-2.0.3/pyecharts/globals.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/options/__init__.py` & `pyecharts-2.0.3/pyecharts/options/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     CalendarMonthLabelOpts,
     CalendarYearLabelOpts,
     DataZoomOpts,
     DatasetTransformOpts,
     Grid3DOpts,
     GridOpts,
     InitOpts,
+    RenderOpts,
     LegendOpts,
     ParallelAxisOpts,
     ParallelOpts,
     PolarOpts,
     RadarIndicatorItem,
     RadiusAxisItem,
     RadiusAxisOpts,
```

### Comparing `pyecharts-2.0.2/pyecharts/options/charts_options.py` & `pyecharts-2.0.3/pyecharts/options/charts_options.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/options/global_options.py` & `pyecharts-2.0.3/pyecharts/options/global_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,28 +82,28 @@
                 "multiple": {
                     "prefix": series_multiple_prefix,
                     "withName": series_multiple_with_name,
                     "withoutName": series_multiple_without_name,
                     "separator": {
                         "middle": series_multiple_separator_middle,
                         "end": series_multiple_separator_end,
-                    }
+                    },
                 },
             },
             "data": {
                 "maxCount": data_max_count,
                 "allData": data_all_data,
                 "partialData": data_partial_data,
                 "withName": data_with_name,
                 "withoutName": data_without_name,
                 "separator": {
                     "middle": data_separator_middle,
                     "end": data_separator_end,
-                }
-            }
+                },
+            },
         }
 
 
 class AriaDecalOpts(BasicOpts):
     def __init__(
         self,
         is_show: bool = False,
@@ -127,15 +127,15 @@
                 "color": decals_color,
                 "backgroundColor": decals_background_color,
                 "dashArrayX": decals_dash_array_x,
                 "dashArrayY": decals_dash_array_y,
                 "rotation": decals_rotation,
                 "maxTileWidth": decals_max_tile_width,
                 "maxTileHeight": decals_max_tile_height,
-            }
+            },
         }
 
 
 class AriaOpts(BasicOpts):
     def __init__(
         self,
         is_enable: bool = False,
@@ -159,15 +159,15 @@
         renderer: str = RenderType.CANVAS,
         page_title: str = CurrentConfig.PAGE_TITLE,
         theme: str = ThemeType.WHITE,
         bg_color: Union[str, dict] = None,
         is_fill_bg_color: bool = False,
         js_host: str = "",
         animation_opts: Union[AnimationOpts, dict] = AnimationOpts(),
-        aria_opts: Union[AriaOpts, dict] = AriaOpts()
+        aria_opts: Union[AriaOpts, dict] = AriaOpts(),
     ):
         self.opts: dict = {
             "width": width,
             "height": height,
             "is_horizontal_center": is_horizontal_center,
             "chart_id": chart_id,
             "renderer": renderer,
@@ -177,14 +177,21 @@
             "fill_bg": is_fill_bg_color,
             "js_host": js_host,
             "animationOpts": animation_opts,
             "ariaOpts": aria_opts,
         }
 
 
+class RenderOpts(BasicOpts):
+    def __init__(self, is_embed_js: bool = False):
+        self.opts: dict = {
+            "embed_js": is_embed_js,
+        }
+
+
 class ToolBoxFeatureSaveAsImageOpts(BasicOpts):
     def __init__(
         self,
         type_: str = "png",
         name: Optional[str] = None,
         background_color: str = "auto",
         connected_background_color: str = "#fff",
@@ -720,15 +727,15 @@
         position: Union[str, Sequence, JSFunc] = None,
         formatter: Optional[JSFunc] = None,
         value_formatter: Optional[JSFunc] = None,
         background_color: Optional[str] = None,
         border_color: Optional[str] = None,
         border_width: Numeric = 0,
         padding: Numeric = 5,
-        textstyle_opts: TextStyleOpts = TextStyleOpts(font_size=14),
+        textstyle_opts: Optional[TextStyleOpts] = TextStyleOpts(font_size=14),
         extra_css_text: Optional[str] = None,
         order: str = "seriesAsc",
     ):
         self.opts: dict = {
             "show": is_show,
             "trigger": trigger,
             "triggerOn": trigger_on,
```

### Comparing `pyecharts-2.0.2/pyecharts/options/series_options.py` & `pyecharts-2.0.3/pyecharts/options/series_options.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/render/display.py` & `pyecharts-2.0.3/pyecharts/render/display.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from ..types import Optional, Sequence, Union
+from urllib.parse import urlparse
+import http.client
 
 
 class HTML:
     def __init__(self, data: Optional[str] = None):
         self.data = data
 
     def _repr_html_(self):
@@ -46,17 +48,39 @@
         if isinstance(css, str):
             css = [css]
         elif css is None:
             css = []
         self.lib = lib
         self.css = css
         self.data = data or ""
+        self.javascript_contents = dict()
 
     def _repr_javascript_(self):
         r = ""
         for c in self.css:
             r += _css_t % c
         for d in self.lib:
             r += _lib_t1 % d
         r += self.data
         r += _lib_t2 * len(self.lib)
         return r
+
+    def load_javascript_contents(self):
+        for lib in self.lib:
+            parsed_url = urlparse(lib)
+
+            host: str = str(parsed_url.hostname)
+            port: int = parsed_url.port
+            path: str = parsed_url.path
+
+            resp: Optional[http.client.HTTPResponse] = None
+            try:
+                conn = http.client.HTTPSConnection(host, port)
+                conn.request("GET", path)
+                resp = conn.getresponse()
+                if resp.status != 200:
+                    raise RuntimeError("Cannot load JavaScript lib: %s" % lib)
+                self.javascript_contents[lib] = resp.read().decode("utf-8")
+            finally:
+                if resp is not None:
+                    resp.close()
+        return self
```

### Comparing `pyecharts-2.0.2/pyecharts/render/engine.py` & `pyecharts-2.0.3/pyecharts/render/engine.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+
 try:
     from collections.abc import Iterable
 except ImportError:
     from collections import Iterable
 
 from jinja2 import Environment
```

### Comparing `pyecharts-2.0.2/pyecharts/render/snapshot.py` & `pyecharts-2.0.3/pyecharts/render/snapshot.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/render/templates/macro` & `pyecharts-2.0.3/pyecharts/render/templates/macro`

 * *Files 6% similar despite different names*

```diff
@@ -77,17 +77,26 @@
             {% endif %}
         {% endfor %}
         });
     </script>
 {%- endmacro %}
 
 {%- macro render_chart_dependencies(c) -%}
-    {% for dep in c.dependencies %}
-        <script type="text/javascript" src="{{ dep }}"></script>
-    {% endfor %}
+    {% if 'embed_js' in c.render_options and 'javascript' in c._render_cache and c.render_options.embed_js -%}
+        {% set _javascript = c._render_cache.javascript %}
+        {% for dep in c.dependencies %}
+            <script type="text/javascript">
+                {{ _javascript.javascript_contents[dep] }}
+            </script>
+        {% endfor %}
+    {%- else -%}
+        {% for dep in c.dependencies %}
+            <script type="text/javascript" src="{{ dep }}"></script>
+        {% endfor %}
+    {%- endif %}
 {%- endmacro %}
 
 {%- macro render_chart_css(c) -%}
     {% for dep in c.css_libs %}
         <link rel="stylesheet"  href="{{ dep }}">
     {% endfor %}
 {%- endmacro %}
```

### Comparing `pyecharts-2.0.2/pyecharts/render/templates/nb_jupyter_globe.html` & `pyecharts-2.0.3/pyecharts/render/templates/nb_jupyter_globe.html`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/render/templates/nb_jupyter_notebook_tab.html` & `pyecharts-2.0.3/pyecharts/render/templates/nb_jupyter_notebook_tab.html`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/render/templates/simple_globe.html` & `pyecharts-2.0.3/pyecharts/render/templates/simple_globe.html`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/render/templates/simple_page.html` & `pyecharts-2.0.3/pyecharts/render/templates/simple_page.html`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/render/templates/simple_tab.html` & `pyecharts-2.0.3/pyecharts/render/templates/simple_tab.html`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/pyecharts/types.py` & `pyecharts-2.0.3/pyecharts/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 )
 
 from . import options as opts
 from .options.charts_options import BaseGraphic, GlobeLayersOpts
 from .options.series_options import JsCode, JSFunc, Numeric
 
 Init = Union[opts.InitOpts, dict]
+RenderInit = Union[opts.RenderOpts, dict]
 
 Axis = Union[opts.AxisOpts, dict, None]
 Axis3D = Union[opts.Axis3DOpts, dict]
 AxisLine = Union[opts.AxisLineOpts, dict, None]
 AxisLabel = Union[opts.LabelOpts, dict, None]
 AxisPointer = Union[opts.AxisPointerOpts, dict, None]
 AxisTick = Union[opts.AxisTickOpts, dict, None]
```

### Comparing `pyecharts-2.0.2/pyecharts.egg-info/PKG-INFO` & `pyecharts-2.0.3/pyecharts.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyecharts
-Version: 2.0.2
+Version: 2.0.3
 Summary: Python options, make charting easier
 Home-page: https://github.com/pyecharts/pyecharts
 Author: chenjiandongx
 Author-email: chenjiandongx@qq.com
 License: MIT
 Description: UNKNOWN
 Keywords: Echarts,charts,plotting-tool
```

### Comparing `pyecharts-2.0.2/pyecharts.egg-info/SOURCES.txt` & `pyecharts-2.0.3/pyecharts.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -105,14 +105,15 @@
 test/test_exception.py
 test/test_faker.py
 test/test_funnel.py
 test/test_gauge.py
 test/test_geo.py
 test/test_global_options.py
 test/test_graph.py
+test/test_graph_gl.py
 test/test_graphic.py
 test/test_grid.py
 test/test_heatmap.py
 test/test_image.py
 test/test_item_style_options.py
 test/test_kline.py
 test/test_line.py
```

### Comparing `pyecharts-2.0.2/setup.py` & `pyecharts-2.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_bar.py` & `pyecharts-2.0.3/test/test_bar.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_bar3d.py` & `pyecharts-2.0.3/test/test_bar3d.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_base.py` & `pyecharts-2.0.3/test/test_map_globe.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,41 +1,46 @@
-from datetime import datetime
 from unittest.mock import patch
 
-from nose.tools import assert_equal, assert_not_in
+from nose.tools import assert_equal, assert_in
 
-from pyecharts.charts import Bar
-from pyecharts.charts.base import Base, default
+from pyecharts.charts import MapGlobe
+from pyecharts.faker import Faker
+from pyecharts.globals import CurrentConfig, NotebookType
 
 
-def test_base_add_functions():
-    c = Base()
-    c.add_js_funcs("console.log('hello')", "console.log('hello')")
-    assert_equal(1, len(c.js_functions.items))
-    assert_equal(["console.log('hello')"], c.js_functions.items)
-
-
-def test_base_init_funcs():
-    c0 = Base({"width": "100px", "height": "200px"})
-    assert_equal(c0.width, "100px")
-    assert_equal(c0.height, "200px")
-
-    c1 = Base(dict(width="110px", height="210px"))
-    assert_equal(c1.width, "110px")
-    assert_equal(c1.height, "210px")
-    assert_not_in(c1.js_host, ["", None])
+@patch("pyecharts.render.engine.write_utf8_html_file")
+def test_map_base(fake_writer):
+    c = MapGlobe().add(
+        "商家A", [list(z) for z in zip(Faker.provinces, Faker.values())], "china"
+    )
+    c.render()
+    _, content = fake_writer.call_args[0]
+    assert_in("document.createElement('canvas')", content)
+    assert_equal(c.theme, "white")
+    assert_equal(c.renderer, "canvas")
+    assert_in("baseTexture", content)
 
 
 @patch("pyecharts.render.engine.write_utf8_html_file")
-def test_render(fake_writer):
-    my_render_content = "my_render_content"
-    bar = Bar()
-    bar.add_xaxis(["1"]).add_yaxis("", [1]).render(my_render_content=my_render_content)
-    assert "test ok" == "test ok"
+def test_map_base_v2(fake_writer):
+    c = (
+        MapGlobe()
+        .add("商家A", [list(z) for z in zip(Faker.provinces, Faker.values())], "china")
+        .add_schema(maptype="china")
+    )
+    c.render()
+    _, content = fake_writer.call_args[0]
+    assert_in("document.createElement('canvas')", content)
+    assert_equal(c.theme, "white")
+    assert_equal(c.renderer, "canvas")
+    assert_in("baseTexture", content)
+
 
+def test_map_globe_in_jupyter():
+    CurrentConfig.NOTEBOOK_TYPE = NotebookType.JUPYTER_NOTEBOOK
 
-def test_base_iso_format():
-    mock_time_str = "2022-04-14 14:42:00"
-    assert (
-        default(datetime.strptime(mock_time_str, "%Y-%m-%d %H:%M:%S"))
-        == "2022-04-14T14:42:00"
+    c = MapGlobe().add(
+        "商家A", [list(z) for z in zip(Faker.provinces, Faker.values())], "china"
     )
+    content = c.render_notebook()._repr_html_()
+    assert_in("document.createElement('canvas')", content)
+    assert_in("baseTexture", content)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `pyecharts-2.0.2/test/test_bmap.py` & `pyecharts-2.0.3/test/test_bmap.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_boxplot.py` & `pyecharts-2.0.3/test/test_boxplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,35 @@
     _, content = fake_writer.call_args[0]
     assert_equal(c.theme, "white")
     assert_equal(c.renderer, "canvas")
     assert_in("boxWidth", content)
 
 
 @patch("pyecharts.render.engine.write_utf8_html_file")
+def test_boxplot_base_v2(fake_writer):
+    v1 = [
+        None,
+        [200, 200, 200],
+    ]
+    v2 = [
+        [1000, None, 1000],
+        [200, 200, 200],
+    ]
+    c = Boxplot()
+    c.add_xaxis(["expr1", "expr2"]).add_yaxis(
+        "A", c.prepare_data(v1), box_width=40
+    ).add_yaxis("B", c.prepare_data(v2))
+    c.render()
+    _, content = fake_writer.call_args[0]
+    assert_equal(c.theme, "white")
+    assert_equal(c.renderer, "canvas")
+    assert_in("boxWidth", content)
+
+
+@patch("pyecharts.render.engine.write_utf8_html_file")
 def test_boxplot_item_base(fake_writer):
     x_axis = ["expr1", "expr2"]
     v1 = [
         [850, 740, 900, 1070, 930, 850, 950, 980, 980, 880, 1000, 980],
         [960, 940, 960, 940, 880, 800, 850, 880, 900, 840, 830, 790],
     ]
     v2 = [
```

### Comparing `pyecharts-2.0.2/test/test_calendar.py` & `pyecharts-2.0.3/test/test_calendar.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,34 +43,31 @@
     begin = datetime.date(2017, 1, 1)
     end = datetime.date(2017, 12, 31)
     data = [
         [str(begin + datetime.timedelta(days=i)), random.randint(1000, 25000)]
         for i in range((end - begin).days + 1)
     ]
 
-    c = (
-        Calendar()
-        .add(
-            "",
-            data,
-            calendar_opts=opts.CalendarOpts(
-                range_="2017",
-                cell_size=15,
-                daylabel_opts=opts.CalendarDayLabelOpts(name_map="cn"),
-                monthlabel_opts=opts.CalendarMonthLabelOpts(name_map="cn"),
-            ),
-            visualmap_opts=opts.VisualMapOpts(
-                max_=20000,
-                min_=500,
-                orient="horizontal",
-                is_piecewise=True,
-                pos_top="230px",
-                pos_left="100px",
-            )
-        )
+    c = Calendar().add(
+        "",
+        data,
+        calendar_opts=opts.CalendarOpts(
+            range_="2017",
+            cell_size=15,
+            daylabel_opts=opts.CalendarDayLabelOpts(name_map="cn"),
+            monthlabel_opts=opts.CalendarMonthLabelOpts(name_map="cn"),
+        ),
+        visualmap_opts=opts.VisualMapOpts(
+            max_=20000,
+            min_=500,
+            orient="horizontal",
+            is_piecewise=True,
+            pos_top="230px",
+            pos_left="100px",
+        ),
     )
     c.render()
     _, content = fake_writer.call_args[0]
     assert_in("cellSize", content)
     assert_in("dayLabel", content)
     assert_in("monthLabel", content)
     assert_in("visualMap", content)
```

### Comparing `pyecharts-2.0.2/test/test_chart.py` & `pyecharts-2.0.3/test/test_chart.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
         .add_xaxis([1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12])
         .add_yaxis("蒸发量", v1)
         .add_yaxis("降水量", v2)
         .extend_axis(
             xaxis=opts.AxisOpts(),
             yaxis=opts.AxisOpts(
                 axislabel_opts=opts.LabelOpts(formatter="{value} °C"), interval=5
-            )
+            ),
         )
         .set_series_opts(label_opts=opts.LabelOpts(is_show=False))
         .set_global_opts(
             title_opts=opts.TitleOpts(title="Overlap-bar+line"),
             yaxis_opts=opts.AxisOpts(
                 axislabel_opts=opts.LabelOpts(formatter="{value} ml")
             ),
```

### Comparing `pyecharts-2.0.2/test/test_chart_options.py` & `pyecharts-2.0.3/test/test_chart_options.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,17 @@
     GlobeLayersOpts,
     GraphCategory,
     ThemeRiverItem,
     TimelineCheckPointerStyle,
     TimelineControlStyle,
     TreeItem,
     TreeMapItemStyleOpts,
+    GraphicImageStyleOpts,
+    GraphicTextStyleOpts,
+    GeoRegionsOpts,
 )
 
 
 def test_bar_background_style_options_remove_none():
     option = BarBackgroundStyleOpts()
     expected = {
         "color": "rgba(180, 180, 180, 0.2)",
@@ -95,7 +98,42 @@
     option = TreeMapItemStyleOpts()
     expected = {
         "gapWidth": 0,
         "borderWidth": 0,
     }
     assert_equal(expected, remove_key_with_none_value(option.opts))
 
+
+def test_graphic_image_style_opts_remove_none():
+    option = GraphicImageStyleOpts(graphic_basicstyle_opts={"fill": "#000"})
+    expected = {
+        "x": 0,
+        "y": 0,
+        "width": 0,
+        "height": 0,
+        "opacity": 1,
+        "fill": "#000",
+    }
+    assert_equal(expected, remove_key_with_none_value(option.opts))
+
+
+def test_graphic_text_style_opts_remove_none():
+    option = GraphicTextStyleOpts(graphic_basicstyle_opts={"fill": "#000"})
+    expected = {
+        "x": 0,
+        "y": 0,
+        "textAlign": "left",
+        "fill": "#000",
+    }
+    assert_equal(expected, remove_key_with_none_value(option.opts))
+
+
+def test_geo_region_opts_remove_none():
+    option = GeoRegionsOpts()
+    expected = {
+        "blur": {},
+        "emphasis": {},
+        "select": {},
+        "selected": False,
+        "silent": False,
+    }
+    assert_equal(expected, remove_key_with_none_value(option.opts))
```

### Comparing `pyecharts-2.0.2/test/test_custom.py` & `pyecharts-2.0.3/test/test_custom.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,44 +5,41 @@
 
 from pyecharts.charts import Custom
 from pyecharts.commons.utils import JsCode
 
 
 @patch("pyecharts.render.engine.write_utf8_html_file")
 def test_custom_base(fake_writer):
-    c = (
-        Custom()
-        .add(
-            series_name="",
-            render_item=JsCode("""
+    c = Custom().add(
+        series_name="",
+        render_item=JsCode(
+            """
             function (params, api) {
                 var categoryIndex = api.value(0);
                 var start = api.coord([api.value(1), categoryIndex]);
                 var end = api.coord([api.value(2), categoryIndex]);
                 var height = api.size([0, 1])[1] * 0.6;
-    
                 var rectShape = echarts.graphic.clipRectByRect({
                     x: start[0],
                     y: start[1] - height / 2,
                     width: end[0] - start[0],
                     height: height
                 }, {
                     x: params.coordSys.x,
                     y: params.coordSys.y,
                     width: params.coordSys.width,
                     height: params.coordSys.height
                 });
-    
                 return rectShape && {
                     type: 'rect',
                     shape: rectShape,
                     style: api.style()
                 };
             }
-            """),
-            data=None,
-        )
+            """
+        ),
+        data=None,
     )
     c.render()
     _, content = fake_writer.call_args[0]
     assert_greater(len(content), 2000)
     assert_in("renderItem", content)
```

### Comparing `pyecharts-2.0.2/test/test_datasets.py` & `pyecharts-2.0.3/test/test_datasets.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import urllib.error
 from unittest.mock import patch
 
-from nose.tools import assert_equal, raises
+from nose.tools import assert_equal, assert_in, raises
 
 from pyecharts.datasets import (
     EXTRA,
     FuzzyDict,
     register_url,
     register_files,
     register_coords,
@@ -17,30 +17,43 @@
 def test_register_url(fake):
     current_path = os.path.dirname(__file__)
     fake_registry = os.path.join(current_path, "fixtures", "registry.json")
     file_name = ["shape-with-internal-borders/an1_hui1_an1_qing4", "js"]
     with open(fake_registry, encoding="utf8") as f:
         fake.return_value = f
         register_url("http://register.url/is/used")
+        # set maxDiff
+        assert_equal.__self__.maxDiff = None
         assert_equal(
-            EXTRA,
+            EXTRA["http://register.url/is/used/js/"],
             {
-                "http://register.url/is/used/js/": {
-                    "安庆": file_name,
-                    "English Name": file_name,
-                }
+                "安庆": file_name,
+                "English Name": file_name,
+            },
+        )
+
+    fake_registry_1 = os.path.join(current_path, "fixtures", "registry_1.json")
+    with open(fake_registry_1, encoding="utf8") as f:
+        fake.return_value = f
+        register_url("http://register.url/is/used")
+        assert_equal(
+            EXTRA["http://register.url/is/used/"],
+            {
+                "安庆": file_name,
+                "English Name": file_name,
             },
         )
 
 
-def test_register_url_error():
-    try:
-        register_url("http://127.0.0.1")
-    except urllib.error.HTTPError as err:
-        assert_equal(type(err), urllib.error.HTTPError)
+# TODO: Github Workflow cannot test it well...Fix it future...
+# def test_register_url_error():
+#     try:
+#         register_url("http://127.0.0.1")
+#     except (urllib.error.HTTPError, ConnectionRefusedError) as err:
+#         assert_in(type(err), [urllib.error.HTTPError, ConnectionRefusedError])
 
 
 def test_fuzzy_search_dict():
     fd = FuzzyDict()
     fd.update({"我是北京市": [1, 2]})
     assert_equal(fd["我是北京"], [1, 2])
```

### Comparing `pyecharts-2.0.2/test/test_display.py` & `pyecharts-2.0.3/test/test_display.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from nose.tools import assert_equal
+from nose.tools import assert_equal, assert_in
 
 from pyecharts.render.display import HTML, Javascript
 
 
 def test_display_html():
     html_content = "<p>hello world<p/>"
     obj = HTML(html_content)
@@ -17,7 +17,15 @@
     assert_equal(obj._repr_javascript_(), js_content)
 
 
 def test_display_javascript_v1():
     js_content = "console.log('hello world')"
     obj = Javascript(js_content, lib="test lib", css="test css")
     assert_equal(obj.data, js_content)
+
+    obj_1 = Javascript(
+        data=js_content,
+        lib=["lib1", "lib2"],
+        css=["css1", "css2"],
+    )
+    assert_equal(obj_1.data, js_content)
+    assert_in(js_content, obj_1._repr_javascript_())
```

### Comparing `pyecharts-2.0.2/test/test_effectscatter.py` & `pyecharts-2.0.3/test/test_effectscatter.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_exception.py` & `pyecharts-2.0.3/test/test_exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             .add_schema(maptype="china")
             .add("geo", [["NonexistentLocation", 123]])
             .set_series_opts(label_opts=opts.LabelOpts(is_show=False))
             .set_global_opts(visualmap_opts=opts.VisualMapOpts())
         )
     except NonexistentCoordinatesException as err:
         assert_equal(type(err), NonexistentCoordinatesException)
-        assert err.__str__() != ''
+        assert err.__str__() != ""
 
 
 def test_geo_ignore_nonexistent_coord_exception():
     (
         Geo(is_ignore_nonexistent_coord=True)
         .add_schema(maptype="china")
         .add("geo", [["NonexistentLocation", 123]])
```

### Comparing `pyecharts-2.0.2/test/test_funnel.py` & `pyecharts-2.0.3/test/test_funnel.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_gauge.py` & `pyecharts-2.0.3/test/test_gauge.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_global_options.py` & `pyecharts-2.0.3/test/test_global_options.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,27 +62,27 @@
             "multiple": {
                 "prefix": "它由{seriesCount}个图表系列组成。",
                 "withName": "图表类型是{seriesType}，表示{seriesName}。",
                 "withoutName": "图表类型是{seriesType}。",
                 "separator": {
                     "middle": "；",
                     "end": "。",
-                }
+                },
             },
         },
         "data": {
             "maxCount": 10,
             "allData": "其数据是——",
             "partialData": "其中，前{displayCnt}项是——",
             "withName": "{name}的数据是{value}",
             "withoutName": "{value}",
             "separator": {
                 "middle": "，",
-            }
-        }
+            },
+        },
     }
     assert_equal(expected, remove_key_with_none_value(option.opts))
 
 
 def test_aria_decal_options_remove_none():
     option = AriaDecalOpts()
     expected = {
@@ -93,29 +93,31 @@
             "symbolKeepAspect": True,
             "color": "rgba(0, 0, 0, 0.2)",
             "dashArrayX": 5,
             "dashArrayY": 5,
             "rotation": 0,
             "maxTileWidth": 512,
             "maxTileHeight": 512,
-        }
+        },
     }
     assert_equal(expected, remove_key_with_none_value(option.opts))
 
 
 def test_init_options_remove_none():
     option = InitOpts(animation_opts={}, aria_opts={})
     expected = {
         "animationOpts": {},
         "height": "500px",
         "page_title": "Awesome-pyecharts",
         "renderer": "canvas",
         "theme": "white",
         "width": "900px",
         "ariaOpts": {},
+        "fill_bg": False,
+        "is_horizontal_center": False,
     }
     assert_equal(expected, remove_key_with_none_value(option.opts))
 
 
 def test_toolbox_feature_options_remove_none():
     save_as_image = ToolBoxFeatureSaveAsImageOpts()
     restore = ToolBoxFeatureRestoreOpts()
@@ -167,14 +169,15 @@
         },
         "brushType": "rect",
         "removeOnClick": True,
         "throttleDelay": 0,
         "throttleType": "fixRate",
         "toolbox": ["rect", "polygon", "keep", "clear"],
         "transformable": True,
+        "z": 10000,
     }
     assert_equal(expected, remove_key_with_none_value(option.opts))
 
 
 def test_data_zoom_options_remove_none():
     option = DataZoomOpts()
     expected = {
@@ -196,14 +199,29 @@
     option = LegendOpts()
     expected = {
         "show": True,
         "padding": 5,
         "itemGap": 10,
         "itemWidth": 25,
         "itemHeight": 14,
+        "backgroundColor": "transparent",
+        "borderColor": "#ccc",
+        "borderWidth": 1,
+        "borderRadius": 0,
+        "pageButtonItemGap": 5,
+        "pageButtonPosition": "end",
+        "pageFormatter": "{current}/{total}",
+        "pageIconColor": "#2f4554",
+        "pageIconInactiveColor": "#aaa",
+        "pageIconSize": 15,
+        "animationDurationUpdate": 800,
+        "selector": False,
+        "selectorPosition": "auto",
+        "selectorItemGap": 7,
+        "selectorButtonGap": 10,
     }
     assert_equal(expected, remove_key_with_none_value(option.opts))
 
 
 def test_visual_map_options_remove_none():
     option = VisualMapOpts(range_opacity=0.1)
     expected = {
@@ -325,12 +343,9 @@
         "minInterval": 0,
     }
     assert_equal(expected, remove_key_with_none_value(option.opts))
 
 
 def test_dataset_transform_options_remove_none():
     option = DatasetTransformOpts()
-    expected = {
-        "type": "filter",
-        "print": False
-    }
+    expected = {"type": "filter", "print": False}
     assert_equal(expected, remove_key_with_none_value(option.opts))
```

### Comparing `pyecharts-2.0.2/test/test_graph.py` & `pyecharts-2.0.3/test/test_graph.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
     assert_equal(c.theme, "white")
     assert_equal(c.renderer, "canvas")
 
 
 @patch("pyecharts.render.engine.write_utf8_html_file")
 def test_graph_base_v2(fake_writer):
     with open(
-        os.path.join("fixtures", "les-miserables.json"), "r", encoding="utf-8"
+        os.path.join("test/fixtures", "les-miserables.json"), "r", encoding="utf-8"
     ) as f:
         j = json.load(f)
         nodes = j["nodes"]
         links = j["links"]
         categories = j["categories"]
 
     categories = [opts.GraphCategory(name=d.get("name")) for d in categories]
```

### Comparing `pyecharts-2.0.2/test/test_graphic.py` & `pyecharts-2.0.3/test/test_graphic.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,38 +19,36 @@
         "item": 1,
     }
     assert_equal(expected, remove_key_with_none_value(group.opts))
 
 
 def test_graphic_image():
     image = opts.GraphicImage(
-        graphic_item={"item": 1},
-        graphic_imagestyle_opts={"opts": 1}
+        graphic_item={"item": 1}, graphic_imagestyle_opts={"opts": 1}
     )
     expected = {
         "type": "image",
         "item": 1,
         "style": {
             "opts": 1,
-        }
+        },
     }
     assert_equal(expected, remove_key_with_none_value(image.opts))
 
 
 def test_graphic_text():
     text = opts.GraphicText(
-        graphic_item={"item": 1},
-        graphic_textstyle_opts={"opts": 1}
+        graphic_item={"item": 1}, graphic_textstyle_opts={"opts": 1}
     )
     expected = {
         "type": "text",
         "item": 1,
         "style": {
             "opts": 1,
-        }
+        },
     }
     assert_equal(expected, remove_key_with_none_value(text.opts))
 
 
 def test_graphic_rect():
     rect = opts.GraphicRect(
         graphic_item={"item": 1},
@@ -59,10 +57,10 @@
     )
     expected = {
         "type": "rect",
         "item": 1,
         "shape": 1,
         "style": {
             "opts": 1,
-        }
+        },
     }
     assert_equal(expected, remove_key_with_none_value(rect.opts))
```

### Comparing `pyecharts-2.0.2/test/test_grid.py` & `pyecharts-2.0.3/test/test_grid.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from unittest.mock import patch
 
 from nose.tools import assert_equal, assert_in
 
 from pyecharts import options as opts
-from pyecharts.charts import Bar, Grid, Line, Geo
-from pyecharts.globals import ThemeType
+from pyecharts.charts import Bar, Grid, Line, Radar, Geo, Map
+from pyecharts.globals import ThemeType, ChartType
 from pyecharts.faker import Faker
 from pyecharts.commons.utils import JsCode
 
 
 def _chart_for_grid() -> Bar:
     x_data = ["{}月".format(i) for i in range(1, 13)]
     bar = (
@@ -107,14 +107,15 @@
         .add_yaxis(
             "平均温度",
             [2.0, 2.2, 3.3, 4.5, 6.3, 10.2, 20.3, 23.4, 23.0, 16.5, 12.0, 6.2],
             yaxis_index=2,
             color="blue",
             label_opts=opts.LabelOpts(is_show=False),
         )
+        .set_global_opts(visualmap_opts=opts.VisualMapOpts())
     )
 
     bar.overlap(line)
     assert_equal(bar.colors[:3], ["red", "green", "blue"])
     return bar
 
 
@@ -135,38 +136,78 @@
 @patch("pyecharts.render.engine.write_utf8_html_file")
 def test_grid_geo_bar(fake_writer):
     bar = (
         Bar()
         .add_xaxis(Faker.choose())
         .add_yaxis("商家A", Faker.values())
         .add_yaxis("商家B", Faker.values())
-        .set_global_opts(legend_opts=opts.LegendOpts(pos_left="20%"))
+        .set_global_opts(
+            title_opts=dict(title="Bar 图"),
+            legend_opts=opts.LegendOpts(pos_left="20%"),
+        )
     )
     geo = (
         Geo()
         .add_schema(maptype="china")
         .add("geo", [list(z) for z in zip(Faker.provinces, Faker.values())])
         .set_series_opts(label_opts=opts.LabelOpts(is_show=False))
         .set_global_opts(
             visualmap_opts=opts.VisualMapOpts(),
-            title_opts=opts.TitleOpts(title="Grid-Geo-Bar"),
+            title_opts=dict(title="Geo 图"),
         )
     )
 
     grid = (
         Grid()
         .add(bar, grid_opts=opts.GridOpts(pos_top="50%", pos_right="75%"))
         .add(geo, grid_opts=opts.GridOpts(pos_left="60%"))
     )
     grid.render()
     _, content = fake_writer.call_args[0]
     assert_in("geo", content)
 
 
 @patch("pyecharts.render.engine.write_utf8_html_file")
+def test_grid_two_radar(fake_writer):
+    schema = [
+        opts.RadarIndicatorItem(name="销售", max_=6500),
+        opts.RadarIndicatorItem(name="管理", max_=16000),
+        opts.RadarIndicatorItem(name="信息技术", max_=30000),
+        opts.RadarIndicatorItem(name="客服", max_=38000),
+        opts.RadarIndicatorItem(name="研发", max_=52000),
+        opts.RadarIndicatorItem(name="市场", max_=25000),
+    ]
+    c = (
+        Radar()
+        .add_schema(schema=schema, center=["25%", "50%"])
+        .add(
+            series_name="预算分配",
+            data=[[4300, 10000, 28000, 35000, 50000, 19000]],
+            radar_index=0,
+        )
+        .set_global_opts(legend_opts=opts.LegendOpts(pos_left="20%"))
+    )
+    c2 = (
+        Radar()
+        .add_schema(schema=schema, center=["75%", "50%"])
+        .add(
+            series_name="实际开销",
+            data=[[5000, 14000, 28000, 31000, 42000, 21000]],
+            radar_index=1,
+        )
+        .set_global_opts(legend_opts=opts.LegendOpts(pos_right="20%"))
+    )
+
+    grid = Grid().add(c, grid_opts=opts.GridOpts()).add(c2, grid_opts=opts.GridOpts())
+    grid.render()
+    _, content = fake_writer.call_args[0]
+    assert_in("radar", content)
+
+
+@patch("pyecharts.render.engine.write_utf8_html_file")
 def test_grid_mutil_yaxis(fake_writer):
     bar = (
         Bar()
         .add_xaxis(["{}月".format(i) for i in range(1, 13)])
         .add_yaxis(
             "蒸发量",
             [2.0, 4.9, 7.0, 23.2, 25.6, 76.7, 135.6, 162.2, 32.6, 20.0, 6.4, 3.3],
@@ -332,7 +373,39 @@
             is_control_axis_index=True,
         )
     )
     grid.render()
     _, content = fake_writer.call_args[0]
     assert_in("xAxis", content)
     assert_in("yAxis", content)
+
+
+@patch("pyecharts.render.engine.write_utf8_html_file")
+def test_grid_geo_map(fake_writer):
+    data_pair = [list(z) for z in zip(Faker.provinces, Faker.values())]
+    geo_chart = (
+        Geo()
+        .add_schema(maptype="china")
+        .add(
+            "geo",
+            data_pair=data_pair,
+            type_=ChartType.SCATTER,
+        )
+        .set_global_opts(
+            visualmap_opts=opts.VisualMapOpts(),
+        )
+    )
+    map_chart = (
+        Map()
+        .add("LCOH", data_pair=data_pair, maptype="china")
+        .set_global_opts(
+            visualmap_opts=opts.VisualMapOpts(),
+        )
+    )
+    grid_chart = (
+        Grid(init_opts=opts.InitOpts())
+        .add(map_chart, grid_opts=opts.GridOpts())
+        .add(geo_chart, grid_opts=opts.GridOpts())
+    )
+    grid_chart.render()
+    _, content = fake_writer.call_args[0]
+    assert_in("geo", content)
```

### Comparing `pyecharts-2.0.2/test/test_heatmap.py` & `pyecharts-2.0.3/test/test_heatmap.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_image.py` & `pyecharts-2.0.3/test/test_image.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_kline.py` & `pyecharts-2.0.3/test/test_kline.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,16 +37,15 @@
 
 
 @patch("pyecharts.render.engine.write_utf8_html_file")
 def test_kline_item_base(fake_writer):
     x_axis = ["2017/7/{}".format(i + 1) for i in range(10)]
     y_axis = data
     kline_item = [
-        opts.CandleStickItem(name=d[0], value=d[1])
-        for d in list(zip(x_axis, y_axis))
+        opts.CandleStickItem(name=d[0], value=d[1]) for d in list(zip(x_axis, y_axis))
     ]
 
     c = (
         Kline()
         .add_xaxis(x_axis)
         .add_yaxis("kline", kline_item)
         .set_global_opts(
```

### Comparing `pyecharts-2.0.2/test/test_line.py` & `pyecharts-2.0.3/test/test_line.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_line3d.py` & `pyecharts-2.0.3/test/test_line3d.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_lines3d.py` & `pyecharts-2.0.3/test/test_lines3d.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 
 from pyecharts import options as opts
 from pyecharts.charts import Lines3D
 
 
 @patch("pyecharts.render.engine.write_utf8_html_file")
 def test_lines3d_base(fake_writer):
-    test_main_url: str = "https://cdn.jsdelivr.net/gh/apache/echarts-website@asf-site/examples"
+    test_main_url: str = (
+        "https://cdn.jsdelivr.net/gh/apache/echarts-website@asf-site/examples"
+    )
     data_json_url = test_main_url + "/data-gl/asset/data/flights.json"
     base_texture = test_main_url + "/data-gl/asset/world.topo.bathy.200401.jpg"
     height_texture = test_main_url + "/data-gl/asset/bathymetry_bw_composite_4k.jpg"
 
     resp = requests.get(data_json_url).json()
     json_routes = resp.get("routes")
     json_airports = resp.get("airports")
```

### Comparing `pyecharts-2.0.2/test/test_liquid.py` & `pyecharts-2.0.3/test/test_liquid.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_map_globe.py` & `pyecharts-2.0.3/test/test_wordcloud.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,62 @@
 from unittest.mock import patch
 
 from nose.tools import assert_equal, assert_in
 
-from pyecharts.charts import MapGlobe
-from pyecharts.faker import Faker
-from pyecharts.globals import CurrentConfig, NotebookType
+from pyecharts.charts import WordCloud
+from pyecharts.commons.utils import JsCode
+from pyecharts.exceptions import WordCloudMaskImageException
+
+words = [
+    ("Sam S Club", 10000),
+    ("Macys", 6181),
+    ("Amy Schumer", 4386),
+    ("Jurassic World", 4055),
+    ("Charter Communications", 2467),
+    ("Chick Fil A", 2244),
+    ("Planet Fitness", 1868),
+    ("Pitch Perfect", 1484),
+]
 
 
 @patch("pyecharts.render.engine.write_utf8_html_file")
-def test_map_base(fake_writer):
-    c = MapGlobe().add(
-        "商家A", [list(z) for z in zip(Faker.provinces, Faker.values())], "china"
-    )
+def test_wordcloud_base(fake_writer):
+    c = WordCloud().add("", words, word_size_range=[20, 100])
     c.render()
     _, content = fake_writer.call_args[0]
-    assert_in("document.createElement('canvas')", content)
     assert_equal(c.theme, "white")
     assert_equal(c.renderer, "canvas")
-    assert_in("baseTexture", content)
 
 
 @patch("pyecharts.render.engine.write_utf8_html_file")
-def test_map_base_v2(fake_writer):
-    c = (
-        MapGlobe()
-        .add("商家A", [list(z) for z in zip(Faker.provinces, Faker.values())], "china")
-        .add_schema(maptype="china")
-    )
+def test_wordcloud_shapes(fake_writer):
+    c = WordCloud().add("", words, word_size_range=[20, 100], shape="cardioid")
     c.render()
     _, content = fake_writer.call_args[0]
-    assert_in("document.createElement('canvas')", content)
     assert_equal(c.theme, "white")
     assert_equal(c.renderer, "canvas")
-    assert_in("baseTexture", content)
 
 
-def test_map_globe_in_jupyter():
-    CurrentConfig.NOTEBOOK_TYPE = NotebookType.JUPYTER_NOTEBOOK
+def test_wordcloud_error_url():
+    try:
+        c = WordCloud().add(
+            "", words, word_size_range=[20, 100], mask_image="error images_url"
+        )
+        c.render()
+    except WordCloudMaskImageException as err:
+        assert_equal(type(err), WordCloudMaskImageException)
+        assert err.__str__() != ""
 
-    c = MapGlobe().add(
-        "商家A", [list(z) for z in zip(Faker.provinces, Faker.values())], "china"
+
+@patch("pyecharts.render.engine.write_utf8_html_file")
+def test_wordcloud_mask_image(fake_writer):
+    c = WordCloud().add(
+        "",
+        words,
+        word_size_range=[20, 100],
+        shape="cardioid",
+        mask_image="test/fixtures/img.png",
     )
-    content = c.render_notebook()._repr_html_()
-    assert_in("document.createElement('canvas')", content)
-    assert_in("baseTexture", content)
+    c.render()
+    _, content = fake_writer.call_args[0]
+    assert_equal(c.theme, "white")
+    assert_equal(c.renderer, "canvas")
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyecharts-2.0.2/test/test_mixins.py` & `pyecharts-2.0.3/test/test_mixins.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,8 +20,7 @@
 def test_composite_mixin_len():
     b_1 = Bar()
     b_2 = Line()
     c = CustomCompositeChart()
     c.add(b_1, "bar")
     c.add(b_2, "line")
     assert len(c) == 2
-
```

### Comparing `pyecharts-2.0.2/test/test_page.py` & `pyecharts-2.0.3/test/test_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,15 +145,15 @@
 
     page2 = _get_new_page(unique=False)
     html2 = page2.save_resize_html(source=page2.render(), cfg_dict=LAYOUT_DICT)
 
     assert_equal(html1, html2)
 
 
-@raises(ValueError)
+@raises(ValueError, FileNotFoundError)
 def test_page_cfg_type():
     page = Page()
     page.save_resize_html()
 
 
 def test_page_iterable():
     page = Page()
@@ -173,12 +173,16 @@
     )
     assert_not_in(".resizable()", content)
     assert_not_in(".draggable()", content)
 
 
 def test_page_resize_cfg():
     page = Page()
-    content = page.save_resize_html(
-        cfg_file="fixtures/resize_cfg.json"
-    )
+    content = page.save_resize_html(cfg_file="test/fixtures/resize_cfg.json")
     assert_not_in(".resizable()", content)
     assert_not_in(".draggable()", content)
+
+
+@raises(ValueError)
+def test_page_no_cfg_dict_or_file():
+    page = Page()
+    page.save_resize_html()
```

### Comparing `pyecharts-2.0.2/test/test_parallel.py` & `pyecharts-2.0.3/test/test_parallel.py`

 * *Files 0% similar despite different names*

```diff
@@ -68,15 +68,15 @@
                 opts.ParallelAxisOpts(
                     dim=7,
                     name="等级",
                     type_="category",
                     data=["优", "良", "轻度污染", "中度污染", "重度污染", "严重污染"],
                 ),
             ],
-            parallel_opts=opts.ParallelOpts()
+            parallel_opts=opts.ParallelOpts(),
         )
         .add("parallel", data)
         .set_global_opts(title_opts=opts.TitleOpts(title="Parallel-Category"))
     )
     c.render()
     _, content = fake_writer.call_args[0]
     assert_equal(c.theme, "white")
```

### Comparing `pyecharts-2.0.2/test/test_pictorialbar.py` & `pyecharts-2.0.3/test/test_pictorialbar.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_pie.py` & `pyecharts-2.0.3/test/test_pie.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_polar.py` & `pyecharts-2.0.3/test/test_polar.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_radar.py` & `pyecharts-2.0.3/test/test_radar.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_sankey.py` & `pyecharts-2.0.3/test/test_sankey.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_scatter.py` & `pyecharts-2.0.3/test/test_scatter.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,28 @@
     c.render()
     _, content = fake_writer.call_args[0]
     assert_equal(c.theme, "white")
     assert_equal(c.renderer, "canvas")
 
 
 @patch("pyecharts.render.engine.write_utf8_html_file")
+def test_scatter_base_no_xaxis(fake_writer):
+    c = (
+        Scatter()
+        .add_xaxis([])
+        .add_yaxis("series0", [1, 2, 4])
+        .add_yaxis("series1", [2, 3, 6])
+    )
+    c.render()
+    _, content = fake_writer.call_args[0]
+    assert_equal(c.theme, "white")
+    assert_equal(c.renderer, "canvas")
+
+
+@patch("pyecharts.render.engine.write_utf8_html_file")
 def test_scatter_item_base(fake_writer):
     x_axis = ["A", "B", "C"]
     y_axis = [1, 2, 4]
     chart_item = [
         opts.ScatterItem(name=d[0], value=d[1]) for d in list(zip(x_axis, y_axis))
     ]
 
@@ -41,15 +55,15 @@
     _, content = fake_writer.call_args[0]
     assert_equal(c.theme, "white")
     assert_equal(c.renderer, "canvas")
 
 
 @patch("pyecharts.render.engine.write_utf8_html_file")
 def test_scatter_dataset(fake_writer):
-    with open("fixtures/life-expectancy-table.json", "r", encoding="utf-8") as f:
+    with open("test/fixtures/life-expectancy-table.json", "r", encoding="utf-8") as f:
         j = json.load(f)
 
     l1_1 = (
         Scatter()
         .add_dataset(
             dimensions=[
                 "Income",
```

### Comparing `pyecharts-2.0.2/test/test_scatter3d.py` & `pyecharts-2.0.3/test/test_scatter3d.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_series_options.py` & `pyecharts-2.0.3/test/test_series_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 )
 
 
 def test_label_options_defaults():
     option = LabelOpts()
     expected = {
         "show": True,
-        "position": "top",
+        "position": None,
         "color": None,
         "distance": None,
         "rotate": None,
         "margin": 8,
         "interval": None,
         "fontSize": None,
         "fontStyle": None,
@@ -42,15 +42,15 @@
 
 def test_label_options_custom():
     option = LabelOpts(
         background_color="red", border_color="green", border_width=1, border_radius=2
     )
     expected = {
         "show": True,
-        "position": "top",
+        "position": None,
         "color": None,
         "distance": None,
         "rotate": None,
         "margin": 8,
         "interval": None,
         "fontSize": None,
         "fontStyle": None,
@@ -78,30 +78,33 @@
     item = MarkLineItem()
     expected = {}
     assert_equal(expected, remove_key_with_none_value(item.opts))
 
 
 def test_mark_area_item_remove_none():
     item = MarkAreaItem()
-    expected = [{
-        "itemStyle": None,
-        "label": None,
-        "name": None,
-        "type": None,
-        "valueDim": None,
-        "valueIndex": None,
-        "xAxis": None,
-        "yAxis": None,
-    }, {
-        "type": None,
-        "valueDim": None,
-        "valueIndex": None,
-        "xAxis": None,
-        "yAxis": None,
-    }]
+    expected = [
+        {
+            "itemStyle": None,
+            "label": None,
+            "name": None,
+            "type": None,
+            "valueDim": None,
+            "valueIndex": None,
+            "xAxis": None,
+            "yAxis": None,
+        },
+        {
+            "type": None,
+            "valueDim": None,
+            "valueIndex": None,
+            "xAxis": None,
+            "yAxis": None,
+        },
+    ]
     assert_equal(expected, remove_key_with_none_value(item.opts))
 
 
 def test_mark_area_options_remove_none():
     label_opts = LabelOpts()
     option = MarkAreaOpts(label_opts=label_opts)
     expected = {
```

### Comparing `pyecharts-2.0.2/test/test_snapshot.py` & `pyecharts-2.0.3/test/test_snapshot.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,29 +21,29 @@
         def make_snapshot(self, *args, **kwargs):
             return self.content
 
     return Engine(content)
 
 
 def test_decode_base64():
-    assert decode_base64(data="abcde12") == b'i\xb7\x1d{]'
+    assert decode_base64(data="abcde12") == b"i\xb7\x1d{]"
 
 
 def test_save_as_png():
-    save_as_png(image_data=b'i\xb7\x1d{]', output_name="text_png.png")
+    save_as_png(image_data=b"i\xb7\x1d{]", output_name="text_png.png")
     os.unlink("text_png.png")
 
 
 def test_save_as_text():
     save_as_text(image_data="test data", output_name="test_txt.txt")
     os.unlink("test_txt.txt")
 
 
 def test_save_as():
-    with open("fixtures/img1.jpg", "rb") as f:
+    with open("test/fixtures/img1.jpg", "rb") as f:
         image_bytes = f.read()
     save_as(image_data=image_bytes, output_name="test_pdf.pdf", file_type="pdf")
     os.unlink("test_pdf.pdf")
     save_as(image_data=image_bytes, output_name="test_gif.gif", file_type="gif")
     os.unlink("test_gif.gif")
     save_as(image_data=image_bytes, output_name="test_eps.eps", file_type="eps")
     os.unlink("test_eps.eps")
@@ -92,7 +92,20 @@
 
 @patch("pyecharts.render.snapshot.save_as_text")
 def test_make_snapshot_text(fake_writer):
     eng = _gen_faker_engine("fake content1,content2")
     make_snapshot(eng, _gen_bar_chart(), "make_snapshot.svg")
     _ = fake_writer.call_args[0]
     assert_equal("test ok", "test ok")
+
+
+@patch("pyecharts.render.snapshot.save_as_text")
+def test_make_snapshot_text_v1(fake_writer):
+    eng = _gen_faker_engine("fake content1,content2")
+    make_snapshot(
+        engine=eng,
+        file_name=_gen_bar_chart(),
+        output_name="make_snapshot.svg",
+        is_remove_html=True,
+    )
+    _ = fake_writer.call_args[0]
+    assert_equal("test ok", "test ok")
```

### Comparing `pyecharts-2.0.2/test/test_sunburst.py` & `pyecharts-2.0.3/test/test_sunburst.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_surface3d.py` & `pyecharts-2.0.3/test/test_surface3d.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_tab.py` & `pyecharts-2.0.3/test/test_tab.py`

 * *Files 6% similar despite different names*

```diff
@@ -50,14 +50,18 @@
     bar = _create_bar()
     line = _create_line()
     content = Tab().add(bar, "bar").add(line, "line").render_embed()
     assert_true(len(content) > 8000)
 
 
 def test_tab_render_notebook():
+    from pyecharts.globals import CurrentConfig, NotebookType
+
+    CurrentConfig.NOTEBOOK_TYPE = NotebookType.JUPYTER_NOTEBOOK
+
     tab = Tab()
     tab.add(_create_line(), "line-example")
     tab.add(_create_bar(), "bar-example")
     tab.add(_create_table(), "table-example")
     html = tab.render_notebook().__html__()
     assert_in("City name", html)
 
@@ -86,7 +90,16 @@
     assert_true(isinstance(tab, Iterable))
 
 
 def test_tab_attr():
     tab = Tab()
     assert_true(isinstance(tab.js_functions, OrderedSet))
     assert_true(isinstance(tab._charts, list))
+
+
+def test_tab_with_chart_container():
+    tab = Tab(
+        tab_css_opts=opts.TabChartGlobalOpts(
+            is_enable=False, tab_base_css={"overflow": "hidden"}
+        )
+    )
+    assert_true(isinstance(tab._charts, list))
```

### Comparing `pyecharts-2.0.2/test/test_table.py` & `pyecharts-2.0.3/test/test_table.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_themeriver.py` & `pyecharts-2.0.3/test/test_themeriver.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_timeline.py` & `pyecharts-2.0.3/test/test_timeline.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_tree.py` & `pyecharts-2.0.3/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_treemap.py` & `pyecharts-2.0.3/test/test_treemap.py`

 * *Files identical despite different names*

### Comparing `pyecharts-2.0.2/test/test_utils.py` & `pyecharts-2.0.3/test/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,41 @@
 from nose.tools import assert_equal
 
 from pyecharts.commons import utils
+from pyecharts.datasets import EXTRA
 
 
 def test_utils_produce_require_dict():
     cfg = utils.produce_require_dict(utils.OrderedSet("echarts"), "https://example.com")
     assert_equal(cfg["config_items"], ["'echarts':'https://example.comecharts.min'"])
     assert_equal(cfg["libraries"], ["'echarts'"])
 
-    cfg_1 = utils.produce_require_dict(utils.OrderedSet("https://api.map.baidu.com"), "https://example.com")
-    print(cfg_1)
-    assert_equal(cfg_1["config_items"], ["'baidu_map_api25':'https://api.map.baidu.com'"])
+    cfg_1 = utils.produce_require_dict(
+        utils.OrderedSet("https://api.map.baidu.com"),
+        "https://example.com",
+    )
+    assert_equal(
+        cfg_1["config_items"],
+        ["'baidu_map_api25':'https://api.map.baidu.com'"],
+    )
     assert_equal(cfg_1["libraries"], ["'baidu_map_api25'"])
 
 
+def test_utils_produce_require_dict_with_extra():
+    global EXTRA
+    EXTRA["https://api.baidu.com"] = {
+        "https://api.baidu.com/test.min": ["https://api.baidu.com/test.min", "css"]
+    }
+    cfg_0 = utils.produce_require_dict(
+        utils.OrderedSet("https://api.baidu.com/test.min"),
+        "https://example.com",
+    )
+    assert_equal(cfg_0["libraries"], ["'https://api.baidu.com/test.min'"])
+
+
 def test_js_code():
     fn = "function() { console.log('test_js_code') }"
     js_code = utils.JsCode(fn)
     assert_equal(js_code.js_code, "--x_x--0_0--{}--x_x--0_0--".format(fn))
 
 
 def test_ordered_set():
```

