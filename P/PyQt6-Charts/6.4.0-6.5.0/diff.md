# Comparing `tmp/PyQt6_Charts-6.4.0.tar.gz` & `tmp/PyQt6_Charts-6.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyQt6_Charts-6.4.0.tar", last modified: Fri Sep 30 10:26:21 2022, max compression
+gzip compressed data, was "PyQt6_Charts-6.5.0.tar", last modified: Tue Apr  4 15:21:13 2023, max compression
```

## Comparing `PyQt6_Charts-6.4.0.tar` & `PyQt6_Charts-6.5.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:26:21.089774 PyQt6_Charts-6.4.0/
--rw-r--r--   0 phil       (501) staff       (20)     3908 2022-09-30 10:26:20.431878 PyQt6_Charts-6.4.0/ChangeLog
--rw-r--r--   0 phil       (501) staff       (20)    35147 2022-09-30 10:26:20.272422 PyQt6_Charts-6.4.0/LICENSE
--rw-r--r--   0 phil       (501) staff       (20)      338 2022-09-30 10:24:58.808776 PyQt6_Charts-6.4.0/NEWS
--rw-r--r--   0 phil       (501) staff       (20)     1551 2022-09-30 10:26:21.089891 PyQt6_Charts-6.4.0/PKG-INFO
--rw-r--r--   0 phil       (501) staff       (20)     1229 2022-09-30 10:26:20.433066 PyQt6_Charts-6.4.0/README
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:26:21.070696 PyQt6_Charts-6.4.0/examples/
--rw-r--r--   0 phil       (501) staff       (20)     2013 2022-09-30 10:24:58.813391 PyQt6_Charts-6.4.0/examples/areachart.py
--rw-r--r--   0 phil       (501) staff       (20)     1934 2022-09-30 10:24:58.814159 PyQt6_Charts-6.4.0/examples/barchart.py
--rw-r--r--   0 phil       (501) staff       (20)     5710 2022-09-30 10:24:58.814884 PyQt6_Charts-6.4.0/examples/barmodelmapper.py
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:26:21.071439 PyQt6_Charts-6.4.0/examples/boxplotchart/
--rw-r--r--   0 phil       (501) staff       (20)     1583 2022-09-30 10:24:58.815593 PyQt6_Charts-6.4.0/examples/boxplotchart/acme_data.txt
--rw-r--r--   0 phil       (501) staff       (20)     3433 2022-09-30 10:24:58.816183 PyQt6_Charts-6.4.0/examples/boxplotchart/boxplotchart.py
--rw-r--r--   0 phil       (501) staff       (20)     1587 2022-09-30 10:24:58.816787 PyQt6_Charts-6.4.0/examples/boxplotchart/boxwhisk_data.txt
--rw-r--r--   0 phil       (501) staff       (20)    12540 2022-09-30 10:24:58.817520 PyQt6_Charts-6.4.0/examples/chartthemes.py
--rw-r--r--   0 phil       (501) staff       (20)     3894 2022-09-30 10:24:58.818090 PyQt6_Charts-6.4.0/examples/donutbreakdown.py
--rw-r--r--   0 phil       (501) staff       (20)     2103 2022-09-30 10:24:58.818675 PyQt6_Charts-6.4.0/examples/horizontalbarchart.py
--rw-r--r--   0 phil       (501) staff       (20)     2100 2022-09-30 10:24:58.819268 PyQt6_Charts-6.4.0/examples/horizontalpercentbarchart.py
--rw-r--r--   0 phil       (501) staff       (20)     2100 2022-09-30 10:24:58.819894 PyQt6_Charts-6.4.0/examples/horizontalstackedbarchart.py
--rw-r--r--   0 phil       (501) staff       (20)     5747 2022-09-30 10:24:58.820508 PyQt6_Charts-6.4.0/examples/modeldata.py
--rw-r--r--   0 phil       (501) staff       (20)     1998 2022-09-30 10:24:58.821106 PyQt6_Charts-6.4.0/examples/percentbarchart.py
--rw-r--r--   0 phil       (501) staff       (20)     5662 2022-09-30 10:24:58.821723 PyQt6_Charts-6.4.0/examples/polarchart.py
--rw-r--r--   0 phil       (501) staff       (20)      793 2022-09-30 10:26:20.433469 PyQt6_Charts-6.4.0/pyproject.toml
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:26:21.071967 PyQt6_Charts-6.4.0/sip/
-drwxr-xr-x   0 phil       (501) staff       (20)        0 2022-09-30 10:26:21.089554 PyQt6_Charts-6.4.0/sip/QtCharts/
--rw-r--r--   0 phil       (501) staff       (20)     3667 2022-09-30 10:26:20.849331 PyQt6_Charts-6.4.0/sip/QtCharts/QtChartsmod.sip
--rw-r--r--   0 phil       (501) staff       (20)     5341 2022-09-30 10:26:20.871734 PyQt6_Charts-6.4.0/sip/QtCharts/qabstractaxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     2795 2022-09-30 10:26:20.850569 PyQt6_Charts-6.4.0/sip/QtCharts/qabstractbarseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     6115 2022-09-30 10:26:20.848616 PyQt6_Charts-6.4.0/sip/QtCharts/qabstractseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1289 2022-09-30 10:26:20.851877 PyQt6_Charts-6.4.0/sip/QtCharts/qarealegendmarker.sip
--rw-r--r--   0 phil       (501) staff       (20)     2869 2022-09-30 10:26:20.879655 PyQt6_Charts-6.4.0/sip/QtCharts/qareaseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     2071 2022-09-30 10:26:20.873541 PyQt6_Charts-6.4.0/sip/QtCharts/qbarcategoryaxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     1338 2022-09-30 10:26:20.875495 PyQt6_Charts-6.4.0/sip/QtCharts/qbarlegendmarker.sip
--rw-r--r--   0 phil       (501) staff       (20)     1197 2022-09-30 10:26:20.854697 PyQt6_Charts-6.4.0/sip/QtCharts/qbarseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     3837 2022-09-30 10:26:20.891482 PyQt6_Charts-6.4.0/sip/QtCharts/qbarset.sip
--rw-r--r--   0 phil       (501) staff       (20)     1310 2022-09-30 10:26:20.851435 PyQt6_Charts-6.4.0/sip/QtCharts/qboxplotlegendmarker.sip
--rw-r--r--   0 phil       (501) staff       (20)     2225 2022-09-30 10:26:20.889654 PyQt6_Charts-6.4.0/sip/QtCharts/qboxplotseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     2224 2022-09-30 10:26:20.849918 PyQt6_Charts-6.4.0/sip/QtCharts/qboxset.sip
--rw-r--r--   0 phil       (501) staff       (20)     1338 2022-09-30 10:26:20.854284 PyQt6_Charts-6.4.0/sip/QtCharts/qcandlesticklegendmarker.sip
--rw-r--r--   0 phil       (501) staff       (20)     1902 2022-09-30 10:26:20.847603 PyQt6_Charts-6.4.0/sip/QtCharts/qcandlestickmodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     3169 2022-09-30 10:26:20.880779 PyQt6_Charts-6.4.0/sip/QtCharts/qcandlestickseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     2005 2022-09-30 10:26:20.889167 PyQt6_Charts-6.4.0/sip/QtCharts/qcandlestickset.sip
--rw-r--r--   0 phil       (501) staff       (20)     1985 2022-09-30 10:26:20.892402 PyQt6_Charts-6.4.0/sip/QtCharts/qcategoryaxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     4333 2022-09-30 10:26:20.879049 PyQt6_Charts-6.4.0/sip/QtCharts/qchart.sip
--rw-r--r--   0 phil       (501) staff       (20)     2358 2022-09-30 10:26:20.885934 PyQt6_Charts-6.4.0/sip/QtCharts/qchartview.sip
--rw-r--r--   0 phil       (501) staff       (20)     1945 2022-09-30 10:26:20.885363 PyQt6_Charts-6.4.0/sip/QtCharts/qcoloraxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     1707 2022-09-30 10:26:20.891953 PyQt6_Charts-6.4.0/sip/QtCharts/qdatetimeaxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     6522 2022-09-30 10:26:20.882419 PyQt6_Charts-6.4.0/sip/QtCharts/qhash.sip
--rw-r--r--   0 phil       (501) staff       (20)     1809 2022-09-30 10:26:20.872868 PyQt6_Charts-6.4.0/sip/QtCharts/qhbarmodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1814 2022-09-30 10:26:20.847037 PyQt6_Charts-6.4.0/sip/QtCharts/qhboxplotmodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1946 2022-09-30 10:26:20.888083 PyQt6_Charts-6.4.0/sip/QtCharts/qhcandlestickmodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1247 2022-09-30 10:26:20.884247 PyQt6_Charts-6.4.0/sip/QtCharts/qhorizontalbarseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1282 2022-09-30 10:26:20.880029 PyQt6_Charts-6.4.0/sip/QtCharts/qhorizontalpercentbarseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1282 2022-09-30 10:26:20.883828 PyQt6_Charts-6.4.0/sip/QtCharts/qhorizontalstackedbarseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1757 2022-09-30 10:26:20.883385 PyQt6_Charts-6.4.0/sip/QtCharts/qhpiemodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1711 2022-09-30 10:26:20.874089 PyQt6_Charts-6.4.0/sip/QtCharts/qhxymodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     3472 2022-09-30 10:26:20.876839 PyQt6_Charts-6.4.0/sip/QtCharts/qlegend.sip
--rw-r--r--   0 phil       (501) staff       (20)     2161 2022-09-30 10:26:20.888592 PyQt6_Charts-6.4.0/sip/QtCharts/qlegendmarker.sip
--rw-r--r--   0 phil       (501) staff       (20)     1193 2022-09-30 10:26:20.851006 PyQt6_Charts-6.4.0/sip/QtCharts/qlineseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1906 2022-09-30 10:26:20.877692 PyQt6_Charts-6.4.0/sip/QtCharts/qlogvalueaxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     1232 2022-09-30 10:26:20.884828 PyQt6_Charts-6.4.0/sip/QtCharts/qpercentbarseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1324 2022-09-30 10:26:20.872284 PyQt6_Charts-6.4.0/sip/QtCharts/qpielegendmarker.sip
--rw-r--r--   0 phil       (501) staff       (20)     2638 2022-09-30 10:26:20.870645 PyQt6_Charts-6.4.0/sip/QtCharts/qpieseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     3064 2022-09-30 10:26:20.853881 PyQt6_Charts-6.4.0/sip/QtCharts/qpieslice.sip
--rw-r--r--   0 phil       (501) staff       (20)     1774 2022-09-30 10:26:20.890065 PyQt6_Charts-6.4.0/sip/QtCharts/qpolarchart.sip
--rw-r--r--   0 phil       (501) staff       (20)     2181 2022-09-30 10:26:20.887625 PyQt6_Charts-6.4.0/sip/QtCharts/qscatterseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1205 2022-09-30 10:26:20.877208 PyQt6_Charts-6.4.0/sip/QtCharts/qsplineseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     1232 2022-09-30 10:26:20.878348 PyQt6_Charts-6.4.0/sip/QtCharts/qstackedbarseries.sip
--rw-r--r--   0 phil       (501) staff       (20)     2336 2022-09-30 10:26:20.887127 PyQt6_Charts-6.4.0/sip/QtCharts/qvalueaxis.sip
--rw-r--r--   0 phil       (501) staff       (20)     1809 2022-09-30 10:26:20.875015 PyQt6_Charts-6.4.0/sip/QtCharts/qvbarmodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1817 2022-09-30 10:26:20.890547 PyQt6_Charts-6.4.0/sip/QtCharts/qvboxplotmodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1910 2022-09-30 10:26:20.874579 PyQt6_Charts-6.4.0/sip/QtCharts/qvcandlestickmodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1757 2022-09-30 10:26:20.882891 PyQt6_Charts-6.4.0/sip/QtCharts/qvpiemodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1711 2022-09-30 10:26:20.886400 PyQt6_Charts-6.4.0/sip/QtCharts/qvxymodelmapper.sip
--rw-r--r--   0 phil       (501) staff       (20)     1275 2022-09-30 10:26:20.876030 PyQt6_Charts-6.4.0/sip/QtCharts/qxylegendmarker.sip
--rw-r--r--   0 phil       (501) staff       (20)     7493 2022-09-30 10:26:20.853181 PyQt6_Charts-6.4.0/sip/QtCharts/qxyseries.sip
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:21:13.516691 PyQt6_Charts-6.5.0/
+-rw-r--r--   0 phil       (501) staff       (20)     4118 2023-04-04 15:21:12.851539 PyQt6_Charts-6.5.0/ChangeLog
+-rw-r--r--   0 phil       (501) staff       (20)    35147 2023-04-04 15:21:12.685804 PyQt6_Charts-6.5.0/LICENSE
+-rw-r--r--   0 phil       (501) staff       (20)      393 2023-04-04 15:19:46.373401 PyQt6_Charts-6.5.0/NEWS
+-rw-r--r--   0 phil       (501) staff       (20)     1551 2023-04-04 15:21:13.516805 PyQt6_Charts-6.5.0/PKG-INFO
+-rw-r--r--   0 phil       (501) staff       (20)     1229 2023-04-04 15:21:12.852507 PyQt6_Charts-6.5.0/README
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:21:13.495249 PyQt6_Charts-6.5.0/examples/
+-rw-r--r--   0 phil       (501) staff       (20)     2013 2023-04-04 15:19:46.377745 PyQt6_Charts-6.5.0/examples/areachart.py
+-rw-r--r--   0 phil       (501) staff       (20)     1934 2023-04-04 15:19:46.378422 PyQt6_Charts-6.5.0/examples/barchart.py
+-rw-r--r--   0 phil       (501) staff       (20)     5710 2023-04-04 15:19:46.378996 PyQt6_Charts-6.5.0/examples/barmodelmapper.py
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:21:13.496150 PyQt6_Charts-6.5.0/examples/boxplotchart/
+-rw-r--r--   0 phil       (501) staff       (20)     1583 2023-04-04 15:19:46.379835 PyQt6_Charts-6.5.0/examples/boxplotchart/acme_data.txt
+-rw-r--r--   0 phil       (501) staff       (20)     3433 2023-04-04 15:19:46.380508 PyQt6_Charts-6.5.0/examples/boxplotchart/boxplotchart.py
+-rw-r--r--   0 phil       (501) staff       (20)     1587 2023-04-04 15:19:46.381010 PyQt6_Charts-6.5.0/examples/boxplotchart/boxwhisk_data.txt
+-rw-r--r--   0 phil       (501) staff       (20)    12540 2023-04-04 15:19:46.381565 PyQt6_Charts-6.5.0/examples/chartthemes.py
+-rw-r--r--   0 phil       (501) staff       (20)     3894 2023-04-04 15:19:46.382125 PyQt6_Charts-6.5.0/examples/donutbreakdown.py
+-rw-r--r--   0 phil       (501) staff       (20)     2103 2023-04-04 15:19:46.382684 PyQt6_Charts-6.5.0/examples/horizontalbarchart.py
+-rw-r--r--   0 phil       (501) staff       (20)     2100 2023-04-04 15:19:46.383229 PyQt6_Charts-6.5.0/examples/horizontalpercentbarchart.py
+-rw-r--r--   0 phil       (501) staff       (20)     2100 2023-04-04 15:19:46.383720 PyQt6_Charts-6.5.0/examples/horizontalstackedbarchart.py
+-rw-r--r--   0 phil       (501) staff       (20)     5747 2023-04-04 15:19:46.384219 PyQt6_Charts-6.5.0/examples/modeldata.py
+-rw-r--r--   0 phil       (501) staff       (20)     1998 2023-04-04 15:19:46.384748 PyQt6_Charts-6.5.0/examples/percentbarchart.py
+-rw-r--r--   0 phil       (501) staff       (20)     5662 2023-04-04 15:19:46.385341 PyQt6_Charts-6.5.0/examples/polarchart.py
+-rw-r--r--   0 phil       (501) staff       (20)      793 2023-04-04 15:21:12.852815 PyQt6_Charts-6.5.0/pyproject.toml
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:21:13.496602 PyQt6_Charts-6.5.0/sip/
+drwxr-xr-x   0 phil       (501) staff       (20)        0 2023-04-04 15:21:13.516306 PyQt6_Charts-6.5.0/sip/QtCharts/
+-rw-r--r--   0 phil       (501) staff       (20)     3682 2023-04-04 15:21:13.283779 PyQt6_Charts-6.5.0/sip/QtCharts/QtChartsmod.sip
+-rw-r--r--   0 phil       (501) staff       (20)     5341 2023-04-04 15:21:13.305215 PyQt6_Charts-6.5.0/sip/QtCharts/qabstractaxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2795 2023-04-04 15:21:13.285104 PyQt6_Charts-6.5.0/sip/QtCharts/qabstractbarseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6115 2023-04-04 15:21:13.283033 PyQt6_Charts-6.5.0/sip/QtCharts/qabstractseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1289 2023-04-04 15:21:13.286500 PyQt6_Charts-6.5.0/sip/QtCharts/qarealegendmarker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2869 2023-04-04 15:21:13.313101 PyQt6_Charts-6.5.0/sip/QtCharts/qareaseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2071 2023-04-04 15:21:13.306819 PyQt6_Charts-6.5.0/sip/QtCharts/qbarcategoryaxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1338 2023-04-04 15:21:13.308878 PyQt6_Charts-6.5.0/sip/QtCharts/qbarlegendmarker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1197 2023-04-04 15:21:13.289508 PyQt6_Charts-6.5.0/sip/QtCharts/qbarseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3837 2023-04-04 15:21:13.324889 PyQt6_Charts-6.5.0/sip/QtCharts/qbarset.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1310 2023-04-04 15:21:13.286047 PyQt6_Charts-6.5.0/sip/QtCharts/qboxplotlegendmarker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2225 2023-04-04 15:21:13.323145 PyQt6_Charts-6.5.0/sip/QtCharts/qboxplotseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2224 2023-04-04 15:21:13.284402 PyQt6_Charts-6.5.0/sip/QtCharts/qboxset.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1338 2023-04-04 15:21:13.289083 PyQt6_Charts-6.5.0/sip/QtCharts/qcandlesticklegendmarker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1902 2023-04-04 15:21:13.281920 PyQt6_Charts-6.5.0/sip/QtCharts/qcandlestickmodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3169 2023-04-04 15:21:13.314208 PyQt6_Charts-6.5.0/sip/QtCharts/qcandlestickseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2005 2023-04-04 15:21:13.322598 PyQt6_Charts-6.5.0/sip/QtCharts/qcandlestickset.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1985 2023-04-04 15:21:13.325836 PyQt6_Charts-6.5.0/sip/QtCharts/qcategoryaxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     4333 2023-04-04 15:21:13.312460 PyQt6_Charts-6.5.0/sip/QtCharts/qchart.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2358 2023-04-04 15:21:13.319234 PyQt6_Charts-6.5.0/sip/QtCharts/qchartview.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1945 2023-04-04 15:21:13.318640 PyQt6_Charts-6.5.0/sip/QtCharts/qcoloraxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1707 2023-04-04 15:21:13.325363 PyQt6_Charts-6.5.0/sip/QtCharts/qdatetimeaxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     6522 2023-04-04 15:21:13.315734 PyQt6_Charts-6.5.0/sip/QtCharts/qhash.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1809 2023-04-04 15:21:13.306258 PyQt6_Charts-6.5.0/sip/QtCharts/qhbarmodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1814 2023-04-04 15:21:13.281323 PyQt6_Charts-6.5.0/sip/QtCharts/qhboxplotmodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1946 2023-04-04 15:21:13.321451 PyQt6_Charts-6.5.0/sip/QtCharts/qhcandlestickmodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1247 2023-04-04 15:21:13.317674 PyQt6_Charts-6.5.0/sip/QtCharts/qhorizontalbarseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1282 2023-04-04 15:21:13.313539 PyQt6_Charts-6.5.0/sip/QtCharts/qhorizontalpercentbarseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1282 2023-04-04 15:21:13.317242 PyQt6_Charts-6.5.0/sip/QtCharts/qhorizontalstackedbarseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1757 2023-04-04 15:21:13.316777 PyQt6_Charts-6.5.0/sip/QtCharts/qhpiemodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1711 2023-04-04 15:21:13.307377 PyQt6_Charts-6.5.0/sip/QtCharts/qhxymodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3472 2023-04-04 15:21:13.310164 PyQt6_Charts-6.5.0/sip/QtCharts/qlegend.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2161 2023-04-04 15:21:13.322038 PyQt6_Charts-6.5.0/sip/QtCharts/qlegendmarker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1193 2023-04-04 15:21:13.285582 PyQt6_Charts-6.5.0/sip/QtCharts/qlineseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1906 2023-04-04 15:21:13.311174 PyQt6_Charts-6.5.0/sip/QtCharts/qlogvalueaxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1232 2023-04-04 15:21:13.318096 PyQt6_Charts-6.5.0/sip/QtCharts/qpercentbarseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1324 2023-04-04 15:21:13.305717 PyQt6_Charts-6.5.0/sip/QtCharts/qpielegendmarker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2638 2023-04-04 15:21:13.304001 PyQt6_Charts-6.5.0/sip/QtCharts/qpieseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     3064 2023-04-04 15:21:13.288648 PyQt6_Charts-6.5.0/sip/QtCharts/qpieslice.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1774 2023-04-04 15:21:13.323603 PyQt6_Charts-6.5.0/sip/QtCharts/qpolarchart.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2181 2023-04-04 15:21:13.320925 PyQt6_Charts-6.5.0/sip/QtCharts/qscatterseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1205 2023-04-04 15:21:13.310601 PyQt6_Charts-6.5.0/sip/QtCharts/qsplineseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1232 2023-04-04 15:21:13.311625 PyQt6_Charts-6.5.0/sip/QtCharts/qstackedbarseries.sip
+-rw-r--r--   0 phil       (501) staff       (20)     2336 2023-04-04 15:21:13.320353 PyQt6_Charts-6.5.0/sip/QtCharts/qvalueaxis.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1809 2023-04-04 15:21:13.308429 PyQt6_Charts-6.5.0/sip/QtCharts/qvbarmodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1817 2023-04-04 15:21:13.324087 PyQt6_Charts-6.5.0/sip/QtCharts/qvboxplotmodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1910 2023-04-04 15:21:13.307914 PyQt6_Charts-6.5.0/sip/QtCharts/qvcandlestickmodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1757 2023-04-04 15:21:13.316261 PyQt6_Charts-6.5.0/sip/QtCharts/qvpiemodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1711 2023-04-04 15:21:13.319733 PyQt6_Charts-6.5.0/sip/QtCharts/qvxymodelmapper.sip
+-rw-r--r--   0 phil       (501) staff       (20)     1275 2023-04-04 15:21:13.309331 PyQt6_Charts-6.5.0/sip/QtCharts/qxylegendmarker.sip
+-rw-r--r--   0 phil       (501) staff       (20)     7542 2023-04-04 15:21:13.287919 PyQt6_Charts-6.5.0/sip/QtCharts/qxyseries.sip
```

### Comparing `PyQt6_Charts-6.4.0/ChangeLog` & `PyQt6_Charts-6.5.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,19 @@
+2023-03-31  Phil Thompson  <phil@riverbankcomputing.com>
+
+	* NEWS, PyQt6-Charts.msp:
+	Updated for Qt v6.5.0.rc.
+	[80730b8fbcef] [6.5.0]
+
 2022-09-30  Phil Thompson  <phil@riverbankcomputing.com>
 
+	* .hgtags:
+	Added tag 6.4.0 for changeset c37cd695337f
+	[534374109ee7]
+
 	* NEWS, PyQt6-Charts.msp:
 	Updated for Qt v6.4.0.
 	[c37cd695337f] [6.4.0]
 
 2022-09-21  Phil Thompson  <phil@riverbankcomputing.com>
 
 	* NEWS, PyQt6-Charts.msp:
```

### Comparing `PyQt6_Charts-6.4.0/LICENSE` & `PyQt6_Charts-6.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/PKG-INFO` & `PyQt6_Charts-6.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyQt6-Charts
-Version: 6.4.0
+Version: 6.5.0
 Requires-Python: >=3.7
 Summary: Python bindings for the Qt Charts library
 Home-Page: https://www.riverbankcomputing.com/software/pyqtchart/
 Author: Riverbank Computing Limited
 Author-Email: info@riverbankcomputing.com
 License: GPL v3
 Requires-Dist: PyQt6 (>=6.2.0)
```

### Comparing `PyQt6_Charts-6.4.0/README` & `PyQt6_Charts-6.5.0/README`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/examples/areachart.py` & `PyQt6_Charts-6.5.0/examples/areachart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/examples/barchart.py` & `PyQt6_Charts-6.5.0/examples/barchart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/examples/barmodelmapper.py` & `PyQt6_Charts-6.5.0/examples/barmodelmapper.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/examples/boxplotchart/acme_data.txt` & `PyQt6_Charts-6.5.0/examples/boxplotchart/acme_data.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/examples/boxplotchart/boxplotchart.py` & `PyQt6_Charts-6.5.0/examples/boxplotchart/boxplotchart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/examples/boxplotchart/boxwhisk_data.txt` & `PyQt6_Charts-6.5.0/examples/boxplotchart/boxwhisk_data.txt`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/examples/chartthemes.py` & `PyQt6_Charts-6.5.0/examples/chartthemes.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/examples/donutbreakdown.py` & `PyQt6_Charts-6.5.0/examples/donutbreakdown.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/examples/horizontalbarchart.py` & `PyQt6_Charts-6.5.0/examples/horizontalbarchart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/examples/horizontalpercentbarchart.py` & `PyQt6_Charts-6.5.0/examples/horizontalpercentbarchart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/examples/horizontalstackedbarchart.py` & `PyQt6_Charts-6.5.0/examples/horizontalstackedbarchart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/examples/modeldata.py` & `PyQt6_Charts-6.5.0/examples/modeldata.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/examples/percentbarchart.py` & `PyQt6_Charts-6.5.0/examples/percentbarchart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/examples/polarchart.py` & `PyQt6_Charts-6.5.0/examples/polarchart.py`

 * *Files identical despite different names*

### Comparing `PyQt6_Charts-6.4.0/pyproject.toml` & `PyQt6_Charts-6.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 [build-system]
 requires = ["sip >=6, <7", "PyQt-builder >=1.10, <2"]
 build-backend = "sipbuild.api"
 
 # Specify the PEP 566 metadata for the project.
 [tool.sip.metadata]
 name = "PyQt6-Charts"
-version = "6.4.0"
+version = "6.5.0"
 summary = "Python bindings for the Qt Charts library"
 home-page = "https://www.riverbankcomputing.com/software/pyqtchart/"
 author = "Riverbank Computing Limited"
 author-email = "info@riverbankcomputing.com"
 license = "GPL v3"
 description-file = "README"
 requires-dist = "PyQt6 (>=6.2.0)"
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/QtChartsmod.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/QtChartsmod.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // QtChartsmod.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -21,18 +21,18 @@
 
 
 %Module(name=PyQt6.QtCharts, keyword_arguments="Optional", use_limited_api=True)
 
 %Import QtGui/QtGuimod.sip
 %Import QtWidgets/QtWidgetsmod.sip
 
-%Timeline {QtCharts_6_0_0 QtCharts_6_1_0 QtCharts_6_2_0 QtCharts_6_3_0 QtCharts_6_4_0}
+%Timeline {QtCharts_6_0_0 QtCharts_6_1_0 QtCharts_6_2_0 QtCharts_6_3_0 QtCharts_6_4_0 QtCharts_6_5_0}
 
 %Copying
-Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 
 This file is part of PyQt6-Charts.
 
 This file may be used under the terms of the GNU General Public License
 version 3.0 as published by the Free Software Foundation and appearing in
 the file LICENSE included in the packaging of this file.  Please review the
 following information to ensure the GNU General Public License version 3.0
@@ -48,16 +48,16 @@
 
 %DefaultSupertype PyQt6.sip.simplewrapper
 
 int PYQT_CHART_VERSION;
 const char *PYQT_CHART_VERSION_STR;
 
 %ModuleCode
-static int PYQT_CHART_VERSION = 0x060400;
-static const char *PYQT_CHART_VERSION_STR = "6.4.0";
+static int PYQT_CHART_VERSION = 0x060500;
+static const char *PYQT_CHART_VERSION_STR = "6.5.0";
 %End
 
 %Include qabstractaxis.sip
 %Include qabstractbarseries.sip
 %Include qabstractseries.sip
 %Include qarealegendmarker.sip
 %Include qareaseries.sip
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qabstractaxis.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qabstractaxis.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractaxis.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qabstractbarseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qabstractbarseries.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractbarseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qabstractseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qabstractseries.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qabstractseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qarealegendmarker.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qarealegendmarker.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qarealegendmarker.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qareaseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qareaseries.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qareaseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qbarcategoryaxis.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qbarcategoryaxis.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbarcategoryaxis.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qbarlegendmarker.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qbarlegendmarker.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbarlegendmarker.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qbarseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qbarseries.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbarseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qbarset.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qbarset.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qbarset.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qboxplotlegendmarker.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qboxplotlegendmarker.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qboxplotlegendmarker.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qboxplotseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qboxplotseries.sip`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qboxplotseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qboxset.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qboxset.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qboxset.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qcandlesticklegendmarker.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qcandlesticklegendmarker.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcandlesticklegendmarker.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qcandlestickmodelmapper.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qcandlestickmodelmapper.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcandlestickmodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qcandlestickseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qcandlestickseries.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcandlestickseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qcandlestickset.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qcandlestickset.sip`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcandlestickset.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qcategoryaxis.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qcategoryaxis.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcategoryaxis.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qchart.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qchart.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qchart.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qchartview.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qchartview.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qchartview.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qcoloraxis.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qcoloraxis.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qcoloraxis.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qdatetimeaxis.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qdatetimeaxis.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qdatetimeaxis.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qhash.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qhash.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 // This is the SIP interface definition for the QHash based mapped types
 // specific to the QtCharts module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qhbarmodelmapper.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qhbarmodelmapper.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhbarmodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qhboxplotmodelmapper.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qhboxplotmodelmapper.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhboxplotmodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qhcandlestickmodelmapper.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qhcandlestickmodelmapper.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhcandlestickmodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qhorizontalbarseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qhorizontalbarseries.sip`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhorizontalbarseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qhorizontalpercentbarseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qhorizontalpercentbarseries.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhorizontalpercentbarseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qhorizontalstackedbarseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qhorizontalstackedbarseries.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhorizontalstackedbarseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qhpiemodelmapper.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qhpiemodelmapper.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhpiemodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qhxymodelmapper.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qhxymodelmapper.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qhxymodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qlegend.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qlegend.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlegend.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qlegendmarker.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qlegendmarker.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlegendmarker.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qlineseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qlineseries.sip`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlineseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qlogvalueaxis.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qlogvalueaxis.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qlogvalueaxis.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qpercentbarseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qpercentbarseries.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpercentbarseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qpielegendmarker.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qpielegendmarker.sip`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpielegendmarker.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qpieseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qpieseries.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpieseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qpieslice.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qpieslice.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpieslice.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qpolarchart.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qpolarchart.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qpolarchart.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qscatterseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qscatterseries.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qscatterseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qsplineseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qsplineseries.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qsplineseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qstackedbarseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qstackedbarseries.sip`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qstackedbarseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qvalueaxis.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qvalueaxis.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvalueaxis.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qvbarmodelmapper.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qvbarmodelmapper.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvbarmodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qvboxplotmodelmapper.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qvboxplotmodelmapper.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvboxplotmodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qvcandlestickmodelmapper.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qvcandlestickmodelmapper.sip`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvcandlestickmodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qvpiemodelmapper.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qvpiemodelmapper.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvpiemodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qvxymodelmapper.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qvxymodelmapper.sip`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qvxymodelmapper.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qxylegendmarker.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qxylegendmarker.sip`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qxylegendmarker.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
```

### Comparing `PyQt6_Charts-6.4.0/sip/QtCharts/qxyseries.sip` & `PyQt6_Charts-6.5.0/sip/QtCharts/qxyseries.sip`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 // qxyseries.sip generated by MetaSIP
 //
 // This file is part of the QtCharts Python extension module.
 //
-// Copyright (c) 2022 Riverbank Computing Limited <info@riverbankcomputing.com>
+// Copyright (c) 2023 Riverbank Computing Limited <info@riverbankcomputing.com>
 // 
 // This file is part of PyQt6-Charts.
 // 
 // This file may be used under the terms of the GNU General Public License
 // version 3.0 as published by the Free Software Foundation and appearing in
 // the file LICENSE included in the packaging of this file.  Please review the
 // following information to ensure the GNU General Public License version 3.0
@@ -98,14 +98,17 @@
 
     enum class PointConfiguration
     {
         Color,
         Size,
         Visibility,
         LabelVisibility,
+%If (QtCharts_6_5_0 -)
+        LabelFormat,
+%End
     };
 
 %End
 %If (QtCharts_6_2_0 -)
     void setSelectedColor(const QColor &color);
 %End
 %If (QtCharts_6_2_0 -)
```

