# Comparing `tmp/pynecone-0.1.22a0.tar.gz` & `tmp/pynecone-0.1.23a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynecone-0.1.22a0.tar", max compression
+gzip compressed data, was "pynecone-0.1.23a0.tar", max compression
```

## Comparing `pynecone-0.1.22a0.tar` & `pynecone-0.1.23a0.tar`

### file list

```diff
@@ -1,149 +1,149 @@
--rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.22a0/LICENSE
--rw-r--r--   0        0        0     8364 2023-03-16 23:51:05.127293 pynecone-0.1.22a0/README.md
--rw-r--r--   0        0        0        0 2022-11-18 20:43:33.738202 pynecone-0.1.22a0/pynecone/.templates/app/__init__.py
--rw-r--r--   0        0        0     1036 2023-03-10 00:25:42.687001 pynecone-0.1.22a0/pynecone/.templates/app/tutorial.py
--rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.22a0/pynecone/.templates/assets/favicon.ico
--rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.22a0/pynecone/.templates/web/.gitignore
--rwxr-xr-x   0        0        0   261125 2023-03-10 00:25:42.688288 pynecone-0.1.22a0/pynecone/.templates/web/bun.lockb
--rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.22a0/pynecone/.templates/web/next.config.js
--rw-r--r--   0        0        0     1017 2023-04-02 23:51:14.630623 pynecone-0.1.22a0/pynecone/.templates/web/package.json
--rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.22a0/pynecone/.templates/web/pages/404.js
--rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.22a0/pynecone/.templates/web/pages/_app.js
--rw-r--r--   0        0        0       28 2023-04-03 00:00:47.639618 pynecone-0.1.22a0/pynecone/.templates/web/pynecone.json
--rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.22a0/pynecone/.templates/web/styles/code/prism.js
--rw-r--r--   0        0        0     6456 2023-04-02 23:51:28.426792 pynecone-0.1.22a0/pynecone/.templates/web/utils/state.js
--rw-r--r--   0        0        0      808 2023-04-08 16:05:43.351479 pynecone-0.1.22a0/pynecone/__init__.py
--rw-r--r--   0        0        0    19946 2023-04-09 05:48:16.467591 pynecone-0.1.22a0/pynecone/app.py
--rw-r--r--   0        0        0     2510 2023-01-30 21:50:18.206745 pynecone-0.1.22a0/pynecone/base.py
--rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.22a0/pynecone/compiler/__init__.py
--rw-r--r--   0        0        0     5737 2023-04-03 21:50:34.663262 pynecone-0.1.22a0/pynecone/compiler/compiler.py
--rw-r--r--   0        0        0     5334 2023-04-02 23:51:14.631307 pynecone-0.1.22a0/pynecone/compiler/templates.py
--rw-r--r--   0        0        0     9084 2023-03-16 23:52:12.744496 pynecone-0.1.22a0/pynecone/compiler/utils.py
--rw-r--r--   0        0        0     6371 2023-04-02 23:51:14.631475 pynecone-0.1.22a0/pynecone/components/__init__.py
--rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.22a0/pynecone/components/base/__init__.py
--rw-r--r--   0        0        0      726 2022-11-18 20:43:33.735684 pynecone-0.1.22a0/pynecone/components/base/bare.py
--rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.22a0/pynecone/components/base/body.py
--rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.22a0/pynecone/components/base/document.py
--rw-r--r--   0        0        0      242 2022-11-18 20:43:33.735533 pynecone-0.1.22a0/pynecone/components/base/head.py
--rw-r--r--   0        0        0      929 2023-03-13 04:10:28.761099 pynecone-0.1.22a0/pynecone/components/base/link.py
--rw-r--r--   0        0        0     1399 2023-03-10 00:25:42.693576 pynecone-0.1.22a0/pynecone/components/base/meta.py
--rw-r--r--   0        0        0    19436 2023-04-04 01:35:33.200080 pynecone-0.1.22a0/pynecone/components/component.py
--rw-r--r--   0        0        0      422 2023-04-02 23:51:14.632016 pynecone-0.1.22a0/pynecone/components/datadisplay/__init__.py
--rw-r--r--   0        0        0      333 2022-11-18 20:43:33.720898 pynecone-0.1.22a0/pynecone/components/datadisplay/badge.py
--rw-r--r--   0        0        0     2486 2023-03-16 23:52:12.744773 pynecone-0.1.22a0/pynecone/components/datadisplay/code.py
--rw-r--r--   0        0        0     4067 2023-04-02 23:51:28.427690 pynecone-0.1.22a0/pynecone/components/datadisplay/datatable.py
--rw-r--r--   0        0        0      536 2022-11-18 20:43:33.720383 pynecone-0.1.22a0/pynecone/components/datadisplay/divider.py
--rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.22a0/pynecone/components/datadisplay/keyboard_key.py
--rw-r--r--   0        0        0     1429 2023-03-13 04:10:28.547828 pynecone-0.1.22a0/pynecone/components/datadisplay/list.py
--rw-r--r--   0        0        0     2156 2023-03-09 23:41:57.135449 pynecone-0.1.22a0/pynecone/components/datadisplay/stat.py
--rw-r--r--   0        0        0     5156 2023-03-10 00:25:42.695438 pynecone-0.1.22a0/pynecone/components/datadisplay/table.py
--rw-r--r--   0        0        0      316 2023-01-24 02:43:48.871608 pynecone-0.1.22a0/pynecone/components/disclosure/__init__.py
--rw-r--r--   0        0        0     2940 2023-03-09 23:41:57.135814 pynecone-0.1.22a0/pynecone/components/disclosure/accordion.py
--rw-r--r--   0        0        0     2776 2023-03-09 23:41:57.135961 pynecone-0.1.22a0/pynecone/components/disclosure/tabs.py
--rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.22a0/pynecone/components/disclosure/visuallyhidden.py
--rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.22a0/pynecone/components/feedback/__init__.py
--rw-r--r--   0        0        0     1570 2023-03-10 00:25:42.695849 pynecone-0.1.22a0/pynecone/components/feedback/alert.py
--rw-r--r--   0        0        0     1904 2023-03-10 00:25:42.696112 pynecone-0.1.22a0/pynecone/components/feedback/circularprogress.py
--rw-r--r--   0        0        0      878 2023-03-10 00:25:42.696451 pynecone-0.1.22a0/pynecone/components/feedback/progress.py
--rw-r--r--   0        0        0     1784 2022-11-18 20:43:33.722941 pynecone-0.1.22a0/pynecone/components/feedback/skeleton.py
--rw-r--r--   0        0        0      677 2022-11-18 20:43:33.724636 pynecone-0.1.22a0/pynecone/components/feedback/spinner.py
--rw-r--r--   0        0        0     1103 2023-03-10 00:25:42.696881 pynecone-0.1.22a0/pynecone/components/forms/__init__.py
--rw-r--r--   0        0        0     1534 2022-11-18 20:43:33.708227 pynecone-0.1.22a0/pynecone/components/forms/button.py
--rw-r--r--   0        0        0     2240 2023-03-10 00:25:42.697372 pynecone-0.1.22a0/pynecone/components/forms/checkbox.py
--rw-r--r--   0        0        0      593 2023-01-30 21:50:18.211339 pynecone-0.1.22a0/pynecone/components/forms/copytoclipboard.py
--rw-r--r--   0        0        0     1964 2023-03-10 00:25:42.697696 pynecone-0.1.22a0/pynecone/components/forms/editable.py
--rw-r--r--   0        0        0     2323 2023-03-09 23:41:57.137070 pynecone-0.1.22a0/pynecone/components/forms/formcontrol.py
--rw-r--r--   0        0        0      801 2022-12-07 23:08:48.791901 pynecone-0.1.22a0/pynecone/components/forms/iconbutton.py
--rw-r--r--   0        0        0     2660 2023-03-10 00:25:42.698121 pynecone-0.1.22a0/pynecone/components/forms/input.py
--rw-r--r--   0        0        0     3916 2023-03-10 00:25:42.698330 pynecone-0.1.22a0/pynecone/components/forms/numberinput.py
--rw-r--r--   0        0        0      252 2023-03-10 00:25:42.698673 pynecone-0.1.22a0/pynecone/components/forms/password.py
--rw-r--r--   0        0        0     2685 2023-03-10 00:25:42.698849 pynecone-0.1.22a0/pynecone/components/forms/pininput.py
--rw-r--r--   0        0        0     3004 2023-03-16 23:52:12.745021 pynecone-0.1.22a0/pynecone/components/forms/radio.py
--rw-r--r--   0        0        0     2868 2023-03-10 00:25:42.699342 pynecone-0.1.22a0/pynecone/components/forms/rangeslider.py
--rw-r--r--   0        0        0     3475 2023-03-16 23:52:12.745104 pynecone-0.1.22a0/pynecone/components/forms/select.py
--rw-r--r--   0        0        0     2782 2023-03-10 00:25:42.699714 pynecone-0.1.22a0/pynecone/components/forms/slider.py
--rw-r--r--   0        0        0     1466 2023-03-10 00:25:42.699988 pynecone-0.1.22a0/pynecone/components/forms/switch.py
--rw-r--r--   0        0        0     1550 2023-03-10 00:25:42.700204 pynecone-0.1.22a0/pynecone/components/forms/textarea.py
--rw-r--r--   0        0        0     2691 2023-04-02 23:51:14.632480 pynecone-0.1.22a0/pynecone/components/forms/upload.py
--rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.22a0/pynecone/components/graphing/__init__.py
--rw-r--r--   0        0        0     1356 2023-04-04 00:07:26.680060 pynecone-0.1.22a0/pynecone/components/graphing/plotly.py
--rw-r--r--   0        0        0    17359 2023-04-02 23:51:28.428293 pynecone-0.1.22a0/pynecone/components/graphing/victory.py
--rw-r--r--   0        0        0      815 2023-04-02 23:51:14.632791 pynecone-0.1.22a0/pynecone/components/layout/__init__.py
--rw-r--r--   0        0        0      323 2023-04-02 23:51:14.632894 pynecone-0.1.22a0/pynecone/components/layout/aspect_ratio.py
--rw-r--r--   0        0        0      768 2022-12-15 19:19:57.795670 pynecone-0.1.22a0/pynecone/components/layout/box.py
--rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.22a0/pynecone/components/layout/center.py
--rw-r--r--   0        0        0     3136 2023-03-16 23:52:12.745203 pynecone-0.1.22a0/pynecone/components/layout/cond.py
--rw-r--r--   0        0        0      362 2022-12-07 23:08:48.792884 pynecone-0.1.22a0/pynecone/components/layout/container.py
--rw-r--r--   0        0        0      655 2022-12-07 23:08:48.793078 pynecone-0.1.22a0/pynecone/components/layout/flex.py
--rw-r--r--   0        0        0     1781 2023-03-10 00:25:42.701858 pynecone-0.1.22a0/pynecone/components/layout/foreach.py
--rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.22a0/pynecone/components/layout/fragment.py
--rw-r--r--   0        0        0     2417 2023-01-28 19:09:51.493446 pynecone-0.1.22a0/pynecone/components/layout/grid.py
--rw-r--r--   0        0        0      979 2023-04-08 16:05:43.352661 pynecone-0.1.22a0/pynecone/components/layout/html.py
--rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.22a0/pynecone/components/layout/responsive.py
--rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.22a0/pynecone/components/layout/spacer.py
--rw-r--r--   0        0        0      994 2022-12-07 23:08:48.793762 pynecone-0.1.22a0/pynecone/components/layout/stack.py
--rw-r--r--   0        0        0     1470 2023-03-09 23:41:57.138212 pynecone-0.1.22a0/pynecone/components/layout/wrap.py
--rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.22a0/pynecone/components/libs/__init__.py
--rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.22a0/pynecone/components/libs/chakra.py
--rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.22a0/pynecone/components/media/__init__.py
--rw-r--r--   0        0        0     1539 2022-11-28 06:46:25.092156 pynecone-0.1.22a0/pynecone/components/media/avatar.py
--rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.22a0/pynecone/components/media/icon.py
--rw-r--r--   0        0        0     1415 2022-12-07 23:08:48.794371 pynecone-0.1.22a0/pynecone/components/media/image.py
--rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.22a0/pynecone/components/navigation/__init__.py
--rw-r--r--   0        0        0     2022 2023-03-09 23:41:57.138732 pynecone-0.1.22a0/pynecone/components/navigation/breadcrumb.py
--rw-r--r--   0        0        0     1005 2023-01-24 01:31:44.831545 pynecone-0.1.22a0/pynecone/components/navigation/link.py
--rw-r--r--   0        0        0      529 2022-12-07 23:08:48.794948 pynecone-0.1.22a0/pynecone/components/navigation/linkoverlay.py
--rw-r--r--   0        0        0      483 2022-12-07 23:08:48.795126 pynecone-0.1.22a0/pynecone/components/navigation/nextlink.py
--rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.22a0/pynecone/components/overlay/__init__.py
--rw-r--r--   0        0        0     5042 2023-03-10 00:25:42.703076 pynecone-0.1.22a0/pynecone/components/overlay/alertdialog.py
--rw-r--r--   0        0        0     4696 2023-03-10 00:25:42.703402 pynecone-0.1.22a0/pynecone/components/overlay/drawer.py
--rw-r--r--   0        0        0     5545 2023-03-10 00:25:42.703834 pynecone-0.1.22a0/pynecone/components/overlay/menu.py
--rw-r--r--   0        0        0     4932 2023-03-10 00:25:42.704095 pynecone-0.1.22a0/pynecone/components/overlay/modal.py
--rw-r--r--   0        0        0     5703 2023-03-09 23:41:57.139627 pynecone-0.1.22a0/pynecone/components/overlay/popover.py
--rw-r--r--   0        0        0     1964 2023-01-28 19:09:51.496014 pynecone-0.1.22a0/pynecone/components/overlay/tooltip.py
--rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.22a0/pynecone/components/tags/__init__.py
--rw-r--r--   0        0        0      840 2023-03-16 23:52:12.745828 pynecone-0.1.22a0/pynecone/components/tags/cond_tag.py
--rw-r--r--   0        0        0     3000 2023-03-16 23:52:12.746048 pynecone-0.1.22a0/pynecone/components/tags/iter_tag.py
--rw-r--r--   0        0        0     6288 2023-04-02 23:51:14.633181 pynecone-0.1.22a0/pynecone/components/tags/tag.py
--rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.22a0/pynecone/components/tags/tagless.py
--rw-r--r--   0        0        0      271 2022-12-07 23:08:48.795802 pynecone-0.1.22a0/pynecone/components/typography/__init__.py
--rw-r--r--   0        0        0      281 2022-12-07 23:08:48.796090 pynecone-0.1.22a0/pynecone/components/typography/heading.py
--rw-r--r--   0        0        0      357 2023-03-09 23:41:57.139928 pynecone-0.1.22a0/pynecone/components/typography/highlight.py
--rw-r--r--   0        0        0     2973 2023-04-08 16:05:43.353266 pynecone-0.1.22a0/pynecone/components/typography/markdown.py
--rw-r--r--   0        0        0      336 2022-12-08 04:28:39.380713 pynecone-0.1.22a0/pynecone/components/typography/span.py
--rw-r--r--   0        0        0      305 2022-12-07 23:08:48.796735 pynecone-0.1.22a0/pynecone/components/typography/text.py
--rw-r--r--   0        0        0     5296 2023-04-08 16:05:43.353608 pynecone-0.1.22a0/pynecone/config.py
--rw-r--r--   0        0        0     8905 2023-04-04 00:07:26.681289 pynecone-0.1.22a0/pynecone/constants.py
--rw-r--r--   0        0        0       73 2023-04-03 21:29:22.111846 pynecone-0.1.22a0/pynecone/el/__init__.py
--rw-r--r--   0        0        0      115 2023-04-03 21:29:22.112002 pynecone-0.1.22a0/pynecone/el/constants/__init__.py
--rw-r--r--   0        0        0     7175 2023-04-03 21:29:22.112233 pynecone-0.1.22a0/pynecone/el/constants/html.py
--rw-r--r--   0        0        0     1719 2023-04-04 00:00:54.955098 pynecone-0.1.22a0/pynecone/el/constants/pynecone.py
--rw-r--r--   0        0        0    15554 2023-04-03 21:29:22.112537 pynecone-0.1.22a0/pynecone/el/constants/react.py
--rw-r--r--   0        0        0     1289 2023-04-04 00:00:54.955401 pynecone-0.1.22a0/pynecone/el/element.py
--rw-r--r--   0        0        0   108515 2023-04-03 21:29:22.113056 pynecone-0.1.22a0/pynecone/el/elements/__init__.py
--rwxr-xr-x   0        0        0     2666 2023-04-04 00:00:54.955649 pynecone-0.1.22a0/pynecone/el/precompile.py
--rw-r--r--   0        0        0     9581 2023-04-08 19:55:02.842558 pynecone-0.1.22a0/pynecone/event.py
--rw-r--r--   0        0        0      163 2022-12-27 07:24:05.349499 pynecone-0.1.22a0/pynecone/middleware/__init__.py
--rw-r--r--   0        0        0     2781 2023-04-08 17:02:14.865880 pynecone-0.1.22a0/pynecone/middleware/hydrate_middleware.py
--rw-r--r--   0        0        0     1022 2023-04-08 16:05:43.354548 pynecone-0.1.22a0/pynecone/middleware/logging_middleware.py
--rw-r--r--   0        0        0     1193 2023-04-08 16:05:43.355024 pynecone-0.1.22a0/pynecone/middleware/middleware.py
--rw-r--r--   0        0        0     1583 2023-04-02 23:51:28.428464 pynecone-0.1.22a0/pynecone/model.py
--rw-r--r--   0        0        0     7580 2023-04-08 16:05:43.355348 pynecone-0.1.22a0/pynecone/pc.py
--rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.22a0/pynecone/py.typed
--rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.22a0/pynecone/route.py
--rw-r--r--   0        0        0    23620 2023-04-08 16:55:17.975051 pynecone-0.1.22a0/pynecone/state.py
--rw-r--r--   0        0        0     1059 2023-03-16 23:52:12.748857 pynecone-0.1.22a0/pynecone/style.py
--rw-r--r--   0        0        0     2411 2023-03-10 00:25:42.708535 pynecone-0.1.22a0/pynecone/telemetry.py
--rw-r--r--   0        0        0     4054 2023-03-16 23:52:12.749028 pynecone-0.1.22a0/pynecone/utils/build.py
--rw-r--r--   0        0        0     1627 2023-03-16 23:52:12.749156 pynecone-0.1.22a0/pynecone/utils/console.py
--rw-r--r--   0        0        0     3795 2023-03-16 23:52:12.756812 pynecone-0.1.22a0/pynecone/utils/exec.py
--rw-r--r--   0        0        0     9766 2023-04-02 23:51:28.428628 pynecone-0.1.22a0/pynecone/utils/format.py
--rw-r--r--   0        0        0      544 2023-03-16 23:52:12.757094 pynecone-0.1.22a0/pynecone/utils/imports.py
--rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.22a0/pynecone/utils/path_ops.py
--rw-r--r--   0        0        0     8615 2023-04-04 00:07:26.681689 pynecone-0.1.22a0/pynecone/utils/prerequisites.py
--rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.22a0/pynecone/utils/processes.py
--rw-r--r--   0        0        0     4299 2023-03-16 23:52:12.757408 pynecone-0.1.22a0/pynecone/utils/types.py
--rw-r--r--   0        0        0    25132 2023-04-02 23:51:28.428813 pynecone-0.1.22a0/pynecone/var.py
--rw-r--r--   0        0        0     2634 2023-03-13 04:10:28.761553 pynecone-0.1.22a0/pynecone/watch.py
--rw-r--r--   0        0        0     1757 2023-04-09 05:55:04.077494 pynecone-0.1.22a0/pyproject.toml
--rw-r--r--   0        0        0     9856 1970-01-01 00:00:00.000000 pynecone-0.1.22a0/PKG-INFO
+-rw-r--r--   0        0        0    11356 2023-01-24 01:31:44.826695 pynecone-0.1.23a0/LICENSE
+-rw-r--r--   0        0        0     8364 2023-03-16 23:51:05.127293 pynecone-0.1.23a0/README.md
+-rw-r--r--   0        0        0        0 2022-11-18 20:43:33.738202 pynecone-0.1.23a0/pynecone/.templates/app/__init__.py
+-rw-r--r--   0        0        0     1036 2023-03-10 00:25:42.687001 pynecone-0.1.23a0/pynecone/.templates/app/tutorial.py
+-rw-r--r--   0        0        0    15406 2022-11-18 20:43:33.740339 pynecone-0.1.23a0/pynecone/.templates/assets/favicon.ico
+-rw-r--r--   0        0        0      417 2022-12-27 07:35:12.085907 pynecone-0.1.23a0/pynecone/.templates/web/.gitignore
+-rwxr-xr-x   0        0        0   261125 2023-03-10 00:25:42.688288 pynecone-0.1.23a0/pynecone/.templates/web/bun.lockb
+-rw-r--r--   0        0        0       47 2022-12-20 23:31:29.590974 pynecone-0.1.23a0/pynecone/.templates/web/next.config.js
+-rw-r--r--   0        0        0     1017 2023-04-02 23:51:14.630623 pynecone-0.1.23a0/pynecone/.templates/web/package.json
+-rw-r--r--   0        0        0      502 2022-11-18 20:43:33.740024 pynecone-0.1.23a0/pynecone/.templates/web/pages/404.js
+-rw-r--r--   0        0        0      564 2023-01-12 05:38:04.342282 pynecone-0.1.23a0/pynecone/.templates/web/pages/_app.js
+-rw-r--r--   0        0        0       28 2023-04-03 00:00:47.639618 pynecone-0.1.23a0/pynecone/.templates/web/pynecone.json
+-rw-r--r--   0        0        0    29404 2022-12-20 23:31:29.592485 pynecone-0.1.23a0/pynecone/.templates/web/styles/code/prism.js
+-rw-r--r--   0        0        0     6456 2023-04-02 23:51:28.426792 pynecone-0.1.23a0/pynecone/.templates/web/utils/state.js
+-rw-r--r--   0        0        0      808 2023-04-08 16:05:43.351479 pynecone-0.1.23a0/pynecone/__init__.py
+-rw-r--r--   0        0        0    19946 2023-04-09 05:48:16.467591 pynecone-0.1.23a0/pynecone/app.py
+-rw-r--r--   0        0        0     2510 2023-01-30 21:50:18.206745 pynecone-0.1.23a0/pynecone/base.py
+-rw-r--r--   0        0        0       29 2022-11-18 20:43:33.740719 pynecone-0.1.23a0/pynecone/compiler/__init__.py
+-rw-r--r--   0        0        0     5737 2023-04-03 21:50:34.663262 pynecone-0.1.23a0/pynecone/compiler/compiler.py
+-rw-r--r--   0        0        0     5334 2023-04-02 23:51:14.631307 pynecone-0.1.23a0/pynecone/compiler/templates.py
+-rw-r--r--   0        0        0     9084 2023-03-16 23:52:12.744496 pynecone-0.1.23a0/pynecone/compiler/utils.py
+-rw-r--r--   0        0        0     6371 2023-04-02 23:51:14.631475 pynecone-0.1.23a0/pynecone/components/__init__.py
+-rw-r--r--   0        0        0      226 2023-03-13 04:10:28.615930 pynecone-0.1.23a0/pynecone/components/base/__init__.py
+-rw-r--r--   0        0        0      726 2022-11-18 20:43:33.735684 pynecone-0.1.23a0/pynecone/components/base/bare.py
+-rw-r--r--   0        0        0      153 2023-03-13 04:10:28.760655 pynecone-0.1.23a0/pynecone/components/base/body.py
+-rw-r--r--   0        0        0      725 2023-01-30 22:40:32.678074 pynecone-0.1.23a0/pynecone/components/base/document.py
+-rw-r--r--   0        0        0      242 2022-11-18 20:43:33.735533 pynecone-0.1.23a0/pynecone/components/base/head.py
+-rw-r--r--   0        0        0      929 2023-03-13 04:10:28.761099 pynecone-0.1.23a0/pynecone/components/base/link.py
+-rw-r--r--   0        0        0     1399 2023-03-10 00:25:42.693576 pynecone-0.1.23a0/pynecone/components/base/meta.py
+-rw-r--r--   0        0        0    19436 2023-04-04 01:35:33.200080 pynecone-0.1.23a0/pynecone/components/component.py
+-rw-r--r--   0        0        0      422 2023-04-02 23:51:14.632016 pynecone-0.1.23a0/pynecone/components/datadisplay/__init__.py
+-rw-r--r--   0        0        0      333 2022-11-18 20:43:33.720898 pynecone-0.1.23a0/pynecone/components/datadisplay/badge.py
+-rw-r--r--   0        0        0     2486 2023-03-16 23:52:12.744773 pynecone-0.1.23a0/pynecone/components/datadisplay/code.py
+-rw-r--r--   0        0        0     4067 2023-04-02 23:51:28.427690 pynecone-0.1.23a0/pynecone/components/datadisplay/datatable.py
+-rw-r--r--   0        0        0      536 2022-11-18 20:43:33.720383 pynecone-0.1.23a0/pynecone/components/datadisplay/divider.py
+-rw-r--r--   0        0        0      187 2023-04-02 23:51:14.632124 pynecone-0.1.23a0/pynecone/components/datadisplay/keyboard_key.py
+-rw-r--r--   0        0        0     1429 2023-03-13 04:10:28.547828 pynecone-0.1.23a0/pynecone/components/datadisplay/list.py
+-rw-r--r--   0        0        0     2156 2023-03-09 23:41:57.135449 pynecone-0.1.23a0/pynecone/components/datadisplay/stat.py
+-rw-r--r--   0        0        0     5156 2023-03-10 00:25:42.695438 pynecone-0.1.23a0/pynecone/components/datadisplay/table.py
+-rw-r--r--   0        0        0      316 2023-01-24 02:43:48.871608 pynecone-0.1.23a0/pynecone/components/disclosure/__init__.py
+-rw-r--r--   0        0        0     2940 2023-03-09 23:41:57.135814 pynecone-0.1.23a0/pynecone/components/disclosure/accordion.py
+-rw-r--r--   0        0        0     2776 2023-03-09 23:41:57.135961 pynecone-0.1.23a0/pynecone/components/disclosure/tabs.py
+-rw-r--r--   0        0        0      285 2022-12-05 22:26:47.605453 pynecone-0.1.23a0/pynecone/components/disclosure/visuallyhidden.py
+-rw-r--r--   0        0        0      313 2022-11-18 20:43:33.723246 pynecone-0.1.23a0/pynecone/components/feedback/__init__.py
+-rw-r--r--   0        0        0     1570 2023-03-10 00:25:42.695849 pynecone-0.1.23a0/pynecone/components/feedback/alert.py
+-rw-r--r--   0        0        0     1904 2023-03-10 00:25:42.696112 pynecone-0.1.23a0/pynecone/components/feedback/circularprogress.py
+-rw-r--r--   0        0        0      878 2023-03-10 00:25:42.696451 pynecone-0.1.23a0/pynecone/components/feedback/progress.py
+-rw-r--r--   0        0        0     1784 2022-11-18 20:43:33.722941 pynecone-0.1.23a0/pynecone/components/feedback/skeleton.py
+-rw-r--r--   0        0        0      677 2022-11-18 20:43:33.724636 pynecone-0.1.23a0/pynecone/components/feedback/spinner.py
+-rw-r--r--   0        0        0     1103 2023-03-10 00:25:42.696881 pynecone-0.1.23a0/pynecone/components/forms/__init__.py
+-rw-r--r--   0        0        0     1534 2022-11-18 20:43:33.708227 pynecone-0.1.23a0/pynecone/components/forms/button.py
+-rw-r--r--   0        0        0     2240 2023-03-10 00:25:42.697372 pynecone-0.1.23a0/pynecone/components/forms/checkbox.py
+-rw-r--r--   0        0        0      593 2023-01-30 21:50:18.211339 pynecone-0.1.23a0/pynecone/components/forms/copytoclipboard.py
+-rw-r--r--   0        0        0     1964 2023-03-10 00:25:42.697696 pynecone-0.1.23a0/pynecone/components/forms/editable.py
+-rw-r--r--   0        0        0     2323 2023-03-09 23:41:57.137070 pynecone-0.1.23a0/pynecone/components/forms/formcontrol.py
+-rw-r--r--   0        0        0      801 2022-12-07 23:08:48.791901 pynecone-0.1.23a0/pynecone/components/forms/iconbutton.py
+-rw-r--r--   0        0        0     2660 2023-03-10 00:25:42.698121 pynecone-0.1.23a0/pynecone/components/forms/input.py
+-rw-r--r--   0        0        0     3916 2023-03-10 00:25:42.698330 pynecone-0.1.23a0/pynecone/components/forms/numberinput.py
+-rw-r--r--   0        0        0      252 2023-03-10 00:25:42.698673 pynecone-0.1.23a0/pynecone/components/forms/password.py
+-rw-r--r--   0        0        0     2685 2023-03-10 00:25:42.698849 pynecone-0.1.23a0/pynecone/components/forms/pininput.py
+-rw-r--r--   0        0        0     3004 2023-03-16 23:52:12.745021 pynecone-0.1.23a0/pynecone/components/forms/radio.py
+-rw-r--r--   0        0        0     2868 2023-03-10 00:25:42.699342 pynecone-0.1.23a0/pynecone/components/forms/rangeslider.py
+-rw-r--r--   0        0        0     3475 2023-03-16 23:52:12.745104 pynecone-0.1.23a0/pynecone/components/forms/select.py
+-rw-r--r--   0        0        0     2782 2023-03-10 00:25:42.699714 pynecone-0.1.23a0/pynecone/components/forms/slider.py
+-rw-r--r--   0        0        0     1466 2023-03-10 00:25:42.699988 pynecone-0.1.23a0/pynecone/components/forms/switch.py
+-rw-r--r--   0        0        0     1550 2023-03-10 00:25:42.700204 pynecone-0.1.23a0/pynecone/components/forms/textarea.py
+-rw-r--r--   0        0        0     2691 2023-04-02 23:51:14.632480 pynecone-0.1.23a0/pynecone/components/forms/upload.py
+-rw-r--r--   0        0        0      351 2023-01-24 02:43:48.879007 pynecone-0.1.23a0/pynecone/components/graphing/__init__.py
+-rw-r--r--   0        0        0     1356 2023-04-04 00:07:26.680060 pynecone-0.1.23a0/pynecone/components/graphing/plotly.py
+-rw-r--r--   0        0        0    17359 2023-04-02 23:51:28.428293 pynecone-0.1.23a0/pynecone/components/graphing/victory.py
+-rw-r--r--   0        0        0      815 2023-04-02 23:51:14.632791 pynecone-0.1.23a0/pynecone/components/layout/__init__.py
+-rw-r--r--   0        0        0      323 2023-04-02 23:51:14.632894 pynecone-0.1.23a0/pynecone/components/layout/aspect_ratio.py
+-rw-r--r--   0        0        0      768 2022-12-15 19:19:57.795670 pynecone-0.1.23a0/pynecone/components/layout/box.py
+-rw-r--r--   0        0        0      396 2022-12-07 23:08:48.792563 pynecone-0.1.23a0/pynecone/components/layout/center.py
+-rw-r--r--   0        0        0     3136 2023-03-16 23:52:12.745203 pynecone-0.1.23a0/pynecone/components/layout/cond.py
+-rw-r--r--   0        0        0      362 2022-12-07 23:08:48.792884 pynecone-0.1.23a0/pynecone/components/layout/container.py
+-rw-r--r--   0        0        0      655 2022-12-07 23:08:48.793078 pynecone-0.1.23a0/pynecone/components/layout/flex.py
+-rw-r--r--   0        0        0     1781 2023-03-10 00:25:42.701858 pynecone-0.1.23a0/pynecone/components/layout/foreach.py
+-rw-r--r--   0        0        0      314 2022-12-20 23:31:29.595612 pynecone-0.1.23a0/pynecone/components/layout/fragment.py
+-rw-r--r--   0        0        0     2417 2023-01-28 19:09:51.493446 pynecone-0.1.23a0/pynecone/components/layout/grid.py
+-rw-r--r--   0        0        0      979 2023-04-08 16:05:43.352661 pynecone-0.1.23a0/pynecone/components/layout/html.py
+-rw-r--r--   0        0        0     1900 2023-03-10 00:25:42.702272 pynecone-0.1.23a0/pynecone/components/layout/responsive.py
+-rw-r--r--   0        0        0      186 2022-12-07 23:08:48.793614 pynecone-0.1.23a0/pynecone/components/layout/spacer.py
+-rw-r--r--   0        0        0      994 2022-12-07 23:08:48.793762 pynecone-0.1.23a0/pynecone/components/layout/stack.py
+-rw-r--r--   0        0        0     1470 2023-03-09 23:41:57.138212 pynecone-0.1.23a0/pynecone/components/layout/wrap.py
+-rw-r--r--   0        0        0       33 2022-11-18 20:43:33.727543 pynecone-0.1.23a0/pynecone/components/libs/__init__.py
+-rw-r--r--   0        0        0      222 2022-11-18 20:43:33.727419 pynecone-0.1.23a0/pynecone/components/libs/chakra.py
+-rw-r--r--   0        0        0      190 2022-11-18 20:43:33.736163 pynecone-0.1.23a0/pynecone/components/media/__init__.py
+-rw-r--r--   0        0        0     1539 2022-11-28 06:46:25.092156 pynecone-0.1.23a0/pynecone/components/media/avatar.py
+-rw-r--r--   0        0        0     2391 2023-03-16 23:52:12.745547 pynecone-0.1.23a0/pynecone/components/media/icon.py
+-rw-r--r--   0        0        0     1415 2022-12-07 23:08:48.794371 pynecone-0.1.23a0/pynecone/components/media/image.py
+-rw-r--r--   0        0        0      282 2023-01-24 02:43:48.884756 pynecone-0.1.23a0/pynecone/components/navigation/__init__.py
+-rw-r--r--   0        0        0     2022 2023-03-09 23:41:57.138732 pynecone-0.1.23a0/pynecone/components/navigation/breadcrumb.py
+-rw-r--r--   0        0        0     1005 2023-01-24 01:31:44.831545 pynecone-0.1.23a0/pynecone/components/navigation/link.py
+-rw-r--r--   0        0        0      529 2022-12-07 23:08:48.794948 pynecone-0.1.23a0/pynecone/components/navigation/linkoverlay.py
+-rw-r--r--   0        0        0      483 2022-12-07 23:08:48.795126 pynecone-0.1.23a0/pynecone/components/navigation/nextlink.py
+-rw-r--r--   0        0        0      850 2023-01-24 02:43:48.892006 pynecone-0.1.23a0/pynecone/components/overlay/__init__.py
+-rw-r--r--   0        0        0     5042 2023-03-10 00:25:42.703076 pynecone-0.1.23a0/pynecone/components/overlay/alertdialog.py
+-rw-r--r--   0        0        0     4696 2023-03-10 00:25:42.703402 pynecone-0.1.23a0/pynecone/components/overlay/drawer.py
+-rw-r--r--   0        0        0     5545 2023-03-10 00:25:42.703834 pynecone-0.1.23a0/pynecone/components/overlay/menu.py
+-rw-r--r--   0        0        0     4932 2023-03-10 00:25:42.704095 pynecone-0.1.23a0/pynecone/components/overlay/modal.py
+-rw-r--r--   0        0        0     5703 2023-03-09 23:41:57.139627 pynecone-0.1.23a0/pynecone/components/overlay/popover.py
+-rw-r--r--   0        0        0     1964 2023-01-28 19:09:51.496014 pynecone-0.1.23a0/pynecone/components/overlay/tooltip.py
+-rw-r--r--   0        0        0      120 2022-11-18 20:43:33.725191 pynecone-0.1.23a0/pynecone/components/tags/__init__.py
+-rw-r--r--   0        0        0      840 2023-03-16 23:52:12.745828 pynecone-0.1.23a0/pynecone/components/tags/cond_tag.py
+-rw-r--r--   0        0        0     3000 2023-03-16 23:52:12.746048 pynecone-0.1.23a0/pynecone/components/tags/iter_tag.py
+-rw-r--r--   0        0        0     6288 2023-04-02 23:51:14.633181 pynecone-0.1.23a0/pynecone/components/tags/tag.py
+-rw-r--r--   0        0        0      591 2023-03-16 23:52:12.746470 pynecone-0.1.23a0/pynecone/components/tags/tagless.py
+-rw-r--r--   0        0        0      271 2022-12-07 23:08:48.795802 pynecone-0.1.23a0/pynecone/components/typography/__init__.py
+-rw-r--r--   0        0        0      281 2022-12-07 23:08:48.796090 pynecone-0.1.23a0/pynecone/components/typography/heading.py
+-rw-r--r--   0        0        0      357 2023-03-09 23:41:57.139928 pynecone-0.1.23a0/pynecone/components/typography/highlight.py
+-rw-r--r--   0        0        0     2973 2023-04-08 16:05:43.353266 pynecone-0.1.23a0/pynecone/components/typography/markdown.py
+-rw-r--r--   0        0        0      336 2022-12-08 04:28:39.380713 pynecone-0.1.23a0/pynecone/components/typography/span.py
+-rw-r--r--   0        0        0      305 2022-12-07 23:08:48.796735 pynecone-0.1.23a0/pynecone/components/typography/text.py
+-rw-r--r--   0        0        0     5296 2023-04-08 16:05:43.353608 pynecone-0.1.23a0/pynecone/config.py
+-rw-r--r--   0        0        0     8905 2023-04-04 00:07:26.681289 pynecone-0.1.23a0/pynecone/constants.py
+-rw-r--r--   0        0        0       73 2023-04-03 21:29:22.111846 pynecone-0.1.23a0/pynecone/el/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-03 21:29:22.112002 pynecone-0.1.23a0/pynecone/el/constants/__init__.py
+-rw-r--r--   0        0        0     7175 2023-04-03 21:29:22.112233 pynecone-0.1.23a0/pynecone/el/constants/html.py
+-rw-r--r--   0        0        0     1719 2023-04-04 00:00:54.955098 pynecone-0.1.23a0/pynecone/el/constants/pynecone.py
+-rw-r--r--   0        0        0    15554 2023-04-03 21:29:22.112537 pynecone-0.1.23a0/pynecone/el/constants/react.py
+-rw-r--r--   0        0        0     1289 2023-04-04 00:00:54.955401 pynecone-0.1.23a0/pynecone/el/element.py
+-rw-r--r--   0        0        0   108515 2023-04-03 21:29:22.113056 pynecone-0.1.23a0/pynecone/el/elements/__init__.py
+-rwxr-xr-x   0        0        0     2666 2023-04-04 00:00:54.955649 pynecone-0.1.23a0/pynecone/el/precompile.py
+-rw-r--r--   0        0        0     9581 2023-04-08 19:55:02.842558 pynecone-0.1.23a0/pynecone/event.py
+-rw-r--r--   0        0        0      163 2022-12-27 07:24:05.349499 pynecone-0.1.23a0/pynecone/middleware/__init__.py
+-rw-r--r--   0        0        0     2781 2023-04-08 17:02:14.865880 pynecone-0.1.23a0/pynecone/middleware/hydrate_middleware.py
+-rw-r--r--   0        0        0     1022 2023-04-08 16:05:43.354548 pynecone-0.1.23a0/pynecone/middleware/logging_middleware.py
+-rw-r--r--   0        0        0     1193 2023-04-08 16:05:43.355024 pynecone-0.1.23a0/pynecone/middleware/middleware.py
+-rw-r--r--   0        0        0     1583 2023-04-02 23:51:28.428464 pynecone-0.1.23a0/pynecone/model.py
+-rw-r--r--   0        0        0     7580 2023-04-08 16:05:43.355348 pynecone-0.1.23a0/pynecone/pc.py
+-rw-r--r--   0        0        0        0 2023-03-10 00:25:42.707141 pynecone-0.1.23a0/pynecone/py.typed
+-rw-r--r--   0        0        0     4108 2023-03-16 23:52:12.748303 pynecone-0.1.23a0/pynecone/route.py
+-rw-r--r--   0        0        0    23620 2023-04-08 16:55:17.975051 pynecone-0.1.23a0/pynecone/state.py
+-rw-r--r--   0        0        0     1059 2023-03-16 23:52:12.748857 pynecone-0.1.23a0/pynecone/style.py
+-rw-r--r--   0        0        0     2411 2023-03-10 00:25:42.708535 pynecone-0.1.23a0/pynecone/telemetry.py
+-rw-r--r--   0        0        0     4054 2023-03-16 23:52:12.749028 pynecone-0.1.23a0/pynecone/utils/build.py
+-rw-r--r--   0        0        0     1627 2023-03-16 23:52:12.749156 pynecone-0.1.23a0/pynecone/utils/console.py
+-rw-r--r--   0        0        0     3795 2023-03-16 23:52:12.756812 pynecone-0.1.23a0/pynecone/utils/exec.py
+-rw-r--r--   0        0        0     9766 2023-04-02 23:51:28.428628 pynecone-0.1.23a0/pynecone/utils/format.py
+-rw-r--r--   0        0        0      544 2023-03-16 23:52:12.757094 pynecone-0.1.23a0/pynecone/utils/imports.py
+-rw-r--r--   0        0        0     2451 2023-03-16 23:52:12.757162 pynecone-0.1.23a0/pynecone/utils/path_ops.py
+-rw-r--r--   0        0        0     8548 2023-04-10 04:57:24.110379 pynecone-0.1.23a0/pynecone/utils/prerequisites.py
+-rw-r--r--   0        0        0     3021 2023-03-16 23:52:12.757337 pynecone-0.1.23a0/pynecone/utils/processes.py
+-rw-r--r--   0        0        0     4299 2023-03-16 23:52:12.757408 pynecone-0.1.23a0/pynecone/utils/types.py
+-rw-r--r--   0        0        0    25132 2023-04-02 23:51:28.428813 pynecone-0.1.23a0/pynecone/var.py
+-rw-r--r--   0        0        0     2634 2023-03-13 04:10:28.761553 pynecone-0.1.23a0/pynecone/watch.py
+-rw-r--r--   0        0        0     1758 2023-04-10 04:58:16.232151 pynecone-0.1.23a0/pyproject.toml
+-rw-r--r--   0        0        0     9856 1970-01-01 00:00:00.000000 pynecone-0.1.23a0/PKG-INFO
```

### Comparing `pynecone-0.1.22a0/LICENSE` & `pynecone-0.1.23a0/LICENSE`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/README.md` & `pynecone-0.1.23a0/README.md`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/.templates/app/tutorial.py` & `pynecone-0.1.23a0/pynecone/.templates/app/tutorial.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/.templates/assets/favicon.ico` & `pynecone-0.1.23a0/pynecone/.templates/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/.templates/web/bun.lockb` & `pynecone-0.1.23a0/pynecone/.templates/web/bun.lockb`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/.templates/web/package.json` & `pynecone-0.1.23a0/pynecone/.templates/web/package.json`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/.templates/web/pages/_app.js` & `pynecone-0.1.23a0/pynecone/.templates/web/pages/_app.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/.templates/web/styles/code/prism.js` & `pynecone-0.1.23a0/pynecone/.templates/web/styles/code/prism.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/.templates/web/utils/state.js` & `pynecone-0.1.23a0/pynecone/.templates/web/utils/state.js`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/__init__.py` & `pynecone-0.1.23a0/pynecone/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/app.py` & `pynecone-0.1.23a0/pynecone/app.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/base.py` & `pynecone-0.1.23a0/pynecone/base.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/compiler/compiler.py` & `pynecone-0.1.23a0/pynecone/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/compiler/templates.py` & `pynecone-0.1.23a0/pynecone/compiler/templates.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/compiler/utils.py` & `pynecone-0.1.23a0/pynecone/compiler/utils.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/__init__.py` & `pynecone-0.1.23a0/pynecone/components/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/base/bare.py` & `pynecone-0.1.23a0/pynecone/components/base/bare.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/base/document.py` & `pynecone-0.1.23a0/pynecone/components/base/document.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/base/link.py` & `pynecone-0.1.23a0/pynecone/components/base/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/base/meta.py` & `pynecone-0.1.23a0/pynecone/components/base/meta.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/component.py` & `pynecone-0.1.23a0/pynecone/components/component.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/datadisplay/code.py` & `pynecone-0.1.23a0/pynecone/components/datadisplay/code.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/datadisplay/datatable.py` & `pynecone-0.1.23a0/pynecone/components/datadisplay/datatable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/datadisplay/divider.py` & `pynecone-0.1.23a0/pynecone/components/datadisplay/divider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/datadisplay/list.py` & `pynecone-0.1.23a0/pynecone/components/datadisplay/list.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/datadisplay/stat.py` & `pynecone-0.1.23a0/pynecone/components/datadisplay/stat.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/datadisplay/table.py` & `pynecone-0.1.23a0/pynecone/components/datadisplay/table.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/disclosure/accordion.py` & `pynecone-0.1.23a0/pynecone/components/disclosure/accordion.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/disclosure/tabs.py` & `pynecone-0.1.23a0/pynecone/components/disclosure/tabs.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/feedback/alert.py` & `pynecone-0.1.23a0/pynecone/components/feedback/alert.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/feedback/circularprogress.py` & `pynecone-0.1.23a0/pynecone/components/feedback/circularprogress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/feedback/progress.py` & `pynecone-0.1.23a0/pynecone/components/feedback/progress.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/feedback/skeleton.py` & `pynecone-0.1.23a0/pynecone/components/feedback/skeleton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/feedback/spinner.py` & `pynecone-0.1.23a0/pynecone/components/feedback/spinner.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/__init__.py` & `pynecone-0.1.23a0/pynecone/components/forms/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/button.py` & `pynecone-0.1.23a0/pynecone/components/forms/button.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/checkbox.py` & `pynecone-0.1.23a0/pynecone/components/forms/checkbox.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/copytoclipboard.py` & `pynecone-0.1.23a0/pynecone/components/forms/copytoclipboard.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/editable.py` & `pynecone-0.1.23a0/pynecone/components/forms/editable.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/formcontrol.py` & `pynecone-0.1.23a0/pynecone/components/forms/formcontrol.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/iconbutton.py` & `pynecone-0.1.23a0/pynecone/components/forms/iconbutton.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/input.py` & `pynecone-0.1.23a0/pynecone/components/forms/input.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/numberinput.py` & `pynecone-0.1.23a0/pynecone/components/forms/numberinput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/pininput.py` & `pynecone-0.1.23a0/pynecone/components/forms/pininput.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/radio.py` & `pynecone-0.1.23a0/pynecone/components/forms/radio.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/rangeslider.py` & `pynecone-0.1.23a0/pynecone/components/forms/rangeslider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/select.py` & `pynecone-0.1.23a0/pynecone/components/forms/select.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/slider.py` & `pynecone-0.1.23a0/pynecone/components/forms/slider.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/switch.py` & `pynecone-0.1.23a0/pynecone/components/forms/switch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/textarea.py` & `pynecone-0.1.23a0/pynecone/components/forms/textarea.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/forms/upload.py` & `pynecone-0.1.23a0/pynecone/components/forms/upload.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/graphing/plotly.py` & `pynecone-0.1.23a0/pynecone/components/graphing/plotly.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/graphing/victory.py` & `pynecone-0.1.23a0/pynecone/components/graphing/victory.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/layout/__init__.py` & `pynecone-0.1.23a0/pynecone/components/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/layout/box.py` & `pynecone-0.1.23a0/pynecone/components/layout/box.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/layout/cond.py` & `pynecone-0.1.23a0/pynecone/components/layout/cond.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/layout/flex.py` & `pynecone-0.1.23a0/pynecone/components/layout/flex.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/layout/foreach.py` & `pynecone-0.1.23a0/pynecone/components/layout/foreach.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/layout/grid.py` & `pynecone-0.1.23a0/pynecone/components/layout/grid.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/layout/html.py` & `pynecone-0.1.23a0/pynecone/components/layout/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/layout/responsive.py` & `pynecone-0.1.23a0/pynecone/components/layout/responsive.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/layout/stack.py` & `pynecone-0.1.23a0/pynecone/components/layout/stack.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/layout/wrap.py` & `pynecone-0.1.23a0/pynecone/components/layout/wrap.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/media/avatar.py` & `pynecone-0.1.23a0/pynecone/components/media/avatar.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/media/icon.py` & `pynecone-0.1.23a0/pynecone/components/media/icon.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/media/image.py` & `pynecone-0.1.23a0/pynecone/components/media/image.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/navigation/breadcrumb.py` & `pynecone-0.1.23a0/pynecone/components/navigation/breadcrumb.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/navigation/link.py` & `pynecone-0.1.23a0/pynecone/components/navigation/link.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/navigation/linkoverlay.py` & `pynecone-0.1.23a0/pynecone/components/navigation/linkoverlay.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/overlay/__init__.py` & `pynecone-0.1.23a0/pynecone/components/overlay/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/overlay/alertdialog.py` & `pynecone-0.1.23a0/pynecone/components/overlay/alertdialog.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/overlay/drawer.py` & `pynecone-0.1.23a0/pynecone/components/overlay/drawer.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/overlay/menu.py` & `pynecone-0.1.23a0/pynecone/components/overlay/menu.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/overlay/modal.py` & `pynecone-0.1.23a0/pynecone/components/overlay/modal.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/overlay/popover.py` & `pynecone-0.1.23a0/pynecone/components/overlay/popover.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/overlay/tooltip.py` & `pynecone-0.1.23a0/pynecone/components/overlay/tooltip.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/tags/cond_tag.py` & `pynecone-0.1.23a0/pynecone/components/tags/cond_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/tags/iter_tag.py` & `pynecone-0.1.23a0/pynecone/components/tags/iter_tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/tags/tag.py` & `pynecone-0.1.23a0/pynecone/components/tags/tag.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/tags/tagless.py` & `pynecone-0.1.23a0/pynecone/components/tags/tagless.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/components/typography/markdown.py` & `pynecone-0.1.23a0/pynecone/components/typography/markdown.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/config.py` & `pynecone-0.1.23a0/pynecone/config.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/constants.py` & `pynecone-0.1.23a0/pynecone/constants.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/el/constants/html.py` & `pynecone-0.1.23a0/pynecone/el/constants/html.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/el/constants/pynecone.py` & `pynecone-0.1.23a0/pynecone/el/constants/pynecone.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/el/constants/react.py` & `pynecone-0.1.23a0/pynecone/el/constants/react.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/el/element.py` & `pynecone-0.1.23a0/pynecone/el/element.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/el/elements/__init__.py` & `pynecone-0.1.23a0/pynecone/el/elements/__init__.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/el/precompile.py` & `pynecone-0.1.23a0/pynecone/el/precompile.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/event.py` & `pynecone-0.1.23a0/pynecone/event.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/middleware/hydrate_middleware.py` & `pynecone-0.1.23a0/pynecone/middleware/hydrate_middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/middleware/logging_middleware.py` & `pynecone-0.1.23a0/pynecone/middleware/logging_middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/middleware/middleware.py` & `pynecone-0.1.23a0/pynecone/middleware/middleware.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/model.py` & `pynecone-0.1.23a0/pynecone/model.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/pc.py` & `pynecone-0.1.23a0/pynecone/pc.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/route.py` & `pynecone-0.1.23a0/pynecone/route.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/state.py` & `pynecone-0.1.23a0/pynecone/state.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/style.py` & `pynecone-0.1.23a0/pynecone/style.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/telemetry.py` & `pynecone-0.1.23a0/pynecone/telemetry.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/utils/build.py` & `pynecone-0.1.23a0/pynecone/utils/build.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/utils/console.py` & `pynecone-0.1.23a0/pynecone/utils/console.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/utils/exec.py` & `pynecone-0.1.23a0/pynecone/utils/exec.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/utils/format.py` & `pynecone-0.1.23a0/pynecone/utils/format.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/utils/imports.py` & `pynecone-0.1.23a0/pynecone/utils/imports.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/utils/path_ops.py` & `pynecone-0.1.23a0/pynecone/utils/path_ops.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/utils/prerequisites.py` & `pynecone-0.1.23a0/pynecone/utils/prerequisites.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,32 +37,29 @@
         version = result.stdout.decode().strip().split("v")[1]
         # Compare the version numbers
         return version.split(".") >= min_version.split(".")
     except Exception:
         return False
 
 
-def get_bun_version() -> str:
+def get_bun_version() -> Optional[str]:
     """Get the version of bun.
 
     Returns:
         The version of bun.
-
-    Raises:
-        FileNotFoundError: If bun is not installed.
     """
     try:
         # Run the bun -v command and capture the output
         result = subprocess.run(
             ["bun", "-v"], stdout=subprocess.PIPE, stderr=subprocess.PIPE
         )
         version = result.stdout.decode().strip()
         return version
     except Exception:
-        raise FileNotFoundError("Pynecone requires bun to be installed.") from None
+        return None
 
 
 def get_package_manager() -> str:
     """Get the package manager executable.
 
     Returns:
         The path to the package manager.
@@ -210,17 +207,18 @@
 
 def install_bun():
     """Install bun onto the user's system.
 
     Raises:
         FileNotFoundError: If the required packages are not installed.
     """
-    if get_bun_version() in constants.INVALID_BUN_VERSIONS:
+    bun_version = get_bun_version()
+    if bun_version is not None and bun_version in constants.INVALID_BUN_VERSIONS:
         console.print(
-            f"[red]Bun version {get_bun_version()} is not supported by Pynecone. Please downgrade to bun version {constants.MIN_BUN_VERSION} or upgrade to {constants.MAX_BUN_VERSION} or higher."
+            f"[red]Bun version {bun_version} is not supported by Pynecone. Please downgrade to bun version {constants.MIN_BUN_VERSION} or upgrade to {constants.MAX_BUN_VERSION} or higher."
         )
         return
 
     # Bun is not supported on Windows.
     if platform.system() == "Windows":
         console.log("Skipping bun installation on Windows.")
         return
```

### Comparing `pynecone-0.1.22a0/pynecone/utils/processes.py` & `pynecone-0.1.23a0/pynecone/utils/processes.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/utils/types.py` & `pynecone-0.1.23a0/pynecone/utils/types.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/var.py` & `pynecone-0.1.23a0/pynecone/var.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pynecone/watch.py` & `pynecone-0.1.23a0/pynecone/watch.py`

 * *Files identical despite different names*

### Comparing `pynecone-0.1.22a0/pyproject.toml` & `pynecone-0.1.23a0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pynecone"
-version = "0.1.22a"
+version = "0.1.23a0"
 description = "Web apps in pure Python."
 license = "Apache-2.0"
 authors = [
     "Nikhil Rao <nikhil@pynecone.io>",
     "Alek Petuskey <alek@pynecone.io>",
 ]
 readme = "README.md"
```

### Comparing `pynecone-0.1.22a0/PKG-INFO` & `pynecone-0.1.23a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynecone
-Version: 0.1.22a0
+Version: 0.1.23a0
 Summary: Web apps in pure Python.
 Home-page: https://pynecone.io
 License: Apache-2.0
 Keywords: web,framework
 Author: Nikhil Rao
 Author-email: nikhil@pynecone.io
 Requires-Python: >=3.7,<4.0
```

