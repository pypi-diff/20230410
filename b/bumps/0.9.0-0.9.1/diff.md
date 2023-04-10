# Comparing `tmp/bumps-0.9.0.tar.gz` & `tmp/bumps-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bumps-0.9.0.tar", last modified: Wed Mar 16 00:43:40 2022, max compression
+gzip compressed data, was "bumps-0.9.1.tar", last modified: Mon Apr 10 16:22:33 2023, max compression
```

## Comparing `bumps-0.9.0.tar` & `bumps-0.9.1.tar`

### file list

```diff
@@ -1,145 +1,147 @@
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2022-03-16 00:43:40.336136 bumps-0.9.0/
--rwxr-xr-x   0 pkienzle (34766)    34766      803 2020-11-19 22:11:15.000000 bumps-0.9.0/MANIFEST.in
--rw-r--r--   0 pkienzle (34766)    34766    11985 2022-03-16 00:43:40.335444 bumps-0.9.0/PKG-INFO
--rwxr-xr-x   0 pkienzle (34766)    34766     9150 2022-03-16 00:33:59.000000 bumps-0.9.0/README.rst
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2022-03-16 00:43:40.157045 bumps-0.9.0/bin/
--rwxr-xr-x   0 pkienzle (34766)    34766      722 2014-02-04 18:07:02.000000 bumps-0.9.0/bin/bumps
--rw-r--r--   0 pkienzle (34766)    34766       33 2020-09-11 19:45:21.000000 bumps-0.9.0/bin/bumps.bat
--rwxr-xr-x   0 pkienzle (34766)    34766      738 2014-02-04 18:07:02.000000 bumps-0.9.0/bin/bumps_gui
--rwxr-xr-x   0 pkienzle (34766)    34766      121 2014-02-04 18:07:02.000000 bumps-0.9.0/bin/bumps_serve
--rwxr-xr-x   0 pkienzle (34766)    34766      841 2014-02-04 18:07:02.000000 bumps-0.9.0/bin/bumps_workerd
--rwxr-xr-x   0 pkienzle (34766)    34766      149 2014-02-04 18:07:02.000000 bumps-0.9.0/bin/launch.bat
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2022-03-16 00:43:40.214360 bumps-0.9.0/bumps/
--rw-r--r--   0 pkienzle (34766)    34766     1222 2022-03-15 22:08:58.000000 bumps-0.9.0/bumps/__init__.py
--rw-r--r--   0 pkienzle (34766)    34766    23582 2021-05-28 20:00:46.000000 bumps-0.9.0/bumps/bounds.py
--rw-r--r--   0 pkienzle (34766)    34766    13115 2020-11-19 22:11:15.000000 bumps-0.9.0/bumps/bspline.py
--rw-r--r--   0 pkienzle (34766)    34766     6579 2017-05-09 19:02:36.000000 bumps-0.9.0/bumps/cheby.py
--rw-r--r--   0 pkienzle (34766)    34766    25958 2020-12-16 20:29:47.000000 bumps-0.9.0/bumps/cli.py
--rw-r--r--   0 pkienzle (34766)    34766    17874 2021-06-15 17:44:44.000000 bumps-0.9.0/bumps/curve.py
--rw-r--r--   0 pkienzle (34766)    34766     8808 2020-11-19 22:11:15.000000 bumps-0.9.0/bumps/data.py
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2022-03-16 00:43:40.263157 bumps-0.9.0/bumps/dream/
--rw-r--r--   0 pkienzle (34766)    34766      675 2016-10-25 13:55:16.000000 bumps-0.9.0/bumps/dream/__init__.py
--rw-r--r--   0 pkienzle (34766)    34766     2884 2015-06-03 19:03:53.000000 bumps-0.9.0/bumps/dream/acr.py
--rw-r--r--   0 pkienzle (34766)    34766     7251 2020-11-19 22:11:15.000000 bumps-0.9.0/bumps/dream/bounds.py
--rw-r--r--   0 pkienzle (34766)    34766      208 2020-11-19 22:11:15.000000 bumps-0.9.0/bumps/dream/compiled.py
--rw-r--r--   0 pkienzle (34766)    34766     9375 2020-12-16 20:29:47.000000 bumps-0.9.0/bumps/dream/convergence.py
--rw-r--r--   0 pkienzle (34766)    34766    19787 2020-12-16 20:29:47.000000 bumps-0.9.0/bumps/dream/core.py
--rw-r--r--   0 pkienzle (34766)    34766     5560 2020-09-11 19:45:22.000000 bumps-0.9.0/bumps/dream/corrplot.py
--rw-r--r--   0 pkienzle (34766)    34766     6586 2020-11-19 22:11:15.000000 bumps-0.9.0/bumps/dream/crossover.py
--rw-r--r--   0 pkienzle (34766)    34766     6181 2020-11-19 22:11:15.000000 bumps-0.9.0/bumps/dream/diffev.py
--rw-r--r--   0 pkienzle (34766)    34766     6686 2020-12-16 20:29:47.000000 bumps-0.9.0/bumps/dream/digits.py
--rw-r--r--   0 pkienzle (34766)    34766    45857 2020-12-16 20:29:47.000000 bumps-0.9.0/bumps/dream/entropy.py
--rw-r--r--   0 pkienzle (34766)    34766     1254 2020-09-11 19:45:22.000000 bumps-0.9.0/bumps/dream/exppow.py
--rw-r--r--   0 pkienzle (34766)    34766    19681 2020-12-16 23:04:24.000000 bumps-0.9.0/bumps/dream/formatnum.py
--rw-r--r--   0 pkienzle (34766)    34766     2745 2021-05-28 20:00:46.000000 bumps-0.9.0/bumps/dream/gelman.py
--rw-r--r--   0 pkienzle (34766)    34766     2134 2020-09-11 19:45:22.000000 bumps-0.9.0/bumps/dream/geweke.py
--rw-r--r--   0 pkienzle (34766)    34766     2953 2016-10-25 13:55:16.000000 bumps-0.9.0/bumps/dream/initpop.py
--rw-r--r--   0 pkienzle (34766)    34766     1159 2020-09-11 19:45:22.000000 bumps-0.9.0/bumps/dream/ksmirnov.py
--rw-r--r--   0 pkienzle (34766)    34766     1672 2015-05-05 21:06:09.000000 bumps-0.9.0/bumps/dream/mahal.py
--rw-r--r--   0 pkienzle (34766)    34766     8025 2020-12-16 20:29:47.000000 bumps-0.9.0/bumps/dream/matlab.py
--rw-r--r--   0 pkienzle (34766)    34766     2661 2020-09-11 19:45:22.000000 bumps-0.9.0/bumps/dream/metropolis.py
--rw-r--r--   0 pkienzle (34766)    34766     7043 2020-11-19 22:11:15.000000 bumps-0.9.0/bumps/dream/model.py
--rw-r--r--   0 pkienzle (34766)    34766     6432 2020-12-16 20:29:47.000000 bumps-0.9.0/bumps/dream/outliers.py
--rw-r--r--   0 pkienzle (34766)    34766     6548 2021-05-28 20:00:46.000000 bumps-0.9.0/bumps/dream/parcoord.py
--rw-r--r--   0 pkienzle (34766)    34766    43644 2020-12-16 20:29:47.000000 bumps-0.9.0/bumps/dream/state.py
--rw-r--r--   0 pkienzle (34766)    34766    10285 2020-12-16 20:29:47.000000 bumps-0.9.0/bumps/dream/stats.py
--rw-r--r--   0 pkienzle (34766)    34766     1541 2017-05-09 20:01:14.000000 bumps-0.9.0/bumps/dream/tile.py
--rw-r--r--   0 pkienzle (34766)    34766     2341 2016-10-25 13:55:16.000000 bumps-0.9.0/bumps/dream/util.py
--rw-r--r--   0 pkienzle (34766)    34766    11510 2022-01-13 19:13:14.000000 bumps-0.9.0/bumps/dream/varplot.py
--rw-r--r--   0 pkienzle (34766)    34766     9021 2022-03-15 23:00:44.000000 bumps-0.9.0/bumps/dream/views.py
--rw-r--r--   0 pkienzle (34766)    34766     3812 2015-07-27 16:17:03.000000 bumps-0.9.0/bumps/dream/walk.py
--rw-r--r--   0 pkienzle (34766)    34766     5134 2020-12-16 20:29:47.000000 bumps-0.9.0/bumps/errplot.py
--rw-r--r--   0 pkienzle (34766)    34766    30067 2022-01-13 19:13:27.000000 bumps-0.9.0/bumps/fitproblem.py
--rw-r--r--   0 pkienzle (34766)    34766     3235 2020-11-19 22:11:15.000000 bumps-0.9.0/bumps/fitservice.py
--rw-r--r--   0 pkienzle (34766)    34766    47892 2022-02-15 17:21:08.000000 bumps-0.9.0/bumps/fitters.py
--rw-r--r--   0 pkienzle (34766)    34766    19680 2020-12-16 23:04:24.000000 bumps-0.9.0/bumps/formatnum.py
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2022-03-16 00:43:40.286725 bumps-0.9.0/bumps/gui/
--rw-r--r--   0 pkienzle (34766)    34766        0 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/gui/__init__.py
--rw-r--r--   0 pkienzle (34766)    34766     7520 2014-05-27 18:39:51.000000 bumps-0.9.0/bumps/gui/about.py
--rw-r--r--   0 pkienzle (34766)    34766     9217 2020-11-19 22:11:15.000000 bumps-0.9.0/bumps/gui/app_frame.py
--rw-r--r--   0 pkienzle (34766)    34766    27819 2021-05-28 20:00:46.000000 bumps-0.9.0/bumps/gui/app_panel.py
--rw-r--r--   0 pkienzle (34766)    34766     6721 2016-10-25 13:55:16.000000 bumps-0.9.0/bumps/gui/console.py
--rw-r--r--   0 pkienzle (34766)    34766     2351 2020-11-19 22:11:15.000000 bumps-0.9.0/bumps/gui/convergence_view.py
--rwxr-xr-x   0 pkienzle (34766)    34766     8337 2021-05-28 20:00:46.000000 bumps-0.9.0/bumps/gui/data_view.py
--rw-r--r--   0 pkienzle (34766)    34766    11556 2020-11-19 22:11:15.000000 bumps-0.9.0/bumps/gui/fit_dialog.py
--rw-r--r--   0 pkienzle (34766)    34766     8830 2020-11-19 22:11:15.000000 bumps-0.9.0/bumps/gui/fit_thread.py
--rwxr-xr-x   0 pkienzle (34766)    34766     1845 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/gui/fit_view.py
--rwxr-xr-x   0 pkienzle (34766)    34766    13695 2021-05-28 20:00:53.000000 bumps-0.9.0/bumps/gui/gui_app.py
--rw-r--r--   0 pkienzle (34766)    34766    49071 2020-11-19 22:11:16.000000 bumps-0.9.0/bumps/gui/input_list.py
--rwxr-xr-x   0 pkienzle (34766)    34766     1339 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/gui/log_view.py
--rw-r--r--   0 pkienzle (34766)    34766     9551 2014-06-02 21:33:58.000000 bumps-0.9.0/bumps/gui/parameter_grid.py
--rwxr-xr-x   0 pkienzle (34766)    34766    13099 2022-01-13 19:13:27.000000 bumps-0.9.0/bumps/gui/parameter_view.py
--rw-r--r--   0 pkienzle (34766)    34766     7415 2020-11-19 22:11:16.000000 bumps-0.9.0/bumps/gui/plot_view.py
--rw-r--r--   0 pkienzle (34766)    34766     5965 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/gui/resfiles.py
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2022-03-16 00:43:40.311404 bumps-0.9.0/bumps/gui/resources/
--rw-r--r--   0 pkienzle (34766)    34766      336 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/gui/resources/__init__.py
--rw-r--r--   0 pkienzle (34766)    34766   353118 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/gui/resources/bumps.ico
--rw-r--r--   0 pkienzle (34766)    34766    73466 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/gui/resources/bumps_splash.jpg
--rw-r--r--   0 pkienzle (34766)    34766     2196 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/gui/resources/done.wav
--rwxr-xr-x   0 pkienzle (34766)    34766     1166 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/gui/resources/import_script.png
--rwxr-xr-x   0 pkienzle (34766)    34766     6235 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/gui/resources/reload.png
--rwxr-xr-x   0 pkienzle (34766)    34766     1675 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/gui/resources/start_fit.png
--rwxr-xr-x   0 pkienzle (34766)    34766     1965 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/gui/resources/stop_fit.png
--rw-r--r--   0 pkienzle (34766)    34766     2019 2020-11-19 22:11:16.000000 bumps-0.9.0/bumps/gui/signal.py
--rwxr-xr-x   0 pkienzle (34766)    34766     8687 2022-01-13 19:13:27.000000 bumps-0.9.0/bumps/gui/summary_view.py
--rw-r--r--   0 pkienzle (34766)    34766     2928 2022-01-13 19:13:27.000000 bumps-0.9.0/bumps/gui/uncertainty_view.py
--rwxr-xr-x   0 pkienzle (34766)    34766     4038 2020-11-19 22:11:16.000000 bumps-0.9.0/bumps/gui/util.py
--rw-r--r--   0 pkienzle (34766)    34766    16655 2020-11-19 22:11:16.000000 bumps-0.9.0/bumps/gui/utilities.py
--rw-r--r--   0 pkienzle (34766)    34766     9320 2017-05-09 19:26:16.000000 bumps-0.9.0/bumps/history.py
--rw-r--r--   0 pkienzle (34766)    34766    11284 2021-11-03 14:46:43.000000 bumps-0.9.0/bumps/initpop.py
--rw-r--r--   0 pkienzle (34766)    34766    15050 2020-11-19 22:11:16.000000 bumps-0.9.0/bumps/lsqerror.py
--rw-r--r--   0 pkienzle (34766)    34766    12108 2020-11-19 22:11:16.000000 bumps-0.9.0/bumps/mapper.py
--rw-r--r--   0 pkienzle (34766)    34766     3565 2017-05-09 19:30:52.000000 bumps-0.9.0/bumps/monitor.py
--rw-r--r--   0 pkienzle (34766)    34766     3775 2017-05-09 19:31:14.000000 bumps-0.9.0/bumps/mono.py
--rw-r--r--   0 pkienzle (34766)    34766    88416 2020-11-19 22:11:16.000000 bumps-0.9.0/bumps/mpfit.py
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2022-03-16 00:43:40.317324 bumps-0.9.0/bumps/mystic/
--rw-r--r--   0 pkienzle (34766)    34766        0 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/mystic/__init__.py
--rw-r--r--   0 pkienzle (34766)    34766     8373 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/mystic/condition.py
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2022-03-16 00:43:40.324741 bumps-0.9.0/bumps/mystic/examples/
--rw-r--r--   0 pkienzle (34766)    34766      571 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/mystic/examples/__init__.py
--rw-r--r--   0 pkienzle (34766)    34766     2476 2014-10-29 14:24:38.000000 bumps-0.9.0/bumps/mystic/examples/circle.py
--rw-r--r--   0 pkienzle (34766)    34766     1711 2014-07-20 22:24:06.000000 bumps-0.9.0/bumps/mystic/examples/corana.py
--rw-r--r--   0 pkienzle (34766)    34766     1462 2014-07-20 22:24:18.000000 bumps-0.9.0/bumps/mystic/examples/decay.py
--rw-r--r--   0 pkienzle (34766)    34766     2195 2016-10-25 13:55:16.000000 bumps-0.9.0/bumps/mystic/examples/model.py
--rw-r--r--   0 pkienzle (34766)    34766       45 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/mystic/examples/simple.py
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2022-03-16 00:43:40.327447 bumps-0.9.0/bumps/mystic/optimizer/
--rw-r--r--   0 pkienzle (34766)    34766        0 2014-02-04 18:07:02.000000 bumps-0.9.0/bumps/mystic/optimizer/__init__.py
--rw-r--r--   0 pkienzle (34766)    34766     8484 2020-11-19 22:11:16.000000 bumps-0.9.0/bumps/mystic/optimizer/de.py
--rw-r--r--   0 pkienzle (34766)    34766     5422 2014-10-29 14:26:28.000000 bumps-0.9.0/bumps/mystic/optimizer/diffev_compat.py
--rw-r--r--   0 pkienzle (34766)    34766    10945 2016-10-25 13:55:16.000000 bumps-0.9.0/bumps/mystic/solver.py
--rw-r--r--   0 pkienzle (34766)    34766    25453 2014-07-20 22:22:45.000000 bumps-0.9.0/bumps/mystic/stop.py
--rw-r--r--   0 pkienzle (34766)    34766     2066 2014-07-20 22:23:38.000000 bumps-0.9.0/bumps/mystic/util.py
--rw-r--r--   0 pkienzle (34766)    34766     2196 2021-05-28 20:00:46.000000 bumps-0.9.0/bumps/names.py
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2022-03-16 00:43:40.334041 bumps-0.9.0/bumps/numdifftools/
--rw-r--r--   0 pkienzle (34766)    34766      103 2016-10-25 13:55:16.000000 bumps-0.9.0/bumps/numdifftools/__init__.py
--rw-r--r--   0 pkienzle (34766)    34766    48121 2020-11-19 22:11:16.000000 bumps-0.9.0/bumps/numdifftools/core.py
--rw-r--r--   0 pkienzle (34766)    34766    11684 2016-10-25 13:55:16.000000 bumps-0.9.0/bumps/numdifftools/extrapolation.py
--rw-r--r--   0 pkienzle (34766)    34766     3228 2020-11-19 22:11:16.000000 bumps-0.9.0/bumps/numdifftools/info.py
--rw-r--r--   0 pkienzle (34766)    34766    10033 2016-10-25 13:55:16.000000 bumps-0.9.0/bumps/numdifftools/multicomplex.py
--rw-r--r--   0 pkienzle (34766)    34766     2128 2017-05-09 19:32:28.000000 bumps-0.9.0/bumps/openmp_ext.py
--rw-r--r--   0 pkienzle (34766)    34766    18944 2020-12-16 20:29:47.000000 bumps-0.9.0/bumps/options.py
--rw-r--r--   0 pkienzle (34766)    34766    36566 2021-05-28 20:00:46.000000 bumps-0.9.0/bumps/parameter.py
--rw-r--r--   0 pkienzle (34766)    34766    12581 2016-10-25 13:55:16.000000 bumps-0.9.0/bumps/partemp.py
--rw-r--r--   0 pkienzle (34766)    34766    10408 2020-11-19 22:11:16.000000 bumps-0.9.0/bumps/pdfwrapper.py
--rw-r--r--   0 pkienzle (34766)    34766     5740 2020-11-19 22:11:16.000000 bumps-0.9.0/bumps/plotutil.py
--rw-r--r--   0 pkienzle (34766)    34766     2770 2021-05-28 20:00:46.000000 bumps-0.9.0/bumps/plugin.py
--rw-r--r--   0 pkienzle (34766)    34766     2396 2021-05-28 20:00:46.000000 bumps-0.9.0/bumps/pmath.py
--rw-r--r--   0 pkienzle (34766)    34766     4657 2020-09-11 19:45:22.000000 bumps-0.9.0/bumps/pymcfit.py
--rw-r--r--   0 pkienzle (34766)    34766    21294 2020-09-11 19:45:22.000000 bumps-0.9.0/bumps/pytwalk.py
--rw-r--r--   0 pkienzle (34766)    34766    28707 2016-10-25 13:55:16.000000 bumps-0.9.0/bumps/quasinewton.py
--rw-r--r--   0 pkienzle (34766)    34766     8975 2020-10-30 19:05:36.000000 bumps-0.9.0/bumps/random_lines.py
--rw-r--r--   0 pkienzle (34766)    34766    11236 2020-09-11 19:45:22.000000 bumps-0.9.0/bumps/simplex.py
--rw-r--r--   0 pkienzle (34766)    34766     9448 2021-06-15 17:44:44.000000 bumps-0.9.0/bumps/util.py
--rw-r--r--   0 pkienzle (34766)    34766    16679 2020-11-19 22:11:16.000000 bumps-0.9.0/bumps/vfs.py
--rw-r--r--   0 pkienzle (34766)    34766    15569 2021-03-10 15:46:52.000000 bumps-0.9.0/bumps/wsolve.py
-drwxr-xr-x   0 pkienzle (34766)    34766        0 2022-03-16 00:43:40.221599 bumps-0.9.0/bumps.egg-info/
--rw-r--r--   0 pkienzle (34766)    34766    11985 2022-03-16 00:43:40.000000 bumps-0.9.0/bumps.egg-info/PKG-INFO
--rw-r--r--   0 pkienzle (34766)    34766     2937 2022-03-16 00:43:40.000000 bumps-0.9.0/bumps.egg-info/SOURCES.txt
--rw-r--r--   0 pkienzle (34766)    34766        1 2022-03-16 00:43:40.000000 bumps-0.9.0/bumps.egg-info/dependency_links.txt
--rw-r--r--   0 pkienzle (34766)    34766        4 2022-03-16 00:43:40.000000 bumps-0.9.0/bumps.egg-info/requires.txt
--rw-r--r--   0 pkienzle (34766)    34766        6 2022-03-16 00:43:40.000000 bumps-0.9.0/bumps.egg-info/top_level.txt
--rwxr-xr-x   0 pkienzle (34766)    34766     9470 2014-11-21 21:09:16.000000 bumps-0.9.0/bumps.iss
--rwxr-xr-x   0 pkienzle (34766)    34766    18906 2015-03-26 17:53:23.000000 bumps-0.9.0/master_builder.py
--rw-r--r--   0 pkienzle (34766)    34766       38 2022-03-16 00:43:40.336270 bumps-0.9.0/setup.cfg
--rwxr-xr-x   0 pkienzle (34766)    34766     1877 2021-05-28 20:00:47.000000 bumps-0.9.0/setup.py
--rwxr-xr-x   0 pkienzle (34766)    34766    11841 2014-11-21 21:09:16.000000 bumps-0.9.0/setup_py2exe.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2023-04-10 16:22:33.255187 bumps-0.9.1/
+-rwxr-xr-x   0 pkienzle (34766)    34766      803 2020-11-19 22:11:15.000000 bumps-0.9.1/MANIFEST.in
+-rw-r--r--   0 pkienzle (34766)    34766    12697 2023-04-10 16:22:33.254483 bumps-0.9.1/PKG-INFO
+-rwxr-xr-x   0 pkienzle (34766)    34766     9752 2023-04-10 15:43:17.000000 bumps-0.9.1/README.rst
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2023-04-10 16:22:33.079215 bumps-0.9.1/bin/
+-rwxr-xr-x   0 pkienzle (34766)    34766      722 2014-02-04 18:07:02.000000 bumps-0.9.1/bin/bumps
+-rw-r--r--   0 pkienzle (34766)    34766       33 2020-09-11 19:45:21.000000 bumps-0.9.1/bin/bumps.bat
+-rwxr-xr-x   0 pkienzle (34766)    34766      738 2014-02-04 18:07:02.000000 bumps-0.9.1/bin/bumps_gui
+-rwxr-xr-x   0 pkienzle (34766)    34766      121 2014-02-04 18:07:02.000000 bumps-0.9.1/bin/bumps_serve
+-rwxr-xr-x   0 pkienzle (34766)    34766      841 2014-02-04 18:07:02.000000 bumps-0.9.1/bin/bumps_workerd
+-rwxr-xr-x   0 pkienzle (34766)    34766      149 2014-02-04 18:07:02.000000 bumps-0.9.1/bin/launch.bat
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2023-04-10 16:22:33.134177 bumps-0.9.1/bumps/
+-rw-r--r--   0 pkienzle (34766)    34766     1202 2023-04-10 16:07:18.000000 bumps-0.9.1/bumps/__init__.py
+-rw-r--r--   0 pkienzle (34766)    34766    23582 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/bounds.py
+-rw-r--r--   0 pkienzle (34766)    34766    13115 2020-11-19 22:11:15.000000 bumps-0.9.1/bumps/bspline.py
+-rw-r--r--   0 pkienzle (34766)    34766     6579 2017-05-09 19:02:36.000000 bumps-0.9.1/bumps/cheby.py
+-rw-r--r--   0 pkienzle (34766)    34766    25958 2023-04-04 14:56:25.000000 bumps-0.9.1/bumps/cli.py
+-rw-r--r--   0 pkienzle (34766)    34766    17884 2023-04-10 15:19:38.000000 bumps-0.9.1/bumps/curve.py
+-rw-r--r--   0 pkienzle (34766)    34766     8808 2020-11-19 22:11:15.000000 bumps-0.9.1/bumps/data.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2023-04-10 16:22:33.197720 bumps-0.9.1/bumps/dream/
+-rw-r--r--   0 pkienzle (34766)    34766      675 2016-10-25 13:55:16.000000 bumps-0.9.1/bumps/dream/__init__.py
+-rw-r--r--   0 pkienzle (34766)    34766     2884 2015-06-03 19:03:53.000000 bumps-0.9.1/bumps/dream/acr.py
+-rw-r--r--   0 pkienzle (34766)    34766     7251 2020-11-19 22:11:15.000000 bumps-0.9.1/bumps/dream/bounds.py
+-rw-r--r--   0 pkienzle (34766)    34766      208 2020-11-19 22:11:15.000000 bumps-0.9.1/bumps/dream/compiled.py
+-rw-r--r--   0 pkienzle (34766)    34766     9375 2020-12-16 20:29:47.000000 bumps-0.9.1/bumps/dream/convergence.py
+-rw-r--r--   0 pkienzle (34766)    34766    19787 2022-06-27 14:15:11.000000 bumps-0.9.1/bumps/dream/core.py
+-rw-r--r--   0 pkienzle (34766)    34766     5560 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/dream/corrplot.py
+-rw-r--r--   0 pkienzle (34766)    34766     6586 2020-11-19 22:11:15.000000 bumps-0.9.1/bumps/dream/crossover.py
+-rw-r--r--   0 pkienzle (34766)    34766     6181 2020-11-19 22:11:15.000000 bumps-0.9.1/bumps/dream/diffev.py
+-rw-r--r--   0 pkienzle (34766)    34766     6686 2020-12-16 20:29:47.000000 bumps-0.9.1/bumps/dream/digits.py
+-rw-r--r--   0 pkienzle (34766)    34766    46065 2023-04-04 14:56:25.000000 bumps-0.9.1/bumps/dream/entropy.py
+-rw-r--r--   0 pkienzle (34766)    34766     1254 2020-09-11 19:45:22.000000 bumps-0.9.1/bumps/dream/exppow.py
+-rw-r--r--   0 pkienzle (34766)    34766    19681 2020-12-16 23:04:24.000000 bumps-0.9.1/bumps/dream/formatnum.py
+-rw-r--r--   0 pkienzle (34766)    34766     2745 2022-04-29 18:13:57.000000 bumps-0.9.1/bumps/dream/gelman.py
+-rw-r--r--   0 pkienzle (34766)    34766     2134 2020-09-11 19:45:22.000000 bumps-0.9.1/bumps/dream/geweke.py
+-rw-r--r--   0 pkienzle (34766)    34766     2953 2016-10-25 13:55:16.000000 bumps-0.9.1/bumps/dream/initpop.py
+-rw-r--r--   0 pkienzle (34766)    34766     1159 2020-09-11 19:45:22.000000 bumps-0.9.1/bumps/dream/ksmirnov.py
+-rw-r--r--   0 pkienzle (34766)    34766     1672 2015-05-05 21:06:09.000000 bumps-0.9.1/bumps/dream/mahal.py
+-rw-r--r--   0 pkienzle (34766)    34766     8025 2020-12-16 20:29:47.000000 bumps-0.9.1/bumps/dream/matlab.py
+-rw-r--r--   0 pkienzle (34766)    34766     2661 2020-09-11 19:45:22.000000 bumps-0.9.1/bumps/dream/metropolis.py
+-rw-r--r--   0 pkienzle (34766)    34766     7043 2020-11-19 22:11:15.000000 bumps-0.9.1/bumps/dream/model.py
+-rw-r--r--   0 pkienzle (34766)    34766     6432 2020-12-16 20:29:47.000000 bumps-0.9.1/bumps/dream/outliers.py
+-rw-r--r--   0 pkienzle (34766)    34766     6548 2022-04-29 18:13:57.000000 bumps-0.9.1/bumps/dream/parcoord.py
+-rw-r--r--   0 pkienzle (34766)    34766    43644 2020-12-16 20:29:47.000000 bumps-0.9.1/bumps/dream/state.py
+-rw-r--r--   0 pkienzle (34766)    34766    10285 2020-12-16 20:29:47.000000 bumps-0.9.1/bumps/dream/stats.py
+-rw-r--r--   0 pkienzle (34766)    34766     1541 2017-05-09 20:01:14.000000 bumps-0.9.1/bumps/dream/tile.py
+-rw-r--r--   0 pkienzle (34766)    34766     2341 2016-10-25 13:55:16.000000 bumps-0.9.1/bumps/dream/util.py
+-rw-r--r--   0 pkienzle (34766)    34766    11510 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/dream/varplot.py
+-rw-r--r--   0 pkienzle (34766)    34766     9021 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/dream/views.py
+-rw-r--r--   0 pkienzle (34766)    34766     3812 2015-07-27 16:17:03.000000 bumps-0.9.1/bumps/dream/walk.py
+-rw-r--r--   0 pkienzle (34766)    34766     5134 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/errplot.py
+-rw-r--r--   0 pkienzle (34766)    34766    30597 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/fitproblem.py
+-rw-r--r--   0 pkienzle (34766)    34766     3235 2020-11-19 22:11:15.000000 bumps-0.9.1/bumps/fitservice.py
+-rw-r--r--   0 pkienzle (34766)    34766    49182 2023-04-10 15:19:38.000000 bumps-0.9.1/bumps/fitters.py
+-rw-r--r--   0 pkienzle (34766)    34766    19680 2020-12-16 23:04:24.000000 bumps-0.9.1/bumps/formatnum.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2023-04-10 16:22:33.220680 bumps-0.9.1/bumps/gui/
+-rw-r--r--   0 pkienzle (34766)    34766        0 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/gui/__init__.py
+-rw-r--r--   0 pkienzle (34766)    34766     7520 2014-05-27 18:39:51.000000 bumps-0.9.1/bumps/gui/about.py
+-rw-r--r--   0 pkienzle (34766)    34766     9217 2020-11-19 22:11:15.000000 bumps-0.9.1/bumps/gui/app_frame.py
+-rw-r--r--   0 pkienzle (34766)    34766    27819 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/gui/app_panel.py
+-rw-r--r--   0 pkienzle (34766)    34766     6721 2016-10-25 13:55:16.000000 bumps-0.9.1/bumps/gui/console.py
+-rw-r--r--   0 pkienzle (34766)    34766     2351 2020-11-19 22:11:15.000000 bumps-0.9.1/bumps/gui/convergence_view.py
+-rwxr-xr-x   0 pkienzle (34766)    34766     8337 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/gui/data_view.py
+-rw-r--r--   0 pkienzle (34766)    34766    11557 2023-04-04 14:56:25.000000 bumps-0.9.1/bumps/gui/fit_dialog.py
+-rw-r--r--   0 pkienzle (34766)    34766     8830 2020-11-19 22:11:15.000000 bumps-0.9.1/bumps/gui/fit_thread.py
+-rwxr-xr-x   0 pkienzle (34766)    34766     1845 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/gui/fit_view.py
+-rwxr-xr-x   0 pkienzle (34766)    34766    13697 2023-04-04 14:56:25.000000 bumps-0.9.1/bumps/gui/gui_app.py
+-rw-r--r--   0 pkienzle (34766)    34766    49071 2020-11-19 22:11:16.000000 bumps-0.9.1/bumps/gui/input_list.py
+-rwxr-xr-x   0 pkienzle (34766)    34766     1339 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/gui/log_view.py
+-rw-r--r--   0 pkienzle (34766)    34766     9551 2014-06-02 21:33:58.000000 bumps-0.9.1/bumps/gui/parameter_grid.py
+-rwxr-xr-x   0 pkienzle (34766)    34766    13099 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/gui/parameter_view.py
+-rw-r--r--   0 pkienzle (34766)    34766     7415 2020-11-19 22:11:16.000000 bumps-0.9.1/bumps/gui/plot_view.py
+-rw-r--r--   0 pkienzle (34766)    34766     5965 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/gui/resfiles.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2023-04-10 16:22:33.232171 bumps-0.9.1/bumps/gui/resources/
+-rw-r--r--   0 pkienzle (34766)    34766      336 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/gui/resources/__init__.py
+-rw-r--r--   0 pkienzle (34766)    34766   353118 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/gui/resources/bumps.ico
+-rw-r--r--   0 pkienzle (34766)    34766    73466 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/gui/resources/bumps_splash.jpg
+-rw-r--r--   0 pkienzle (34766)    34766     2196 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/gui/resources/done.wav
+-rwxr-xr-x   0 pkienzle (34766)    34766     1166 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/gui/resources/import_script.png
+-rwxr-xr-x   0 pkienzle (34766)    34766     6235 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/gui/resources/reload.png
+-rwxr-xr-x   0 pkienzle (34766)    34766     1675 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/gui/resources/start_fit.png
+-rwxr-xr-x   0 pkienzle (34766)    34766     1965 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/gui/resources/stop_fit.png
+-rw-r--r--   0 pkienzle (34766)    34766     2019 2020-11-19 22:11:16.000000 bumps-0.9.1/bumps/gui/signal.py
+-rwxr-xr-x   0 pkienzle (34766)    34766     8687 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/gui/summary_view.py
+-rw-r--r--   0 pkienzle (34766)    34766     2928 2022-04-29 18:13:57.000000 bumps-0.9.1/bumps/gui/uncertainty_view.py
+-rwxr-xr-x   0 pkienzle (34766)    34766     4038 2020-11-19 22:11:16.000000 bumps-0.9.1/bumps/gui/util.py
+-rw-r--r--   0 pkienzle (34766)    34766    16656 2023-04-04 14:56:25.000000 bumps-0.9.1/bumps/gui/utilities.py
+-rw-r--r--   0 pkienzle (34766)    34766    10134 2023-04-04 14:56:25.000000 bumps-0.9.1/bumps/history.py
+-rw-r--r--   0 pkienzle (34766)    34766    11306 2023-04-04 14:56:25.000000 bumps-0.9.1/bumps/initpop.py
+-rw-r--r--   0 pkienzle (34766)    34766    15805 2023-04-04 14:56:25.000000 bumps-0.9.1/bumps/lsqerror.py
+-rw-r--r--   0 pkienzle (34766)    34766    12406 2023-04-04 14:56:25.000000 bumps-0.9.1/bumps/mapper.py
+-rw-r--r--   0 pkienzle (34766)    34766     4209 2023-04-10 15:48:43.000000 bumps-0.9.1/bumps/monitor.py
+-rw-r--r--   0 pkienzle (34766)    34766     3775 2017-05-09 19:31:14.000000 bumps-0.9.1/bumps/mono.py
+-rw-r--r--   0 pkienzle (34766)    34766    88892 2023-04-10 15:48:43.000000 bumps-0.9.1/bumps/mpfit.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2023-04-10 16:22:33.236895 bumps-0.9.1/bumps/mystic/
+-rw-r--r--   0 pkienzle (34766)    34766        0 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/mystic/__init__.py
+-rw-r--r--   0 pkienzle (34766)    34766     8373 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/mystic/condition.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2023-04-10 16:22:33.243576 bumps-0.9.1/bumps/mystic/examples/
+-rw-r--r--   0 pkienzle (34766)    34766      571 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/mystic/examples/__init__.py
+-rw-r--r--   0 pkienzle (34766)    34766     2476 2014-10-29 14:24:38.000000 bumps-0.9.1/bumps/mystic/examples/circle.py
+-rw-r--r--   0 pkienzle (34766)    34766     1711 2014-07-20 22:24:06.000000 bumps-0.9.1/bumps/mystic/examples/corana.py
+-rw-r--r--   0 pkienzle (34766)    34766     1462 2014-07-20 22:24:18.000000 bumps-0.9.1/bumps/mystic/examples/decay.py
+-rw-r--r--   0 pkienzle (34766)    34766     2195 2016-10-25 13:55:16.000000 bumps-0.9.1/bumps/mystic/examples/model.py
+-rw-r--r--   0 pkienzle (34766)    34766       45 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/mystic/examples/simple.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2023-04-10 16:22:33.246400 bumps-0.9.1/bumps/mystic/optimizer/
+-rw-r--r--   0 pkienzle (34766)    34766        0 2014-02-04 18:07:02.000000 bumps-0.9.1/bumps/mystic/optimizer/__init__.py
+-rw-r--r--   0 pkienzle (34766)    34766     8484 2020-11-19 22:11:16.000000 bumps-0.9.1/bumps/mystic/optimizer/de.py
+-rw-r--r--   0 pkienzle (34766)    34766     5422 2014-10-29 14:26:28.000000 bumps-0.9.1/bumps/mystic/optimizer/diffev_compat.py
+-rw-r--r--   0 pkienzle (34766)    34766    10945 2016-10-25 13:55:16.000000 bumps-0.9.1/bumps/mystic/solver.py
+-rw-r--r--   0 pkienzle (34766)    34766    25453 2014-07-20 22:22:45.000000 bumps-0.9.1/bumps/mystic/stop.py
+-rw-r--r--   0 pkienzle (34766)    34766     2066 2014-07-20 22:23:38.000000 bumps-0.9.1/bumps/mystic/util.py
+-rw-r--r--   0 pkienzle (34766)    34766     2196 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/names.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2023-04-10 16:22:33.252516 bumps-0.9.1/bumps/numdifftools/
+-rw-r--r--   0 pkienzle (34766)    34766      103 2016-10-25 13:55:16.000000 bumps-0.9.1/bumps/numdifftools/__init__.py
+-rw-r--r--   0 pkienzle (34766)    34766    48284 2022-05-02 18:28:11.000000 bumps-0.9.1/bumps/numdifftools/core.py
+-rw-r--r--   0 pkienzle (34766)    34766    11684 2016-10-25 13:55:16.000000 bumps-0.9.1/bumps/numdifftools/extrapolation.py
+-rw-r--r--   0 pkienzle (34766)    34766     3228 2020-11-19 22:11:16.000000 bumps-0.9.1/bumps/numdifftools/info.py
+-rw-r--r--   0 pkienzle (34766)    34766    10033 2016-10-25 13:55:16.000000 bumps-0.9.1/bumps/numdifftools/multicomplex.py
+-rw-r--r--   0 pkienzle (34766)    34766     2128 2017-05-09 19:32:28.000000 bumps-0.9.1/bumps/openmp_ext.py
+-rw-r--r--   0 pkienzle (34766)    34766    18922 2022-07-13 23:04:10.000000 bumps-0.9.1/bumps/options.py
+-rw-r--r--   0 pkienzle (34766)    34766    36566 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/parameter.py
+-rw-r--r--   0 pkienzle (34766)    34766    12581 2016-10-25 13:55:16.000000 bumps-0.9.1/bumps/partemp.py
+-rw-r--r--   0 pkienzle (34766)    34766    10408 2020-11-19 22:11:16.000000 bumps-0.9.1/bumps/pdfwrapper.py
+-rw-r--r--   0 pkienzle (34766)    34766     5740 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/plotutil.py
+-rw-r--r--   0 pkienzle (34766)    34766     2770 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/plugin.py
+-rw-r--r--   0 pkienzle (34766)    34766     2396 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/pmath.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2023-04-10 16:22:33.253564 bumps-0.9.1/bumps/private/
+-rw-r--r--   0 pkienzle (34766)    34766        0 2023-03-22 20:05:34.000000 bumps-0.9.1/bumps/private/__init__.py
+-rw-r--r--   0 pkienzle (34766)    34766     4657 2020-09-11 19:45:22.000000 bumps-0.9.1/bumps/pymcfit.py
+-rw-r--r--   0 pkienzle (34766)    34766    21294 2020-09-11 19:45:22.000000 bumps-0.9.1/bumps/pytwalk.py
+-rw-r--r--   0 pkienzle (34766)    34766    28707 2016-10-25 13:55:16.000000 bumps-0.9.1/bumps/quasinewton.py
+-rw-r--r--   0 pkienzle (34766)    34766     8975 2020-10-30 19:05:36.000000 bumps-0.9.1/bumps/random_lines.py
+-rw-r--r--   0 pkienzle (34766)    34766    11236 2022-05-02 18:28:11.000000 bumps-0.9.1/bumps/simplex.py
+-rw-r--r--   0 pkienzle (34766)    34766     9686 2023-04-05 21:57:25.000000 bumps-0.9.1/bumps/util.py
+-rw-r--r--   0 pkienzle (34766)    34766    16679 2020-11-19 22:11:16.000000 bumps-0.9.1/bumps/vfs.py
+-rw-r--r--   0 pkienzle (34766)    34766    15569 2021-03-10 15:46:52.000000 bumps-0.9.1/bumps/wsolve.py
+drwxr-xr-x   0 pkienzle (34766)    34766        0 2023-04-10 16:22:33.138997 bumps-0.9.1/bumps.egg-info/
+-rw-r--r--   0 pkienzle (34766)    34766    12697 2023-04-10 16:22:32.000000 bumps-0.9.1/bumps.egg-info/PKG-INFO
+-rw-r--r--   0 pkienzle (34766)    34766     2963 2023-04-10 16:22:32.000000 bumps-0.9.1/bumps.egg-info/SOURCES.txt
+-rw-r--r--   0 pkienzle (34766)    34766        1 2023-04-10 16:22:32.000000 bumps-0.9.1/bumps.egg-info/dependency_links.txt
+-rw-r--r--   0 pkienzle (34766)    34766        4 2023-04-10 16:22:32.000000 bumps-0.9.1/bumps.egg-info/requires.txt
+-rw-r--r--   0 pkienzle (34766)    34766        6 2023-04-10 16:22:32.000000 bumps-0.9.1/bumps.egg-info/top_level.txt
+-rwxr-xr-x   0 pkienzle (34766)    34766     9470 2014-11-21 21:09:16.000000 bumps-0.9.1/bumps.iss
+-rwxr-xr-x   0 pkienzle (34766)    34766    18906 2015-03-26 17:53:23.000000 bumps-0.9.1/master_builder.py
+-rw-r--r--   0 pkienzle (34766)    34766       38 2023-04-10 16:22:33.255347 bumps-0.9.1/setup.cfg
+-rwxr-xr-x   0 pkienzle (34766)    34766     1859 2023-04-05 21:57:25.000000 bumps-0.9.1/setup.py
+-rwxr-xr-x   0 pkienzle (34766)    34766    11841 2014-11-21 21:09:16.000000 bumps-0.9.1/setup_py2exe.py
```

### Comparing `bumps-0.9.0/MANIFEST.in` & `bumps-0.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/PKG-INFO` & `bumps-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
 Name: bumps
-Version: 0.9.0
+Version: 0.9.1
 Summary: Data fitting with bayesian uncertainty analysis
-Home-page: http://www.reflectometry.org/danse/software.html
+Home-page: https://github.com/bumps/bumps
 Author: Paul Kienzle
 Author-email: paul.kienzle@nist.gov
 License: UNKNOWN
 Description: ==============================================
         Bumps: data fitting and uncertainty estimation
         ==============================================
         
@@ -44,30 +44,46 @@
         .. |RTD| image:: https://readthedocs.org/projects/bumps/badge/?version=latest
            :alt: Documentation status
            :target: https://bumps.readthedocs.io/en/latest/?badge=latest
         
         Release notes
         =============
         
+        v0.9.1 2023-04-10
+        -----------------
+        * added support for python 3.11, scipy 1.10, numpy 1.24, wx 4.1.1
+        * fixed covariance calculation for n-D datasets
+        * fixed batch mode I/O redirection cleanup
+        * fixed issue with DREAM bounds checker when running in parallel
+        * default to single precision derivatives with lm (fixes issue in SasView
+          where OpenCL models failed with Levenberg-Marquardt)
+        * improved support for repeat fitting within scripts and notebooks
+          (*start_mapper* should now work after *stop_mapper*)
+        
         v0.9.0 2022-03-15
         -----------------
         * use MPFit in place of scipy.leastsq for bounds-constrained Levenberg-Marquardt
-        * weights are properly applied to models (nllf) in FitProblem
+        
+        Breaking change:
+        * simultaneous fit now scales individual nllfs by squared weight rather than weight
         
         v0.8.1 2021-11-18
         -----------------
         * "apply parameters" action added to GUI menu (does the same as --pars flag in CLI)
         * operators refactored (no more eval)
         * BoundedNormal keywords renamed (sigma, mu) -> (std, mean)
         * support for numba usage in models
         * fixed Parameters view jumping to top after toggling fit (linux, Mac)
         * fixed Summary view sliders disappearing in linux
         * fixed uncertainty plots regenerating at each parameter update
         * improved documentation of uncertainty analysis
         
+        Breaking change:
+        * python 2.7 support discontinued
+        
         v0.8.0 2020-12-16
         -----------------
         * add stopping conditions to DREAM, using *--alpha=p-value* to reject convergence
         * require *--overwrite* or *--resume* when reusing a store directory
         * enable outlier trimming in DREAM with --outliers=iqr
         * add fitted slope and loglikelihood distribution to the loglikelihood plot
         * display seed value used for fit so it can be rerun with *--seed*
```

### Comparing `bumps-0.9.0/README.rst` & `bumps-0.9.1/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -36,30 +36,46 @@
 .. |RTD| image:: https://readthedocs.org/projects/bumps/badge/?version=latest
    :alt: Documentation status
    :target: https://bumps.readthedocs.io/en/latest/?badge=latest
 
 Release notes
 =============
 
+v0.9.1 2023-04-10
+-----------------
+* added support for python 3.11, scipy 1.10, numpy 1.24, wx 4.1.1
+* fixed covariance calculation for n-D datasets
+* fixed batch mode I/O redirection cleanup
+* fixed issue with DREAM bounds checker when running in parallel
+* default to single precision derivatives with lm (fixes issue in SasView
+  where OpenCL models failed with Levenberg-Marquardt)
+* improved support for repeat fitting within scripts and notebooks
+  (*start_mapper* should now work after *stop_mapper*)
+
 v0.9.0 2022-03-15
 -----------------
 * use MPFit in place of scipy.leastsq for bounds-constrained Levenberg-Marquardt
-* weights are properly applied to models (nllf) in FitProblem
+
+Breaking change:
+* simultaneous fit now scales individual nllfs by squared weight rather than weight
 
 v0.8.1 2021-11-18
 -----------------
 * "apply parameters" action added to GUI menu (does the same as --pars flag in CLI)
 * operators refactored (no more eval)
 * BoundedNormal keywords renamed (sigma, mu) -> (std, mean)
 * support for numba usage in models
 * fixed Parameters view jumping to top after toggling fit (linux, Mac)
 * fixed Summary view sliders disappearing in linux
 * fixed uncertainty plots regenerating at each parameter update
 * improved documentation of uncertainty analysis
 
+Breaking change:
+* python 2.7 support discontinued
+
 v0.8.0 2020-12-16
 -----------------
 * add stopping conditions to DREAM, using *--alpha=p-value* to reject convergence
 * require *--overwrite* or *--resume* when reusing a store directory
 * enable outlier trimming in DREAM with --outliers=iqr
 * add fitted slope and loglikelihood distribution to the loglikelihood plot
 * display seed value used for fit so it can be rerun with *--seed*
```

### Comparing `bumps-0.9.0/bin/bumps` & `bumps-0.9.1/bin/bumps`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bin/bumps_gui` & `bumps-0.9.1/bin/bumps_gui`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bin/bumps_workerd` & `bumps-0.9.1/bin/bumps_workerd`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/__init__.py` & `bumps-0.9.1/bumps/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 
 This package provides tools for modeling parametric systems in a Bayesian
 context, with routines for finding the maximum likelihood and the
 posterior probability density function.
 
 A graphical interface allows direct manipulation of the model parameters.
 
-See http://www.reflectometry.org/danse/reflectometry for online manuals.
+See https://bumps.readthedocs.io for online manuals.
 """
 
-__version__ = "0.9.0"
+__version__ = "0.9.1"
 
 def data_files():
     """
     Return the data files associated with the package for setup_py2exe.py.
 
     The format is a list of (directory, [files...]) pairs which can be
     used directly in the py2exe setup script as::
```

### Comparing `bumps-0.9.0/bumps/bounds.py` & `bumps-0.9.1/bumps/bounds.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/bspline.py` & `bumps-0.9.1/bumps/bspline.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/cheby.py` & `bumps-0.9.1/bumps/cheby.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/cli.py` & `bumps-0.9.1/bumps/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,15 +507,15 @@
 
 
 def setup_logging():
     """Start logger"""
     import logging
     logging.basicConfig(level=logging.INFO)
 
-# from http://stackoverflow.com/questions/22373927/get-traceback-of-warnings
+# From http://stackoverflow.com/questions/22373927/get-traceback-of-warnings
 # answered by mgab (2014-03-13)
 # edited by Gareth Rees (2015-11-28)
 def warn_with_traceback(message, category, filename, lineno,
                         file=None, line=None):
     """
     Alternate warning printer which shows a traceback with the warning.
 
@@ -711,16 +711,16 @@
             fitdriver.show_cov()
         if opts.entropy:
             fitdriver.show_entropy(opts.entropy)
         mapper.stop_mapper(fitdriver.mapper)
 
         # If in batch mode then explicitly close the monitor file on completion
         if opts.batch:
-            sys.stderr.close()
-            sys.stderr = sys.__stderr__
+            sys.stdout.close()
+            sys.stdout = sys.__stdout__
 
         # Display the plots
         if not opts.batch and not opts.mpi and not opts.noshow:
             beep()
             import pylab
             pylab.show()
```

### Comparing `bumps-0.9.0/bumps/curve.py` & `bumps-0.9.1/bumps/curve.py`

 * *Files 0% similar despite different names*

```diff
@@ -207,21 +207,20 @@
             if num_curves > 1:
                 line_labels = ['y%d'%k for k in range(num_curves)]
             else:
                 line_labels = [labels[1]]
             labels = list(labels) + line_labels
         self.labels = labels
 
-
         # TODO: self.fn is a duplicate of self._function below. Deprecated?
         self.fn = fn
         self.name = name # if name else fn.__name__ + " "
         self.plot_x = plot_x
 
-        pars, state = _parse_pars(fn, init=kwargs, skip=1)
+        pars, state = _parse_pars(fn, init=kwargs, skip=1, name=name)
 
         # Make parameters accessible as model attributes
         _assign_pars(self, pars)
         #_assign_pars(state, self)  # ... and state variables as well
 
         # Remember the function, parameters, and number of parameters
         # Note: we are remembering the parameter names and not the
```

### Comparing `bumps-0.9.0/bumps/data.py` & `bumps-0.9.1/bumps/data.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/__init__.py` & `bumps-0.9.1/bumps/dream/__init__.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/acr.py` & `bumps-0.9.1/bumps/dream/acr.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/bounds.py` & `bumps-0.9.1/bumps/dream/bounds.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/convergence.py` & `bumps-0.9.1/bumps/dream/convergence.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/core.py` & `bumps-0.9.1/bumps/dream/core.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/corrplot.py` & `bumps-0.9.1/bumps/dream/corrplot.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/crossover.py` & `bumps-0.9.1/bumps/dream/crossover.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/diffev.py` & `bumps-0.9.1/bumps/dream/diffev.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/digits.py` & `bumps-0.9.1/bumps/dream/digits.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/entropy.py` & `bumps-0.9.1/bumps/dream/entropy.py`

 * *Files 1% similar despite different names*

```diff
@@ -855,16 +855,22 @@
     def logpdf(self, theta):
         return self.dist.logpdf(theta)
 
     def rvs(self, size=1):
         return self.dist.rvs(size=size)
 
     def entropy(self, N=10000):
+        # CRUFT scipy==1.10.0: scipy.stats briefly removed the dist.cov attribute.
+        if hasattr(self.dist, 'cov'):
+            cov = self.dist.cov
+        else:
+            cov = self.dist.cov_object.covariance
+
         with np.errstate(divide='ignore'):
-            return 0.5*log(np.linalg.det((2*pi*np.e)*self.dist.cov))
+            return 0.5*log(np.linalg.det((2*pi*np.e)*cov))
 
 class GaussianMixture:
     def __init__(self, w, mu=None, sigma=None):
         mu = np.asarray(mu)
         dim = mu.shape[1]
         if sigma is None:
             sigma = [None] * len(mu)
```

### Comparing `bumps-0.9.0/bumps/dream/exppow.py` & `bumps-0.9.1/bumps/dream/exppow.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/formatnum.py` & `bumps-0.9.1/bumps/dream/formatnum.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/gelman.py` & `bumps-0.9.1/bumps/dream/gelman.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/geweke.py` & `bumps-0.9.1/bumps/dream/geweke.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/initpop.py` & `bumps-0.9.1/bumps/dream/initpop.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/ksmirnov.py` & `bumps-0.9.1/bumps/dream/ksmirnov.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/mahal.py` & `bumps-0.9.1/bumps/dream/mahal.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/matlab.py` & `bumps-0.9.1/bumps/dream/matlab.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/metropolis.py` & `bumps-0.9.1/bumps/dream/metropolis.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/model.py` & `bumps-0.9.1/bumps/dream/model.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/outliers.py` & `bumps-0.9.1/bumps/dream/outliers.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/parcoord.py` & `bumps-0.9.1/bumps/dream/parcoord.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/state.py` & `bumps-0.9.1/bumps/dream/state.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/stats.py` & `bumps-0.9.1/bumps/dream/stats.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/tile.py` & `bumps-0.9.1/bumps/dream/tile.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/util.py` & `bumps-0.9.1/bumps/dream/util.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/varplot.py` & `bumps-0.9.1/bumps/dream/varplot.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/views.py` & `bumps-0.9.1/bumps/dream/views.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/dream/walk.py` & `bumps-0.9.1/bumps/dream/walk.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/errplot.py` & `bumps-0.9.1/bumps/errplot.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/fitproblem.py` & `bumps-0.9.1/bumps/fitproblem.py`

 * *Files 2% similar despite different names*

```diff
@@ -147,26 +147,31 @@
     """default constraints function for FitProblem"""
     return 0
 
 
 # TODO: refactor FitProblem definition
 # deprecate the direct use of MultiFitProblem
 def FitProblem(*args, **kw):
-    """
+    r"""
     Return a fit problem instance for the fitness function(s).
 
     For an individual model:
 
         *fitness* is a :class:`Fitness` instance.
 
     For a set of models:
 
         *models* is a sequence of :class:`Fitness` instances.
 
-        *weights* is an optional scale factor for each model
+        *weights* is an optional scale factor for each model. A weighted fit
+        returns nllf $L = \sum w_k^2 L_k$. If an individual nllf is the sum
+        squared residuals then this is equivalent to scaling the measurement
+        uncertainty by $1/w$. Unless the measurement uncertainty is unknown,
+        weights should be in [0, 1], representing an unknown systematic
+        uncertainty spread across the individual measurements.
 
         *freevars* is :class:`.parameter.FreeVariables` instance defining the
         per-model parameter assignments.  See :ref:`freevariables` for details.
 
 
     Additional parameters:
 
@@ -185,14 +190,17 @@
 
         *penalty_nllf* is the nllf to use for *fitness* when *constraints*
         is greater than *soft_limit*.
 
     Total nllf is the sum of the parameter nllf, the constraints nllf and the
     depending on whether constraints is greater than soft_limit, either the
     fitness nllf or the penalty nllf.
+
+    New in 0.9.0: weights are now squared when computing the sum rather than
+    linear.
     """
     if len(args) > 0:
         if isinstance(args[0], (list, tuple)):
             return MultiFitProblem(args[0], *args[1:], **kw)
         else:
             return BaseFitProblem(*args, **kw)
     else:
@@ -598,15 +606,16 @@
     def __setstate__(self, state):
         self.fitness, self.partial, self.name, self.penalty_nllf, \
             self.soft_limit, self.constraints = state
         self.model_reset()
 
 class MultiFitProblem(BaseFitProblem):
     """
-    Weighted fits for multiple models.
+    Weighted fits for multiple models. See :func:`FitProblem` for an
+    explanation of weights.
     """
     def __init__(self, models, weights=None, name=None,
                  constraints=None,
                  soft_limit=np.inf, penalty_nllf=1e6,
                  freevars=None):
         self.partial = False
         self.constraints = constraints
```

### Comparing `bumps-0.9.0/bumps/fitservice.py` & `bumps-0.9.1/bumps/fitservice.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/fitters.py` & `bumps-0.9.1/bumps/fitters.py`

 * *Files 2% similar despite different names*

```diff
@@ -566,14 +566,15 @@
 
         result = mpfit(
             fcn=self._residuals,
             xall=x0,
             parinfo=parinfo,
             autoderivative=True,
             fastnorm=True,
+            double=0, # use single precision machine epsilon for derivative step
             #damp=0,  # no damping when damp=0
             # Stopping conditions
             ftol=options['ftol'],
             xtol=options['xtol'],
             #gtol=1e-100, # exclude gtol test
             maxiter=options['steps'],
             # Progress monitor
@@ -1095,33 +1096,57 @@
 
     def show(self):
         if hasattr(self.fitter, 'show'):
             self.fitter.show()
         if hasattr(self.problem, 'show'):
             self.problem.show()
 
-    def show_err(self):
+
+    # TODO: reenable the "implied variance" calculation
+    def _unused_show_err(self):
         """
         Display the error approximation from the numerical derivative.
 
         Warning: cost grows as the cube of the number of parameters.
         """
         # TODO: need cheaper uncertainty estimate
         # Note: error estimated from hessian diagonal is insufficient.
         err = self.stderr_from_cov()
+        # TODO: citation needed
+        # The "implied variance" column is obtained by scaling the covariance
+        # matrix so that chisq = DOF. Any excess chisq implies increased
+        # variance in the measurements, so increased variance in the parameters.
+        # This is well defined for linear systems with equal but unknown
+        # variance in each measurement, and assumed to be approximately true
+        # for nonlinear systems, with the unexplained variance distributed
+        # proportionately amongst the measurement uncertainties.
         norm = np.sqrt(self.chisq())
         print("=== Uncertainty from curvature:     name"
               " value(unc.)    "
               " value(unc./chi)) ===")
         for k, v, dv in zip(self.problem.labels(), self.problem.getp(), err):
             print("%40s %-15s %-15s" % (k,
                   format_uncertainty(v, dv),
                   format_uncertainty(v, dv/norm)))
         print("="*75)
 
+    def show_err(self):
+        """
+        Display the error approximation from the numerical derivative.
+
+        Warning: cost grows as the cube of the number of parameters.
+        """
+        # TODO: need cheaper uncertainty estimate
+        # Note: error estimated from hessian diagonal is insufficient.
+        err = self.stderr_from_cov()
+        print("=== Uncertainty from curvature:     name   value(unc.) ===")
+        for k, v, dv in zip(self.problem.labels(), self.problem.getp(), err):
+            print(f"{k:>40s}   {format_uncertainty(v, dv):<15s}")
+        print("="*58)
+
     def show_cov(self):
         cov = self.cov()
         maxn = 1000 # max array dims to print
         cov_str = np.array2string(
             cov,
             max_line_width=20*maxn, threshold=maxn*maxn,
             precision=6, #suppress_small=True,
```

### Comparing `bumps-0.9.0/bumps/formatnum.py` & `bumps-0.9.1/bumps/formatnum.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/about.py` & `bumps-0.9.1/bumps/gui/about.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/app_frame.py` & `bumps-0.9.1/bumps/gui/app_frame.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/app_panel.py` & `bumps-0.9.1/bumps/gui/app_panel.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/console.py` & `bumps-0.9.1/bumps/gui/console.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/convergence_view.py` & `bumps-0.9.1/bumps/gui/convergence_view.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/data_view.py` & `bumps-0.9.1/bumps/gui/data_view.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/fit_dialog.py` & `bumps-0.9.1/bumps/gui/fit_dialog.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
             font.SetPointSize(fontsize)
             self.SetFont(font)
 
         # Section 1
         self.panel1 = wx.Panel(self, -1)
         static_box1 = wx.StaticBox(self.panel1, -1, "Fit Algorithms")
 
-        rows = (len(self.active_ids)+1)/2
+        rows = (len(self.active_ids)+1)//2
 
         flexsizer = wx.FlexGridSizer(rows, 2, hgap=20, vgap=10)
 
         self.fitter_button = {}
         for fitter in self.active_ids:
             button = wx.RadioButton(self.panel1, -1,
                     label=config.names[fitter], name=fitter)
```

### Comparing `bumps-0.9.0/bumps/gui/fit_thread.py` & `bumps-0.9.1/bumps/gui/fit_thread.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/fit_view.py` & `bumps-0.9.1/bumps/gui/fit_view.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/gui_app.py` & `bumps-0.9.1/bumps/gui/gui_app.py`

 * *Files 0% similar despite different names*

```diff
@@ -189,16 +189,16 @@
         h -= 20  # to make room for Mac window decorations
         if len(sys.argv) > 1 and '--platform' in sys.argv[1:]:
             j, k = wx.DisplaySize()  # size includes task bar area
             print("*** Reported screen size including taskbar is %d x %d"%(j, k))
             print("*** Reported screen size excluding taskbar is %d x %d"%(w, h))
 
         if w > 1920: w = 1280  # display on left side, not centered on screen
-        if w > desired_width:  xpos = x + (w - desired_width)/2
-        if h > desired_height: ypos = y + (h - desired_height)/2
+        if w > desired_width:  xpos = x + (w - desired_width)//2
+        if h > desired_height: ypos = y + (h - desired_height)//2
 
         # Return the suggested position and size for the application frame.
         return (xpos, ypos), (min(w, desired_width), min(h, desired_height))
 
     def display_splash_screen(self, img_name=None, pos=None, size=(320, 240)):
         """Displays a splash screen and the specified position and size."""
         # Prepare the picture.
```

### Comparing `bumps-0.9.0/bumps/gui/input_list.py` & `bumps-0.9.1/bumps/gui/input_list.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/log_view.py` & `bumps-0.9.1/bumps/gui/log_view.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/parameter_grid.py` & `bumps-0.9.1/bumps/gui/parameter_grid.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/parameter_view.py` & `bumps-0.9.1/bumps/gui/parameter_view.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/plot_view.py` & `bumps-0.9.1/bumps/gui/plot_view.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/resfiles.py` & `bumps-0.9.1/bumps/gui/resfiles.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/resources/bumps.ico` & `bumps-0.9.1/bumps/gui/resources/bumps.ico`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/resources/bumps_splash.jpg` & `bumps-0.9.1/bumps/gui/resources/bumps_splash.jpg`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/resources/done.wav` & `bumps-0.9.1/bumps/gui/resources/done.wav`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/resources/import_script.png` & `bumps-0.9.1/bumps/gui/resources/import_script.png`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/resources/reload.png` & `bumps-0.9.1/bumps/gui/resources/reload.png`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/resources/start_fit.png` & `bumps-0.9.1/bumps/gui/resources/start_fit.png`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/resources/stop_fit.png` & `bumps-0.9.1/bumps/gui/resources/stop_fit.png`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/signal.py` & `bumps-0.9.1/bumps/gui/signal.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/summary_view.py` & `bumps-0.9.1/bumps/gui/summary_view.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/uncertainty_view.py` & `bumps-0.9.1/bumps/gui/uncertainty_view.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/util.py` & `bumps-0.9.1/bumps/gui/util.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/gui/utilities.py` & `bumps-0.9.1/bumps/gui/utilities.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     the point size of the font, and the resolution of the installed font as
     measured in dots-per-inch (aka points-per-inch).
     """
 
     frame = wx.Frame(parent=None, id=wx.ID_ANY, title="")
     if fontname is None:
         fontname = frame.GetFont().GetFaceName()
-    max_width = BENCHMARK_WIDTH + BENCHMARK_WIDTH/100
+    max_width = BENCHMARK_WIDTH + BENCHMARK_WIDTH//100
 
     for fontsize in range(12, 5, -1):
         frame.SetFont(wx.Font(fontsize, wx.SWISS, wx.NORMAL, wx.NORMAL, False,
                               fontname))
         benchmark = wx.StaticText(frame, wx.ID_ANY, label="")
         w, h = benchmark.GetTextExtent(BENCHMARK_TEXT)
         benchmark.Destroy()
```

### Comparing `bumps-0.9.0/bumps/history.py` & `bumps-0.9.1/bumps/history.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,54 +17,71 @@
 History consists of a set of traces.  The content of the traces
 themselves is provided by the computation, but various stake holders
 can use them.  For example, the user may wish to log the set of points
 that have been evaluated and their values using the system logger
 and an optimizer may require a certain amount of history to calculate
 the next set of values.
 
-New traces are provided using :meth:`History.provides`.  For example,
+New traces are defined using :meth:`History.provides`.  For example,
 the following adds traces for 'value' and 'point' to the history, and
-requires the best value on the two previous cycles in order to do its work:
+requires the value on the two previous cycles in order to do its work:
 
     >>> from bumps.history import History
-    >>> h = History()
-    >>> h.provides(value=2, point=0)
+    >>> h = History(value=2, point=0) # keep two values and zero points
 
 Initially the history is empty:
 
     >>> print(len(h.value))
     0
 
-After three updates we see that only two values are kept:
+After three updates we see that only two values are kept.
 
-    >>> h.update(value=2,point=[1,1,1])
-    >>> h.update(value=1,point=[1,0.5,1])
-    >>> h.update(value=0.5,point=[1,0.5,0.9])
+    >>> h.update(value=2.6, point=[1,1,1])
+    >>> h.update(value=1, point=[1,0.5,1])
+    >>> h.update(value=0.5, point=[1,0.5,0.9])
     >>> print(h.value)
     Trace value: 0.5, 1
     >>> print(len(h.value))
     2
 
-Note that point is not monitored since it is not required:
+Since the required length of 'point' is zero no values are kept:
 
     >>> print(h.point[0])
     Traceback (most recent call last):
         ...
     IndexError: point has not accumulated enough history
 
-Traces may be used as accumulators.  In that case, the next
-value is added to the tail value before appending to the trace.
-For example:
+A history consumer can override this, and require a certain length of a trace.
+Then future values will be preserved:
+
+    >>> h.requires(point=1)
+    >>> h.update(value=0.25, point=[1,0.5,0.92])
+    >>> print(h.point[0])
+    [1, 0.5, 0.92]
+
+Traces are independent of each other. A new trace can be added to the history
+and updated separately from the existing traces. This can be handy if there
+are separate sources of history though it may be difficult to keep the in sync.
+The following adds a 'step' to the existing history, initialized to 15, without
+changing 'value' or 'point':
+
+    >>> h.provides(step=2) # keep two steps
+    >>> h.update(step=15) # initialize step to 15
+    >>> print(h.step)
+    Trace step: 15
+
+Traces may be used as accumulators, with the delta added to the existing value
+before being stored in the trace. For example:
 
-    >>> h = History()
-    >>> h.provides(step=1)
-    >>> h.accumulate(step=1)
     >>> h.accumulate(step=1)
-    >>> print(h.step[0])
-    2
+    >>> print(h.step)
+    Trace step: 16, 15
+
+Within bumps, history is used by monitors, with bumps.fitters.MonitorRunner
+managing updates to history and feeding them to the fit progress monitors.
 """
 
 # Design questions:
 # 1. Can optimizer function evaluators add traces?  Can they use traces?
 # 2. Do we want to support a skip option on traces, so that only every nth
 #    item is preserved?  This is probably too hard.
 
@@ -85,18 +102,18 @@
         Specify additional provided fields.
 
         Raises AttributeError if trace is already provided or if the trace
         name matches the name of one of the history methods.
         """
         for k, v in kw.items():
             # Make sure the additional trait is not already provided.
-            # This test should also catch methods such as provides/requires
+            # This test will also catch methods such as provides/requires
             # and static properties such as bounds that are set from outside.
             if hasattr(self, k):
-                raise AttributeError("history already provides " + k)
+                raise AttributeError("History already provides " + k)
             else:
                 mon = self._new_trace(keep=v, name=k)
                 setattr(self, k, mon)
 
     def requires(self, **kw):
         """
         Specify required fields, and their history length.
```

### Comparing `bumps-0.9.0/bumps/initpop.py` & `bumps-0.9.1/bumps/initpop.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     semi-definite and indefinite bounds use the standard normal distribution
     for the underlying probability, with a scale factor determined by the
     initial value of the parameter.
 
     If *use_point* is True, then the current value of the parameters
     is returned as the first point in the population.
     """
-    population = problem.randomize(n)
+    population = np.ascontiguousarray(problem.randomize(n))
     if use_point:
         population[0] = clip(initial, *bounds)
     return population
 
 
 def eps_init(n, initial, bounds, use_point=False, eps=1e-6):
     # type: (int, np.ndarray, np.ndarray, bool, float) -> np.ndarray
```

### Comparing `bumps-0.9.0/bumps/lsqerror.py` & `bumps-0.9.1/bumps/lsqerror.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,44 +64,54 @@
     Returns the derivative wrt the fit parameters at point p.
 
     Numeric derivatives are calculated based on step, where step is
     the portion of the total range for parameter j, or the portion of
     point value p_j if the range on parameter j is infinite.
 
     The current point is preserved.
+
+    Note that the problem.residuals() method should not reuse memory for the
+    returned value otherwise the derivative calculation (f(x+dx) - f(x))/dx
+    will always be zero. The returned value need not be 1D, but it should be
+    contiguous so that it can be reshaped to 1D without an extra copy. This
+    will only be an issue for very large datasets.
     """
     p_init = problem.getp()
     if p is None:
         p = p_init
     p = np.asarray(p)
     bounds = getattr(problem, 'bounds', lambda: None)()
     def f(p):
         problem.setp(p)
-        return problem.residuals()
+        # Return residuals as a vector even if f(x) returns a matrix otherwise
+        # we cannot build a stacked Jacobian. We use reshape() rather than
+        # flatten since this will avoid an unnecessary copy.
+        return np.reshape(problem.residuals(), -1)
     J = _jacobian_forward(f, p, bounds, eps=step)
     #J = nd.Jacobian(problem.residuals)(p)
     problem.setp(p_init)
     return J
 
 def _jacobian_forward(f, p, bounds, eps=None):
     n = len(p)
     # TODO: default to double precision epsilon
     step = 1e-4 if eps is None else np.sqrt(eps)
-    fx = f(p)
 
     #print("p",p,"step",step)
     h = abs(p)*step
     h[h == 0] = step
     if bounds is not None:
         h[h+p > bounds[1]] *= -1.0  # step backward if forward step is out of bounds
     ee = np.diag(h)
 
+    fx = f(p) # Maybe fx.copy() to protect against reuse
     J = []
     for i in range(n):
-        J.append((f(p + ee[i, :]) - fx)/h[i])
+        fx_plus = f(p + ee[i, :])
+        J.append((fx_plus - fx)/h[i])
     return np.vstack(J).T
 
 def _jacobian_central(f, p, bounds, eps=None):
     n = len(p)
     # TODO: default to double precision epsilon
     step = 1e-4 if eps is None else np.sqrt(eps)
 
@@ -110,15 +120,17 @@
     h[h == 0] = step
     #if bounds is not None:
     #    h[h+p>bounds[1]] *= -1.0  # step backward if forward step is out of bounds
     ee = np.diag(h)
 
     J = []
     for i in range(n):
-        J.append((f(p + ee[i, :]) - f(p - ee[i, :])) / (2.0*h[i]))
+        fx_minus = f(p - ee[i, :]) # Maybe fx.copy() to protect against reuse
+        fx_plus = f(p + ee[i, :])
+        J.append((fx_plus - fx_minus) / (2.0*h[i]))
     return np.vstack(J).T
 
 
 def hessian(problem, p=None, step=None):
     """
     Returns the derivative wrt to the fit parameters at point p.
```

### Comparing `bumps-0.9.0/bumps/mapper.py` & `bumps-0.9.1/bumps/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,15 +86,15 @@
 class SerialMapper(object):
 
     @staticmethod
     def start_worker(problem):
         pass
 
     @staticmethod
-    def start_mapper(problem, modelargs, cpus=0):
+    def start_mapper(problem, modelargs=None, cpus=0):
         # Note: map is n iterator in python 3.x
         return lambda points: list(map(problem.nllf, points))
 
     @staticmethod
     def stop_mapper(mapper):
         pass
 
@@ -134,15 +134,15 @@
     problem_id = 0
 
     @staticmethod
     def start_worker(problem):
         pass
 
     @staticmethod
-    def start_mapper(problem, modelargs, cpus=0):
+    def start_mapper(problem, modelargs=None, cpus=0):
         import multiprocessing
 
         # Set up the process pool on the first call.
         if MPMapper.pool is None:
             # Create a sync namespace to distribute the problem description.
             MPMapper.manager = multiprocessing.Manager()
             MPMapper.namespace = MPMapper.manager.Namespace()
@@ -168,15 +168,22 @@
         # Set the mapper to send problem_id/point value pairs
         mapper = lambda points: MPMapper.pool.map(
             _MP_run_problem, ((MPMapper.problem_id, p) for p in points))
         return mapper
 
     @staticmethod
     def stop_mapper(mapper):
+        # reset pool and manager
         MPMapper.pool.terminate()
+        MPMapper.manager.shutdown()
+        MPMapper.pool = None
+        MPMapper.manager = None
+        MPMapper.namespace = None
+        # Don't reset problem id; it keeps count even when mapper is restarted.
+        ##MPMapper.problem_id = 0
 
 def _MPI_set_problem(problem, comm, root=0):
     import dill
     pickled_problem = dill.dumps(problem, recurse=True) if comm.rank == root else None
     pickled_problem = comm.bcast(pickled_problem, root=root)
     return problem if comm.rank == root else dill.loads(pickled_problem)
 
@@ -253,15 +260,15 @@
             # Exit the program after the worker is done. Don't return
             # to the caller since that is continuing on with the main
             # thread, and in particular, attempting to rerun the fit on
             # each worker.
             sys.exit(0)
 
     @staticmethod
-    def start_mapper(problem, modelargs, cpus=0):
+    def start_mapper(problem, modelargs=None, cpus=0):
         # Only root can get here---worker is stuck in start_worker
         from mpi4py import MPI
         comm, root = MPI.COMM_WORLD, 0
         import numpy as np
 
         # Signal new problem then send it, but not on the first fit. We do this
         # so that we can still run MPI fits even if the problem itself cannot
@@ -298,15 +305,15 @@
         server = connect(SERVICE_HOST)
         #os.system("echo 'serving' > /tmp/map.%d"%(os.getpid()))
         # print "worker is serving"; sys.stdout.flush()
         serve(server, "bumps", problem.nllf)
         #print >>sys.stderr,"worker ended"; sys.stdout.flush()
 
     @staticmethod
-    def start_mapper(problem, modelargs, cpus=0):
+    def start_mapper(problem, modelargs=None, cpus=0):
         import sys
         import multiprocessing
         import subprocess
         from amqp_map.config import SERVICE_HOST
         from amqp_map.core import connect, Mapper
 
         server = connect(SERVICE_HOST)
```

### Comparing `bumps-0.9.0/bumps/monitor.py` & `bumps-0.9.1/bumps/monitor.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 # This program is in the public domain
 """
 Progress monitors.
 
 Process monitors accept a :class:`bumps.history.History` object each cycle
 and perform some sort of work.
+
+Monitors have a :meth:`Monitor.config_history` method which calls
+*history.requires()* to set the amount of history it needs and a 
+*Monitor.__call__* method which takes the updated history and
+generates the monitor output.
+
+Most monitors are subclassed from :class:`TimedUpdate` to set a minimum
+time between updates and to only show updates when there is an improvement.
+The *TimedUpdate* subclasses must override :meth:`TimedUpdate.show_progress`
+and :meth:`TimedUpdate.show_improvement` to control the output form. History
+must be updated with time, value, point and step. The
+bumps.fitters.MonitorRunner class manages history and updates.
 """
 from __future__ import print_function
 
 __all__ = ['Monitor', 'Logger', 'TimedUpdate']
 
 from numpy import inf
 
@@ -83,15 +95,15 @@
 
     *progress* is the number of seconds to go before showing progress, such
     as time or step number.
 
     *improvement* is the number of seconds to go before showing
     improvements to value.
 
-    By default, the updater only prints step number and improved value.
+    By default, the update only prints step number and improved value.
     Subclass TimedUpdate with replaced :meth:`show_progress` and
     :meth:`show_improvement` to trigger GUI updates or show parameter
     values.
     """
     def __init__(self, progress=60, improvement=5):
         self.progress_delta = progress
         self.improvement_delta = improvement
```

### Comparing `bumps-0.9.0/bumps/mono.py` & `bumps-0.9.1/bumps/mono.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/mpfit.py` & `bumps-0.9.1/bumps/mpfit.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,20 @@
   Mark Rivers created this Python version from Craig's IDL version.
     Mark Rivers, University of Chicago
     Building 434A, Argonne National Laboratory
     9700 South Cass Avenue, Argonne, IL 60439
     rivers@cars.uchicago.edu
     Updated versions can be found at http://cars.uchicago.edu/software
 
+  2022-09-21 [PAK] add 'double' parameter to select machine precision for
+  the objective function. This mainly affects numerical derivatives, forcing
+  the step size to be large enough that x + h != x, but will also change the
+  criteria for correcting degenerate qr decomposition and maybe stopping
+  conditions and returned status codes.
+
 
                                  DESCRIPTION
 
  MPFIT uses the Levenberg-Marquardt technique to solve the
  least-squares problem.  In its typical use, MPFIT will be used to
  fit a user-supplied function (the "model") to user-supplied data
  points (the "data") by adjusting a set of parameters.  MPFIT is
@@ -131,15 +137,15 @@
     # FJAC contains an array of len(p), where each entry
     # is 1 if that parameter is free and 0 if it is fixed.
     model = F(x, p)
     Non-negative status value means MPFIT should continue, negative means
     # stop the calculation.
     status = 0
     if (dojac):
-       pderiv = numpy.zeros([len(x), len(p)], numpy.float)
+       pderiv = numpy.zeros([len(x), len(p)], numpy.float64)
        for j in range(len(p)):
          pderiv[:,j] = FGRAD(x, p, j)
     else:
        pderiv = None
     return([status, (y-model)/err, pderiv]
 
  where FGRAD(x, p, i) is a user function which must compute the
@@ -269,15 +275,15 @@
  constrained to be above 50.
 
 
                                    EXAMPLE
 
    import mpfit
    import numpy
-   x = numpy.arange(100, numpy.float)
+   x = numpy.arange(100, numpy.float64)
    p0 = [5.7, 2.2, 500., 1.5, 2000.]
    y = ( p[0] + p[1]*[x] + p[2]*[x**2] + p[3]*numpy.sqrt(x) +
          p[4]*numpy.log(x))
    fa = {'x':x, 'y':y, 'err':err}
    m = mpfit('myfunct', p0, functkw=fa)
    print 'status = ', m.status
    if (m.status <= 0): print 'error message = ', m.errmsg
@@ -588,15 +594,15 @@
 
 class mpfit:
    def __init__(self, fcn, xall=None, functkw={}, parinfo=None,
                 ftol=1.e-10, xtol=1.e-10, gtol=1.e-10,
                 damp=0., maxiter=200, factor=100., nprint=1,
                 iterfunct='default', iterkw={}, nocovar=0,
                 fastnorm=0, rescale=0, autoderivative=1, quiet=0,
-                diag=None, epsfcn=None, debug=0):
+                diag=None, epsfcn=None, debug=0, double=1):
       """
 Inputs:
   fcn:
      The function to be minimized.  The function should return the weighted
      deviations between the model and the data, as described above.
 
   xall:
@@ -741,14 +747,17 @@
    xtol:
       A nonnegative input variable. Termination occurs when the relative error
       between two consecutive iterates is at most xtol (and status is
       accordingly set to 2 or 3).  Therefore, xtol measures the relative error
       desired in the approximate solution.
       Default: 1E-10
 
+   double:
+      Use double=1 if fcn is double precision or double=0 for single precision. 
+
  Outputs:
 
    Returns an object of type mpfit.  The results are attributes of this class,
    e.g. mpfit.status, mpfit.errmsg, mpfit.params, npfit.niter, mpfit.covar.
 
    .status
       An integer status code is returned.  All values greater than zero can
@@ -843,15 +852,15 @@
       self.perror = None
       self.status = 0  # Invalid input flag set while we check inputs
       self.debug = debug
       self.errmsg = ''
       self.fastnorm = fastnorm
       self.nfev = 0
       self.damp = damp
-      self.machar = machar(double=1)
+      self.machar = machar(double=double)
       machep = self.machar.machep
 
       if (fcn is None):
          self.errmsg = "Usage: parms = mpfit('myfunt', ... )"
          return
 
       if (iterfunct == 'default'): iterfunct = self.defiter
@@ -884,16 +893,16 @@
       ## extract them from PARINFO
       if (xall is None):
          xall = self.parinfo(parinfo, 'value')
          if (xall is None):
             self.errmsg = 'ERROR: either P or PARINFO(*)["value"] must be supplied.'
             return
 
-      ## Make sure parameters are numpy arrays of type numpy.float
-      xall = numpy.asarray(xall, numpy.float)
+      ## Make sure parameters are numpy arrays of type numpy.float64
+      xall = numpy.asarray(xall, numpy.float64)
 
       npar = len(xall)
       self.fnorm  = -1.
       fnorm1 = -1.
 
       ## TIED parameters?
       ptied = self.parinfo(parinfo, 'tied', default='', n=npar)
@@ -982,16 +991,16 @@
       if (rescale != 0):
          self.errmsg = 'ERROR: DIAG parameter scales are inconsistent'
          if (len(diag) < n): return
          wh, = numpy.nonzero(diag <= 0)
          if (len(wh) > 0): return
          self.errmsg = ''
 
-      # Make sure x is a numpy array of type numpy.float
-      x = numpy.asarray(x, numpy.float)
+      # Make sure x is a numpy array of type numpy.float64
+      x = numpy.asarray(x, numpy.float64)
 
       [self.status, fvec] = self.call(fcn, self.params, functkw)
       if (self.status < 0):
          self.errmsg = 'ERROR: first call to "'+str(fcn)+'" failed'
          return
 
       m = len(fvec)
@@ -1316,22 +1325,22 @@
             catch_msg = 'computing the covariance matrix'
             cv = self.calc_covar(fjac[0:n,0:n], ipvt[0:n])
             cv.shape = [n, n]
             nn = len(xall)
 
             ## Fill in actual covariance matrix, accounting for fixed
             ## parameters.
-            self.covar = numpy.zeros([nn, nn], numpy.float)
+            self.covar = numpy.zeros([nn, nn], numpy.float64)
             for i in range(n):
                indices = ifree+ifree[i]*n
                numpy.put(self.covar, indices, cv[:,i])
 
             ## Compute errors in parameters
             catch_msg = 'computing parameter errors'
-            self.perror = numpy.zeros(nn, numpy.float)
+            self.perror = numpy.zeros(nn, numpy.float64)
             d = numpy.diagonal(self.covar).copy()
             wh, = numpy.nonzero(d >= 0)
             if len(wh) > 0:
               numpy.put(self.perror, wh, numpy.sqrt(numpy.take(d, wh)))
       return
 
 
@@ -1395,17 +1404,17 @@
          else:
            values.append(default)
 
       # Convert to numeric arrays if possible
       test = default
       if isinstance(default, list): test=default[0]
       if isinstance(test, int):
-         values = numpy.asarray(values, numpy.int)
+         values = numpy.asarray(values, numpy.int32)
       elif isinstance(test, float):
-         values = numpy.asarray(values, numpy.float)
+         values = numpy.asarray(values, numpy.float64)
       return(values)
 
 
    ## Call user function or procedure, with _EXTRA or not, with
    ## derivatives or not.
    def call(self, fcn, x, functkw, fjac=None):
       if (self.debug): print('Entering call...')
@@ -1469,15 +1478,15 @@
       eps = numpy.sqrt(max([epsfcn, machep]))
       m = len(fvec)
       n = len(x)
 
       ## Compute analytical derivative if requested
       if (autoderivative == 0):
          mperr = 0
-         fjac = numpy.zeros(nall, numpy.float)
+         fjac = numpy.zeros(nall, numpy.float64)
          numpy.put(fjac, ifree, 1.0)  ## Specify which parameters need derivatives
          [status, fp, pderiv] = self.call(fcn, xall, functkw, fjac=fjac)
 
          fjac = pderiv
 
          if fjac.shape != (m, nall):
              print('ERROR: Derivative matrix was not computed properly.')
@@ -1489,15 +1498,15 @@
 
          ## Select only the free parameters
          if len(ifree) < nall:
             fjac = fjac[:,ifree]
             fjac.shape = [m, n]
             return(fjac)
 
-      fjac = numpy.zeros([m, n], numpy.float)
+      fjac = numpy.zeros([m, n], numpy.float64)
 
       h = eps * abs(x)
 
       ## if STEP is given, use that
       if step is not None:
          stepi = numpy.take(step, ifree)
          wh, = numpy.nonzero(stepi > 0)
@@ -1674,15 +1683,15 @@
       if (self.debug): print('Entering qrfac...')
       machep = self.machar.machep
       sz = numpy.shape(a)
       m = sz[0]
       n = sz[1]
 
       ## Compute the initial column norms and initialize arrays
-      acnorm = numpy.zeros(n, numpy.float)
+      acnorm = numpy.zeros(n, numpy.float64)
       for j in range(n):
          acnorm[j] = self.enorm(a[:,j])
       rdiag = acnorm.copy()
       wa = rdiag.copy()
       ipvt = numpy.arange(n)
 
       ## Reduce a to r with householder transformations
```

### Comparing `bumps-0.9.0/bumps/mystic/condition.py` & `bumps-0.9.1/bumps/mystic/condition.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/mystic/examples/__init__.py` & `bumps-0.9.1/bumps/mystic/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/mystic/examples/circle.py` & `bumps-0.9.1/bumps/mystic/examples/circle.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/mystic/examples/corana.py` & `bumps-0.9.1/bumps/mystic/examples/corana.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/mystic/examples/decay.py` & `bumps-0.9.1/bumps/mystic/examples/decay.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/mystic/examples/model.py` & `bumps-0.9.1/bumps/mystic/examples/model.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/mystic/optimizer/de.py` & `bumps-0.9.1/bumps/mystic/optimizer/de.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/mystic/optimizer/diffev_compat.py` & `bumps-0.9.1/bumps/mystic/optimizer/diffev_compat.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/mystic/solver.py` & `bumps-0.9.1/bumps/mystic/solver.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/mystic/stop.py` & `bumps-0.9.1/bumps/mystic/stop.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/mystic/util.py` & `bumps-0.9.1/bumps/mystic/util.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/names.py` & `bumps-0.9.1/bumps/names.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/numdifftools/core.py` & `bumps-0.9.1/bumps/numdifftools/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -1019,14 +1019,16 @@
         partials = [(f(x + hi, *args, **kwds) - fx) for hi in increments]
         return np.array(partials).T
 
     @staticmethod
     def _complex(f, fx, x, h, *args, **kwds):
         # From Guilherme P. de Freitas, numpy mailing list
         # http://mail.scipy.org/pipermail/numpy-discussion/2010-May/050250.html
+        # [PAK] Updated link to mailing list
+        # https://mail.python.org/archives/list/numpy-discussion@python.org/message/U76RNZMZNFO2UNYTZNVL5ZC665JOBP6C/
         n = len(x)
         increments = np.identity(n) * 1j * h
         partials = [f(x + ih, *args, **kwds).imag for ih in increments]
         return np.array(partials).T
 
     @staticmethod
     def _complex_odd(f, fx, x, h, *args, **kwds):
```

### Comparing `bumps-0.9.0/bumps/numdifftools/extrapolation.py` & `bumps-0.9.1/bumps/numdifftools/extrapolation.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/numdifftools/info.py` & `bumps-0.9.1/bumps/numdifftools/info.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/numdifftools/multicomplex.py` & `bumps-0.9.1/bumps/numdifftools/multicomplex.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/openmp_ext.py` & `bumps-0.9.1/bumps/openmp_ext.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/options.py` & `bumps-0.9.1/bumps/options.py`

 * *Files 0% similar despite different names*

```diff
@@ -303,15 +303,15 @@
     IMPLICIT_VALUES = {
         'parallel': '0',
         'entropy': 'llf',
         'resume': '-',
         }
     pars = None
     notify = ""
-    queue = "http://reflectometry.org/queue"
+    queue = None
     resynth = "0"
     noise = "5"
     starts = "1"
     seed = ""
     time = "inf"
     checkpoint = "0"
     parallel = ""
@@ -373,20 +373,14 @@
         run fit using multiprocessing for parallelism; use --parallel=0 for all cpus
     --mpi
         run fit using MPI for parallelism (use command "mpirun -n cpus ...")
     --batch
         batch mode; save output in .mon file and don't show plots after fit
     --noshow
         semi-batch; send output to console but don't show plots after fit
-    --remote
-        queue fit to run on remote server
-    --notify=user@email
-        remote fit notification
-    --queue=http://reflectometry.org
-        remote job queue
     --time=inf
         run for a maximum number of hours
     --checkpoint=0
         save fit state every n hours, or 0 for no checkpoints
 
     --fit=amoeba    [%(fitter)s]
         fitting engine to use; see manual for details
@@ -453,14 +447,20 @@
         start the interactive interpreter
     -?/-h/--help
         display this help
 """ % {'fitter': '|'.join(sorted(FIT_AVAILABLE_IDS)),
        'plotter': '|'.join(PLOTTERS),
       }
 
+#    --remote
+#        queue fit to run on remote server
+#    --notify=user@email
+#        remote fit notification
+#    --queue=http://reflectometry.org
+#        remote job queue
 #    --transport=mp  {amqp|mp|mpi}
 #        use amqp/multiprocessing/mpi for parallel evaluation
 
     _plot = 'log'
 
     def _set_plot(self, value):
         if value not in set(self.PLOTTERS):
```

### Comparing `bumps-0.9.0/bumps/parameter.py` & `bumps-0.9.1/bumps/parameter.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/partemp.py` & `bumps-0.9.1/bumps/partemp.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/pdfwrapper.py` & `bumps-0.9.1/bumps/pdfwrapper.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/plotutil.py` & `bumps-0.9.1/bumps/plotutil.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/plugin.py` & `bumps-0.9.1/bumps/plugin.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/pmath.py` & `bumps-0.9.1/bumps/pmath.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/pymcfit.py` & `bumps-0.9.1/bumps/pymcfit.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/pytwalk.py` & `bumps-0.9.1/bumps/pytwalk.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/quasinewton.py` & `bumps-0.9.1/bumps/quasinewton.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/random_lines.py` & `bumps-0.9.1/bumps/random_lines.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/simplex.py` & `bumps-0.9.1/bumps/simplex.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #__docformat__ = "restructuredtext en"
 # ******NOTICE***************
-# from optimize.py module by Travis E. Oliphant
+# From optimize.py module by Travis E. Oliphant
 #
 # You may copy and use this module as you see fit with no
 # guarantee implied provided you keep this notice in all copies.
 # *****END NOTICE************
 #
 # Modified by Paul Kienzle to support bounded minimization
 """
```

### Comparing `bumps-0.9.0/bumps/util.py` & `bumps-0.9.1/bumps/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,14 +98,18 @@
         return sys.stdin in i
 
 
 class DynamicModule(types.ModuleType):
     def __init__(self, path, name):
        self.__path__ = [path]
        self.__name__ = name
+       # In the bowels of importlib the parent spec attribute is used to
+       # avoid circular imports, but only if spec is not None. This behaviour
+       # was observed on python 3.11, and perhaps earlier.
+       self.__spec__ = None
 
 
 def relative_import(filename, module_name="relative_import"):
     """
     Define an empty module allowing relative imports from a script.
 
     By setting :code:`__package__ = relative_import(__file__)` at the top of
```

### Comparing `bumps-0.9.0/bumps/vfs.py` & `bumps-0.9.1/bumps/vfs.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps/wsolve.py` & `bumps-0.9.1/bumps/wsolve.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/bumps.egg-info/PKG-INFO` & `bumps-0.9.1/bumps.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 1.1
 Name: bumps
-Version: 0.9.0
+Version: 0.9.1
 Summary: Data fitting with bayesian uncertainty analysis
-Home-page: http://www.reflectometry.org/danse/software.html
+Home-page: https://github.com/bumps/bumps
 Author: Paul Kienzle
 Author-email: paul.kienzle@nist.gov
 License: UNKNOWN
 Description: ==============================================
         Bumps: data fitting and uncertainty estimation
         ==============================================
         
@@ -44,30 +44,46 @@
         .. |RTD| image:: https://readthedocs.org/projects/bumps/badge/?version=latest
            :alt: Documentation status
            :target: https://bumps.readthedocs.io/en/latest/?badge=latest
         
         Release notes
         =============
         
+        v0.9.1 2023-04-10
+        -----------------
+        * added support for python 3.11, scipy 1.10, numpy 1.24, wx 4.1.1
+        * fixed covariance calculation for n-D datasets
+        * fixed batch mode I/O redirection cleanup
+        * fixed issue with DREAM bounds checker when running in parallel
+        * default to single precision derivatives with lm (fixes issue in SasView
+          where OpenCL models failed with Levenberg-Marquardt)
+        * improved support for repeat fitting within scripts and notebooks
+          (*start_mapper* should now work after *stop_mapper*)
+        
         v0.9.0 2022-03-15
         -----------------
         * use MPFit in place of scipy.leastsq for bounds-constrained Levenberg-Marquardt
-        * weights are properly applied to models (nllf) in FitProblem
+        
+        Breaking change:
+        * simultaneous fit now scales individual nllfs by squared weight rather than weight
         
         v0.8.1 2021-11-18
         -----------------
         * "apply parameters" action added to GUI menu (does the same as --pars flag in CLI)
         * operators refactored (no more eval)
         * BoundedNormal keywords renamed (sigma, mu) -> (std, mean)
         * support for numba usage in models
         * fixed Parameters view jumping to top after toggling fit (linux, Mac)
         * fixed Summary view sliders disappearing in linux
         * fixed uncertainty plots regenerating at each parameter update
         * improved documentation of uncertainty analysis
         
+        Breaking change:
+        * python 2.7 support discontinued
+        
         v0.8.0 2020-12-16
         -----------------
         * add stopping conditions to DREAM, using *--alpha=p-value* to reject convergence
         * require *--overwrite* or *--resume* when reusing a store directory
         * enable outlier trimming in DREAM with --outliers=iqr
         * add fitted slope and loglikelihood distribution to the loglikelihood plot
         * display seed value used for fit so it can be rerun with *--seed*
```

### Comparing `bumps-0.9.0/bumps.egg-info/SOURCES.txt` & `bumps-0.9.1/bumps.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -125,8 +125,9 @@
 bumps/mystic/optimizer/__init__.py
 bumps/mystic/optimizer/de.py
 bumps/mystic/optimizer/diffev_compat.py
 bumps/numdifftools/__init__.py
 bumps/numdifftools/core.py
 bumps/numdifftools/extrapolation.py
 bumps/numdifftools/info.py
-bumps/numdifftools/multicomplex.py
+bumps/numdifftools/multicomplex.py
+bumps/private/__init__.py
```

### Comparing `bumps-0.9.0/bumps.iss` & `bumps-0.9.1/bumps.iss`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/master_builder.py` & `bumps-0.9.1/master_builder.py`

 * *Files identical despite different names*

### Comparing `bumps-0.9.0/setup.py` & `bumps-0.9.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 scripts = ['bin/bumps.bat'] if os.name == 'nt' else ['bin/bumps']
 #sys.dont_write_bytecode = False
 dist = setup(
     name='bumps',
     version=bumps.__version__,
     author='Paul Kienzle',
     author_email='paul.kienzle@nist.gov',
-    url='http://www.reflectometry.org/danse/software.html',
+    url='https://github.com/bumps/bumps',
     description='Data fitting with bayesian uncertainty analysis',
     long_description=open('README.rst').read(),
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
         'License :: Public Domain',
```

### Comparing `bumps-0.9.0/setup_py2exe.py` & `bumps-0.9.1/setup_py2exe.py`

 * *Files identical despite different names*

