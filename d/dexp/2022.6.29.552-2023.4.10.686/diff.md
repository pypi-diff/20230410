# Comparing `tmp/dexp-2022.6.29.552.tar.gz` & `tmp/dexp-2023.4.10.686.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexp-2022.6.29.552.tar", last modified: Wed Jun 29 16:12:19 2022, max compression
+gzip compressed data, was "dexp-2023.4.10.686.tar", last modified: Mon Apr 10 18:26:06 2023, max compression
```

## Comparing `dexp-2022.6.29.552.tar` & `dexp-2023.4.10.686.tar`

### file list

```diff
@@ -1,361 +1,362 @@
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.887153 dexp-2022.6.29.552/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1504 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/LICENSE.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     7461 2022-06-29 16:12:19.883154 dexp-2022.6.29.552/PKG-INFO
--rwxrwxr-x   0 jordao    (1000) jordao    (1000)     6191 2022-06-29 16:10:35.000000 dexp-2022.6.29.552/README.md
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.851153 dexp-2022.6.29.552/dexp/
--rwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.851153 dexp-2022.6.29.552/dexp/cli/
--rwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/cli/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      541 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/cli/config.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      102 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/cli/defaults.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.855153 dexp-2022.6.29.552/dexp/cli/dexp_commands/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1797 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/add.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1999 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/background.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      729 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/check.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1746 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/copy.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1647 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/crop.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5215 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/deconv.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1210 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/denoise.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3431 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/deskew.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1952 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/extract_psf.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1397 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/fastcopy.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1009 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/fromraw.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     7512 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/fuse.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2510 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/generic.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1097 2022-06-29 16:07:58.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/histogram.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      462 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/info.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6248 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/projrender.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4182 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/register.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2524 2022-06-29 16:07:58.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/segment.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      171 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/speedtest.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5675 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/stabilize.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2281 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/tiff.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2683 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_commands/view.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2881 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/cli/dexp_main.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1302 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/cli/install_main.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    12560 2022-06-29 16:07:58.000000 dexp-2022.6.29.552/dexp/cli/parsing.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.855153 dexp-2022.6.29.552/dexp/cli/video_commands/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/cli/video_commands/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4475 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/cli/video_commands/blend.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5212 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/cli/video_commands/mp4.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5400 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/cli/video_commands/overlay.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4071 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/cli/video_commands/resize.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4373 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/cli/video_commands/stack.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    13309 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/cli/video_commands/volrender.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      978 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/cli/video_main.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1022 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/conftest.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.859154 dexp-2022.6.29.552/dexp/datasets/
--rwxrwxr-x   0 jordao    (1000) jordao    (1000)      261 2022-02-24 16:40:24.000000 dexp-2022.6.29.552/dexp/datasets/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3845 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/base_dataset.py
--rwxrwxr-x   0 jordao    (1000) jordao    (1000)     8871 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/clearcontrol_dataset.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.859154 dexp-2022.6.29.552/dexp/datasets/demo/
--rwxrwxr-x   0 jordao    (1000) jordao    (1000)     1911 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/datasets/demo/demo_dataset.py
--rwxrwxr-x   0 jordao    (1000) jordao    (1000)     6513 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/joined_dataset.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1006 2022-06-17 00:16:51.000000 dexp-2022.6.29.552/dexp/datasets/ome_dataset.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2525 2022-04-01 22:48:19.000000 dexp-2022.6.29.552/dexp/datasets/open_dataset.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.859154 dexp-2022.6.29.552/dexp/datasets/operations/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/datasets/operations/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3114 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/background.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2424 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/copy.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4207 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/crop.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     7257 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/deconv.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.859154 dexp-2022.6.29.552/dexp/datasets/operations/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3292 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/demo/demo_copy.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3941 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/demo/demo_deconv.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3380 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/demo/demo_deskew.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3718 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/demo/demo_deskew_real.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3174 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/demo/demo_projrender.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     7005 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/demo/demo_stabilize.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4605 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/demo/demo_tiff.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2548 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/denoise.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3411 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/deskew.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1928 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/extract_psf.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2838 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/fromraw.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    10249 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/fuse.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1819 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/generic.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2555 2022-06-17 00:16:51.000000 dexp-2022.6.29.552/dexp/datasets/operations/histogram.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2569 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/projrender.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4634 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/register.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6484 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/segment.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    12467 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/stabilize.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4294 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/tiff.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6171 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/operations/view.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1197 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/stack_iterator.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.859154 dexp-2022.6.29.552/dexp/datasets/synthetic_datasets/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      351 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/synthetic_datasets/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2243 2022-01-07 19:48:45.000000 dexp-2022.6.29.552/dexp/datasets/synthetic_datasets/binary_blobs.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2234 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/synthetic_datasets/dexp_dataset.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5329 2022-01-07 19:48:45.000000 dexp-2022.6.29.552/dexp/datasets/synthetic_datasets/multiview_data.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3854 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/synthetic_datasets/nuclei_background_data.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2439 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/tiff_dataset.py
--rwxrwxr-x   0 jordao    (1000) jordao    (1000)    27300 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/datasets/zarr_dataset.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.859154 dexp-2022.6.29.552/dexp/io/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/io/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3925 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/io/compress_array.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      952 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/io/io.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.859154 dexp-2022.6.29.552/dexp/optics/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/optics/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.859154 dexp-2022.6.29.552/dexp/optics/psf/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-12-20 18:30:21.000000 dexp-2022.6.29.552/dexp/optics/psf/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.859154 dexp-2022.6.29.552/dexp/optics/psf/demo/
--rwxrwxr-x   0 jordao    (1000) jordao    (1000)      493 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/optics/psf/demo/demo.py
--rwxrwxr-x   0 jordao    (1000) jordao    (1000)    18943 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/optics/psf/microscope_psf.py
--rwxrwxr-x   0 jordao    (1000) jordao    (1000)     1689 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/optics/psf/standard_psfs.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.859154 dexp-2022.6.29.552/dexp/processing/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/processing/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.863154 dexp-2022.6.29.552/dexp/processing/color/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/processing/color/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     8825 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/blend.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1674 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/border.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1064 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/cairo_utils.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3827 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/colormap.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      919 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/conversions.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3713 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/crop_resize_pad.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.863154 dexp-2022.6.29.552/dexp/processing/color/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3112 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/demo/demo_blend.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1539 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/demo/demo_border.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1367 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/demo/demo_colormap.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1439 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/demo/demo_crop_resize_pad.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2109 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/demo/demo_insert.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4451 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/demo/demo_projection.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2479 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/demo/demo_scale_bar.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2274 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/demo/demo_time_stamp.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4594 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/insert.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    10165 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/projection.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4254 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/projection_legend.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5011 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/color/scale_bar.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5202 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/processing/color/time_stamp.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.863154 dexp-2022.6.29.552/dexp/processing/crop/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/crop/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.863154 dexp-2022.6.29.552/dexp/processing/crop/_test/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/crop/_test/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      624 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/crop/_test/test_rep_crop.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1784 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/crop/background.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.863154 dexp-2022.6.29.552/dexp/processing/crop/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/crop/demo/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1501 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/crop/demo/demo_rep_crop.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     8535 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/crop/representative_crop.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.863154 dexp-2022.6.29.552/dexp/processing/deconvolution/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      350 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4042 2022-06-16 22:43:54.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/admm_deconvolution.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2769 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/admm_utils.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2860 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/blind_deconvolution.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.867154 dexp-2022.6.29.552/dexp/processing/deconvolution/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2400 2022-02-01 20:02:04.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_admm_deconvolution_3d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2675 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_blind_deconv_3d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2089 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_inversion_deconvolution_3d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1811 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_lr_deconvolution_2d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2026 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_lr_deconvolution_2d_bs.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1778 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_lr_deconvolution_2d_wb.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2238 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2285 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d_bs.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2450 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d_sg.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4039 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d_wb.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2345 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/inversion_deconvolution.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     9853 2022-03-01 19:13:39.000000 dexp-2022.6.29.552/dexp/processing/deconvolution/lr_deconvolution.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.867154 dexp-2022.6.29.552/dexp/processing/denoising/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      114 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/denoising/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.867154 dexp-2022.6.29.552/dexp/processing/denoising/_test/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/denoising/_test/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      251 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/denoising/_test/test_butterworth.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      231 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/denoising/_test/test_gaussian.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      193 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/denoising/_test/test_noise.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    11874 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/denoising/butterworth.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.867154 dexp-2022.6.29.552/dexp/processing/denoising/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/denoising/demo/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1904 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/denoising/demo/demo_2D_butterworth.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1878 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/denoising/demo/demo_2D_gaussian.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2112 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/denoising/demo/demo_3D_butterworth.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1460 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/denoising/demo/demo_noise.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3989 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/denoising/gaussian.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    10959 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/denoising/j_invariance.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6407 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/denoising/metrics.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1168 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/denoising/noise.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.871153 dexp-2022.6.29.552/dexp/processing/deskew/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      248 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/deskew/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6147 2022-06-27 18:50:21.000000 dexp-2022.6.29.552/dexp/processing/deskew/classic_deskew.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.871153 dexp-2022.6.29.552/dexp/processing/deskew/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3864 2022-06-28 18:28:44.000000 dexp-2022.6.29.552/dexp/processing/deskew/demo/demo_classic_deskew.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4107 2022-06-28 18:28:44.000000 dexp-2022.6.29.552/dexp/processing/deskew/demo/demo_yang_deskew.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1777 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/deskew/utils.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     8308 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/deskew/yang_deskew.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.871153 dexp-2022.6.29.552/dexp/processing/equalise/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/processing/equalise/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.871153 dexp-2022.6.29.552/dexp/processing/equalise/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2163 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/equalise/demo/demo_equalise_intensity.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6017 2022-06-27 18:10:54.000000 dexp-2022.6.29.552/dexp/processing/equalise/equalise_intensity.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.871153 dexp-2022.6.29.552/dexp/processing/filters/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/processing/filters/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2582 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/filters/butterworth_filter.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.871153 dexp-2022.6.29.552/dexp/processing/filters/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1355 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/filters/demo/demo_butterworth_filter.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1467 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/filters/demo/demo_fft_convolve.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1573 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/filters/demo/demo_sobel.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2549 2022-01-07 01:10:08.000000 dexp-2022.6.29.552/dexp/processing/filters/fft_convolve.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.871153 dexp-2022.6.29.552/dexp/processing/filters/kernels/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/processing/filters/kernels/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2662 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/filters/kernels/butterworth.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.871153 dexp-2022.6.29.552/dexp/processing/filters/kernels/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1060 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/filters/kernels/demo/demo_butterworth.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      762 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/filters/kernels/demo/demo_gaussian.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1262 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/filters/kernels/demo/demo_wiener.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1395 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/filters/kernels/demo/demo_wiener_butterworth.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      974 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/filters/kernels/gaussian.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      904 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/filters/kernels/wiener.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3899 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/filters/kernels/wiener_butterworth.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3437 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/filters/sobel_filter.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.871153 dexp-2022.6.29.552/dexp/processing/fusion/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/processing/fusion/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2636 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/fusion/dct_fusion.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.875153 dexp-2022.6.29.552/dexp/processing/fusion/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2515 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/fusion/demo/demo_fusion.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2747 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/fusion/dft_fusion.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6734 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/fusion/tg_fusion.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.875153 dexp-2022.6.29.552/dexp/processing/interpolation/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/processing/interpolation/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.875153 dexp-2022.6.29.552/dexp/processing/interpolation/_cupy/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/processing/interpolation/_cupy/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2667 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/interpolation/_cupy/warp_1d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3440 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/interpolation/_cupy/warp_2d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4004 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/interpolation/_cupy/warp_3d.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.875153 dexp-2022.6.29.552/dexp/processing/interpolation/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1253 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/interpolation/demo/demo_warp_1d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1462 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/interpolation/demo/demo_warp_2d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2032 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/interpolation/demo/demo_warp_3d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3711 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/interpolation/warp.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.875153 dexp-2022.6.29.552/dexp/processing/morphology/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      142 2022-01-11 19:25:44.000000 dexp-2022.6.29.552/dexp/processing/morphology/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6145 2022-02-18 20:38:34.000000 dexp-2022.6.29.552/dexp/processing/morphology/component_tree.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      337 2022-02-01 20:02:04.000000 dexp-2022.6.29.552/dexp/processing/morphology/utils.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.875153 dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.875153 dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/deconvolution/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/deconvolution/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.875153 dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/deconvolution/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3912 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/deconvolution/demo/demo_simview_deconv.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.875153 dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/fusion/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/fusion/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2113 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/fusion/basefusion.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.875153 dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/fusion/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2232 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/fusion/demo/demo_mvsols_fusion.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2305 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/fusion/demo/demo_simview_fusion.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    17527 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/fusion/mvsols.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    13521 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/fusion/simview.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.875153 dexp-2022.6.29.552/dexp/processing/optimization/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-12-21 22:02:04.000000 dexp-2022.6.29.552/dexp/processing/optimization/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1833 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/optimization/grid_search.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.875153 dexp-2022.6.29.552/dexp/processing/registration/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/processing/registration/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.879154 dexp-2022.6.29.552/dexp/processing/registration/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5495 2022-01-07 19:48:45.000000 dexp-2022.6.29.552/dexp/processing/registration/demo/demo_sequence_2d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5990 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/demo/demo_sequence_3d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2512 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/demo/demo_translation_2d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3003 2022-01-07 19:48:45.000000 dexp-2022.6.29.552/dexp/processing/registration/demo/demo_translation_3d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2921 2022-01-07 19:48:45.000000 dexp-2022.6.29.552/dexp/processing/registration/demo/demo_translation_3d_proj.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2828 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/demo/demo_translation_3d_proj_difficult.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2327 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/demo/demo_warp_2d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2608 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/demo/demo_warp_2d_blobs.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3344 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/demo/demo_warp_3d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2315 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/demo/demo_warp_ms_2d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2981 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/demo/demo_warp_ms_3d.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.879154 dexp-2022.6.29.552/dexp/processing/registration/model/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      327 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/processing/registration/model/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.879154 dexp-2022.6.29.552/dexp/processing/registration/model/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2046 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/model/demo/demo_translation_model.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1788 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/model/demo/demo_warp_model.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2401 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/model/model_io.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1834 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/processing/registration/model/pairwise_registration_model.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     7592 2022-02-18 20:18:51.000000 dexp-2022.6.29.552/dexp/processing/registration/model/sequence_registration_model.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6552 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/model/translation_registration_model.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6846 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/model/warp_registration_model.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    11048 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/sequence.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5259 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/sequence_proj.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1921 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/translation_2d.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     7862 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/registration/translation_nd.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6432 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/registration/translation_nd_proj.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5418 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/registration/warp_multiscale_nd.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2027 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/registration/warp_nd.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.879154 dexp-2022.6.29.552/dexp/processing/remove_beads/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      107 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/remove_beads/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     7827 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/remove_beads/beadsremover.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.879154 dexp-2022.6.29.552/dexp/processing/restoration/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/processing/restoration/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2826 2022-03-01 19:13:39.000000 dexp-2022.6.29.552/dexp/processing/restoration/aap_correction.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1687 2022-03-01 19:13:39.000000 dexp-2022.6.29.552/dexp/processing/restoration/clean_dark_regions.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4366 2022-03-29 15:49:10.000000 dexp-2022.6.29.552/dexp/processing/restoration/dehazing.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.879154 dexp-2022.6.29.552/dexp/processing/restoration/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1373 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/restoration/demo/demo_aap_correction.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1595 2022-02-01 20:02:04.000000 dexp-2022.6.29.552/dexp/processing/restoration/demo/demo_clean_dark_regions.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2104 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/restoration/demo/demo_dehaze.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1442 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/restoration/demo/demo_lipschitz_continuity_correction.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3249 2022-03-01 19:13:39.000000 dexp-2022.6.29.552/dexp/processing/restoration/lipshitz_correction.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.879154 dexp-2022.6.29.552/dexp/processing/segmentation/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)       77 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/segmentation/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1108 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/segmentation/watershed.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.879154 dexp-2022.6.29.552/dexp/processing/utils/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)       62 2022-02-01 20:02:04.000000 dexp-2022.6.29.552/dexp/processing/utils/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      662 2022-02-01 20:02:04.000000 dexp-2022.6.29.552/dexp/processing/utils/apply.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1623 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/utils/blend_images.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3693 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/utils/center_of_mass.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1663 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/utils/element_wise_affine.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1055 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/utils/fit_shape.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2385 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/utils/linear_solver.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1486 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/utils/mkl_util.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      864 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/utils/nan_to_zero.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1352 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/processing/utils/nd_slice.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4643 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/utils/normalise.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2307 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/processing/utils/projection_generator.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5492 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/utils/scatter_gather_i2i.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4605 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/processing/utils/scatter_gather_i2v.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.883154 dexp-2022.6.29.552/dexp/utils/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1054 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/utils/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.883154 dexp-2022.6.29.552/dexp/utils/backends/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      247 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/utils/backends/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.883154 dexp-2022.6.29.552/dexp/utils/backends/_cupy/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/utils/backends/_cupy/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.883154 dexp-2022.6.29.552/dexp/utils/backends/_cupy/texture/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/utils/backends/_cupy/texture/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4756 2022-01-07 19:48:45.000000 dexp-2022.6.29.552/dexp/utils/backends/_cupy/texture/texture.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6943 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/utils/backends/backend.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      564 2022-02-28 23:26:27.000000 dexp-2022.6.29.552/dexp/utils/backends/best_backend.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     9363 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/utils/backends/cupy_backend.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2351 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/utils/backends/numpy_backend.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      337 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/utils/config.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      462 2022-04-01 22:12:08.000000 dexp-2022.6.29.552/dexp/utils/dask.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      563 2022-01-07 19:48:45.000000 dexp-2022.6.29.552/dexp/utils/fft.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      516 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/utils/lock.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      302 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/utils/misc.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1969 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/utils/robocopy.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      715 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/utils/slicing.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2130 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/utils/speed_test.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.883154 dexp-2022.6.29.552/dexp/utils/testing/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      277 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/utils/testing/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     1890 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/utils/testing/testing.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      307 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/utils/timeit.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.883154 dexp-2022.6.29.552/dexp/video/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/video/__init__.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     7190 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/video/blend.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     5036 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/video/crop_resize_pad.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.883154 dexp-2022.6.29.552/dexp/video/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4564 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/video/demo/demo_blend.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2862 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/video/demo/demo_crop_resize_pad.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     3015 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/video/demo/demo_overlay.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     6948 2022-01-04 17:40:33.000000 dexp-2022.6.29.552/dexp/video/overlay.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.883154 dexp-2022.6.29.552/dexp/volumerender/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2022.6.29.552/dexp/volumerender/__init__.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.883154 dexp-2022.6.29.552/dexp/volumerender/demo/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      824 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/volumerender/demo/demo_volumerender.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     2722 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/volumerender/quaternion.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     4192 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/dexp/volumerender/transform_matrices.py
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    17465 2021-12-30 22:06:16.000000 dexp-2022.6.29.552/dexp/volumerender/volumerender.py
-drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2022-06-29 16:12:19.851153 dexp-2022.6.29.552/dexp.egg-info/
--rw-rw-r--   0 jordao    (1000) jordao    (1000)     7461 2022-06-29 16:12:19.000000 dexp-2022.6.29.552/dexp.egg-info/PKG-INFO
--rw-rw-r--   0 jordao    (1000) jordao    (1000)    11973 2022-06-29 16:12:19.000000 dexp-2022.6.29.552/dexp.egg-info/SOURCES.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        1 2022-06-29 16:12:19.000000 dexp-2022.6.29.552/dexp.egg-info/dependency_links.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      127 2022-06-29 16:12:19.000000 dexp-2022.6.29.552/dexp.egg-info/entry_points.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      644 2022-06-29 16:12:19.000000 dexp-2022.6.29.552/dexp.egg-info/requires.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)        5 2022-06-29 16:12:19.000000 dexp-2022.6.29.552/dexp.egg-info/top_level.txt
--rw-rw-r--   0 jordao    (1000) jordao    (1000)      252 2022-01-11 18:38:18.000000 dexp-2022.6.29.552/pyproject.toml
--rw-rw-r--   0 jordao    (1000) jordao    (1000)       38 2022-06-29 16:12:19.887153 dexp-2022.6.29.552/setup.cfg
--rwxrwxr-x   0 jordao    (1000) jordao    (1000)     6127 2022-06-29 16:02:05.000000 dexp-2022.6.29.552/setup.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.012754 dexp-2023.4.10.686/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1504 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/LICENSE.txt
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     7821 2023-04-10 18:26:06.012754 dexp-2023.4.10.686/PKG-INFO
+-rwxrwxr-x   0 jordao    (1000) jordao    (1000)     6571 2022-08-01 17:47:30.000000 dexp-2023.4.10.686/README.md
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:05.996754 dexp-2023.4.10.686/dexp/
+-rwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:05.996754 dexp-2023.4.10.686/dexp/cli/
+-rwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/cli/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      541 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/cli/config.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      102 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/cli/defaults.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:05.996754 dexp-2023.4.10.686/dexp/cli/dexp_commands/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1797 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/add.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1999 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/background.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      729 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/check.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1746 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/copy.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1647 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/crop.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5215 2022-08-29 21:18:55.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/deconv.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1210 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/denoise.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3431 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/deskew.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1952 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/extract_psf.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1397 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/fastcopy.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1009 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/fromraw.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     7787 2023-03-01 16:44:33.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/fuse.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2510 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/generic.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1097 2022-07-06 20:37:14.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/histogram.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      462 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/info.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     6248 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/projrender.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4182 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/register.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2524 2022-07-06 20:37:14.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/segment.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      171 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/speedtest.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5675 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/stabilize.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2281 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/tiff.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2683 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_commands/view.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2881 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/cli/dexp_main.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1302 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/cli/install_main.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)    12560 2022-08-29 21:18:55.000000 dexp-2023.4.10.686/dexp/cli/parsing.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:05.996754 dexp-2023.4.10.686/dexp/cli/video_commands/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/cli/video_commands/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4475 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/cli/video_commands/blend.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5212 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/cli/video_commands/mp4.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5400 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/cli/video_commands/overlay.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4071 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/cli/video_commands/resize.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4373 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/cli/video_commands/stack.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)    13309 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/cli/video_commands/volrender.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      978 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/cli/video_main.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1022 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/conftest.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/datasets/
+-rwxrwxr-x   0 jordao    (1000) jordao    (1000)      261 2022-02-24 16:40:24.000000 dexp-2023.4.10.686/dexp/datasets/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3895 2023-03-01 16:44:33.000000 dexp-2023.4.10.686/dexp/datasets/base_dataset.py
+-rwxrwxr-x   0 jordao    (1000) jordao    (1000)     8871 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/clearcontrol_dataset.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/datasets/demo/
+-rwxrwxr-x   0 jordao    (1000) jordao    (1000)     1911 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/datasets/demo/demo_dataset.py
+-rwxrwxr-x   0 jordao    (1000) jordao    (1000)     6513 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/joined_dataset.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1006 2022-06-17 00:16:51.000000 dexp-2023.4.10.686/dexp/datasets/ome_dataset.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2525 2022-04-01 22:48:19.000000 dexp-2023.4.10.686/dexp/datasets/open_dataset.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/datasets/operations/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/datasets/operations/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3031 2022-12-22 23:06:30.000000 dexp-2023.4.10.686/dexp/datasets/operations/background.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2424 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/operations/copy.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4207 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/operations/crop.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     7174 2023-03-01 16:44:33.000000 dexp-2023.4.10.686/dexp/datasets/operations/deconv.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/datasets/operations/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3292 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/operations/demo/demo_copy.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3941 2022-08-29 21:18:55.000000 dexp-2023.4.10.686/dexp/datasets/operations/demo/demo_deconv.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3380 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/operations/demo/demo_deskew.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3718 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/operations/demo/demo_deskew_real.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3174 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/operations/demo/demo_projrender.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     7005 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/operations/demo/demo_stabilize.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4605 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/operations/demo/demo_tiff.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2465 2022-12-22 23:06:30.000000 dexp-2023.4.10.686/dexp/datasets/operations/denoise.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3328 2022-12-22 23:06:30.000000 dexp-2023.4.10.686/dexp/datasets/operations/deskew.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1845 2022-12-22 23:06:30.000000 dexp-2023.4.10.686/dexp/datasets/operations/extract_psf.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2838 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/operations/fromraw.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)    10351 2023-04-10 17:48:20.000000 dexp-2023.4.10.686/dexp/datasets/operations/fuse.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1736 2022-12-22 23:06:30.000000 dexp-2023.4.10.686/dexp/datasets/operations/generic.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2555 2022-06-17 00:16:51.000000 dexp-2023.4.10.686/dexp/datasets/operations/histogram.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2569 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/operations/projrender.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4566 2023-04-10 17:48:20.000000 dexp-2023.4.10.686/dexp/datasets/operations/register.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     6543 2022-12-22 23:06:30.000000 dexp-2023.4.10.686/dexp/datasets/operations/segment.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)    12554 2022-08-01 17:47:30.000000 dexp-2023.4.10.686/dexp/datasets/operations/stabilize.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4292 2022-12-22 23:06:30.000000 dexp-2023.4.10.686/dexp/datasets/operations/tiff.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     6171 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/operations/view.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1225 2023-03-01 16:44:33.000000 dexp-2023.4.10.686/dexp/datasets/stack_iterator.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/datasets/synthetic_datasets/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      351 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/synthetic_datasets/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2243 2022-01-07 19:48:45.000000 dexp-2023.4.10.686/dexp/datasets/synthetic_datasets/binary_blobs.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2234 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/synthetic_datasets/dexp_dataset.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5329 2022-01-07 19:48:45.000000 dexp-2023.4.10.686/dexp/datasets/synthetic_datasets/multiview_data.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3854 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/synthetic_datasets/nuclei_background_data.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2439 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/datasets/tiff_dataset.py
+-rwxrwxr-x   0 jordao    (1000) jordao    (1000)    27361 2023-04-10 15:28:59.000000 dexp-2023.4.10.686/dexp/datasets/zarr_dataset.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/io/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/io/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3925 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/io/compress_array.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      964 2022-12-22 23:06:30.000000 dexp-2023.4.10.686/dexp/io/io.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/optics/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/optics/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/optics/psf/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-12-20 18:30:21.000000 dexp-2023.4.10.686/dexp/optics/psf/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/optics/psf/demo/
+-rwxrwxr-x   0 jordao    (1000) jordao    (1000)      493 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/optics/psf/demo/demo.py
+-rwxrwxr-x   0 jordao    (1000) jordao    (1000)    18943 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/optics/psf/microscope_psf.py
+-rwxrwxr-x   0 jordao    (1000) jordao    (1000)     1689 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/optics/psf/standard_psfs.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/processing/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/processing/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/processing/color/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/processing/color/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     8825 2022-08-29 15:36:00.000000 dexp-2023.4.10.686/dexp/processing/color/blend.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1674 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/border.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1064 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/cairo_utils.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3835 2022-12-22 23:06:30.000000 dexp-2023.4.10.686/dexp/processing/color/colormap.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      919 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/conversions.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3713 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/crop_resize_pad.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/processing/color/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3112 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/demo/demo_blend.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1539 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/demo/demo_border.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1367 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/demo/demo_colormap.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1439 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/demo/demo_crop_resize_pad.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2109 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/demo/demo_insert.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4451 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/demo/demo_projection.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2479 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/demo/demo_scale_bar.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2274 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/demo/demo_time_stamp.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4594 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/insert.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)    10165 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/projection.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4254 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/color/projection_legend.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5011 2022-08-29 15:36:00.000000 dexp-2023.4.10.686/dexp/processing/color/scale_bar.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5202 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/processing/color/time_stamp.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/processing/crop/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/crop/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/processing/crop/_test/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/crop/_test/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      624 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/crop/_test/test_rep_crop.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1789 2022-08-01 17:47:30.000000 dexp-2023.4.10.686/dexp/processing/crop/background.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.000753 dexp-2023.4.10.686/dexp/processing/crop/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/crop/demo/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1501 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/crop/demo/demo_rep_crop.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     8535 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/crop/representative_crop.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/deconvolution/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      350 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4042 2022-06-16 22:43:54.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/admm_deconvolution.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2769 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/admm_utils.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2860 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/blind_deconvolution.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/deconvolution/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2400 2022-02-01 20:02:04.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_admm_deconvolution_3d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2675 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_blind_deconv_3d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2089 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_inversion_deconvolution_3d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1811 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_lr_deconvolution_2d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2026 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_lr_deconvolution_2d_bs.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1778 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_lr_deconvolution_2d_wb.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2238 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2285 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d_bs.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2450 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d_sg.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4039 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d_wb.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2345 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/inversion_deconvolution.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     9853 2022-03-01 19:13:39.000000 dexp-2023.4.10.686/dexp/processing/deconvolution/lr_deconvolution.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/denoising/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      114 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/denoising/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/denoising/_test/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/denoising/_test/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      251 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/denoising/_test/test_butterworth.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      231 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/denoising/_test/test_gaussian.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      193 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/denoising/_test/test_noise.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)    11874 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/denoising/butterworth.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/denoising/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/denoising/demo/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1904 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/denoising/demo/demo_2D_butterworth.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1878 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/denoising/demo/demo_2D_gaussian.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2112 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/denoising/demo/demo_3D_butterworth.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1484 2023-04-10 17:48:20.000000 dexp-2023.4.10.686/dexp/processing/denoising/demo/demo_noise.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3989 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/denoising/gaussian.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)    10959 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/denoising/j_invariance.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     6407 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/denoising/metrics.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1168 2023-04-10 15:27:47.000000 dexp-2023.4.10.686/dexp/processing/denoising/noise.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/deskew/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      248 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/deskew/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     6147 2022-06-27 18:50:21.000000 dexp-2023.4.10.686/dexp/processing/deskew/classic_deskew.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/deskew/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3864 2022-06-28 18:28:44.000000 dexp-2023.4.10.686/dexp/processing/deskew/demo/demo_classic_deskew.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4107 2022-06-28 18:28:44.000000 dexp-2023.4.10.686/dexp/processing/deskew/demo/demo_yang_deskew.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1777 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/deskew/utils.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     8308 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/deskew/yang_deskew.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/equalise/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/processing/equalise/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/equalise/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2163 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/equalise/demo/demo_equalise_intensity.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     6004 2023-03-01 16:44:33.000000 dexp-2023.4.10.686/dexp/processing/equalise/equalise_intensity.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/filters/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/processing/filters/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2582 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/filters/butterworth_filter.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/filters/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1355 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/filters/demo/demo_butterworth_filter.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1467 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/filters/demo/demo_fft_convolve.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1573 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/filters/demo/demo_sobel.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2549 2022-01-07 01:10:08.000000 dexp-2023.4.10.686/dexp/processing/filters/fft_convolve.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/filters/kernels/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/processing/filters/kernels/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2662 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/filters/kernels/butterworth.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/filters/kernels/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1060 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/filters/kernels/demo/demo_butterworth.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      762 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/filters/kernels/demo/demo_gaussian.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1262 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/filters/kernels/demo/demo_wiener.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1395 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/filters/kernels/demo/demo_wiener_butterworth.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      974 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/filters/kernels/gaussian.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      904 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/filters/kernels/wiener.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3899 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/filters/kernels/wiener_butterworth.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3437 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/filters/sobel_filter.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/fusion/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/processing/fusion/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2636 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/fusion/dct_fusion.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/fusion/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2515 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/fusion/demo/demo_fusion.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2747 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/fusion/dft_fusion.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     6734 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/fusion/tg_fusion.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/interpolation/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/processing/interpolation/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/interpolation/_cupy/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/processing/interpolation/_cupy/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2667 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/interpolation/_cupy/warp_1d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3440 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/interpolation/_cupy/warp_2d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4004 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/interpolation/_cupy/warp_3d.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/interpolation/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1253 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/interpolation/demo/demo_warp_1d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1462 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/interpolation/demo/demo_warp_2d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2032 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/interpolation/demo/demo_warp_3d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3711 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/interpolation/warp.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/morphology/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      142 2022-01-11 19:25:44.000000 dexp-2023.4.10.686/dexp/processing/morphology/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     6145 2022-02-18 20:38:34.000000 dexp-2023.4.10.686/dexp/processing/morphology/component_tree.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      337 2022-02-01 20:02:04.000000 dexp-2023.4.10.686/dexp/processing/morphology/utils.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/deconvolution/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/deconvolution/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.004753 dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/deconvolution/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3912 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/deconvolution/demo/demo_simview_deconv.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.008753 dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/fusion/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/fusion/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2113 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/fusion/basefusion.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.008753 dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/fusion/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2232 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/fusion/demo/demo_mvsols_fusion.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2305 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/fusion/demo/demo_simview_fusion.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)    17527 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/fusion/mvsols.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)    13521 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/fusion/simview.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.008753 dexp-2023.4.10.686/dexp/processing/optimization/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-12-21 22:02:04.000000 dexp-2023.4.10.686/dexp/processing/optimization/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1833 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/optimization/grid_search.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.008753 dexp-2023.4.10.686/dexp/processing/registration/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/processing/registration/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.008753 dexp-2023.4.10.686/dexp/processing/registration/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5495 2022-01-07 19:48:45.000000 dexp-2023.4.10.686/dexp/processing/registration/demo/demo_sequence_2d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5990 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/demo/demo_sequence_3d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2512 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/demo/demo_translation_2d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3003 2022-01-07 19:48:45.000000 dexp-2023.4.10.686/dexp/processing/registration/demo/demo_translation_3d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2921 2022-01-07 19:48:45.000000 dexp-2023.4.10.686/dexp/processing/registration/demo/demo_translation_3d_proj.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2828 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/demo/demo_translation_3d_proj_difficult.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2327 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/demo/demo_warp_2d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2608 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/demo/demo_warp_2d_blobs.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3344 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/demo/demo_warp_3d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2315 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/demo/demo_warp_ms_2d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2981 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/demo/demo_warp_ms_3d.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.008753 dexp-2023.4.10.686/dexp/processing/registration/model/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      327 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/processing/registration/model/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.008753 dexp-2023.4.10.686/dexp/processing/registration/model/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2046 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/model/demo/demo_translation_model.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1788 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/model/demo/demo_warp_model.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2401 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/model/model_io.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1834 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/processing/registration/model/pairwise_registration_model.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     7592 2022-02-18 20:18:51.000000 dexp-2023.4.10.686/dexp/processing/registration/model/sequence_registration_model.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     6552 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/model/translation_registration_model.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     6846 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/model/warp_registration_model.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)    11048 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/sequence.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5259 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/sequence_proj.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1921 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/registration/translation_2d.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     7862 2023-02-23 19:16:01.000000 dexp-2023.4.10.686/dexp/processing/registration/translation_nd.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     6432 2023-01-13 23:34:03.000000 dexp-2023.4.10.686/dexp/processing/registration/translation_nd_proj.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5418 2023-02-23 19:16:01.000000 dexp-2023.4.10.686/dexp/processing/registration/warp_multiscale_nd.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2027 2023-02-23 19:16:01.000000 dexp-2023.4.10.686/dexp/processing/registration/warp_nd.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.008753 dexp-2023.4.10.686/dexp/processing/remove_beads/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      107 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/remove_beads/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     7827 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/remove_beads/beadsremover.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.008753 dexp-2023.4.10.686/dexp/processing/restoration/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/processing/restoration/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2826 2022-03-01 19:13:39.000000 dexp-2023.4.10.686/dexp/processing/restoration/aap_correction.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1687 2022-03-01 19:13:39.000000 dexp-2023.4.10.686/dexp/processing/restoration/clean_dark_regions.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4366 2022-03-29 15:49:10.000000 dexp-2023.4.10.686/dexp/processing/restoration/dehazing.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.008753 dexp-2023.4.10.686/dexp/processing/restoration/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1373 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/restoration/demo/demo_aap_correction.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1595 2022-02-01 20:02:04.000000 dexp-2023.4.10.686/dexp/processing/restoration/demo/demo_clean_dark_regions.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2104 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/restoration/demo/demo_dehaze.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1442 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/restoration/demo/demo_lipschitz_continuity_correction.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3249 2022-03-01 19:13:39.000000 dexp-2023.4.10.686/dexp/processing/restoration/lipshitz_correction.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.008753 dexp-2023.4.10.686/dexp/processing/segmentation/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)       77 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/segmentation/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1108 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/segmentation/watershed.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.008753 dexp-2023.4.10.686/dexp/processing/utils/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)       62 2022-02-01 20:02:04.000000 dexp-2023.4.10.686/dexp/processing/utils/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      662 2022-02-01 20:02:04.000000 dexp-2023.4.10.686/dexp/processing/utils/apply.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1623 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/utils/blend_images.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3693 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/utils/center_of_mass.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1663 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/utils/element_wise_affine.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1055 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/utils/fit_shape.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2385 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/utils/linear_solver.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1486 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/utils/mkl_util.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      864 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/utils/nan_to_zero.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1352 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/processing/utils/nd_slice.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4643 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/utils/normalise.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      716 2022-08-01 17:47:30.000000 dexp-2023.4.10.686/dexp/processing/utils/pad.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2307 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/processing/utils/projection_generator.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5492 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/utils/scatter_gather_i2i.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4605 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/processing/utils/scatter_gather_i2v.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.008753 dexp-2023.4.10.686/dexp/utils/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1054 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/utils/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.012754 dexp-2023.4.10.686/dexp/utils/backends/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      247 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/utils/backends/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.012754 dexp-2023.4.10.686/dexp/utils/backends/_cupy/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/utils/backends/_cupy/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.012754 dexp-2023.4.10.686/dexp/utils/backends/_cupy/texture/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/utils/backends/_cupy/texture/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4756 2023-01-12 23:18:58.000000 dexp-2023.4.10.686/dexp/utils/backends/_cupy/texture/texture.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     6943 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/utils/backends/backend.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      564 2022-02-28 23:26:27.000000 dexp-2023.4.10.686/dexp/utils/backends/best_backend.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     9363 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/utils/backends/cupy_backend.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2351 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/utils/backends/numpy_backend.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      337 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/utils/config.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      571 2022-12-22 23:06:30.000000 dexp-2023.4.10.686/dexp/utils/dask.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      563 2022-01-07 19:48:45.000000 dexp-2023.4.10.686/dexp/utils/fft.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      516 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/utils/lock.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      302 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/utils/misc.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1969 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/utils/robocopy.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      743 2023-03-01 16:44:33.000000 dexp-2023.4.10.686/dexp/utils/slicing.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2130 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/utils/speed_test.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.012754 dexp-2023.4.10.686/dexp/utils/testing/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      277 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/utils/testing/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     1890 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/utils/testing/testing.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      307 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/utils/timeit.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.012754 dexp-2023.4.10.686/dexp/video/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/video/__init__.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     7190 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/video/blend.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     5036 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/video/crop_resize_pad.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.012754 dexp-2023.4.10.686/dexp/video/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4564 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/video/demo/demo_blend.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2862 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/video/demo/demo_crop_resize_pad.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     3015 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/video/demo/demo_overlay.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     6948 2022-01-04 17:40:33.000000 dexp-2023.4.10.686/dexp/video/overlay.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.012754 dexp-2023.4.10.686/dexp/volumerender/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        0 2021-10-28 22:00:45.000000 dexp-2023.4.10.686/dexp/volumerender/__init__.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:06.012754 dexp-2023.4.10.686/dexp/volumerender/demo/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      824 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/volumerender/demo/demo_volumerender.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     2722 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/volumerender/quaternion.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     4192 2022-06-29 16:02:05.000000 dexp-2023.4.10.686/dexp/volumerender/transform_matrices.py
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)    17465 2021-12-30 22:06:16.000000 dexp-2023.4.10.686/dexp/volumerender/volumerender.py
+drwxrwxr-x   0 jordao    (1000) jordao    (1000)        0 2023-04-10 18:26:05.996754 dexp-2023.4.10.686/dexp.egg-info/
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)     7821 2023-04-10 18:26:05.000000 dexp-2023.4.10.686/dexp.egg-info/PKG-INFO
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)    12002 2023-04-10 18:26:05.000000 dexp-2023.4.10.686/dexp.egg-info/SOURCES.txt
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        1 2023-04-10 18:26:05.000000 dexp-2023.4.10.686/dexp.egg-info/dependency_links.txt
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      126 2023-04-10 18:26:05.000000 dexp-2023.4.10.686/dexp.egg-info/entry_points.txt
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      653 2023-04-10 18:26:05.000000 dexp-2023.4.10.686/dexp.egg-info/requires.txt
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)        5 2023-04-10 18:26:05.000000 dexp-2023.4.10.686/dexp.egg-info/top_level.txt
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)      252 2022-01-11 18:38:18.000000 dexp-2023.4.10.686/pyproject.toml
+-rw-rw-r--   0 jordao    (1000) jordao    (1000)       38 2023-04-10 18:26:06.012754 dexp-2023.4.10.686/setup.cfg
+-rwxrwxr-x   0 jordao    (1000) jordao    (1000)     6148 2022-08-01 17:47:30.000000 dexp-2023.4.10.686/setup.py
```

### Comparing `dexp-2022.6.29.552/LICENSE.txt` & `dexp-2023.4.10.686/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/PKG-INFO` & `dexp-2023.4.10.686/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dexp
-Version: 2022.6.29.552
+Version: 2023.4.10.686
 Summary: Light-sheet Dataset EXploration and Processing
 Home-page: https://github.com/royerlab/dexp
 Author: Jordao Bragantini, Ahmet Can Solak, Bin Yang, Loic A Royer
 Author-email: jordao.bragantini@czbiohub.org, ahmetcan.solak@czbiohub.org, bin.yang@czbiohub.org, loic.royer@czbiohub.org
 License: BSD 3-Clause
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -70,34 +69,43 @@
 **For OSX users:** Before installating dexp, you will first need to install cairo:
 ```
 brew install cairo
 ```
 
 ### Quick conda environment setup and installation:
 
-The following commands delete any existing dexp environment, recreate it, install **dexp** with CUDA support and [napari](https://napari.org/):
-```
-conda deactivate
-conda env remove --name dexp
-conda create -y --name dexp python=3.9
-conda activate dexp
-conda install cupy
-pip install napari[all]
-```
+There are multiple options when using a conda environment:
 
-If you are having problems with the cuda/cuda-toolkit the best is to use conda to install the correct version of the cudatoolkit:
-```
-conda install -c conda-forge cudatoolkit==11.2.2
-```
-You can check [here](https://anaconda.org/conda-forge/cudatoolkit/files) for the best matching version.
+- You can create our suggested DEXP (and some additional packages) environment by, it requires GPU:
 
-Notes:
-- You might get some error messages recommending you install missing libraries such as CUDNN, CuTensor, nccl, etc... These messages often come with instructions on what to do.
-- Adjust your driver version (here 11.2) to your card(s) and drivers.
-- Windows users should call `conda install -c conda-forge pyopencl` before running the second to last step.
+   ```
+   conda env create --name dexp --file env-linux-gpu.yaml
+   ```
+
+- Or create your own conda environment from scratch with the following commands delete any existing dexp environment, recreate it, install **dexp** with CUDA support and [napari](https://napari.org/):
+   ```
+   conda deactivate
+   conda env remove --name dexp
+   conda create -y --name dexp python=3.9
+   conda activate dexp
+   conda install cupy
+   pip install dexp[optional,colored]
+   pip install napari[all]
+   ```
+
+   If you are having problems with the cuda/cuda-toolkit the best is to use conda to install the correct version of the cudatoolkit:
+   ```
+   conda install -c conda-forge cudatoolkit==11.2.2
+   ```
+   You can check [here](https://anaconda.org/conda-forge/cudatoolkit/files) for the best matching version.
+
+   Notes:
+   - You might get some error messages recommending you install missing libraries such as CUDNN, CuTensor, nccl, etc... These messages often come with instructions on what to do.
+   - Adjust your driver version (here 11.2) to your card(s) and drivers.
+   - Windows users should call `conda install -c conda-forge pyopencl` before running the second to last step.
 
 ### Leveraging extra CUDA libraries for faster processing:
 
 If you want you **dexp** CUDA-based processing to be even faster, you can install additional libraries such as CUDNN and CUTENSOR
 with the following command:
 
 ```
@@ -155,9 +163,7 @@
 ### How to use **dexp** ?
 
 In depth documentation can be found [here](https://royerlab.github.io/dexp/index.html) for both command line  commands and for the python API.
 
 ### Contributors:
 
 Jordao Bragantini, Ahmet Can Solak, Bin Yang, and Loic A Royer
-
-
```

### Comparing `dexp-2022.6.29.552/README.md` & `dexp-2023.4.10.686/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -33,34 +33,43 @@
 **For OSX users:** Before installating dexp, you will first need to install cairo:
 ```
 brew install cairo
 ```
 
 ### Quick conda environment setup and installation:
 
-The following commands delete any existing dexp environment, recreate it, install **dexp** with CUDA support and [napari](https://napari.org/):
-```
-conda deactivate
-conda env remove --name dexp
-conda create -y --name dexp python=3.9
-conda activate dexp
-conda install cupy
-pip install napari[all]
-```
+There are multiple options when using a conda environment:
 
-If you are having problems with the cuda/cuda-toolkit the best is to use conda to install the correct version of the cudatoolkit:
-```
-conda install -c conda-forge cudatoolkit==11.2.2
-```
-You can check [here](https://anaconda.org/conda-forge/cudatoolkit/files) for the best matching version.
+- You can create our suggested DEXP (and some additional packages) environment by, it requires GPU:
 
-Notes:
-- You might get some error messages recommending you install missing libraries such as CUDNN, CuTensor, nccl, etc... These messages often come with instructions on what to do.
-- Adjust your driver version (here 11.2) to your card(s) and drivers.
-- Windows users should call `conda install -c conda-forge pyopencl` before running the second to last step.
+   ```
+   conda env create --name dexp --file env-linux-gpu.yaml
+   ```
+
+- Or create your own conda environment from scratch with the following commands delete any existing dexp environment, recreate it, install **dexp** with CUDA support and [napari](https://napari.org/):
+   ```
+   conda deactivate
+   conda env remove --name dexp
+   conda create -y --name dexp python=3.9
+   conda activate dexp
+   conda install cupy
+   pip install dexp[optional,colored]
+   pip install napari[all]
+   ```
+
+   If you are having problems with the cuda/cuda-toolkit the best is to use conda to install the correct version of the cudatoolkit:
+   ```
+   conda install -c conda-forge cudatoolkit==11.2.2
+   ```
+   You can check [here](https://anaconda.org/conda-forge/cudatoolkit/files) for the best matching version.
+
+   Notes:
+   - You might get some error messages recommending you install missing libraries such as CUDNN, CuTensor, nccl, etc... These messages often come with instructions on what to do.
+   - Adjust your driver version (here 11.2) to your card(s) and drivers.
+   - Windows users should call `conda install -c conda-forge pyopencl` before running the second to last step.
 
 ### Leveraging extra CUDA libraries for faster processing:
 
 If you want you **dexp** CUDA-based processing to be even faster, you can install additional libraries such as CUDNN and CUTENSOR
 with the following command:
 
 ```
```

### Comparing `dexp-2022.6.29.552/dexp/cli/config.py` & `dexp-2023.4.10.686/dexp/cli/config.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/add.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/add.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/background.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/background.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/check.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/check.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/copy.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/copy.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/crop.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/crop.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/deconv.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/deconv.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/denoise.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/denoise.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/deskew.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/deskew.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/extract_psf.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/extract_psf.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/fastcopy.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/fastcopy.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/fromraw.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/fromraw.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/fuse.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/fuse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Sequence, Tuple
+from typing import Optional, Sequence, Tuple
 
 import click
 from arbol.arbol import aprint, asection
 
 from dexp.cli.parsing import (
     channels_option,
     input_dataset_argument,
@@ -179,14 +179,21 @@
 @click.option(
     "--remove-beads",
     "-rb",
     is_flag=True,
     default=False,
     help="Use this flag to remove beads before equalizing and fusing",
 )
+@click.option(
+    "--equalisation-ratios",
+    "-eqr",
+    default=None,
+    callback=tuple_callback(dtype=float),
+    help="Manually set equalisation ratios",
+)
 def fuse(
     input_dataset: BaseDataset,
     output_dataset: ZDataset,
     channels: Sequence[str],
     microscope: str,
     equalise: bool,
     equalisemode: str,
@@ -206,14 +213,15 @@
     maxproj: bool,
     hugedataset: bool,
     devices: Sequence[int],
     pad: bool,
     white_top_hat_size: float,
     white_top_hat_sampling: int,
     remove_beads: bool,
+    equalisation_ratios: Optional[Tuple[float]],
 ):
     """Fuses the views of a multi-view light-sheet microscope dataset (available: simview and mvsols)"""
 
     with asection(
         f"Fusing dataset: {input_dataset.path}, saving it at: {output_dataset.path},"
         + f"for channels: {channels}, slicing: {input_dataset.slicing}"
     ):
@@ -243,12 +251,13 @@
             maxproj=maxproj,
             huge_dataset=hugedataset,
             devices=devices,
             pad=pad,
             white_top_hat_size=white_top_hat_size,
             white_top_hat_sampling=white_top_hat_sampling,
             remove_beads=remove_beads,
+            equalisation_ratios=equalisation_ratios,
         )
 
         input_dataset.close()
         output_dataset.close()
         aprint("Done!")
```

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/generic.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/generic.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/histogram.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/histogram.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/projrender.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/projrender.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/register.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/register.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/segment.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/segment.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/stabilize.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/stabilize.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/tiff.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/tiff.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_commands/view.py` & `dexp-2023.4.10.686/dexp/cli/dexp_commands/view.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/dexp_main.py` & `dexp-2023.4.10.686/dexp/cli/dexp_main.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/install_main.py` & `dexp-2023.4.10.686/dexp/cli/install_main.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/parsing.py` & `dexp-2023.4.10.686/dexp/cli/parsing.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/video_commands/blend.py` & `dexp-2023.4.10.686/dexp/cli/video_commands/blend.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/video_commands/mp4.py` & `dexp-2023.4.10.686/dexp/cli/video_commands/mp4.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/video_commands/overlay.py` & `dexp-2023.4.10.686/dexp/cli/video_commands/overlay.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/video_commands/resize.py` & `dexp-2023.4.10.686/dexp/cli/video_commands/resize.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/video_commands/stack.py` & `dexp-2023.4.10.686/dexp/cli/video_commands/stack.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/video_commands/volrender.py` & `dexp-2023.4.10.686/dexp/cli/video_commands/volrender.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/cli/video_main.py` & `dexp-2023.4.10.686/dexp/cli/video_main.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/conftest.py` & `dexp-2023.4.10.686/dexp/conftest.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/base_dataset.py` & `dexp-2023.4.10.686/dexp/datasets/base_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,19 +107,20 @@
     def write_stack(self, channel: str, time_point: int, stack: numpy.ndarray):
         pass
 
     @abstractmethod
     def check_integrity(self, channels: Sequence[str]) -> bool:
         pass
 
-    def set_slicing(self, slicing: slice) -> None:
+    def set_slicing(self, slicing: slice) -> "BaseDataset":
         self._slicing = slicing
+        return self
 
     @property
-    def slicing(self) -> slice:
+    def slicing(self) -> Union[slice, Tuple[slice]]:
         return self._slicing
 
     def __getitem__(self, channel: str) -> StackIterator:
         return StackIterator(self.get_array(channel), self._slicing)
 
     @property
     def path(self) -> str:
```

### Comparing `dexp-2022.6.29.552/dexp/datasets/clearcontrol_dataset.py` & `dexp-2023.4.10.686/dexp/datasets/clearcontrol_dataset.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/demo/demo_dataset.py` & `dexp-2023.4.10.686/dexp/datasets/demo/demo_dataset.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/joined_dataset.py` & `dexp-2023.4.10.686/dexp/datasets/joined_dataset.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/ome_dataset.py` & `dexp-2023.4.10.686/dexp/datasets/ome_dataset.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/open_dataset.py` & `dexp-2023.4.10.686/dexp/datasets/open_dataset.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/background.py` & `dexp-2023.4.10.686/dexp/datasets/operations/background.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from typing import Callable, Dict, Optional, Sequence
 
 import dask
 import numpy as np
 from arbol import aprint, asection, section
-from dask.distributed import Client
-from dask_cuda import LocalCUDACluster
 from toolz import curry, reduce
 
 from dexp.datasets import BaseDataset, ZDataset
 from dexp.datasets.stack_iterator import StackIterator
 from dexp.processing.crop.background import foreground_mask
 from dexp.utils.backends.cupy_backend import CupyBackend
+from dexp.utils.dask import get_dask_client
 
 
 @dask.delayed
 @curry
 def _process(
     time_point: int,
     time_scale: Dict[str, int],
@@ -77,15 +76,14 @@
     )
 
     for ch in channels:
         output_dataset.add_channel(ch, input_dataset.shape(ch), input_dataset.dtype(ch))
 
     lazy_computations = [process(time_point=t) for t in range(max_t)]
 
-    cluster = LocalCUDACluster(CUDA_VISIBLE_DEVICES=devices)
-    client = Client(cluster)
+    client = get_dask_client(devices)
     aprint("Dask client", client)
 
     # Compute everything
     dask.compute(*lazy_computations)
 
     output_dataset.check_integrity()
```

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/copy.py` & `dexp-2023.4.10.686/dexp/datasets/operations/copy.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/crop.py` & `dexp-2023.4.10.686/dexp/datasets/operations/crop.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/deconv.py` & `dexp-2023.4.10.686/dexp/datasets/operations/deconv.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,28 @@
 from pathlib import Path
 from typing import Callable, List, Optional, Sequence, Tuple
 
 import dask
 import numpy as np
 import scipy
 from arbol.arbol import aprint, asection
-from dask.distributed import Client
-from dask_cuda import LocalCUDACluster
 from toolz import curry
 
 from dexp.datasets import BaseDataset
 from dexp.datasets.stack_iterator import StackIterator
 from dexp.datasets.zarr_dataset import ZDataset
 from dexp.optics.psf.standard_psfs import nikon16x08na, olympus20x10na
 from dexp.processing.deconvolution import (
     admm_deconvolution,
     lucy_richardson_deconvolution,
 )
 from dexp.processing.filters.fft_convolve import fft_convolve
 from dexp.processing.utils.scatter_gather_i2i import scatter_gather_i2i
 from dexp.utils.backends import BestBackend
+from dexp.utils.dask import get_dask_client
 
 
 def get_psf(
     psf_objective: str,
     psf_na: float,
     psf_dxy: float,
     psf_dz: float,
@@ -184,14 +183,18 @@
     psf_dz: float,
     psf_xy_size: int,
     psf_z_size: int,
     psf_show: bool,
     scaling: Tuple[float],
     devices: List[int],
 ):
+    # CUDA DASK cluster
+    client = get_dask_client(devices)
+    aprint("Dask Client", client)
+
     aprint(f"Input images will be scaled by: (sz,sy,sx)={scaling}")
 
     psf_kernel = get_psf(psf_objective, psf_na, psf_dxy, psf_dz, psf_z_size, psf_xy_size, scaling, psf_show)
     margins = max(psf_kernel.shape[1], psf_kernel.shape[0])
 
     deconv_func = get_deconv_func(
         method,
@@ -231,17 +234,12 @@
         )
 
         for t in range(len(stacks)):
             lazy_computation.append(process(time_point=t))
 
     dask.compute(*lazy_computation)
 
-    # CUDA DASK cluster
-    cluster = LocalCUDACluster(CUDA_VISIBLE_DEVICES=devices)
-    client = Client(cluster)
-    aprint("Dask Client", client)
-
     # Dataset info:
     aprint(output_dataset.info())
 
     # Check dataset integrity:
     output_dataset.check_integrity()
```

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/demo/demo_copy.py` & `dexp-2023.4.10.686/dexp/datasets/operations/demo/demo_copy.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/demo/demo_deconv.py` & `dexp-2023.4.10.686/dexp/datasets/operations/demo/demo_deconv.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/demo/demo_deskew.py` & `dexp-2023.4.10.686/dexp/datasets/operations/demo/demo_deskew.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/demo/demo_deskew_real.py` & `dexp-2023.4.10.686/dexp/datasets/operations/demo/demo_deskew_real.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/demo/demo_projrender.py` & `dexp-2023.4.10.686/dexp/datasets/operations/demo/demo_projrender.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/demo/demo_stabilize.py` & `dexp-2023.4.10.686/dexp/datasets/operations/demo/demo_stabilize.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/demo/demo_tiff.py` & `dexp-2023.4.10.686/dexp/datasets/operations/demo/demo_tiff.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/denoise.py` & `dexp-2023.4.10.686/dexp/datasets/operations/deskew.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,116 @@
-from typing import Callable, Sequence, Tuple
+from typing import Callable, List, Optional, Sequence
 
 import dask
-from arbol import aprint, asection
-from dask.distributed import Client
-from dask_cuda import LocalCUDACluster
+import fasteners
+from arbol.arbol import aprint, asection
 from toolz import curry
 
-from dexp.datasets import BaseDataset, ZDataset
+from dexp.datasets import BaseDataset
 from dexp.datasets.stack_iterator import StackIterator
-from dexp.processing.denoising import calibrate_denoise_butterworth, denoise_butterworth
-from dexp.processing.utils.scatter_gather_i2i import scatter_gather_i2i
-from dexp.utils.backends import CupyBackend
-from dexp.utils.fft import clear_fft_plan_cache
+from dexp.datasets.zarr_dataset import ZDataset
+from dexp.processing.deskew import deskew_functions
+from dexp.utils.backends import BestBackend
+from dexp.utils.dask import get_dask_client
+from dexp.utils.lock import create_lock
 
 
+@dask.delayed
 @curry
 def _process(
+    time_point: int,
     stacks: StackIterator,
-    out_dataset: ZDataset,
     channel: str,
-    time_point: int,
-    scatter_gather: Callable,
+    output_dataset: ZDataset,
+    lock: fasteners.InterProcessLock,
+    deskew_func: Callable,
 ) -> None:
+    with asection(f"Deskweing channel {channel} at time point {time_point}."):
+        with BestBackend() as bkd:
+            with asection("Loading data"):
+                stack = bkd.to_backend(stacks[time_point])
+            with asection("Processing"):
+                stack = deskew_func(stack)
+            stack = bkd.to_numpy(stack)
+
+        with lock:
+            if channel not in output_dataset:
+                output_dataset.add_channel(
+                    channel,
+                    (len(stacks),) + stack.shape,
+                    dtype=stack.dtype,
+                )
 
-    with CupyBackend() as bkd:
-        with asection(f"Calibrating and denoising channel {channel} time point {time_point}"):
-            stack = bkd.to_backend(stacks[time_point])
-            _, best_params = calibrate_denoise_butterworth(stack)
-            denoise_fun = curry(denoise_butterworth, **best_params)
-
-            with asection("Denoising"):
-                denoised = scatter_gather(function=denoise_fun, image=stack)
-
-            out_dataset.write_stack(channel, time_point, bkd.to_numpy(denoised))
-            clear_fft_plan_cache()
+        with asection("Saving deskwed array"):
+            output_dataset.write_stack(channel, time_point, stack)
 
 
-def dataset_denoise(
+def dataset_deskew(
     input_dataset: BaseDataset,
     output_dataset: ZDataset,
     channels: Sequence[str],
-    tilesize: Tuple[int],
-    devices: Sequence[int],
+    dx: Optional[float],
+    dz: Optional[float],
+    angle: Optional[float],
+    flips: Sequence[bool],
+    camera_orientation: int,
+    depth_axis: int,
+    lateral_axis: int,
+    mode: str,
+    padding: bool,
+    devices: List[int],
 ):
-    # NOTE:
-    #   we might want in the future to smooth the parameters estimation over neighboring time points.
-    lazy_computations = []
+    # Default flipping:
+    if flips is None:
+        flips = (False,) * len(channels)
+
+    # Metadata for deskewing:
+    metadata = input_dataset.get_metadata()
+    aprint(f"Dataset metadata: {metadata}")
+    if dx is None and "res" in metadata:
+        dx = float(metadata["res"])
+    if dz is None and "dz" in metadata:
+        dz = float(metadata["dz"])
+    if angle is None and "angle" in metadata:
+        angle = float(metadata["angle"])
+
+    # setting up fixed parameters
+    aprint(f"Deskew parameters: dx={dx}, dz={dz}, angle={angle}")
+    deskew_func = curry(
+        deskew_functions[mode],
+        depth_axis=depth_axis,
+        lateral_axis=lateral_axis,
+        dx=dx,
+        dz=dz,
+        angle=angle,
+        camera_orientation=camera_orientation,
+        padding=padding,
+    )
 
-    for ch in channels:
-        stacks = input_dataset[ch]
-        output_dataset.add_channel(ch, stacks.shape, dtype=input_dataset.dtype(ch))
+    lazy_computations = []
 
-        # Create processing function with default parameters
-        process = dask.delayed(
+    # Iterate through channels
+    for i, channel in enumerate(channels):
+        stacks = input_dataset[channel]
+        lock = create_lock(channel)
+        lazy_computations += [
             _process(
+                time_point=t,
                 stacks=stacks,
-                out_dataset=output_dataset,
-                channel=ch,
-                scatter_gather=curry(scatter_gather_i2i, tiles=tilesize, margins=32),
+                channel=channel,
+                lock=lock,
+                output_dataset=output_dataset,
+                deskew_func=deskew_func(flip_depth_axis=flips[i]),
             )
-        )  # using 32 because Jordao assumed it's good enough and 320 (default tile) + 64 = 384
-        # has a nice prime factorization, speeding up fft computation
+            for t in range(len(stacks))
+        ]
 
-        # Stores functions to be computed
-        lazy_computations += [process(time_point=t) for t in range(len(stacks))]
+    # setting up dask compute scheduler
+    client = get_dask_client(devices)
 
-    cluster = LocalCUDACluster(CUDA_VISIBLE_DEVICES=devices)
-    client = Client(cluster)
     aprint("Dask client", client)
-
-    # Compute everything
     dask.compute(*lazy_computations)
 
+    # shape and dtype of views to deskew:
     output_dataset.check_integrity()
+
+    aprint(output_dataset.info())
```

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/deskew.py` & `dexp-2023.4.10.686/dexp/datasets/operations/projrender.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,118 +1,84 @@
-from typing import Callable, List, Optional, Sequence
+from pathlib import Path
+from typing import Callable, Sequence
 
 import dask
-import fasteners
+import imageio
+import numpy as np
 from arbol.arbol import aprint, asection
 from dask.distributed import Client
-from dask_cuda import LocalCUDACluster
 from toolz import curry
 
 from dexp.datasets import BaseDataset
 from dexp.datasets.stack_iterator import StackIterator
-from dexp.datasets.zarr_dataset import ZDataset
-from dexp.processing.deskew import deskew_functions
+from dexp.processing.color.projection import project_image
 from dexp.utils.backends import BestBackend
-from dexp.utils.lock import create_lock
+from dexp.utils.backends.cupy_backend import is_cupy_available
 
 
 @dask.delayed
 @curry
-def _process(
-    time_point: int,
-    stacks: StackIterator,
-    channel: str,
-    output_dataset: ZDataset,
-    lock: fasteners.InterProcessLock,
-    deskew_func: Callable,
-) -> None:
-    with asection(f"Deskweing channel {channel} at time point {time_point}."):
-        with BestBackend() as bkd:
-            with asection("Loading data"):
-                stack = bkd.to_backend(stacks[time_point])
-            with asection("Processing"):
-                stack = deskew_func(stack)
-            stack = bkd.to_numpy(stack)
-
-        with lock:
-            if channel not in output_dataset:
-                output_dataset.add_channel(
-                    channel,
-                    (len(stacks),) + stack.shape,
-                    dtype=stack.dtype,
-                )
+def _process(time_point: int, stacks: StackIterator, outpath: Path, project_func: Callable, overwrite: bool) -> None:
+    with asection(f"Rendering Frame \t: {time_point:05}"):
 
-        with asection("Saving deskwed array"):
-            output_dataset.write_stack(channel, time_point, stack)
+        filename = outpath / f"frame_{time_point:05}.png"
 
+        if overwrite or not filename.exists():
 
-def dataset_deskew(
+            with asection("Loading stack..."):
+                stack = np.asarray(stacks[time_point])
+
+            with BestBackend() as bkd:
+                with asection(f"Projecting image of shape: {stack.shape} "):
+                    projection = bkd.to_numpy(project_func(bkd.to_backend(stack)))
+
+                with asection(f"Saving frame {time_point} as: {filename}"):
+                    imageio.imwrite(filename, projection, compress_level=1)
+
+
+def dataset_projection_rendering(
     input_dataset: BaseDataset,
-    output_dataset: ZDataset,
+    output_path: Path,
     channels: Sequence[str],
-    dx: Optional[float],
-    dz: Optional[float],
-    angle: Optional[float],
-    flips: Sequence[bool],
-    camera_orientation: int,
-    depth_axis: int,
-    lateral_axis: int,
-    mode: str,
-    padding: bool,
-    devices: List[int],
+    overwrite: bool,
+    devices: Sequence[int],
+    **kwargs,
 ):
-    # Default flipping:
-    if flips is None:
-        flips = (False,) * len(channels)
-
-    # Metadata for deskewing:
-    metadata = input_dataset.get_metadata()
-    aprint(f"Dataset metadata: {metadata}")
-    if dx is None and "res" in metadata:
-        dx = float(metadata["res"])
-    if dz is None and "dz" in metadata:
-        dz = float(metadata["dz"])
-    if angle is None and "angle" in metadata:
-        angle = float(metadata["angle"])
-
-    # setting up fixed parameters
-    aprint(f"Deskew parameters: dx={dx}, dz={dz}, angle={angle}")
-    deskew_func = curry(
-        deskew_functions[mode],
-        depth_axis=depth_axis,
-        lateral_axis=lateral_axis,
-        dx=dx,
-        dz=dz,
-        angle=angle,
-        camera_orientation=camera_orientation,
-        padding=padding,
-    )
-
+    project_func = curry(project_image, **kwargs)
     lazy_computations = []
 
-    # Iterate through channels
-    for i, channel in enumerate(channels):
+    for channel in channels:
+        # Ensures that the output folder exists per channel:
+        if len(channels) == 1:
+            channel_output_path = output_path
+        else:
+            channel_output_path = output_path / channel
+
+        channel_output_path.mkdir(exist_ok=True, parents=True)
+
         stacks = input_dataset[channel]
-        lock = create_lock(channel)
-        lazy_computations += [
-            _process(
-                time_point=t,
-                stacks=stacks,
-                channel=channel,
-                lock=lock,
-                output_dataset=output_dataset,
-                deskew_func=deskew_func(flip_depth_axis=flips[i]),
-            )
-            for t in range(len(stacks))
-        ]
-
-    # setting up dask compute scheduler
-    cluster = LocalCUDACluster(CUDA_VISIBLE_DEVICES=devices)
-    client = Client(cluster)
 
+        process = _process(
+            stacks=stacks,
+            outpath=channel_output_path,
+            project_func=project_func,
+            overwrite=overwrite,
+        )
+
+        with asection(f"Channel '{channel}' shape: {stacks.shape}:"):
+            aprint(input_dataset.info(channel))
+
+        lazy_computations += [process(time_point=t) for t in range(len(stacks))]
+
+    if len(devices) > 0 and is_cupy_available():
+        from dask_cuda import LocalCUDACluster
+
+        cluster = LocalCUDACluster(CUDA_VISIBLE_DEVICES=devices)
+        client = Client(cluster)
+    else:
+        client = Client()
     aprint("Dask client", client)
-    dask.compute(*lazy_computations)
 
-    # shape and dtype of views to deskew:
-    output_dataset.check_integrity()
+    # Compute everything
+    dask.compute(*lazy_computations)
 
-    aprint(output_dataset.info())
+    client.close()
```

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/extract_psf.py` & `dexp-2023.4.10.686/dexp/datasets/operations/extract_psf.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import warnings
 from typing import Callable, Sequence
 
 import dask
 import numpy as np
 from arbol import aprint, asection
-from dask.distributed import Client
-from dask_cuda import LocalCUDACluster
 from toolz import curry
 
 from dexp.datasets.stack_iterator import StackIterator
 from dexp.datasets.zarr_dataset import ZDataset
 from dexp.processing.remove_beads import BeadsRemover
 from dexp.utils.backends.best_backend import BestBackend
+from dexp.utils.dask import get_dask_client
 
 
 @curry
 def _process(
     time_point: int,
     stacks: StackIterator,
     create_beads_remover: Callable[..., BeadsRemover],
@@ -40,16 +39,15 @@
     """
     Computes PSF from beads.
     Additional information at dexp.processing.remove_beads.beadremover documentation.
     """
     warnings.warn("This command is subpar, it should be improved.")
     dest_path = dest_path.split(".")[0]
 
-    cluster = LocalCUDACluster(CUDA_VISIBLE_DEVICES=devices)
-    client = Client(cluster)
+    client = get_dask_client(devices)
     aprint("Dask client", client)
 
     def create_beads_remover() -> BeadsRemover:
         return BeadsRemover(
             peak_threshold=peak_threshold, similarity_threshold=similarity_threshold, psf_size=psf_size, verbose=verbose
         )
```

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/fromraw.py` & `dexp-2023.4.10.686/dexp/datasets/operations/fromraw.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/fuse.py` & `dexp-2023.4.10.686/dexp/datasets/operations/fuse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from pathlib import Path
 from typing import Callable, Dict, List, Optional, Sequence, Tuple
 
 import dask
 import numpy as np
 from arbol.arbol import aprint, asection
-from dask.distributed import Client
-from dask_cuda import LocalCUDACluster
 from toolz import curry
 
 from dexp.datasets import BaseDataset, ZDataset
 from dexp.datasets.stack_iterator import StackIterator
 from dexp.processing.multiview_lightsheet.fusion.mvsols import msols_fuse_1C2L
 from dexp.processing.multiview_lightsheet.fusion.simview import SimViewFusion
 from dexp.processing.registration.model.model_io import (
@@ -17,14 +15,15 @@
     model_list_to_file,
 )
 from dexp.processing.registration.model.pairwise_registration_model import (
     PairwiseRegistrationModel,
 )
 from dexp.utils import xpArray
 from dexp.utils.backends import Backend, BestBackend
+from dexp.utils.dask import get_dask_client
 
 
 def load_registration_models(model_list_filename: Path, n_time_pts: int) -> Sequence[PairwiseRegistrationModel]:
     aprint(f"Loading registration shifts from existing file! ({model_list_filename})")
     models = model_list_from_file(model_list_filename)
     if len(models) == 1:
         models = [models[0] for _ in range(n_time_pts)]
@@ -207,19 +206,20 @@
     registration_edge_filter: bool,
     maxproj: bool,
     huge_dataset: bool,
     pad: bool,
     white_top_hat_size: float,
     white_top_hat_sampling: int,
     remove_beads: bool,
+    equalisation_ratios: Optional[Tuple[float]],
     devices: Sequence[int],
 ):
 
     views = {channel.split("-")[-1]: input_dataset[channel] for channel in channels}
-    n_time_pts = len(list(views.values())[0])
+    n_time_pts = min(arr.shape[0] for arr in views.values())
 
     with asection("Views:"):
         for channel, view in views.items():
             aprint(f"View: {channel} of shape: {view.shape} and dtype: {view.dtype}")
 
     if microscope == "simview":
         views = SimViewFusion.validate_views(views)
@@ -249,32 +249,34 @@
         pad=pad,
         loadreg=loadreg,
         white_top_hat_size=white_top_hat_size,
         white_top_hat_sampling=white_top_hat_sampling,
         remove_beads=remove_beads,
     )
 
+    if equalisation_ratios is not None:
+        equalisation_ratios = list(equalisation_ratios)
+
     # it creates the output dataset from the first time point output shape
-    equalisation_ratios, model = _process(
+    first_eq_ratios, model = _process(
         time_point=0,
         views=views,
         out_dataset=output_dataset,
         fusion_func=fusion_func(
             model=models[0] if loadreg else None,
-            equalisation_ratios=None,
+            equalisation_ratios=equalisation_ratios,
         ),
     )
 
-    if equalise_mode == "all":
-        equalisation_ratios = None
+    if equalise_mode == "first":
+        equalisation_ratios = first_eq_ratios
 
     output_models = [model]
 
-    cluster = LocalCUDACluster(CUDA_VISIBLE_DEVICES=devices)
-    client = Client(cluster)
+    client = get_dask_client(devices)
     aprint("Dask Client", client)
 
     lazy_computations = []
     for t in range(1, n_time_pts):
         lazy_computations.append(
             dask.delayed(_process)(
                 time_point=t,
```

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/generic.py` & `dexp-2023.4.10.686/dexp/datasets/operations/generic.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from typing import Callable, Optional, Sequence, Tuple
 
 import dask
 from arbol import aprint, asection
-from dask.distributed import Client
-from dask_cuda import LocalCUDACluster
 from toolz import curry
 
 from dexp.datasets import BaseDataset, ZDataset
 from dexp.datasets.stack_iterator import StackIterator
 from dexp.processing.utils.scatter_gather_i2i import scatter_gather_i2i
 from dexp.utils.backends import CupyBackend
+from dexp.utils.dask import get_dask_client
 
 
 @dask.delayed
 @curry
 def _process(
     time_point: int,
     stacks: StackIterator,
@@ -47,15 +46,14 @@
         output_dataset.add_channel(ch, stacks.shape, dtype=input_dataset.dtype(ch))
 
         process = _process(stacks=stacks, out_dataset=output_dataset, channel=ch, func=func)
 
         # Stores functions to be computed
         lazy_computations += [process(time_point=t) for t in range(len(stacks))]
 
-    cluster = LocalCUDACluster(CUDA_VISIBLE_DEVICES=devices)
-    client = Client(cluster)
+    client = get_dask_client(devices)
     aprint("Dask client", client)
 
     # Compute everything
     dask.compute(*lazy_computations)
 
     output_dataset.check_integrity()
```

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/histogram.py` & `dexp-2023.4.10.686/dexp/datasets/operations/histogram.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/register.py` & `dexp-2023.4.10.686/dexp/datasets/operations/register.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from copy import deepcopy
 from typing import Dict, List, Sequence
 
 import dask
 import numpy
 import numpy as np
 from arbol.arbol import aprint, asection
-from dask.distributed import Client
-from dask_cuda import LocalCUDACluster
 from toolz import curry
 
 from dexp.datasets.base_dataset import BaseDataset
 from dexp.datasets.stack_iterator import StackIterator
 from dexp.processing.multiview_lightsheet.fusion.basefusion import BaseFusion
 from dexp.processing.multiview_lightsheet.fusion.simview import SimViewFusion
 from dexp.processing.registration.model.model_io import model_list_to_file
 from dexp.processing.registration.model.translation_registration_model import (
     TranslationRegistrationModel,
 )
 from dexp.utils.backends import BestBackend
+from dexp.utils.dask import get_dask_client
 
 
 @dask.delayed
 @curry
 def _process(
     tp: int,
     views: Dict[str, StackIterator],
@@ -66,15 +65,15 @@
     white_top_hat_size: float,
     white_top_hat_sampling: int,
     remove_beads: bool,
     devices: Sequence[int],
 ) -> None:
 
     views = {channel.split("-")[-1]: dataset[channel] for channel in channels}
-    n_time_pts = len(list(views.values())[0])
+    n_time_pts = min(arr.shape[0] for arr in views.values())
 
     with asection("Views:"):
         for channel, view in views.items():
             aprint(f"View: {channel} of shape: {view.shape} and dtype: {view.dtype}")
 
     if microscope == "simview":
         fuse_model = SimViewFusion(
@@ -102,16 +101,15 @@
     else:
         raise NotImplementedError
 
     process = _process(
         views=views, fuse_model=fuse_model, max_proj=max_proj, registration_edge_filter=registration_edge_filter
     )
 
-    cluster = LocalCUDACluster(CUDA_VISIBLE_DEVICES=devices)
-    client = Client(cluster)
+    client = get_dask_client(devices)
     aprint("Dask Client", client)
 
     lazy_computations = []
     for i in range(n_time_pts):
         lazy_computations.append(process(tp=i))
 
     models = dask.compute(*lazy_computations)
```

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/segment.py` & `dexp-2023.4.10.686/dexp/datasets/operations/segment.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from typing import Sequence
 
 import dask
 import numpy as np
 import pandas as pd
 from arbol import aprint, asection
-from dask.distributed import Client
-from dask_cuda import LocalCUDACluster
 from skimage.measure import regionprops_table
 from toolz import curry
 
 from dexp.datasets import BaseDataset, ZDataset
 from dexp.datasets.stack_iterator import StackIterator
 from dexp.processing.morphology import area_white_top_hat
 from dexp.processing.segmentation import roi_watershed_from_minima
 from dexp.utils.backends import CupyBackend
+from dexp.utils.dask import get_dask_client
 
 
 def intensity_sum(mask: np.ndarray, intensities: np.ndarray) -> float:
     """Sums the intensity inside the mask"""
     return intensities[mask].sum(axis=0, dtype=float)
 
 
@@ -72,27 +71,31 @@
                     ch_detection = wth > threshold_otsu(wth)
                     del wth
 
                     # removing small white/black elements
                     ch_detection = morph.binary_opening(ch_detection, morph.ball(2))
                     ch_detection = morph.binary_closing(ch_detection, morph.ball(2))
 
+                    # FIXME: it needs to be executed after labeling
                     # ch_detection = morph.remove_small_objects(ch_detection, min_size=minimum_area)
+
                     detection |= ch_detection
+                    del ch_detection
 
             count = detection.sum()
             aprint(f"Number of detected cell-pixels {count} proportion {detection.sum() / detection.size}.")
 
             if basins is None:  # using EDT
                 with asection("Computing EDT for watershed basins ..."):
                     basins = bkd.to_backend(edt(bkd.to_numpy(detection), anisotropy=(z_scale, 1, 1)))
 
             basins = basins.max() - basins
             basins = bkd.to_numpy(basins)
             detection = bkd.to_numpy(detection)
+            bkd.clear_memory_pool()
 
             with asection("Segmenting ..."):
                 labels = roi_watershed_from_minima(
                     image=basins,
                     mask=detection,
                     H_minima=h_minima,
                     compactness=0 if use_edt else compactness,
@@ -168,16 +171,15 @@
             use_edt=use_edt,
             out_channel=out_channel,
         )
     )
 
     lazy_computations = [process(time_point=t) for t in range(n_time_pts)]
 
-    cluster = LocalCUDACluster(CUDA_VISIBLE_DEVICES=devices)
-    client = Client(cluster)
+    client = get_dask_client(devices)
     aprint("Dask client", client)
 
     df_path = output_dataset.path.replace(".zarr", ".csv")
     df = pd.concat(dask.compute(*lazy_computations))
     df.to_csv(df_path, index=False)
 
     output_dataset.append_metadata({"features": features_channels})
```

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/stabilize.py` & `dexp-2023.4.10.686/dexp/datasets/operations/stabilize.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 from dexp.processing.registration.model.model_io import from_json
 from dexp.processing.registration.model.sequence_registration_model import (
     SequenceRegistrationModel,
 )
 from dexp.processing.registration.sequence import image_stabilisation
 from dexp.processing.registration.sequence_proj import image_stabilisation_proj_
 from dexp.utils.backends import BestBackend, NumpyBackend
+from dexp.utils.fft import clear_fft_plan_cache
 from dexp.utils.misc import compute_num_workers
 
 
 def _compute_model(
     input_dataset: BaseDataset,
     channel: str,
     max_range: int,
@@ -131,14 +132,15 @@
                     tp_array = model.apply(tp_array, index=i, pad=pad, integral=integral)
 
             with asection(
                 f"Saving stabilized stack for time point {i}/{len(array)}, shape:{tp_array.shape}, "
                 + "dtype:{array.dtype}"
             ):
                 output_dataset.write_stack(channel=channel, time_point=i, stack_array=tp_array)
+                clear_fft_plan_cache()
 
 
 def dataset_stabilize(
     input_dataset: BaseDataset,
     output_dataset: ZDataset,
     channels: Sequence[str],
     model_output_path: str,
```

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/tiff.py` & `dexp-2023.4.10.686/dexp/datasets/operations/tiff.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
                 aprint(f"Projecting along axis {project}")
                 stack = stack.max(axis=project)
 
             aprint(
                 f"Writing time point: {tp} of shape: {stack.shape}, dtype:{stack.dtype} "
                 + f"as TIFF file: '{tiff_file_path}', with compression: {clevel}"
             )
-            tiff_save(tiff_file_path, stack, compress=clevel)
+            tiff_save(tiff_file_path, stack, clevel=clevel)
             aprint(f"Done writing time point: {tp} !")
         else:
             aprint(f"File for time point (or z slice): {tp} already exists.")
 
 
 @curry
 def _save_single_file(tp: int, stacks: StackIterator, memmap_image: np.memmap, project: bool) -> None:
```

### Comparing `dexp-2022.6.29.552/dexp/datasets/operations/view.py` & `dexp-2023.4.10.686/dexp/datasets/operations/view.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/stack_iterator.py` & `dexp-2023.4.10.686/dexp/datasets/stack_iterator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from typing import Optional, Tuple
+from typing import Optional, Tuple, Union
 
 import numpy as np
 import zarr
 
 from dexp.utils.slicing import slice_from_shape
 
 
 class StackIterator:
-    def __init__(self, array: zarr.Array, slicing: Optional[slice]):
+    def __init__(self, array: zarr.Array, slicing: Optional[Union[slice, Tuple[slice]]]):
 
         self._out_shape, self._volume_slicing, self._time_points = slice_from_shape(array.shape, slicing)
         self._slicing = slicing
 
         self._array = array
 
     @property
```

### Comparing `dexp-2022.6.29.552/dexp/datasets/synthetic_datasets/binary_blobs.py` & `dexp-2023.4.10.686/dexp/datasets/synthetic_datasets/binary_blobs.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/synthetic_datasets/dexp_dataset.py` & `dexp-2023.4.10.686/dexp/datasets/synthetic_datasets/dexp_dataset.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/synthetic_datasets/multiview_data.py` & `dexp-2023.4.10.686/dexp/datasets/synthetic_datasets/multiview_data.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/synthetic_datasets/nuclei_background_data.py` & `dexp-2023.4.10.686/dexp/datasets/synthetic_datasets/nuclei_background_data.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/tiff_dataset.py` & `dexp-2023.4.10.686/dexp/datasets/tiff_dataset.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/datasets/zarr_dataset.py` & `dexp-2023.4.10.686/dexp/datasets/zarr_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -582,33 +582,36 @@
         initialized = {
             int(k.split(".", 1)[0]) for k in zarr.storage.listdir(array.chunk_store, array._path) if prog.match(k)
         }
         return max(initialized)
 
     def to_ome_zarr(self, path: str, force_dtype: Optional[int] = None, n_scales: int = 3) -> None:
         ch = self.channels()[0]
-        dexp_shape = self.shape(ch)
+        dexp_shape = self[ch].shape
 
         dtype = force_dtype if force_dtype is not None else self.dtype(ch)
 
+        dexp_arrays = []
         for _ch in self.channels():
-            if dexp_shape != self.shape(_ch):
+            arr = self[_ch]
+            if dexp_shape != arr.shape:
                 raise ValueError(
                     f"Channels {ch} and {_ch} have different "
                     f"shapes ({dexp_shape} and {self.shape(_ch)} "
                     "could not convert to ome-zarr."
                 )
             if dtype != self.dtype(_ch) and force_dtype is None:
                 raise ValueError(
                     f"Channels {ch} and {_ch} have different "
-                    f"dtypes ({dtype} and {self.dtype(_ch)} "
+                    f"dtypes ({dtype} and {self.dtype(_ch)}) "
                     "could not convert to ome-zarr."
                 )
+            dexp_arrays.append(arr)
 
-        ome_zarr_shape = (dexp_shape[0], len(self.channels()), *dexp_shape[1:])
+        ome_zarr_shape = (dexp_shape[0], len(dexp_arrays), *dexp_shape[1:])
 
         group = zarr.group(zarr.NestedDirectoryStore(path))
 
         arrays = []
         datasets = []
         for i in range(n_scales):
             factor = 2**i
@@ -621,18 +624,18 @@
                 {
                     "path": array_path,
                     "coordinateTransformations": create_coord_transform(self.get_resolution(), factor),
                 }
             )
 
         with BestBackend() as bkd:
-            for t in range(self.nb_timepoints(ch)):
+            for t in range(dexp_shape[0]):
                 aprint(f"Converting time point {t} ...", end="\r")
-                for c, channel in enumerate(self.channels()):
-                    stack = self.get_stack(channel, t)
+                for c, arr in enumerate(dexp_arrays):
+                    stack = numpy.asarray(arr[t])
                     arrays[0][t, c] = stack
                     stack = bkd.to_backend(stack)
                     for i in range(1, n_scales):
                         factors = (2**i,) * stack.ndim
                         arrays[i][t, c] = bkd.to_numpy(downscale_local_mean(stack, factors))
 
         aprint("Done conversion to OME zarr")
```

### Comparing `dexp-2022.6.29.552/dexp/io/compress_array.py` & `dexp-2023.4.10.686/dexp/io/compress_array.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/io/io.py` & `dexp-2023.4.10.686/dexp/io/io.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import numpy as np
-from tifffile import imsave
+from tifffile import imwrite
 
 
-def tiff_save(file, img, axes="ZYX", compress=0, **imsave_kwargs):
+def tiff_save(file, img, axes="ZYX", clevel=0, **imsave_kwargs):
     """Save image in ImageJ-compatible TIFF format.
 
     Parameters
     ----------
     file : str
         File name
     img : numpy.ndarray
@@ -29,8 +29,8 @@
     else:
         t_new = t
     img = img.astype(t_new, copy=False)
     if t != t_new:
         print(f"Converting data type from '{t}' to ImageJ-compatible '{np.dtype(t_new)}'.")
 
     imsave_kwargs["imagej"] = True
-    imsave(file, img, **imsave_kwargs, compress=compress, metadata={"axes": axes})  # ,
+    imwrite(file, img, **imsave_kwargs, metadata={"axes": axes}, compressionargs={"clevel": clevel})
```

### Comparing `dexp-2022.6.29.552/dexp/optics/psf/microscope_psf.py` & `dexp-2023.4.10.686/dexp/optics/psf/microscope_psf.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/optics/psf/standard_psfs.py` & `dexp-2023.4.10.686/dexp/optics/psf/standard_psfs.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/blend.py` & `dexp-2023.4.10.686/dexp/processing/color/blend.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/border.py` & `dexp-2023.4.10.686/dexp/processing/color/border.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/cairo_utils.py` & `dexp-2023.4.10.686/dexp/processing/color/cairo_utils.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/colormap.py` & `dexp-2023.4.10.686/dexp/processing/color/colormap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Callable, Union
 
-from matplotlib.cm import get_cmap
+from matplotlib import colormaps
 from matplotlib.colors import LinearSegmentedColormap, ListedColormap
 
 from dexp.utils import xpArray
 from dexp.utils.backends import Backend, NumpyBackend
 
 
 def rgb_colormap(image: xpArray, cmap: Union[str, Callable] = None, bytes: bool = False, internal_dtype=None):
@@ -58,15 +58,15 @@
 def _normalise_colormap(cmap):
     if type(cmap) == str:
         cmap = "cet_rainbow" if cmap == "rainbow" else cmap
         cmap = "cet_bmy" if cmap == "bmy" else cmap
         from colorcet import rgb_to_hex
 
         rgb_to_hex(0, 0, 0)  # this is a dummy call to prevent elimination of the colorcet import by IDEs
-        cmap = get_cmap(cmap)
+        cmap = colormaps.get_cmap(cmap)
     elif type(cmap) == LinearSegmentedColormap or type(cmap) == ListedColormap:
         # all good here...
         cmap = cmap
     else:
         raise ValueError(f"Unknown colormap: {cmap}")
     return cmap
```

### Comparing `dexp-2022.6.29.552/dexp/processing/color/conversions.py` & `dexp-2023.4.10.686/dexp/processing/color/conversions.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/crop_resize_pad.py` & `dexp-2023.4.10.686/dexp/processing/color/crop_resize_pad.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/demo/demo_blend.py` & `dexp-2023.4.10.686/dexp/processing/color/demo/demo_blend.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/demo/demo_border.py` & `dexp-2023.4.10.686/dexp/processing/color/demo/demo_border.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/demo/demo_colormap.py` & `dexp-2023.4.10.686/dexp/processing/color/demo/demo_colormap.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/demo/demo_crop_resize_pad.py` & `dexp-2023.4.10.686/dexp/processing/color/demo/demo_crop_resize_pad.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/demo/demo_insert.py` & `dexp-2023.4.10.686/dexp/processing/color/demo/demo_insert.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/demo/demo_projection.py` & `dexp-2023.4.10.686/dexp/processing/color/demo/demo_projection.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/demo/demo_scale_bar.py` & `dexp-2023.4.10.686/dexp/processing/color/demo/demo_scale_bar.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/demo/demo_time_stamp.py` & `dexp-2023.4.10.686/dexp/processing/color/demo/demo_time_stamp.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/insert.py` & `dexp-2023.4.10.686/dexp/processing/color/insert.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/projection.py` & `dexp-2023.4.10.686/dexp/processing/color/projection.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/projection_legend.py` & `dexp-2023.4.10.686/dexp/processing/color/projection_legend.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/scale_bar.py` & `dexp-2023.4.10.686/dexp/processing/color/scale_bar.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/color/time_stamp.py` & `dexp-2023.4.10.686/dexp/processing/color/time_stamp.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/crop/_test/test_rep_crop.py` & `dexp-2023.4.10.686/dexp/processing/crop/_test/test_rep_crop.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/crop/background.py` & `dexp-2023.4.10.686/dexp/processing/crop/background.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from scipy.signal._signaltools import _centered
-
+from dexp.processing.utils.pad import fit_to_shape
 from dexp.utils import xpArray
 from dexp.utils.backends import Backend
 
 
 def foreground_mask(
     array: xpArray,
     intensity_threshold: int = 10,
@@ -42,15 +41,15 @@
     small = ndi.grey_opening(small, ndim * (3,))
     small = ndi.grey_closing(small, ndim * (7,))
     small = small > intensity_threshold
     small = ndi.grey_dilation(small, ndim * (9,))
 
     small = morph.remove_small_objects(small, binary_area_threshold)
     mask = ndi.zoom(small, (downsample,) * ndim, order=0)
-    mask = _centered(mask, array.shape)
+    mask = fit_to_shape(mask, array.shape)
 
     if display:
         import napari
 
         v = napari.Viewer()
         v.add_image(Backend.to_numpy(array))
         v.add_labels(Backend.to_numpy(mask))
```

### Comparing `dexp-2022.6.29.552/dexp/processing/crop/demo/demo_rep_crop.py` & `dexp-2023.4.10.686/dexp/processing/crop/demo/demo_rep_crop.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/crop/representative_crop.py` & `dexp-2023.4.10.686/dexp/processing/crop/representative_crop.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/admm_deconvolution.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/admm_deconvolution.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/admm_utils.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/admm_utils.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/blind_deconvolution.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/blind_deconvolution.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_admm_deconvolution_3d.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_admm_deconvolution_3d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_blind_deconv_3d.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_blind_deconv_3d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_inversion_deconvolution_3d.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_inversion_deconvolution_3d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_lr_deconvolution_2d.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_lr_deconvolution_2d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_lr_deconvolution_2d_bs.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_lr_deconvolution_2d_bs.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_lr_deconvolution_2d_wb.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_lr_deconvolution_2d_wb.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d_bs.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d_bs.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d_sg.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d_sg.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d_wb.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/demo/demo_lr_deconvolution_3d_wb.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/inversion_deconvolution.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/inversion_deconvolution.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deconvolution/lr_deconvolution.py` & `dexp-2023.4.10.686/dexp/processing/deconvolution/lr_deconvolution.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/denoising/butterworth.py` & `dexp-2023.4.10.686/dexp/processing/denoising/butterworth.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/denoising/demo/demo_2D_butterworth.py` & `dexp-2023.4.10.686/dexp/processing/denoising/demo/demo_2D_butterworth.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/denoising/demo/demo_2D_gaussian.py` & `dexp-2023.4.10.686/dexp/processing/denoising/demo/demo_2D_gaussian.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/denoising/demo/demo_3D_butterworth.py` & `dexp-2023.4.10.686/dexp/processing/denoising/demo/demo_3D_butterworth.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/denoising/demo/demo_noise.py` & `dexp-2023.4.10.686/dexp/processing/denoising/demo/demo_noise.py`

 * *Files 12% similar despite different names*

```diff
@@ -29,24 +29,24 @@
     """
     Arbol.enable_output = True
     Arbol.set_log_max_depth(5)
 
     image = data.astronaut()
     image = rgb2gray(image)
 
-    noisy = add_noise(image)
+    noisy = add_noise(image, seed=1)
 
     image = numpy.clip(image, 0, 1)
     noisy = numpy.clip(noisy, 0, 1)
     psnr_noisy = psnr(image.astype(noisy.dtype), noisy)
-    ssim_noisy = ssim(image, noisy)
+    ssim_noisy = ssim(image, noisy, data_range=1.0)
     print("         noisy   :", psnr_noisy, ssim_noisy)
 
     assert psnr_noisy > 12 and psnr_noisy < 13
-    assert ssim_noisy > 0.28 and ssim_noisy < 0.29
+    assert ssim_noisy > 0.23 and ssim_noisy < 0.24
 
     if display:
         import napari
 
         viewer = napari.Viewer()
         viewer.add_image(image, name="image")
         viewer.add_image(noisy, name="noisy")
```

### Comparing `dexp-2022.6.29.552/dexp/processing/denoising/gaussian.py` & `dexp-2023.4.10.686/dexp/processing/denoising/gaussian.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/denoising/j_invariance.py` & `dexp-2023.4.10.686/dexp/processing/denoising/j_invariance.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/denoising/metrics.py` & `dexp-2023.4.10.686/dexp/processing/denoising/metrics.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/denoising/noise.py` & `dexp-2023.4.10.686/dexp/processing/denoising/noise.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deskew/classic_deskew.py` & `dexp-2023.4.10.686/dexp/processing/deskew/classic_deskew.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deskew/demo/demo_classic_deskew.py` & `dexp-2023.4.10.686/dexp/processing/deskew/demo/demo_classic_deskew.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deskew/demo/demo_yang_deskew.py` & `dexp-2023.4.10.686/dexp/processing/deskew/demo/demo_yang_deskew.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deskew/utils.py` & `dexp-2023.4.10.686/dexp/processing/deskew/utils.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/deskew/yang_deskew.py` & `dexp-2023.4.10.686/dexp/processing/deskew/yang_deskew.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/equalise/demo/demo_equalise_intensity.py` & `dexp-2023.4.10.686/dexp/processing/equalise/demo/demo_equalise_intensity.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/equalise/equalise_intensity.py` & `dexp-2023.4.10.686/dexp/processing/equalise/equalise_intensity.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 
 def equalise_intensity(
     image1: xpArray,
     image2: xpArray,
     zero_level=90,
     quantile_low=0.01,
-    quantile_high=0.99,
+    quantile_high=0.999,
     project_axis: int = 0,
     max_voxels: int = 1e7,
     correction_ratio: float = None,
     copy: bool = True,
     internal_dtype=None,
 ):
     """
@@ -69,16 +69,16 @@
 
         # instead of computing the rations on all voxels, we reduce to a dense subset:
         reduction = max(1, 4 * (int(proj_image1.size / max_voxels) // 4))
         strided_image1 = proj_image1.ravel()[::reduction].astype(numpy.float32, copy=False)
         strided_image2 = proj_image2.ravel()[::reduction].astype(numpy.float32, copy=False)
 
         # We determine a robust maximum for voxel intensities:
-        highvalue1 = xp.percentile(strided_image1, q=quantile_high * 100, interpolation="higher")
-        highvalue2 = xp.percentile(strided_image2, q=quantile_high * 100, interpolation="higher")
+        highvalue1 = xp.percentile(strided_image1, q=quantile_high * 100, method="higher")
+        highvalue2 = xp.percentile(strided_image2, q=quantile_high * 100, method="higher")
 
         # we set a 'high-value' threshold to the minimum of both robust maximums:
         threshold = min(highvalue1, highvalue2)
 
         # We find the voxels that are above that threshold in both images:
         mask1 = strided_image1 >= threshold
         mask2 = strided_image2 >= threshold
```

### Comparing `dexp-2022.6.29.552/dexp/processing/filters/butterworth_filter.py` & `dexp-2023.4.10.686/dexp/processing/filters/butterworth_filter.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/filters/demo/demo_butterworth_filter.py` & `dexp-2023.4.10.686/dexp/processing/filters/demo/demo_butterworth_filter.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/filters/demo/demo_fft_convolve.py` & `dexp-2023.4.10.686/dexp/processing/filters/demo/demo_fft_convolve.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/filters/demo/demo_sobel.py` & `dexp-2023.4.10.686/dexp/processing/filters/demo/demo_sobel.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/filters/fft_convolve.py` & `dexp-2023.4.10.686/dexp/processing/filters/fft_convolve.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/filters/kernels/butterworth.py` & `dexp-2023.4.10.686/dexp/processing/filters/kernels/butterworth.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/filters/kernels/demo/demo_butterworth.py` & `dexp-2023.4.10.686/dexp/processing/filters/kernels/demo/demo_butterworth.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/filters/kernels/demo/demo_gaussian.py` & `dexp-2023.4.10.686/dexp/processing/filters/kernels/demo/demo_gaussian.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/filters/kernels/demo/demo_wiener.py` & `dexp-2023.4.10.686/dexp/processing/filters/kernels/demo/demo_wiener.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/filters/kernels/demo/demo_wiener_butterworth.py` & `dexp-2023.4.10.686/dexp/processing/filters/kernels/demo/demo_wiener_butterworth.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/filters/kernels/gaussian.py` & `dexp-2023.4.10.686/dexp/processing/filters/kernels/gaussian.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/filters/kernels/wiener.py` & `dexp-2023.4.10.686/dexp/processing/filters/kernels/wiener.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/filters/kernels/wiener_butterworth.py` & `dexp-2023.4.10.686/dexp/processing/filters/kernels/wiener_butterworth.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/filters/sobel_filter.py` & `dexp-2023.4.10.686/dexp/processing/filters/sobel_filter.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/fusion/dct_fusion.py` & `dexp-2023.4.10.686/dexp/processing/fusion/dct_fusion.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/fusion/demo/demo_fusion.py` & `dexp-2023.4.10.686/dexp/processing/fusion/demo/demo_fusion.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/fusion/dft_fusion.py` & `dexp-2023.4.10.686/dexp/processing/fusion/dft_fusion.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/fusion/tg_fusion.py` & `dexp-2023.4.10.686/dexp/processing/fusion/tg_fusion.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/interpolation/_cupy/warp_1d.py` & `dexp-2023.4.10.686/dexp/processing/interpolation/_cupy/warp_1d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/interpolation/_cupy/warp_2d.py` & `dexp-2023.4.10.686/dexp/processing/interpolation/_cupy/warp_2d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/interpolation/_cupy/warp_3d.py` & `dexp-2023.4.10.686/dexp/processing/interpolation/_cupy/warp_3d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/interpolation/demo/demo_warp_1d.py` & `dexp-2023.4.10.686/dexp/processing/interpolation/demo/demo_warp_1d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/interpolation/demo/demo_warp_2d.py` & `dexp-2023.4.10.686/dexp/processing/interpolation/demo/demo_warp_2d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/interpolation/demo/demo_warp_3d.py` & `dexp-2023.4.10.686/dexp/processing/interpolation/demo/demo_warp_3d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/interpolation/warp.py` & `dexp-2023.4.10.686/dexp/processing/interpolation/warp.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/morphology/component_tree.py` & `dexp-2023.4.10.686/dexp/processing/morphology/component_tree.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/deconvolution/demo/demo_simview_deconv.py` & `dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/deconvolution/demo/demo_simview_deconv.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/fusion/basefusion.py` & `dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/fusion/basefusion.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/fusion/demo/demo_mvsols_fusion.py` & `dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/fusion/demo/demo_mvsols_fusion.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/fusion/demo/demo_simview_fusion.py` & `dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/fusion/demo/demo_simview_fusion.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/fusion/mvsols.py` & `dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/fusion/mvsols.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/multiview_lightsheet/fusion/simview.py` & `dexp-2023.4.10.686/dexp/processing/multiview_lightsheet/fusion/simview.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/optimization/grid_search.py` & `dexp-2023.4.10.686/dexp/processing/optimization/grid_search.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/demo/demo_sequence_2d.py` & `dexp-2023.4.10.686/dexp/processing/registration/demo/demo_sequence_2d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/demo/demo_sequence_3d.py` & `dexp-2023.4.10.686/dexp/processing/registration/demo/demo_sequence_3d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/demo/demo_translation_2d.py` & `dexp-2023.4.10.686/dexp/processing/registration/demo/demo_translation_2d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/demo/demo_translation_3d.py` & `dexp-2023.4.10.686/dexp/processing/registration/demo/demo_translation_3d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/demo/demo_translation_3d_proj.py` & `dexp-2023.4.10.686/dexp/processing/registration/demo/demo_translation_3d_proj.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/demo/demo_translation_3d_proj_difficult.py` & `dexp-2023.4.10.686/dexp/processing/registration/demo/demo_translation_3d_proj_difficult.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/demo/demo_warp_2d.py` & `dexp-2023.4.10.686/dexp/processing/registration/demo/demo_warp_2d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/demo/demo_warp_2d_blobs.py` & `dexp-2023.4.10.686/dexp/processing/registration/demo/demo_warp_2d_blobs.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/demo/demo_warp_3d.py` & `dexp-2023.4.10.686/dexp/processing/registration/demo/demo_warp_3d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/demo/demo_warp_ms_2d.py` & `dexp-2023.4.10.686/dexp/processing/registration/demo/demo_warp_ms_2d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/demo/demo_warp_ms_3d.py` & `dexp-2023.4.10.686/dexp/processing/registration/demo/demo_warp_ms_3d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/model/demo/demo_translation_model.py` & `dexp-2023.4.10.686/dexp/processing/registration/model/demo/demo_translation_model.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/model/demo/demo_warp_model.py` & `dexp-2023.4.10.686/dexp/processing/registration/model/demo/demo_warp_model.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/model/model_io.py` & `dexp-2023.4.10.686/dexp/processing/registration/model/model_io.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/model/pairwise_registration_model.py` & `dexp-2023.4.10.686/dexp/processing/registration/model/pairwise_registration_model.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/model/sequence_registration_model.py` & `dexp-2023.4.10.686/dexp/processing/registration/model/sequence_registration_model.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/model/translation_registration_model.py` & `dexp-2023.4.10.686/dexp/processing/registration/model/translation_registration_model.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/model/warp_registration_model.py` & `dexp-2023.4.10.686/dexp/processing/registration/model/warp_registration_model.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/sequence.py` & `dexp-2023.4.10.686/dexp/processing/registration/sequence.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/sequence_proj.py` & `dexp-2023.4.10.686/dexp/processing/registration/sequence_proj.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/translation_2d.py` & `dexp-2023.4.10.686/dexp/processing/registration/translation_2d.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/translation_nd.py` & `dexp-2023.4.10.686/dexp/processing/registration/translation_nd.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/translation_nd_proj.py` & `dexp-2023.4.10.686/dexp/processing/registration/translation_nd_proj.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/warp_multiscale_nd.py` & `dexp-2023.4.10.686/dexp/processing/registration/warp_multiscale_nd.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/registration/warp_nd.py` & `dexp-2023.4.10.686/dexp/processing/registration/warp_nd.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/remove_beads/beadsremover.py` & `dexp-2023.4.10.686/dexp/processing/remove_beads/beadsremover.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/restoration/aap_correction.py` & `dexp-2023.4.10.686/dexp/processing/restoration/aap_correction.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/restoration/clean_dark_regions.py` & `dexp-2023.4.10.686/dexp/processing/restoration/clean_dark_regions.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/restoration/dehazing.py` & `dexp-2023.4.10.686/dexp/processing/restoration/dehazing.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/restoration/demo/demo_aap_correction.py` & `dexp-2023.4.10.686/dexp/processing/restoration/demo/demo_aap_correction.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/restoration/demo/demo_clean_dark_regions.py` & `dexp-2023.4.10.686/dexp/processing/restoration/demo/demo_clean_dark_regions.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/restoration/demo/demo_dehaze.py` & `dexp-2023.4.10.686/dexp/processing/restoration/demo/demo_dehaze.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/restoration/demo/demo_lipschitz_continuity_correction.py` & `dexp-2023.4.10.686/dexp/processing/restoration/demo/demo_lipschitz_continuity_correction.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/restoration/lipshitz_correction.py` & `dexp-2023.4.10.686/dexp/processing/restoration/lipshitz_correction.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/segmentation/watershed.py` & `dexp-2023.4.10.686/dexp/processing/segmentation/watershed.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/utils/apply.py` & `dexp-2023.4.10.686/dexp/processing/utils/apply.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/utils/blend_images.py` & `dexp-2023.4.10.686/dexp/processing/utils/blend_images.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/utils/center_of_mass.py` & `dexp-2023.4.10.686/dexp/processing/utils/center_of_mass.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/utils/element_wise_affine.py` & `dexp-2023.4.10.686/dexp/processing/utils/element_wise_affine.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/utils/fit_shape.py` & `dexp-2023.4.10.686/dexp/processing/utils/fit_shape.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/utils/linear_solver.py` & `dexp-2023.4.10.686/dexp/processing/utils/linear_solver.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/utils/mkl_util.py` & `dexp-2023.4.10.686/dexp/processing/utils/mkl_util.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/utils/nan_to_zero.py` & `dexp-2023.4.10.686/dexp/processing/utils/nan_to_zero.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/utils/nd_slice.py` & `dexp-2023.4.10.686/dexp/processing/utils/nd_slice.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/utils/normalise.py` & `dexp-2023.4.10.686/dexp/processing/utils/normalise.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/utils/projection_generator.py` & `dexp-2023.4.10.686/dexp/processing/utils/projection_generator.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/utils/scatter_gather_i2i.py` & `dexp-2023.4.10.686/dexp/processing/utils/scatter_gather_i2i.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/processing/utils/scatter_gather_i2v.py` & `dexp-2023.4.10.686/dexp/processing/utils/scatter_gather_i2v.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/utils/__init__.py` & `dexp-2023.4.10.686/dexp/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/utils/backends/_cupy/texture/texture.py` & `dexp-2023.4.10.686/dexp/utils/backends/_cupy/texture/texture.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/utils/backends/backend.py` & `dexp-2023.4.10.686/dexp/utils/backends/backend.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/utils/backends/best_backend.py` & `dexp-2023.4.10.686/dexp/utils/backends/best_backend.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/utils/backends/cupy_backend.py` & `dexp-2023.4.10.686/dexp/utils/backends/cupy_backend.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/utils/backends/numpy_backend.py` & `dexp-2023.4.10.686/dexp/utils/backends/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/utils/fft.py` & `dexp-2023.4.10.686/dexp/utils/fft.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/utils/lock.py` & `dexp-2023.4.10.686/dexp/utils/lock.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/utils/robocopy.py` & `dexp-2023.4.10.686/dexp/utils/robocopy.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/utils/slicing.py` & `dexp-2023.4.10.686/dexp/utils/slicing.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-from typing import List, Tuple
+from typing import List, Tuple, Union
 
 import numpy as np
 
 
-def slice_from_shape(shape: Tuple[int], slicing: slice) -> Tuple[Tuple[int], slice, List[int]]:
+def slice_from_shape(shape: Tuple[int], slicing: Union[slice, Tuple[slice]]) -> Tuple[Tuple[int], slice, List[int]]:
     time_points = list(range(shape[0]))
     if slicing is not None:
         if isinstance(slicing, tuple):
             time_points = time_points[slicing[0]]
             volume_slicing = slicing[1:]
             new_shape = (len(time_points),) + np.empty(shape=shape[1:], dtype=bool)[slicing[1:]].shape
         else:
```

### Comparing `dexp-2022.6.29.552/dexp/utils/speed_test.py` & `dexp-2023.4.10.686/dexp/utils/speed_test.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/utils/testing/testing.py` & `dexp-2023.4.10.686/dexp/utils/testing/testing.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/video/blend.py` & `dexp-2023.4.10.686/dexp/video/blend.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/video/crop_resize_pad.py` & `dexp-2023.4.10.686/dexp/video/crop_resize_pad.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/video/demo/demo_blend.py` & `dexp-2023.4.10.686/dexp/video/demo/demo_blend.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/video/demo/demo_crop_resize_pad.py` & `dexp-2023.4.10.686/dexp/video/demo/demo_crop_resize_pad.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/video/demo/demo_overlay.py` & `dexp-2023.4.10.686/dexp/video/demo/demo_overlay.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/video/overlay.py` & `dexp-2023.4.10.686/dexp/video/overlay.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/volumerender/demo/demo_volumerender.py` & `dexp-2023.4.10.686/dexp/volumerender/demo/demo_volumerender.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/volumerender/quaternion.py` & `dexp-2023.4.10.686/dexp/volumerender/quaternion.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/volumerender/transform_matrices.py` & `dexp-2023.4.10.686/dexp/volumerender/transform_matrices.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp/volumerender/volumerender.py` & `dexp-2023.4.10.686/dexp/volumerender/volumerender.py`

 * *Files identical despite different names*

### Comparing `dexp-2022.6.29.552/dexp.egg-info/PKG-INFO` & `dexp-2023.4.10.686/dexp.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: dexp
-Version: 2022.6.29.552
+Version: 2023.4.10.686
 Summary: Light-sheet Dataset EXploration and Processing
 Home-page: https://github.com/royerlab/dexp
 Author: Jordao Bragantini, Ahmet Can Solak, Bin Yang, Loic A Royer
 Author-email: jordao.bragantini@czbiohub.org, ahmetcan.solak@czbiohub.org, bin.yang@czbiohub.org, loic.royer@czbiohub.org
 License: BSD 3-Clause
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Environment :: GPU :: NVIDIA CUDA :: 11.1
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
@@ -70,34 +69,43 @@
 **For OSX users:** Before installating dexp, you will first need to install cairo:
 ```
 brew install cairo
 ```
 
 ### Quick conda environment setup and installation:
 
-The following commands delete any existing dexp environment, recreate it, install **dexp** with CUDA support and [napari](https://napari.org/):
-```
-conda deactivate
-conda env remove --name dexp
-conda create -y --name dexp python=3.9
-conda activate dexp
-conda install cupy
-pip install napari[all]
-```
+There are multiple options when using a conda environment:
 
-If you are having problems with the cuda/cuda-toolkit the best is to use conda to install the correct version of the cudatoolkit:
-```
-conda install -c conda-forge cudatoolkit==11.2.2
-```
-You can check [here](https://anaconda.org/conda-forge/cudatoolkit/files) for the best matching version.
+- You can create our suggested DEXP (and some additional packages) environment by, it requires GPU:
 
-Notes:
-- You might get some error messages recommending you install missing libraries such as CUDNN, CuTensor, nccl, etc... These messages often come with instructions on what to do.
-- Adjust your driver version (here 11.2) to your card(s) and drivers.
-- Windows users should call `conda install -c conda-forge pyopencl` before running the second to last step.
+   ```
+   conda env create --name dexp --file env-linux-gpu.yaml
+   ```
+
+- Or create your own conda environment from scratch with the following commands delete any existing dexp environment, recreate it, install **dexp** with CUDA support and [napari](https://napari.org/):
+   ```
+   conda deactivate
+   conda env remove --name dexp
+   conda create -y --name dexp python=3.9
+   conda activate dexp
+   conda install cupy
+   pip install dexp[optional,colored]
+   pip install napari[all]
+   ```
+
+   If you are having problems with the cuda/cuda-toolkit the best is to use conda to install the correct version of the cudatoolkit:
+   ```
+   conda install -c conda-forge cudatoolkit==11.2.2
+   ```
+   You can check [here](https://anaconda.org/conda-forge/cudatoolkit/files) for the best matching version.
+
+   Notes:
+   - You might get some error messages recommending you install missing libraries such as CUDNN, CuTensor, nccl, etc... These messages often come with instructions on what to do.
+   - Adjust your driver version (here 11.2) to your card(s) and drivers.
+   - Windows users should call `conda install -c conda-forge pyopencl` before running the second to last step.
 
 ### Leveraging extra CUDA libraries for faster processing:
 
 If you want you **dexp** CUDA-based processing to be even faster, you can install additional libraries such as CUDNN and CUTENSOR
 with the following command:
 
 ```
@@ -155,9 +163,7 @@
 ### How to use **dexp** ?
 
 In depth documentation can be found [here](https://royerlab.github.io/dexp/index.html) for both command line  commands and for the python API.
 
 ### Contributors:
 
 Jordao Bragantini, Ahmet Can Solak, Bin Yang, and Loic A Royer
-
-
```

### Comparing `dexp-2022.6.29.552/dexp.egg-info/SOURCES.txt` & `dexp-2023.4.10.686/dexp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,15 @@
 dexp/processing/utils/element_wise_affine.py
 dexp/processing/utils/fit_shape.py
 dexp/processing/utils/linear_solver.py
 dexp/processing/utils/mkl_util.py
 dexp/processing/utils/nan_to_zero.py
 dexp/processing/utils/nd_slice.py
 dexp/processing/utils/normalise.py
+dexp/processing/utils/pad.py
 dexp/processing/utils/projection_generator.py
 dexp/processing/utils/scatter_gather_i2i.py
 dexp/processing/utils/scatter_gather_i2v.py
 dexp/utils/__init__.py
 dexp/utils/config.py
 dexp/utils/dask.py
 dexp/utils/fft.py
```

### Comparing `dexp-2022.6.29.552/dexp.egg-info/requires.txt` & `dexp-2023.4.10.686/dexp.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -51,14 +51,15 @@
 
 [cuda114]
 cupy-cuda114==10.1.0
 
 [dev]
 flake8
 pytest
+coverage
 
 [gpu]
 gputools
 cucim
 
 [napari]
 napari[all]
```

### Comparing `dexp-2022.6.29.552/setup.py` & `dexp-2023.4.10.686/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
     "gpu": [
         "gputools",
         "cucim",
     ],
     "dev": [
         "flake8",
         "pytest",
+        "coverage",
     ],
 }
 
 
 # The rest you shouldn't have to touch too much :)
 # ------------------------------------------------
 # Except, perhaps the License and Trove Classifiers!
```

