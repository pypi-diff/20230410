# Comparing `tmp/prettyqt-1.0.0.tar.gz` & `tmp/prettyqt-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettyqt-1.0.0.tar", max compression
+gzip compressed data, was "prettyqt-1.1.0.tar", max compression
```

## Comparing `prettyqt-1.0.0.tar` & `prettyqt-1.1.0.tar`

### file list

```diff
@@ -1,744 +1,744 @@
--rw-r--r--   0        0        0     1078 2023-04-07 02:23:06.195781 prettyqt-1.0.0/LICENSE
--rw-r--r--   0        0        0     2875 2023-04-07 02:23:06.195781 prettyqt-1.0.0/docs/index.md
--rw-r--r--   0        0        0      687 2023-04-07 02:23:06.195781 prettyqt-1.0.0/prettyqt/__init__.py
--rw-r--r--   0        0        0      122 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/__pyinstaller/__init__.py
--rw-r--r--   0        0        0      860 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/__pyinstaller/hook-prettyqt.py
--rw-r--r--   0        0        0      517 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/bluetooth/__init__.py
--rw-r--r--   0        0        0      334 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/bluetooth/bluetoothaddress.py
--rw-r--r--   0        0        0     2649 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/bluetooth/bluetoothdevicediscoveryagent.py
--rw-r--r--   0        0        0     1421 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/bluetooth/bluetoothservicediscoveryagent.py
--rw-r--r--   0        0        0     1872 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/bluetooth/bluetoothserviceinfo.py
--rw-r--r--   0        0        0    11927 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/bluetooth/bluetoothuuid.py
--rw-r--r--   0        0        0     1792 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/__init__.py
--rw-r--r--   0        0        0     2245 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/abstractaxis.py
--rw-r--r--   0        0        0     1603 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/abstractbarseries.py
--rw-r--r--   0        0        0      554 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/abstractseries.py
--rw-r--r--   0        0        0      517 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/barcategoryaxis.py
--rw-r--r--   0        0        0      177 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/barseries.py
--rw-r--r--   0        0        0      932 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/barset.py
--rw-r--r--   0        0        0     1692 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/boxset.py
--rw-r--r--   0        0        0      609 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/candlestickset.py
--rw-r--r--   0        0        0     1767 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/categoryaxis.py
--rw-r--r--   0        0        0     5315 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/chart.py
--rw-r--r--   0        0        0     5622 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/chartview.py
--rw-r--r--   0        0        0      381 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/datetimeaxis.py
--rw-r--r--   0        0        0      197 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/horizontalbarseries.py
--rw-r--r--   0        0        0      217 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/horizontalpercentbarseries.py
--rw-r--r--   0        0        0      217 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/horizontalstackedbarseries.py
--rw-r--r--   0        0        0     2742 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/legend.py
--rw-r--r--   0        0        0      645 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/lineseries.py
--rw-r--r--   0        0        0      178 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/logvalueaxis.py
--rw-r--r--   0        0        0      191 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/percentbarseries.py
--rw-r--r--   0        0        0     2038 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/pieslice.py
--rw-r--r--   0        0        0      739 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/polarchart.py
--rw-r--r--   0        0        0      176 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/scatterseries.py
--rw-r--r--   0        0        0      191 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/stackedbarseries.py
--rw-r--r--   0        0        0     1044 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/valueaxis.py
--rw-r--r--   0        0        0     1219 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/charts/xyseries.py
--rw-r--r--   0        0        0    34636 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/constants/__init__.py
--rw-r--r--   0        0        0     9001 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/__init__.py
--rw-r--r--   0        0        0     1098 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/_calendar.py
--rw-r--r--   0        0        0     2000 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/_datetime.py
--rw-r--r--   0        0        0      478 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/_time.py
--rw-r--r--   0        0        0     3286 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/abstractanimation.py
--rw-r--r--   0        0        0      186 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/abstracteventdispatcher.py
--rw-r--r--   0        0        0     5354 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/abstractitemmodel.py
--rw-r--r--   0        0        0      250 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/abstractlistmodel.py
--rw-r--r--   0        0        0      146 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/abstractnativeeventfilter.py
--rw-r--r--   0        0        0      254 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/abstractproxymodel.py
--rw-r--r--   0        0        0      254 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/abstracttablemodel.py
--rw-r--r--   0        0        0     2060 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/animationgroup.py
--rw-r--r--   0        0        0      533 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/basictimer.py
--rw-r--r--   0        0        0      154 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/buffer.py
--rw-r--r--   0        0        0      173 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/bytearray.py
--rw-r--r--   0        0        0      369 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/bytearraymatcher.py
--rw-r--r--   0        0        0      959 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/collator.py
--rw-r--r--   0        0        0      126 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/collatorsortkey.py
--rw-r--r--   0        0        0      324 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/commandlineoption.py
--rw-r--r--   0        0        0     2231 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/commandlineparser.py
--rw-r--r--   0        0        0      211 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/concatenatetablesproxymodel.py
--rw-r--r--   0        0        0     3940 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/coreapplication.py
--rw-r--r--   0        0        0     2038 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/cryptographichash.py
--rw-r--r--   0        0        0     3426 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/datastream.py
--rw-r--r--   0        0        0      470 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/date.py
--rw-r--r--   0        0        0      766 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/deadlinetimer.py
--rw-r--r--   0        0        0     1153 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/debug.py
--rw-r--r--   0        0        0     4369 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/dir.py
--rw-r--r--   0        0        0      264 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/diriterator.py
--rw-r--r--   0        0        0     4500 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/easingcurve.py
--rw-r--r--   0        0        0      918 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/elapsedtimer.py
--rw-r--r--   0        0        0     7128 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/event.py
--rw-r--r--   0        0        0     1225 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/eventloop.py
--rw-r--r--   0        0        0      191 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/file.py
--rw-r--r--   0        0        0     3694 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/filedevice.py
--rw-r--r--   0        0        0     1492 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/fileinfo.py
--rw-r--r--   0        0        0      560 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/fileselector.py
--rw-r--r--   0        0        0      879 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/filesystemwatcher.py
--rw-r--r--   0        0        0      188 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/identityproxymodel.py
--rw-r--r--   0        0        0     1485 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/iodevice.py
--rw-r--r--   0        0        0      122 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/itemselection.py
--rw-r--r--   0        0        0      176 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/itemselectionmodel.py
--rw-r--r--   0        0        0      696 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/itemselectionrange.py
--rw-r--r--   0        0        0     1661 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/jsondocument.py
--rw-r--r--   0        0        0      538 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/jsonvalue.py
--rw-r--r--   0        0        0     1248 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/library.py
--rw-r--r--   0        0        0     1692 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/libraryinfo.py
--rw-r--r--   0        0        0     1868 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/line.py
--rw-r--r--   0        0        0     1997 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/linef.py
--rw-r--r--   0        0        0    16492 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/locale.py
--rw-r--r--   0        0        0      810 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/lockfile.py
--rw-r--r--   0        0        0      708 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/margins.py
--rw-r--r--   0        0        0      713 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/marginsf.py
--rw-r--r--   0        0        0     1110 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/metaenum.py
--rw-r--r--   0        0        0     1423 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/metamethod.py
--rw-r--r--   0        0        0     3703 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/metaobject.py
--rw-r--r--   0        0        0      511 2023-04-07 02:23:06.199781 prettyqt-1.0.0/prettyqt/core/metaproperty.py
--rw-r--r--   0        0        0     1802 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/mimedata.py
--rw-r--r--   0        0        0      948 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/mimedatabase.py
--rw-r--r--   0        0        0      208 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/mimetype.py
--rw-r--r--   0        0        0      176 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/modelindex.py
--rw-r--r--   0        0        0      336 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/mutex.py
--rw-r--r--   0        0        0     3583 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/object.py
--rw-r--r--   0        0        0     2562 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/operatingsystemversion.py
--rw-r--r--   0        0        0      356 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/parallelanimationgroup.py
--rw-r--r--   0        0        0      253 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/pauseanimation.py
--rw-r--r--   0        0        0      338 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/persistentmodelindex.py
--rw-r--r--   0        0        0      811 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/pluginloader.py
--rw-r--r--   0        0        0      349 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/point.py
--rw-r--r--   0        0        0      353 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/pointf.py
--rw-r--r--   0        0        0     4839 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/process.py
--rw-r--r--   0        0        0     1340 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/processenvironment.py
--rw-r--r--   0        0        0      774 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/propertyanimation.py
--rw-r--r--   0        0        0      126 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/randomgenerator.py
--rw-r--r--   0        0        0      231 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/randomgenerator64.py
--rw-r--r--   0        0        0      878 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/rect.py
--rw-r--r--   0        0        0      442 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/rectf.py
--rw-r--r--   0        0        0     6515 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/regularexpression.py
--rw-r--r--   0        0        0     2579 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/regularexpressionmatch.py
--rw-r--r--   0        0        0      613 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/regularexpressionmatchiterator.py
--rw-r--r--   0        0        0     1702 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/resource.py
--rw-r--r--   0        0        0      112 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/runnable.py
--rw-r--r--   0        0        0      160 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/savefile.py
--rw-r--r--   0        0        0      281 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/semaphore.py
--rw-r--r--   0        0        0      202 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/sequentialanimationgroup.py
--rw-r--r--   0        0        0     6990 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/settings.py
--rw-r--r--   0        0        0      122 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/signalblocker.py
--rw-r--r--   0        0        0      451 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/signalmapper.py
--rw-r--r--   0        0        0     1124 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/size.py
--rw-r--r--   0        0        0     1142 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/sizef.py
--rw-r--r--   0        0        0      471 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/slot.py
--rw-r--r--   0        0        0      930 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/socketnotifier.py
--rw-r--r--   0        0        0     2681 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/sortfilterproxymodel.py
--rw-r--r--   0        0        0     2622 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/standardpaths.py
--rw-r--r--   0        0        0     1184 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/storageinfo.py
--rw-r--r--   0        0        0      339 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/stringlistmodel.py
--rw-r--r--   0        0        0      980 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/temporarydir.py
--rw-r--r--   0        0        0      164 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/temporaryfile.py
--rw-r--r--   0        0        0     2583 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/textboundaryfinder.py
--rw-r--r--   0        0        0     3862 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/textstream.py
--rw-r--r--   0        0        0      108 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/thread.py
--rw-r--r--   0        0        0      160 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/threadpool.py
--rw-r--r--   0        0        0     2291 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/timeline.py
--rw-r--r--   0        0        0     1761 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/timer.py
--rw-r--r--   0        0        0     2076 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/timezone.py
--rw-r--r--   0        0        0     1722 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/translator.py
--rw-r--r--   0        0        0      190 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/transposeproxymodel.py
--rw-r--r--   0        0        0     3968 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/url.py
--rw-r--r--   0        0        0      770 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/urlquery.py
--rw-r--r--   0        0        0     1837 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/uuid.py
--rw-r--r--   0        0        0     1519 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/variantanimation.py
--rw-r--r--   0        0        0     2614 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/versionnumber.py
--rw-r--r--   0        0        0     2614 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/core/xmlstreamreader.py
--rw-r--r--   0        0        0      253 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_animations/__init__.py
--rw-r--r--   0        0        0     1579 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_animations/bounceanimation.py
--rw-r--r--   0        0        0      644 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_animations/fadeinanimation.py
--rw-r--r--   0        0        0      978 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_animations/slideanimation.py
--rw-r--r--   0        0        0      535 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_delegates/__init__.py
--rw-r--r--   0        0        0      887 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_delegates/buttondelegate.py
--rw-r--r--   0        0        0     1001 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_delegates/checkboxdelegate.py
--rw-r--r--   0        0        0     2556 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_delegates/icondelegate.py
--rw-r--r--   0        0        0      596 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_delegates/nofocusdelegate.py
--rw-r--r--   0        0        0     1474 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_delegates/progressbardelegate.py
--rw-r--r--   0        0        0     4731 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_delegates/radiodelegate.py
--rw-r--r--   0        0        0     2574 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_delegates/renderlinkdelegate.py
--rw-r--r--   0        0        0     6634 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_delegates/stardelegate.py
--rw-r--r--   0        0        0      735 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_models/__init__.py
--rw-r--r--   0        0        0     5921 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_models/columnitemmodel.py
--rw-r--r--   0        0        0     3585 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_models/importlibdistributionmodel.py
--rw-r--r--   0        0        0     4214 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_models/jsonmodel.py
--rw-r--r--   0        0        0     3099 2023-04-07 02:23:06.203781 prettyqt-1.0.0/prettyqt/custom_models/listmixin.py
--rw-r--r--   0        0        0     2553 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_models/modelmixin.py
--rw-r--r--   0        0        0     2298 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_models/nesteditem.py
--rw-r--r--   0        0        0     2177 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_models/nestedmodel.py
--rw-r--r--   0        0        0     2114 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_models/regexmatchesmodel.py
--rw-r--r--   0        0        0     1689 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_models/selectionmixin.py
--rw-r--r--   0        0        0     5230 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_models/storageinfomodel.py
--rw-r--r--   0        0        0     2858 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_models/subsequencesortfilterproxymodel.py
--rw-r--r--   0        0        0      635 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_validators/__init__.py
--rw-r--r--   0        0        0     2060 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_validators/compositevalidator.py
--rw-r--r--   0        0        0     1114 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_validators/integervalidator.py
--rw-r--r--   0        0        0      704 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_validators/notemptyvalidator.py
--rw-r--r--   0        0        0      700 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_validators/notzerovalidator.py
--rw-r--r--   0        0        0      620 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_validators/pathvalidator.py
--rw-r--r--   0        0        0     1554 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_validators/regexpatternvalidator.py
--rw-r--r--   0        0        0     3143 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_validators/regexvalidators.py
--rw-r--r--   0        0        0     2704 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/__init__.py
--rw-r--r--   0        0        0     1638 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/booldicttoolbutton.py
--rw-r--r--   0        0        0     7588 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/borderlayout.py
--rw-r--r--   0        0        0     3046 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/codeeditor.py
--rw-r--r--   0        0        0     2588 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/collapsibleframe.py
--rw-r--r--   0        0        0     2468 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/colorchooserbutton.py
--rw-r--r--   0        0        0     7429 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/completionwidget.py
--rw-r--r--   0        0        0    17651 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/dataset.py
--rw-r--r--   0        0        0     2219 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/elidedlabel.py
--rw-r--r--   0        0        0     3429 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/expandableline.py
--rw-r--r--   0        0        0     3194 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/filechooserbutton.py
--rw-r--r--   0        0        0     2155 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/flagselectionwidget.py
--rw-r--r--   0        0        0     3847 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/flowlayout.py
--rw-r--r--   0        0        0     2156 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/fontchooserbutton.py
--rw-r--r--   0        0        0     9168 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/framelesswindow.py
--rw-r--r--   0        0        0     5371 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/iconbrowser.py
--rw-r--r--   0        0        0     1311 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/iconlabel.py
--rw-r--r--   0        0        0     1661 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/iconwidget.py
--rw-r--r--   0        0        0     1292 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/image.py
--rw-r--r--   0        0        0      644 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/imageviewer.py
--rw-r--r--   0        0        0     1931 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/inputandslider.py
--rw-r--r--   0        0        0     2106 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/joystickbutton.py
--rw-r--r--   0        0        0     4175 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/labeledslider.py
--rw-r--r--   0        0        0     1214 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/listinput.py
--rw-r--r--   0        0        0     8209 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/logtextedit.py
--rw-r--r--   0        0        0      738 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/mappedcheckbox.py
--rw-r--r--   0        0        0     2388 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/markdownwidget.py
--rw-r--r--   0        0        0     6576 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/menurecentfiles.py
--rw-r--r--   0        0        0    18758 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/notification.py
--rw-r--r--   0        0        0     1038 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/optionalwidget.py
--rw-r--r--   0        0        0     1332 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/popupinfo.py
--rw-r--r--   0        0        0      145 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/regexeditor/__init__.py
--rw-r--r--   0        0        0      431 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/regexeditor/__main__.py
--rw-r--r--   0        0        0     1039 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/regexeditor/quick_ref.py
--rw-r--r--   0        0        0    19388 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/regexeditor/ref.html
--rw-r--r--   0        0        0     6186 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/regexeditor/regexeditorwidget.py
--rw-r--r--   0        0        0     3110 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/regexinput.py
--rw-r--r--   0        0        0    10458 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/roundprogressbar.py
--rw-r--r--   0        0        0     4250 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/selectionwidget.py
--rw-r--r--   0        0        0     6318 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/sidebarwidget.py
--rw-r--r--   0        0        0     1036 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/singlelinetextedit.py
--rw-r--r--   0        0        0    18587 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/spanslider.py
--rw-r--r--   0        0        0     1286 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/standardiconswidget.py
--rw-r--r--   0        0        0     2289 2023-04-07 02:23:06.207780 prettyqt-1.0.0/prettyqt/custom_widgets/stringornumberwidget.py
--rw-r--r--   0        0        0     1774 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/custom_widgets/subsequencecompleter.py
--rw-r--r--   0        0        0     8034 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/custom_widgets/timeline.py
--rw-r--r--   0        0        0     9009 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/custom_widgets/waitingspinner.py
--rw-r--r--   0        0        0      255 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/eventfilters/__init__.py
--rw-r--r--   0        0        0     2485 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/eventfilters/animatedtooltipeventfilter.py
--rw-r--r--   0        0        0      751 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/eventfilters/hovericoneventfilter.py
--rw-r--r--   0        0        0     7619 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/__init__.py
--rw-r--r--   0        0        0     1269 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/abstracttextdocumentlayout.py
--rw-r--r--   0        0        0      235 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/bitmap.py
--rw-r--r--   0        0        0      979 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/brush.py
--rw-r--r--   0        0        0     2490 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/clipboard.py
--rw-r--r--   0        0        0     6681 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/color.py
--rw-r--r--   0        0        0     3045 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/colorspace.py
--rw-r--r--   0        0        0      485 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/conicalgradient.py
--rw-r--r--   0        0        0     1255 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/cursor.py
--rw-r--r--   0        0        0      439 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/desktopservices.py
--rw-r--r--   0        0        0     1094 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/doublevalidator.py
--rw-r--r--   0        0        0      973 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/drag.py
--rw-r--r--   0        0        0     9049 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/font.py
--rw-r--r--   0        0        0     4694 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/fontdatabase.py
--rw-r--r--   0        0        0      243 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/fontinfo.py
--rw-r--r--   0        0        0      878 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/fontmetrics.py
--rw-r--r--   0        0        0      719 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/fontmetricsf.py
--rw-r--r--   0        0        0     5331 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/gradient.py
--rw-r--r--   0        0        0     5027 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/guiapplication.py
--rw-r--r--   0        0        0     3970 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/icon.py
--rw-r--r--   0        0        0     4053 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/iconengine.py
--rw-r--r--   0        0        0     1260 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/image.py
--rw-r--r--   0        0        0     3778 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/imageiohandler.py
--rw-r--r--   0        0        0     3838 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/imagereader.py
--rw-r--r--   0        0        0     2791 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/imagewriter.py
--rw-r--r--   0        0        0     1315 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/inputmethod.py
--rw-r--r--   0        0        0      921 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/intvalidator.py
--rw-r--r--   0        0        0     6168 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/keysequence.py
--rw-r--r--   0        0        0      636 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/lineargradient.py
--rw-r--r--   0        0        0      302 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/matrix4x4.py
--rw-r--r--   0        0        0     1969 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/movie.py
--rw-r--r--   0        0        0      297 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/pagedpaintdevice.py
--rw-r--r--   0        0        0     2923 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/pagelayout.py
--rw-r--r--   0        0        0     7838 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/pagesize.py
--rw-r--r--   0        0        0     1676 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/paintdevice.py
--rw-r--r--   0        0        0      319 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/paintdevicewindow.py
--rw-r--r--   0        0        0     7557 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/painter.py
--rw-r--r--   0        0        0     2425 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/painterpath.py
--rw-r--r--   0        0        0     1641 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/painterpathstroker.py
--rw-r--r--   0        0        0     5859 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/palette.py
--rw-r--r--   0        0        0     1026 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/pdfwriter.py
--rw-r--r--   0        0        0     2841 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/pen.py
--rw-r--r--   0        0        0      471 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/picture.py
--rw-r--r--   0        0        0     4827 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/pixmap.py
--rw-r--r--   0        0        0      796 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/pixmapcache.py
--rw-r--r--   0        0        0     3489 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/polygon.py
--rw-r--r--   0        0        0     4325 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/polygonf.py
--rw-r--r--   0        0        0      898 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/radialgradient.py
--rw-r--r--   0        0        0      233 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/rasterwindow.py
--rw-r--r--   0        0        0     1145 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/region.py
--rw-r--r--   0        0        0     1290 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/regularexpressionvalidator.py
--rw-r--r--   0        0        0     2963 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/screen.py
--rw-r--r--   0        0        0     1291 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/sessionmanager.py
--rw-r--r--   0        0        0     6188 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/standarditem.py
--rw-r--r--   0        0        0     4758 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/standarditemmodel.py
--rw-r--r--   0        0        0     2225 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/statictext.py
--rw-r--r--   0        0        0     1303 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/surface.py
--rw-r--r--   0        0        0     1352 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/syntaxhighlighter.py
--rw-r--r--   0        0        0     5251 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/textblock.py
--rw-r--r--   0        0        0      623 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/textblockgroup.py
--rw-r--r--   0        0        0      536 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/textblockuserdata.py
--rw-r--r--   0        0        0     4878 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/textcharformat.py
--rw-r--r--   0        0        0     5551 2023-04-07 02:23:06.211781 prettyqt-1.0.0/prettyqt/gui/textcursor.py
--rw-r--r--   0        0        0     7781 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/textdocument.py
--rw-r--r--   0        0        0      949 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/textdocumentfragment.py
--rw-r--r--   0        0        0     1062 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/textdocumentwriter.py
--rw-r--r--   0        0        0     3262 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/textformat.py
--rw-r--r--   0        0        0      534 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/textframe.py
--rw-r--r--   0        0        0     3627 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/textframeformat.py
--rw-r--r--   0        0        0      297 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/textimageformat.py
--rw-r--r--   0        0        0      517 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/textlayout.py
--rw-r--r--   0        0        0      725 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/textlength.py
--rw-r--r--   0        0        0     1649 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/textline.py
--rw-r--r--   0        0        0     1327 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/textlistformat.py
--rw-r--r--   0        0        0      445 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/textobject.py
--rw-r--r--   0        0        0      199 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/textobjectinterface.py
--rw-r--r--   0        0        0     1560 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/textoption.py
--rw-r--r--   0        0        0     4104 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/texttablecellformat.py
--rw-r--r--   0        0        0     2605 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/transform.py
--rw-r--r--   0        0        0      755 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/validator.py
--rw-r--r--   0        0        0      575 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/vector3d.py
--rw-r--r--   0        0        0      578 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/vector4d.py
--rw-r--r--   0        0        0     2338 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/gui/window.py
--rw-r--r--   0        0        0    10227 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/iconprovider/__init__.py
--rw-r--r--   0        0        0     1387 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/iconprovider/animation.py
--rw-r--r--   0        0        0     3059 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/iconprovider/awesomefileiconprovider.py
--rw-r--r--   0        0        0      539 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/iconprovider/awesomequickimageprovider.py
--rw-r--r--   0        0        0      832 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/iconprovider/chariconengine.py
--rw-r--r--   0        0        0    10996 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/codicon-charmap.json
--rw-r--r--   0        0        0    68076 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/codicon.ttf
--rw-r--r--   0        0        0     7924 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/elusiveicons-webfont-charmap.json
--rw-r--r--   0        0        0    79556 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/elusiveicons-webfont.ttf
--rw-r--r--   0        0        0    11206 2023-04-07 02:23:06.215781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont-charmap.json
--rw-r--r--   0        0        0   134316 2023-04-07 02:23:06.219781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont.ttf
--rw-r--r--   0        0        0     3947 2023-04-07 02:23:06.219781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont-charmap.json
--rw-r--r--   0        0        0    33692 2023-04-07 02:23:06.219781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont.ttf
--rw-r--r--   0        0        0    25663 2023-04-07 02:23:06.219781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont-charmap.json
--rw-r--r--   0        0        0   203644 2023-04-07 02:23:06.219781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont.ttf
--rw-r--r--   0        0        0   200215 2023-04-07 02:23:06.223781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont-charmap.json
--rw-r--r--   0        0        0  1026284 2023-04-07 02:23:06.231781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont.ttf
--rw-r--r--   0        0        0   216192 2023-04-07 02:23:06.231781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont-charmap.json
--rw-r--r--   0        0        0  1108672 2023-04-07 02:23:06.235781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont.ttf
--rw-r--r--   0        0        0   151941 2023-04-07 02:23:06.235781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/phosphor-charmap.json
--rw-r--r--   0        0        0  1392088 2023-04-07 02:23:06.243781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/phosphor.ttf
--rw-r--r--   0        0        0    72655 2023-04-07 02:23:06.247781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/remixicon-charmap.json
--rw-r--r--   0        0        0   403056 2023-04-07 02:23:06.247781 prettyqt-1.0.0/prettyqt/iconprovider/fonts/remixicon.ttf
--rw-r--r--   0        0        0     8417 2023-04-07 02:23:06.247781 prettyqt-1.0.0/prettyqt/iconprovider/iconic_font.py
--rw-r--r--   0        0        0     2468 2023-04-07 02:23:06.247781 prettyqt-1.0.0/prettyqt/iconprovider/svgbuffericonengine.py
--rw-r--r--   0        0        0   154232 2023-04-07 02:23:06.251781 prettyqt-1.0.0/prettyqt/localization/language_ar.qm
--rw-r--r--   0        0        0   155315 2023-04-07 02:23:06.251781 prettyqt-1.0.0/prettyqt/localization/language_bg.qm
--rw-r--r--   0        0        0   178552 2023-04-07 02:23:06.251781 prettyqt-1.0.0/prettyqt/localization/language_ca.qm
--rw-r--r--   0        0        0   151054 2023-04-07 02:23:06.251781 prettyqt-1.0.0/prettyqt/localization/language_cs.qm
--rw-r--r--   0        0        0   179910 2023-04-07 02:23:06.251781 prettyqt-1.0.0/prettyqt/localization/language_da.qm
--rw-r--r--   0        0        0   212675 2023-04-07 02:23:06.255781 prettyqt-1.0.0/prettyqt/localization/language_de.qm
--rw-r--r--   0        0        0   154543 2023-04-07 02:23:06.255781 prettyqt-1.0.0/prettyqt/localization/language_es.qm
--rw-r--r--   0        0        0    97872 2023-04-07 02:23:06.255781 prettyqt-1.0.0/prettyqt/localization/language_fa.qm
--rw-r--r--   0        0        0   174500 2023-04-07 02:23:06.255781 prettyqt-1.0.0/prettyqt/localization/language_fi.qm
--rw-r--r--   0        0        0   154190 2023-04-07 02:23:06.259781 prettyqt-1.0.0/prettyqt/localization/language_fr.qm
--rw-r--r--   0        0        0   183091 2023-04-07 02:23:06.259781 prettyqt-1.0.0/prettyqt/localization/language_gd.qm
--rw-r--r--   0        0        0   108600 2023-04-07 02:23:06.259781 prettyqt-1.0.0/prettyqt/localization/language_gl.qm
--rw-r--r--   0        0        0   130568 2023-04-07 02:23:06.259781 prettyqt-1.0.0/prettyqt/localization/language_he.qm
--rw-r--r--   0        0        0   150033 2023-04-07 02:23:06.263781 prettyqt-1.0.0/prettyqt/localization/language_hu.qm
--rw-r--r--   0        0        0   153570 2023-04-07 02:23:06.263781 prettyqt-1.0.0/prettyqt/localization/language_it.qm
--rw-r--r--   0        0        0   122385 2023-04-07 02:23:06.263781 prettyqt-1.0.0/prettyqt/localization/language_ja.qm
--rw-r--r--   0        0        0   120318 2023-04-07 02:23:06.263781 prettyqt-1.0.0/prettyqt/localization/language_ko.qm
--rw-r--r--   0        0        0    90502 2023-04-07 02:23:06.267781 prettyqt-1.0.0/prettyqt/localization/language_lt.qm
--rw-r--r--   0        0        0   143558 2023-04-07 02:23:06.267781 prettyqt-1.0.0/prettyqt/localization/language_lv.qm
--rw-r--r--   0        0        0   161318 2023-04-07 02:23:06.267781 prettyqt-1.0.0/prettyqt/localization/language_pl.qm
--rw-r--r--   0        0        0    50541 2023-04-07 02:23:06.267781 prettyqt-1.0.0/prettyqt/localization/language_pt.qm
--rw-r--r--   0        0        0   197476 2023-04-07 02:23:06.267781 prettyqt-1.0.0/prettyqt/localization/language_ru.qm
--rw-r--r--   0        0        0   115250 2023-04-07 02:23:06.271781 prettyqt-1.0.0/prettyqt/localization/language_sk.qm
--rw-r--r--   0        0        0    96357 2023-04-07 02:23:06.271781 prettyqt-1.0.0/prettyqt/localization/language_sl.qm
--rw-r--r--   0        0        0    47206 2023-04-07 02:23:06.271781 prettyqt-1.0.0/prettyqt/localization/language_sv.qm
--rw-r--r--   0        0        0   148437 2023-04-07 02:23:06.271781 prettyqt-1.0.0/prettyqt/localization/language_uk.qm
--rw-r--r--   0        0        0    61089 2023-04-07 02:23:06.275781 prettyqt-1.0.0/prettyqt/localization/language_zh_CN.qm
--rw-r--r--   0        0        0   125250 2023-04-07 02:23:06.275781 prettyqt-1.0.0/prettyqt/localization/language_zh_TW.qm
--rw-r--r--   0        0        0     2384 2023-04-07 02:23:06.275781 prettyqt-1.0.0/prettyqt/location/__init__.py
--rw-r--r--   0        0        0      387 2023-04-07 02:23:06.275781 prettyqt-1.0.0/prettyqt/location/geocodingmanager.py
--rw-r--r--   0        0        0     2867 2023-04-07 02:23:06.275781 prettyqt-1.0.0/prettyqt/location/geomaneuver.py
--rw-r--r--   0        0        0     1055 2023-04-07 02:23:06.275781 prettyqt-1.0.0/prettyqt/location/georoute.py
--rw-r--r--   0        0        0     5266 2023-04-07 02:23:06.275781 prettyqt-1.0.0/prettyqt/location/georouterequest.py
--rw-r--r--   0        0        0      657 2023-04-07 02:23:06.275781 prettyqt-1.0.0/prettyqt/location/georoutesegment.py
--rw-r--r--   0        0        0     2021 2023-04-07 02:23:06.275781 prettyqt-1.0.0/prettyqt/location/georoutingmanager.py
--rw-r--r--   0        0        0     5880 2023-04-07 02:23:06.275781 prettyqt-1.0.0/prettyqt/location/geoserviceprovider.py
--rw-r--r--   0        0        0     2387 2023-04-07 02:23:06.275781 prettyqt-1.0.0/prettyqt/location/place.py
--rw-r--r--   0        0        0      864 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placeattribute.py
--rw-r--r--   0        0        0      737 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placecategory.py
--rw-r--r--   0        0        0      844 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placecontactdetail.py
--rw-r--r--   0        0        0     1030 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placecontent.py
--rw-r--r--   0        0        0     1275 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placecontentreply.py
--rw-r--r--   0        0        0      947 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placecontentrequest.py
--rw-r--r--   0        0        0      562 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placedetailsreply.py
--rw-r--r--   0        0        0      849 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placeicon.py
--rw-r--r--   0        0        0     1185 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placeidreply.py
--rw-r--r--   0        0        0     2233 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placemanager.py
--rw-r--r--   0        0        0     1066 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placematchreply.py
--rw-r--r--   0        0        0      726 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placematchrequest.py
--rw-r--r--   0        0        0      223 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placeproposedsearchresult.py
--rw-r--r--   0        0        0      316 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placeratings.py
--rw-r--r--   0        0        0     1923 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placereply.py
--rw-r--r--   0        0        0      267 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placeresult.py
--rw-r--r--   0        0        0     1651 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placesearchreply.py
--rw-r--r--   0        0        0     2230 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placesearchrequest.py
--rw-r--r--   0        0        0      884 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placesearchresult.py
--rw-r--r--   0        0        0      675 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placesupplier.py
--rw-r--r--   0        0        0      215 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/placeuser.py
--rw-r--r--   0        0        0      621 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/location/qlocation.py
--rw-r--r--   0        0        0      167 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/multimediawidgets/__init__.py
--rw-r--r--   0        0        0     1353 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/multimediawidgets/graphicsvideoitem.py
--rw-r--r--   0        0        0      872 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/multimediawidgets/videowidget.py
--rw-r--r--   0        0        0     1172 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/__init__.py
--rw-r--r--   0        0        0     8113 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/abstractsocket.py
--rw-r--r--   0        0        0     1775 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/hostaddress.py
--rw-r--r--   0        0        0     1465 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/httpmultipart.py
--rw-r--r--   0        0        0      823 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/httppart.py
--rw-r--r--   0        0        0     1310 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/localserver.py
--rw-r--r--   0        0        0     2392 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/localsocket.py
--rw-r--r--   0        0        0     2313 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/networkaccessmanager.py
--rw-r--r--   0        0        0     2000 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/networkaddressentry.py
--rw-r--r--   0        0        0     1551 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/networkcookie.py
--rw-r--r--   0        0        0      850 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/networkcookiejar.py
--rw-r--r--   0        0        0      627 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/networkdatagram.py
--rw-r--r--   0        0        0     3011 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/networkinterface.py
--rw-r--r--   0        0        0     3361 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/networkproxy.py
--rw-r--r--   0        0        0     6462 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/networkrequest.py
--rw-r--r--   0        0        0      779 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/tcpserver.py
--rw-r--r--   0        0        0      178 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/tcpsocket.py
--rw-r--r--   0        0        0      671 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/network/udpsocket.py
--rw-r--r--   0        0        0       26 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/objbrowser/__init__.py
--rw-r--r--   0        0        0     9184 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/objbrowser/attribute_model.py
--rw-r--r--   0        0        0    14897 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/objbrowser/objectbrowser.py
--rw-r--r--   0        0        0    17704 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/objbrowser/objectbrowsertreemodel.py
--rw-r--r--   0        0        0      356 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/paths.py
--rw-r--r--   0        0        0     1169 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/__init__.py
--rw-r--r--   0        0        0      171 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/geoaddress.py
--rw-r--r--   0        0        0     1157 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/geoareamonitorinfo.py
--rw-r--r--   0        0        0     1260 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/geoareamonitorsource.py
--rw-r--r--   0        0        0     1072 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/geocircle.py
--rw-r--r--   0        0        0     1172 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/geocoordinate.py
--rw-r--r--   0        0        0      706 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/geolocation.py
--rw-r--r--   0        0        0     1021 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/geopath.py
--rw-r--r--   0        0        0     1145 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/geopolygon.py
--rw-r--r--   0        0        0     1687 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/geopositioninfo.py
--rw-r--r--   0        0        0     2960 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/geopositioninfosource.py
--rw-r--r--   0        0        0      769 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/georectangle.py
--rw-r--r--   0        0        0     1861 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/geosatelliteinfo.py
--rw-r--r--   0        0        0     1110 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/geosatelliteinfosource.py
--rw-r--r--   0        0        0      755 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/geoshape.py
--rw-r--r--   0        0        0     1196 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/positioning/nmeapositioninginfosource.py
--rw-r--r--   0        0        0        0 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/py.typed
--rw-r--r--   0        0        0      943 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qml/__init__.py
--rw-r--r--   0        0        0     1212 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qml/jsengine.py
--rw-r--r--   0        0        0     2351 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qml/jsvalue.py
--rw-r--r--   0        0        0      295 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qml/jsvalueiterator.py
--rw-r--r--   0        0        0      955 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qml/qmlapplicationengine.py
--rw-r--r--   0        0        0      907 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qml/qmlcomponent.py
--rw-r--r--   0        0        0     2020 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qml/qmlengine.py
--rw-r--r--   0        0        0      536 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qml/qmlimageproviderbase.py
--rw-r--r--   0        0        0      185 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qml/qmlparserstatus.py
--rw-r--r--   0        0        0      251 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qt/Qsci/__init__.py
--rw-r--r--   0        0        0      268 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qt/QtBluetooth/__init__.py
--rw-r--r--   0        0        0      683 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qt/QtCharts/__init__.py
--rw-r--r--   0        0        0     3505 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qt/QtCore/__init__.py
--rw-r--r--   0        0        0      739 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qt/QtGui/__init__.py
--rw-r--r--   0        0        0      303 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qt/QtHelp/__init__.py
--rw-r--r--   0        0        0      335 2023-04-07 02:23:06.279781 prettyqt-1.0.0/prettyqt/qt/QtLocation/__init__.py
--rw-r--r--   0        0        0      327 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtMultimedia/__init__.py
--rw-r--r--   0        0        0      355 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtMultimediaWidgets/__init__.py
--rw-r--r--   0        0        0      331 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtNetwork/__init__.py
--rw-r--r--   0        0        0      331 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtPositioning/__init__.py
--rw-r--r--   0        0        0      315 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtQml/__init__.py
--rw-r--r--   0        0        0      323 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtQuick/__init__.py
--rw-r--r--   0        0        0      307 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtScxml/__init__.py
--rw-r--r--   0        0        0      601 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtStateMachine/__init__.py
--rw-r--r--   0        0        0      381 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtSvg/__init__.py
--rw-r--r--   0        0        0      319 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtTest/__init__.py
--rw-r--r--   0        0        0      213 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtTextToSpeech/__init__.py.old
--rw-r--r--   0        0        0      614 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtUiTools/__init__.py
--rw-r--r--   0        0        0      330 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtWebChannel/__init__.py
--rw-r--r--   0        0        0      715 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtWebEngineCore/__init__.py
--rw-r--r--   0        0        0      351 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtWebEngineWidgets/__init__.py
--rw-r--r--   0        0        0     1408 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/QtWidgets/__init__.py
--rw-r--r--   0        0        0     1431 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qt/__init__.py
--rw-r--r--   0        0        0      969 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qthelp/__init__.py
--rw-r--r--   0        0        0      271 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qthelp/helpcontentitem.py
--rw-r--r--   0        0        0      183 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qthelp/helpcontentmodel.py
--rw-r--r--   0        0        0      460 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qthelp/helpcontentwidget.py
--rw-r--r--   0        0        0      260 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qthelp/helpengine.py
--rw-r--r--   0        0        0      978 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qthelp/helpenginecore.py
--rw-r--r--   0        0        0      302 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qthelp/helpfilterengine.py
--rw-r--r--   0        0        0      177 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qthelp/helpindexmodel.py
--rw-r--r--   0        0        0      178 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qthelp/helpindexwidget.py
--rw-r--r--   0        0        0      442 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qthelp/helpsearchengine.py
--rw-r--r--   0        0        0      188 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qthelp/helpsearchquerywidget.py
--rw-r--r--   0        0        0      216 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qthelp/helpsearchresult.py
--rw-r--r--   0        0        0      403 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qthelp/helpsearchresultwidget.py
--rw-r--r--   0        0        0     8290 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/qtre.py
--rw-r--r--   0        0        0      868 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/quick/__init__.py
--rw-r--r--   0        0        0      208 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/quick/quickasyncimageprovider.py
--rw-r--r--   0        0        0      257 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/quick/quickimageprovider.py
--rw-r--r--   0        0        0      239 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/quick/quickimageresponse.py
--rw-r--r--   0        0        0     3753 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/quick/quickitem.py
--rw-r--r--   0        0        0      519 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/quick/quickitemgrabresult.py
--rw-r--r--   0        0        0     1495 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/quick/quickpainteditem.py
--rw-r--r--   0        0        0      239 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/quick/quickrendercontrol.py
--rw-r--r--   0        0        0      271 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/quick/quicktextdocument.py
--rw-r--r--   0        0        0     1204 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/quick/quickview.py
--rw-r--r--   0        0        0     3637 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/quick/quickwindow.py
--rw-r--r--   0        0        0      123 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/scintilla/__init__.py
--rw-r--r--   0        0        0     9347 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/scintilla/sciscintilla.py
--rw-r--r--   0        0        0      193 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/scxml/__init__.py
--rw-r--r--   0        0        0      362 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/scxml/scxmlcompiler.py
--rw-r--r--   0        0        0      176 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/scxml/scxmlstatemachine.py
--rw-r--r--   0        0        0      785 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/statemachine/__init__.py
--rw-r--r--   0        0        0      361 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/statemachine/abstractstate.py
--rw-r--r--   0        0        0     1159 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/statemachine/abstracttransition.py
--rw-r--r--   0        0        0      220 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/statemachine/eventtransition.py
--rw-r--r--   0        0        0      199 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/statemachine/finalstate.py
--rw-r--r--   0        0        0     1104 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/statemachine/historystate.py
--rw-r--r--   0        0        0      223 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/statemachine/keyeventtransition.py
--rw-r--r--   0        0        0      227 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/statemachine/mouseeventtransition.py
--rw-r--r--   0        0        0      222 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/statemachine/signaltransition.py
--rw-r--r--   0        0        0     1276 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/statemachine/state.py
--rw-r--r--   0        0        0     2222 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/statemachine/statemachine.py
--rw-r--r--   0        0        0      368 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/svg/__init__.py
--rw-r--r--   0        0        0      182 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/svg/graphicssvgitem.py
--rw-r--r--   0        0        0      405 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/svg/svggenerator.py
--rw-r--r--   0        0        0     1080 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/svg/svgrenderer.py
--rw-r--r--   0        0        0      279 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/svg/svgwidget.py
--rw-r--r--   0        0        0      675 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/syntaxhighlighters/__init__.py
--rw-r--r--   0        0        0     1236 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/syntaxhighlighters/highlightrule.py
--rw-r--r--   0        0        0     1271 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/syntaxhighlighters/jsonhighlighter.py
--rw-r--r--   0        0        0     3178 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/syntaxhighlighters/markdownhighlighter.py
--rw-r--r--   0        0        0      872 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/syntaxhighlighters/pygments/regularexpressionlexer.py
--rw-r--r--   0        0        0     8523 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/syntaxhighlighters/pygmentshighlighter.py
--rw-r--r--   0        0        0     4836 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/syntaxhighlighters/pythonhighlighter.py
--rw-r--r--   0        0        0     2079 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/syntaxhighlighters/regexmatchhighlighter.py
--rw-r--r--   0        0        0     2192 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/syntaxhighlighters/xmlhighlighter.py
--rw-r--r--   0        0        0     2106 2023-04-07 02:23:06.283781 prettyqt-1.0.0/prettyqt/syntaxhighlighters/yamlhighlighter.py
--rw-r--r--   0        0        0      180 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/texttospeech/__init__.py
--rw-r--r--   0        0        0     1327 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/texttospeech/texttospeech.py
--rw-r--r--   0        0        0      903 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/texttospeech/voice.py
--rw-r--r--   0        0        0    15547 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/themes/darktheme.qss
--rw-r--r--   0        0        0      845 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/utils/__init__.py
--rw-r--r--   0        0        0     3534 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/utils/autoslot.py
--rw-r--r--   0        0        0     3307 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/utils/colors.py
--rw-r--r--   0        0        0     2337 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/utils/debugging.py
--rw-r--r--   0        0        0     3598 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/utils/helpers.py
--rw-r--r--   0        0        0      939 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/utils/mappers.py
--rw-r--r--   0        0        0     1054 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/utils/prettyprinter.py
--rw-r--r--   0        0        0     5537 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/utils/searchandreplacemixin.py
--rw-r--r--   0        0        0      629 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/utils/signallogger.py
--rw-r--r--   0        0        0     2306 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/utils/singleapplication.py
--rw-r--r--   0        0        0      493 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/utils/singleton.py
--rw-r--r--   0        0        0     2142 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/utils/syncedproperty.py
--rw-r--r--   0        0        0     1887 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/utils/treeitem.py
--rw-r--r--   0        0        0     3738 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/utils/types.py
--rw-r--r--   0        0        0      303 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webchannel/__init__.py
--rw-r--r--   0        0        0      228 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webchannel/webchannel.py
--rw-r--r--   0        0        0     1337 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginecore/__init__.py
--rw-r--r--   0        0        0     3315 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginecore/webenginecontextmenurequest.py
--rw-r--r--   0        0        0     4498 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginecore/webenginedownloadrequest.py
--rw-r--r--   0        0        0     1299 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginecore/webenginehistory.py
--rw-r--r--   0        0        0      422 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginecore/webenginehistoryitem.py
--rw-r--r--   0        0        0     1776 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginecore/webenginehttprequest.py
--rw-r--r--   0        0        0    14235 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginecore/webenginepage.py
--rw-r--r--   0        0        0     2461 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginecore/webengineprofile.py
--rw-r--r--   0        0        0     1574 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginecore/webenginescript.py
--rw-r--r--   0        0        0     1429 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginecore/webenginescriptcollection.py
--rw-r--r--   0        0        0     7469 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginecore/webenginesettings.py
--rw-r--r--   0        0        0     2044 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginecore/webengineurlscheme.py
--rw-r--r--   0        0        0      282 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginecore/webengineurlschemehandler.py
--rw-r--r--   0        0        0      330 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginewidgets/__init__.py
--rw-r--r--   0        0        0     4593 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/webenginewidgets/webengineview.py
--rw-r--r--   0        0        0    13586 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/__init__.py
--rw-r--r--   0        0        0     3797 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/abstractbutton.py
--rw-r--r--   0        0        0      406 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/abstractgraphicsshapeitem.py
--rw-r--r--   0        0        0      257 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/abstractitemdelegate.py
--rw-r--r--   0        0        0    11893 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/abstractitemview.py
--rw-r--r--   0        0        0     5361 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/abstractscrollarea.py
--rw-r--r--   0        0        0     5560 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/abstractslider.py
--rw-r--r--   0        0        0     3715 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/abstractspinbox.py
--rw-r--r--   0        0        0     8383 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/action.py
--rw-r--r--   0        0        0     2143 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/actiongroup.py
--rw-r--r--   0        0        0     7998 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/application.py
--rw-r--r--   0        0        0     2754 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/boxlayout.py
--rw-r--r--   0        0        0      342 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/buttongroup.py
--rw-r--r--   0        0        0     2960 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/calendarwidget.py
--rw-r--r--   0        0        0     1647 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/checkbox.py
--rw-r--r--   0        0        0     3856 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/colordialog.py
--rw-r--r--   0        0        0      331 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/columnview.py
--rw-r--r--   0        0        0     7000 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/combobox.py
--rw-r--r--   0        0        0      365 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/commandlinkbutton.py
--rw-r--r--   0        0        0      280 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/commonstyle.py
--rw-r--r--   0        0        0     3501 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/completer.py
--rw-r--r--   0        0        0     2700 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/datawidgetmapper.py
--rw-r--r--   0        0        0     1412 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/dateedit.py
--rw-r--r--   0        0        0     4324 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/datetimeedit.py
--rw-r--r--   0        0        0     1079 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/dial.py
--rw-r--r--   0        0        0     2813 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/dialog.py
--rw-r--r--   0        0        0     5950 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/dialogbuttonbox.py
--rw-r--r--   0        0        0     2356 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/dockwidget.py
--rw-r--r--   0        0        0     1772 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/doublespinbox.py
--rw-r--r--   0        0        0      328 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/errormessage.py
--rw-r--r--   0        0        0     7406 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/filedialog.py
--rw-r--r--   0        0        0     1256 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/fileiconprovider.py
--rw-r--r--   0        0        0     3492 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/filesystemmodel.py
--rw-r--r--   0        0        0      289 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/focusframe.py
--rw-r--r--   0        0        0     2477 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/fontcombobox.py
--rw-r--r--   0        0        0      363 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/fontdialog.py
--rw-r--r--   0        0        0     4998 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/formlayout.py
--rw-r--r--   0        0        0     2540 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/frame.py
--rw-r--r--   0        0        0     1822 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/gesture.py
--rw-r--r--   0        0        0     2334 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/graphicsanchorlayout.py
--rw-r--r--   0        0        0     1360 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/graphicsblureffect.py
--rw-r--r--   0        0        0      469 2023-04-07 02:23:06.287781 prettyqt-1.0.0/prettyqt/widgets/graphicscolorizeeffect.py
--rw-r--r--   0        0        0      435 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicsdropshadoweffect.py
--rw-r--r--   0        0        0      416 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicseffect.py
--rw-r--r--   0        0        0      559 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicsellipseitem.py
--rw-r--r--   0        0        0     3589 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicsgridlayout.py
--rw-r--r--   0        0        0     4694 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicsitem.py
--rw-r--r--   0        0        0      192 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicsitemgroup.py
--rw-r--r--   0        0        0     1173 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicslayout.py
--rw-r--r--   0        0        0      262 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicslayoutitem.py
--rw-r--r--   0        0        0     1098 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicslinearlayout.py
--rw-r--r--   0        0        0      651 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicslineitem.py
--rw-r--r--   0        0        0      700 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicsobject.py
--rw-r--r--   0        0        0      538 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicsopacityeffect.py
--rw-r--r--   0        0        0      209 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicspathitem.py
--rw-r--r--   0        0        0     2241 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicspixmapitem.py
--rw-r--r--   0        0        0      800 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicspolygonitem.py
--rw-r--r--   0        0        0      198 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicsproxywidget.py
--rw-r--r--   0        0        0      542 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicsrectitem.py
--rw-r--r--   0        0        0      495 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicsrotation.py
--rw-r--r--   0        0        0      250 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicsscale.py
--rw-r--r--   0        0        0     8553 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicsscene.py
--rw-r--r--   0        0        0      293 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicssimpletextitem.py
--rw-r--r--   0        0        0      707 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicstextitem.py
--rw-r--r--   0        0        0      310 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicstransform.py
--rw-r--r--   0        0        0     8390 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicsview.py
--rw-r--r--   0        0        0     2753 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/graphicswidget.py
--rw-r--r--   0        0        0     4121 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/gridlayout.py
--rw-r--r--   0        0        0     1955 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/groupbox.py
--rw-r--r--   0        0        0     5318 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/headerview.py
--rw-r--r--   0        0        0     3755 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/inputdialog.py
--rw-r--r--   0        0        0      190 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/itemdelegate.py
--rw-r--r--   0        0        0      144 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/itemeditorcreatorbase.py
--rw-r--r--   0        0        0     2331 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/itemeditorfactory.py
--rw-r--r--   0        0        0      846 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/keysequenceedit.py
--rw-r--r--   0        0        0     8512 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/label.py
--rw-r--r--   0        0        0     3961 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/layout.py
--rw-r--r--   0        0        0     1272 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/layoutitem.py
--rw-r--r--   0        0        0     2416 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/lcdnumber.py
--rw-r--r--   0        0        0     6525 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/lineedit.py
--rw-r--r--   0        0        0     5606 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/listview.py
--rw-r--r--   0        0        0     5823 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/listwidget.py
--rw-r--r--   0        0        0     2851 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/listwidgetitem.py
--rw-r--r--   0        0        0     6705 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/mainwindow.py
--rw-r--r--   0        0        0     4584 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/mdiarea.py
--rw-r--r--   0        0        0      689 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/mdisubwindow.py
--rw-r--r--   0        0        0     4397 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/menu.py
--rw-r--r--   0        0        0     2145 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/menubar.py
--rw-r--r--   0        0        0     7314 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/messagebox.py
--rw-r--r--   0        0        0      542 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/pangesture.py
--rw-r--r--   0        0        0     1902 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/pinchgesture.py
--rw-r--r--   0        0        0      415 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/plaintextdocumentlayout.py
--rw-r--r--   0        0        0     9079 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/plaintextedit.py
--rw-r--r--   0        0        0     3564 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/progressbar.py
--rw-r--r--   0        0        0     1029 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/progressdialog.py
--rw-r--r--   0        0        0      231 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/proxystyle.py
--rw-r--r--   0        0        0      795 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/pushbutton.py
--rw-r--r--   0        0        0      517 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/radiobutton.py
--rw-r--r--   0        0        0      758 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/rubberband.py
--rw-r--r--   0        0        0      611 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/scrollarea.py
--rw-r--r--   0        0        0      707 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/scrollbar.py
--rw-r--r--   0        0        0     3060 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/scroller.py
--rw-r--r--   0        0        0     3937 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/scrollerproperties.py
--rw-r--r--   0        0        0     1399 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/shortcut.py
--rw-r--r--   0        0        0      309 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/sizegrip.py
--rw-r--r--   0        0        0     5373 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/sizepolicy.py
--rw-r--r--   0        0        0     2654 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/slider.py
--rw-r--r--   0        0        0     1297 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/spaceritem.py
--rw-r--r--   0        0        0     1837 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/spinbox.py
--rw-r--r--   0        0        0     1181 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/splashscreen.py
--rw-r--r--   0        0        0     3908 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/splitter.py
--rw-r--r--   0        0        0     1417 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/splitterhandle.py
--rw-r--r--   0        0        0      983 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/stackedlayout.py
--rw-r--r--   0        0        0     1372 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/stackedwidget.py
--rw-r--r--   0        0        0     1677 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/statusbar.py
--rw-r--r--   0        0        0    19383 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/style.py
--rw-r--r--   0        0        0      208 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/styleditemdelegate.py
--rw-r--r--   0        0        0      126 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/stylefactory.py
--rw-r--r--   0        0        0      318 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/styleoption.py
--rw-r--r--   0        0        0      686 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/styleoptionbutton.py
--rw-r--r--   0        0        0      208 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/styleoptioncombobox.py
--rw-r--r--   0        0        0      260 2023-04-07 02:23:06.291781 prettyqt-1.0.0/prettyqt/widgets/styleoptioncomplex.py
--rw-r--r--   0        0        0      199 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptiondockwidget.py
--rw-r--r--   0        0        0      197 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptionfocusrect.py
--rw-r--r--   0        0        0      189 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptionframe.py
--rw-r--r--   0        0        0      209 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptiongraphicsitem.py
--rw-r--r--   0        0        0      197 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptiongroupbox.py
--rw-r--r--   0        0        0      912 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptionheader.py
--rw-r--r--   0        0        0     1032 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptionmenuitem.py
--rw-r--r--   0        0        0      201 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptionprogressbar.py
--rw-r--r--   0        0        0      199 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptionrubberband.py
--rw-r--r--   0        0        0      208 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptionsizegrip.py
--rw-r--r--   0        0        0     1046 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptionslider.py
--rw-r--r--   0        0        0      195 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptionspinbox.py
--rw-r--r--   0        0        0     1135 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptiontab.py
--rw-r--r--   0        0        0      199 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptiontabbarbase.py
--rw-r--r--   0        0        0      213 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptiontabwidgetframe.py
--rw-r--r--   0        0        0      197 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptiontitlebar.py
--rw-r--r--   0        0        0      397 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptiontoolbar.py
--rw-r--r--   0        0        0     1176 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptiontoolbox.py
--rw-r--r--   0        0        0      201 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptiontoolbutton.py
--rw-r--r--   0        0        0     1344 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/styleoptionviewitem.py
--rw-r--r--   0        0        0      397 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/stylepainter.py
--rw-r--r--   0        0        0     1311 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/swipegesture.py
--rw-r--r--   0        0        0     1732 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/systemtrayicon.py
--rw-r--r--   0        0        0     5232 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/tabbar.py
--rw-r--r--   0        0        0     3112 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/tableview.py
--rw-r--r--   0        0        0     1085 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/tablewidget.py
--rw-r--r--   0        0        0     3368 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/tablewidgetitem.py
--rw-r--r--   0        0        0     1920 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/tablewidgetselectionrange.py
--rw-r--r--   0        0        0    10591 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/tabwidget.py
--rw-r--r--   0        0        0      392 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/tapandholdgesture.py
--rw-r--r--   0        0        0      371 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/tapgesture.py
--rw-r--r--   0        0        0     2400 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/textbrowser.py
--rw-r--r--   0        0        0     6089 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/textedit.py
--rw-r--r--   0        0        0     1526 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/timeedit.py
--rw-r--r--   0        0        0     4981 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/toolbar.py
--rw-r--r--   0        0        0     2568 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/toolbox.py
--rw-r--r--   0        0        0     3175 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/toolbutton.py
--rw-r--r--   0        0        0      710 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/tooltip.py
--rw-r--r--   0        0        0     2532 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/treeview.py
--rw-r--r--   0        0        0      630 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/treewidget.py
--rw-r--r--   0        0        0     4841 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/treewidgetitem.py
--rw-r--r--   0        0        0     4142 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/treewidgetitemiterator.py
--rw-r--r--   0        0        0      652 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/undocommand.py
--rw-r--r--   0        0        0      368 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/undogroup.py
--rw-r--r--   0        0        0      986 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/undostack.py
--rw-r--r--   0        0        0     1011 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/undoview.py
--rw-r--r--   0        0        0      552 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/whatsthis.py
--rw-r--r--   0        0        0    19395 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/widget.py
--rw-r--r--   0        0        0      545 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/widgetaction.py
--rw-r--r--   0        0        0      248 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/widgetitem.py
--rw-r--r--   0        0        0     9052 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/wizard.py
--rw-r--r--   0        0        0     1997 2023-04-07 02:23:06.295781 prettyqt-1.0.0/prettyqt/widgets/wizardpage.py
--rw-r--r--   0        0        0     4767 2023-04-07 02:23:06.295781 prettyqt-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4515 1970-01-01 00:00:00.000000 prettyqt-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-04-09 22:54:45.725040 prettyqt-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2875 2023-04-09 22:54:45.725040 prettyqt-1.1.0/docs/index.md
+-rw-r--r--   0        0        0      687 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/__init__.py
+-rw-r--r--   0        0        0      122 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/__pyinstaller/__init__.py
+-rw-r--r--   0        0        0      860 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/__pyinstaller/hook-prettyqt.py
+-rw-r--r--   0        0        0      517 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/bluetooth/__init__.py
+-rw-r--r--   0        0        0      334 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/bluetooth/bluetoothaddress.py
+-rw-r--r--   0        0        0     2649 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/bluetooth/bluetoothdevicediscoveryagent.py
+-rw-r--r--   0        0        0     1421 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/bluetooth/bluetoothservicediscoveryagent.py
+-rw-r--r--   0        0        0     1872 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/bluetooth/bluetoothserviceinfo.py
+-rw-r--r--   0        0        0    11927 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/bluetooth/bluetoothuuid.py
+-rw-r--r--   0        0        0     1792 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/__init__.py
+-rw-r--r--   0        0        0     2245 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/abstractaxis.py
+-rw-r--r--   0        0        0     1603 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/abstractbarseries.py
+-rw-r--r--   0        0        0      554 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/abstractseries.py
+-rw-r--r--   0        0        0      517 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/barcategoryaxis.py
+-rw-r--r--   0        0        0      177 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/barseries.py
+-rw-r--r--   0        0        0      932 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/barset.py
+-rw-r--r--   0        0        0     1692 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/boxset.py
+-rw-r--r--   0        0        0      609 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/candlestickset.py
+-rw-r--r--   0        0        0     1767 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/categoryaxis.py
+-rw-r--r--   0        0        0     5315 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/chart.py
+-rw-r--r--   0        0        0     5665 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/chartview.py
+-rw-r--r--   0        0        0      381 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/datetimeaxis.py
+-rw-r--r--   0        0        0      197 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/horizontalbarseries.py
+-rw-r--r--   0        0        0      217 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/horizontalpercentbarseries.py
+-rw-r--r--   0        0        0      217 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/horizontalstackedbarseries.py
+-rw-r--r--   0        0        0     2742 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/legend.py
+-rw-r--r--   0        0        0      645 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/lineseries.py
+-rw-r--r--   0        0        0      178 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/logvalueaxis.py
+-rw-r--r--   0        0        0      191 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/percentbarseries.py
+-rw-r--r--   0        0        0     2038 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/pieslice.py
+-rw-r--r--   0        0        0      739 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/polarchart.py
+-rw-r--r--   0        0        0      176 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/scatterseries.py
+-rw-r--r--   0        0        0      191 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/stackedbarseries.py
+-rw-r--r--   0        0        0     1044 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/valueaxis.py
+-rw-r--r--   0        0        0     1219 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/charts/xyseries.py
+-rw-r--r--   0        0        0    34636 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/constants/__init__.py
+-rw-r--r--   0        0        0     9001 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/__init__.py
+-rw-r--r--   0        0        0     1098 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/_calendar.py
+-rw-r--r--   0        0        0     2000 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/_datetime.py
+-rw-r--r--   0        0        0      478 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/_time.py
+-rw-r--r--   0        0        0     3286 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/abstractanimation.py
+-rw-r--r--   0        0        0      186 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/abstracteventdispatcher.py
+-rw-r--r--   0        0        0     5354 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/abstractitemmodel.py
+-rw-r--r--   0        0        0      250 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/abstractlistmodel.py
+-rw-r--r--   0        0        0      146 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/abstractnativeeventfilter.py
+-rw-r--r--   0        0        0      254 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/abstractproxymodel.py
+-rw-r--r--   0        0        0      254 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/abstracttablemodel.py
+-rw-r--r--   0        0        0     2060 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/animationgroup.py
+-rw-r--r--   0        0        0      533 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/basictimer.py
+-rw-r--r--   0        0        0      154 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/buffer.py
+-rw-r--r--   0        0        0      173 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/bytearray.py
+-rw-r--r--   0        0        0      369 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/bytearraymatcher.py
+-rw-r--r--   0        0        0      959 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/collator.py
+-rw-r--r--   0        0        0      126 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/collatorsortkey.py
+-rw-r--r--   0        0        0      324 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/commandlineoption.py
+-rw-r--r--   0        0        0     2231 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/commandlineparser.py
+-rw-r--r--   0        0        0      211 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/concatenatetablesproxymodel.py
+-rw-r--r--   0        0        0     3949 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/coreapplication.py
+-rw-r--r--   0        0        0     2038 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/cryptographichash.py
+-rw-r--r--   0        0        0     3426 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/datastream.py
+-rw-r--r--   0        0        0      470 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/date.py
+-rw-r--r--   0        0        0      766 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/deadlinetimer.py
+-rw-r--r--   0        0        0     1153 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/debug.py
+-rw-r--r--   0        0        0     4369 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/dir.py
+-rw-r--r--   0        0        0      264 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/diriterator.py
+-rw-r--r--   0        0        0     4527 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/easingcurve.py
+-rw-r--r--   0        0        0      918 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/elapsedtimer.py
+-rw-r--r--   0        0        0     7128 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/event.py
+-rw-r--r--   0        0        0     1225 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/eventloop.py
+-rw-r--r--   0        0        0      191 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/file.py
+-rw-r--r--   0        0        0     3694 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/filedevice.py
+-rw-r--r--   0        0        0     1492 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/fileinfo.py
+-rw-r--r--   0        0        0      560 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/fileselector.py
+-rw-r--r--   0        0        0      879 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/filesystemwatcher.py
+-rw-r--r--   0        0        0      188 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/identityproxymodel.py
+-rw-r--r--   0        0        0     1485 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/iodevice.py
+-rw-r--r--   0        0        0      122 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/itemselection.py
+-rw-r--r--   0        0        0      176 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/itemselectionmodel.py
+-rw-r--r--   0        0        0      696 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/itemselectionrange.py
+-rw-r--r--   0        0        0     1661 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/jsondocument.py
+-rw-r--r--   0        0        0      538 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/jsonvalue.py
+-rw-r--r--   0        0        0     1248 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/library.py
+-rw-r--r--   0        0        0     1692 2023-04-09 22:54:45.725040 prettyqt-1.1.0/prettyqt/core/libraryinfo.py
+-rw-r--r--   0        0        0     1868 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/line.py
+-rw-r--r--   0        0        0     1997 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/linef.py
+-rw-r--r--   0        0        0    16492 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/locale.py
+-rw-r--r--   0        0        0      810 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/lockfile.py
+-rw-r--r--   0        0        0      708 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/margins.py
+-rw-r--r--   0        0        0      713 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/marginsf.py
+-rw-r--r--   0        0        0     1110 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/metaenum.py
+-rw-r--r--   0        0        0     1423 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/metamethod.py
+-rw-r--r--   0        0        0     3703 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/metaobject.py
+-rw-r--r--   0        0        0      511 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/metaproperty.py
+-rw-r--r--   0        0        0     1802 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/mimedata.py
+-rw-r--r--   0        0        0      948 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/mimedatabase.py
+-rw-r--r--   0        0        0      208 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/mimetype.py
+-rw-r--r--   0        0        0      176 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/modelindex.py
+-rw-r--r--   0        0        0      336 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/mutex.py
+-rw-r--r--   0        0        0     3583 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/object.py
+-rw-r--r--   0        0        0     2562 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/operatingsystemversion.py
+-rw-r--r--   0        0        0      356 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/parallelanimationgroup.py
+-rw-r--r--   0        0        0      253 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/pauseanimation.py
+-rw-r--r--   0        0        0      338 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/persistentmodelindex.py
+-rw-r--r--   0        0        0      811 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/pluginloader.py
+-rw-r--r--   0        0        0      349 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/point.py
+-rw-r--r--   0        0        0      353 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/pointf.py
+-rw-r--r--   0        0        0     4839 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/process.py
+-rw-r--r--   0        0        0     1340 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/processenvironment.py
+-rw-r--r--   0        0        0      774 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/propertyanimation.py
+-rw-r--r--   0        0        0      126 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/randomgenerator.py
+-rw-r--r--   0        0        0      231 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/randomgenerator64.py
+-rw-r--r--   0        0        0      878 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/rect.py
+-rw-r--r--   0        0        0      442 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/rectf.py
+-rw-r--r--   0        0        0     6515 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/regularexpression.py
+-rw-r--r--   0        0        0     2579 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/regularexpressionmatch.py
+-rw-r--r--   0        0        0      613 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/regularexpressionmatchiterator.py
+-rw-r--r--   0        0        0     1702 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/resource.py
+-rw-r--r--   0        0        0      112 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/runnable.py
+-rw-r--r--   0        0        0      160 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/savefile.py
+-rw-r--r--   0        0        0      281 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/semaphore.py
+-rw-r--r--   0        0        0      202 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/sequentialanimationgroup.py
+-rw-r--r--   0        0        0     6990 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/settings.py
+-rw-r--r--   0        0        0      122 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/signalblocker.py
+-rw-r--r--   0        0        0      451 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/signalmapper.py
+-rw-r--r--   0        0        0     1124 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/size.py
+-rw-r--r--   0        0        0     1142 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/sizef.py
+-rw-r--r--   0        0        0      471 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/slot.py
+-rw-r--r--   0        0        0      930 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/socketnotifier.py
+-rw-r--r--   0        0        0     2681 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/sortfilterproxymodel.py
+-rw-r--r--   0        0        0     2622 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/standardpaths.py
+-rw-r--r--   0        0        0     1184 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/storageinfo.py
+-rw-r--r--   0        0        0      339 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/stringlistmodel.py
+-rw-r--r--   0        0        0      980 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/temporarydir.py
+-rw-r--r--   0        0        0      164 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/temporaryfile.py
+-rw-r--r--   0        0        0     2583 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/textboundaryfinder.py
+-rw-r--r--   0        0        0     3862 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/textstream.py
+-rw-r--r--   0        0        0      108 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/thread.py
+-rw-r--r--   0        0        0      160 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/threadpool.py
+-rw-r--r--   0        0        0     2318 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/timeline.py
+-rw-r--r--   0        0        0     1770 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/timer.py
+-rw-r--r--   0        0        0     2076 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/timezone.py
+-rw-r--r--   0        0        0     1722 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/translator.py
+-rw-r--r--   0        0        0      190 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/transposeproxymodel.py
+-rw-r--r--   0        0        0     3968 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/url.py
+-rw-r--r--   0        0        0      770 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/urlquery.py
+-rw-r--r--   0        0        0     1837 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/uuid.py
+-rw-r--r--   0        0        0     1501 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/variantanimation.py
+-rw-r--r--   0        0        0     2614 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/versionnumber.py
+-rw-r--r--   0        0        0     2614 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/core/xmlstreamreader.py
+-rw-r--r--   0        0        0      253 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_animations/__init__.py
+-rw-r--r--   0        0        0     1579 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_animations/bounceanimation.py
+-rw-r--r--   0        0        0      644 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_animations/fadeinanimation.py
+-rw-r--r--   0        0        0      978 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_animations/slideanimation.py
+-rw-r--r--   0        0        0      535 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_delegates/__init__.py
+-rw-r--r--   0        0        0      887 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_delegates/buttondelegate.py
+-rw-r--r--   0        0        0     1001 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_delegates/checkboxdelegate.py
+-rw-r--r--   0        0        0     2570 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_delegates/icondelegate.py
+-rw-r--r--   0        0        0      596 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_delegates/nofocusdelegate.py
+-rw-r--r--   0        0        0     1474 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_delegates/progressbardelegate.py
+-rw-r--r--   0        0        0     4789 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_delegates/radiodelegate.py
+-rw-r--r--   0        0        0     2574 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_delegates/renderlinkdelegate.py
+-rw-r--r--   0        0        0     6634 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_delegates/stardelegate.py
+-rw-r--r--   0        0        0      735 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_models/__init__.py
+-rw-r--r--   0        0        0     5965 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_models/columnitemmodel.py
+-rw-r--r--   0        0        0     3297 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_models/importlibdistributionmodel.py
+-rw-r--r--   0        0        0     4313 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_models/jsonmodel.py
+-rw-r--r--   0        0        0     3083 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_models/listmixin.py
+-rw-r--r--   0        0        0     2562 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_models/modelmixin.py
+-rw-r--r--   0        0        0     2298 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_models/nesteditem.py
+-rw-r--r--   0        0        0     2177 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_models/nestedmodel.py
+-rw-r--r--   0        0        0     2112 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_models/regexmatchesmodel.py
+-rw-r--r--   0        0        0     1698 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_models/selectionmixin.py
+-rw-r--r--   0        0        0     5288 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_models/storageinfomodel.py
+-rw-r--r--   0        0        0     2858 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_models/subsequencesortfilterproxymodel.py
+-rw-r--r--   0        0        0      635 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_validators/__init__.py
+-rw-r--r--   0        0        0     2060 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_validators/compositevalidator.py
+-rw-r--r--   0        0        0     1114 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_validators/integervalidator.py
+-rw-r--r--   0        0        0      704 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_validators/notemptyvalidator.py
+-rw-r--r--   0        0        0      700 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_validators/notzerovalidator.py
+-rw-r--r--   0        0        0      620 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_validators/pathvalidator.py
+-rw-r--r--   0        0        0     1554 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_validators/regexpatternvalidator.py
+-rw-r--r--   0        0        0     3143 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_validators/regexvalidators.py
+-rw-r--r--   0        0        0     2704 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_widgets/__init__.py
+-rw-r--r--   0        0        0     1638 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_widgets/booldicttoolbutton.py
+-rw-r--r--   0        0        0     7718 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_widgets/borderlayout.py
+-rw-r--r--   0        0        0     3046 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_widgets/codeeditor.py
+-rw-r--r--   0        0        0     2588 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_widgets/collapsibleframe.py
+-rw-r--r--   0        0        0     2468 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_widgets/colorchooserbutton.py
+-rw-r--r--   0        0        0     7480 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_widgets/completionwidget.py
+-rw-r--r--   0        0        0    17651 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_widgets/dataset.py
+-rw-r--r--   0        0        0     2219 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_widgets/elidedlabel.py
+-rw-r--r--   0        0        0     3429 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_widgets/expandableline.py
+-rw-r--r--   0        0        0     3194 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_widgets/filechooserbutton.py
+-rw-r--r--   0        0        0     2155 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_widgets/flagselectionwidget.py
+-rw-r--r--   0        0        0     3847 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_widgets/flowlayout.py
+-rw-r--r--   0        0        0     2156 2023-04-09 22:54:45.729040 prettyqt-1.1.0/prettyqt/custom_widgets/fontchooserbutton.py
+-rw-r--r--   0        0        0     9168 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/framelesswindow.py
+-rw-r--r--   0        0        0     5371 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/iconbrowser.py
+-rw-r--r--   0        0        0     1311 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/iconlabel.py
+-rw-r--r--   0        0        0     1661 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/iconwidget.py
+-rw-r--r--   0        0        0     1292 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/image.py
+-rw-r--r--   0        0        0      644 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/imageviewer.py
+-rw-r--r--   0        0        0     1931 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/inputandslider.py
+-rw-r--r--   0        0        0     2106 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/joystickbutton.py
+-rw-r--r--   0        0        0     4175 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/labeledslider.py
+-rw-r--r--   0        0        0     1214 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/listinput.py
+-rw-r--r--   0        0        0     8209 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/logtextedit.py
+-rw-r--r--   0        0        0      738 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/mappedcheckbox.py
+-rw-r--r--   0        0        0     2388 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/markdownwidget.py
+-rw-r--r--   0        0        0     6576 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/menurecentfiles.py
+-rw-r--r--   0        0        0    18785 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/notification.py
+-rw-r--r--   0        0        0     1038 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/optionalwidget.py
+-rw-r--r--   0        0        0     1332 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/popupinfo.py
+-rw-r--r--   0        0        0      145 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/regexeditor/__init__.py
+-rw-r--r--   0        0        0      431 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/regexeditor/__main__.py
+-rw-r--r--   0        0        0     1039 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/regexeditor/quick_ref.py
+-rw-r--r--   0        0        0    19388 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/regexeditor/ref.html
+-rw-r--r--   0        0        0     6186 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/regexeditor/regexeditorwidget.py
+-rw-r--r--   0        0        0     3110 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/regexinput.py
+-rw-r--r--   0        0        0    10698 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/roundprogressbar.py
+-rw-r--r--   0        0        0     4284 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/selectionwidget.py
+-rw-r--r--   0        0        0     6345 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/sidebarwidget.py
+-rw-r--r--   0        0        0     1036 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/singlelinetextedit.py
+-rw-r--r--   0        0        0    18739 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/spanslider.py
+-rw-r--r--   0        0        0     1286 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/standardiconswidget.py
+-rw-r--r--   0        0        0     2289 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/stringornumberwidget.py
+-rw-r--r--   0        0        0     1774 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/subsequencecompleter.py
+-rw-r--r--   0        0        0     8034 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/timeline.py
+-rw-r--r--   0        0        0     9009 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/custom_widgets/waitingspinner.py
+-rw-r--r--   0        0        0      255 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/eventfilters/__init__.py
+-rw-r--r--   0        0        0     2613 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/eventfilters/animatedtooltipeventfilter.py
+-rw-r--r--   0        0        0      751 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/eventfilters/hovericoneventfilter.py
+-rw-r--r--   0        0        0     7774 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/__init__.py
+-rw-r--r--   0        0        0     1269 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/abstracttextdocumentlayout.py
+-rw-r--r--   0        0        0      235 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/bitmap.py
+-rw-r--r--   0        0        0      979 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/brush.py
+-rw-r--r--   0        0        0     2490 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/clipboard.py
+-rw-r--r--   0        0        0     6808 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/color.py
+-rw-r--r--   0        0        0     3045 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/colorspace.py
+-rw-r--r--   0        0        0      485 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/conicalgradient.py
+-rw-r--r--   0        0        0     1255 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/cursor.py
+-rw-r--r--   0        0        0      439 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/desktopservices.py
+-rw-r--r--   0        0        0     1094 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/doublevalidator.py
+-rw-r--r--   0        0        0      973 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/drag.py
+-rw-r--r--   0        0        0     9049 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/font.py
+-rw-r--r--   0        0        0     4694 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/fontdatabase.py
+-rw-r--r--   0        0        0      243 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/fontinfo.py
+-rw-r--r--   0        0        0      878 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/fontmetrics.py
+-rw-r--r--   0        0        0      719 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/fontmetricsf.py
+-rw-r--r--   0        0        0     5331 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/gradient.py
+-rw-r--r--   0        0        0     5027 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/guiapplication.py
+-rw-r--r--   0        0        0     3970 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/icon.py
+-rw-r--r--   0        0        0     4053 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/iconengine.py
+-rw-r--r--   0        0        0     1711 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/image.py
+-rw-r--r--   0        0        0     3778 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/imageiohandler.py
+-rw-r--r--   0        0        0     3838 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/imagereader.py
+-rw-r--r--   0        0        0     2791 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/imagewriter.py
+-rw-r--r--   0        0        0     1315 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/inputmethod.py
+-rw-r--r--   0        0        0      921 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/intvalidator.py
+-rw-r--r--   0        0        0     6168 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/keysequence.py
+-rw-r--r--   0        0        0      636 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/lineargradient.py
+-rw-r--r--   0        0        0      302 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/matrix4x4.py
+-rw-r--r--   0        0        0     1969 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/movie.py
+-rw-r--r--   0        0        0      297 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/pagedpaintdevice.py
+-rw-r--r--   0        0        0     2923 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/pagelayout.py
+-rw-r--r--   0        0        0     7838 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/pagesize.py
+-rw-r--r--   0        0        0     1676 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/paintdevice.py
+-rw-r--r--   0        0        0      319 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/paintdevicewindow.py
+-rw-r--r--   0        0        0     7557 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/painter.py
+-rw-r--r--   0        0        0     2425 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/painterpath.py
+-rw-r--r--   0        0        0     1641 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/painterpathstroker.py
+-rw-r--r--   0        0        0     5859 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/palette.py
+-rw-r--r--   0        0        0     1026 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/pdfwriter.py
+-rw-r--r--   0        0        0     2841 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/pen.py
+-rw-r--r--   0        0        0      471 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/picture.py
+-rw-r--r--   0        0        0     4827 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/pixmap.py
+-rw-r--r--   0        0        0      796 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/pixmapcache.py
+-rw-r--r--   0        0        0     3489 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/polygon.py
+-rw-r--r--   0        0        0     4325 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/polygonf.py
+-rw-r--r--   0        0        0      898 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/radialgradient.py
+-rw-r--r--   0        0        0      233 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/rasterwindow.py
+-rw-r--r--   0        0        0     1145 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/region.py
+-rw-r--r--   0        0        0     1290 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/regularexpressionvalidator.py
+-rw-r--r--   0        0        0     2963 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/screen.py
+-rw-r--r--   0        0        0     1291 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/sessionmanager.py
+-rw-r--r--   0        0        0     6188 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/standarditem.py
+-rw-r--r--   0        0        0     4758 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/standarditemmodel.py
+-rw-r--r--   0        0        0     2225 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/statictext.py
+-rw-r--r--   0        0        0     1303 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/surface.py
+-rw-r--r--   0        0        0     1352 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/syntaxhighlighter.py
+-rw-r--r--   0        0        0     5251 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/textblock.py
+-rw-r--r--   0        0        0      623 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/textblockgroup.py
+-rw-r--r--   0        0        0      536 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/textblockuserdata.py
+-rw-r--r--   0        0        0     4878 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/textcharformat.py
+-rw-r--r--   0        0        0     5551 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/textcursor.py
+-rw-r--r--   0        0        0     7781 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/textdocument.py
+-rw-r--r--   0        0        0      949 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/textdocumentfragment.py
+-rw-r--r--   0        0        0     1062 2023-04-09 22:54:45.733040 prettyqt-1.1.0/prettyqt/gui/textdocumentwriter.py
+-rw-r--r--   0        0        0     3262 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/textformat.py
+-rw-r--r--   0        0        0      534 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/textframe.py
+-rw-r--r--   0        0        0     3627 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/textframeformat.py
+-rw-r--r--   0        0        0      297 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/textimageformat.py
+-rw-r--r--   0        0        0      517 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/textlayout.py
+-rw-r--r--   0        0        0      725 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/textlength.py
+-rw-r--r--   0        0        0     1649 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/textline.py
+-rw-r--r--   0        0        0     1327 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/textlistformat.py
+-rw-r--r--   0        0        0      445 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/textobject.py
+-rw-r--r--   0        0        0      199 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/textobjectinterface.py
+-rw-r--r--   0        0        0     1560 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/textoption.py
+-rw-r--r--   0        0        0     4104 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/texttablecellformat.py
+-rw-r--r--   0        0        0     2659 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/transform.py
+-rw-r--r--   0        0        0      640 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/undocommand.py
+-rw-r--r--   0        0        0      356 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/undogroup.py
+-rw-r--r--   0        0        0      971 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/undostack.py
+-rw-r--r--   0        0        0      755 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/validator.py
+-rw-r--r--   0        0        0      575 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/vector3d.py
+-rw-r--r--   0        0        0      578 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/vector4d.py
+-rw-r--r--   0        0        0     2338 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/gui/window.py
+-rw-r--r--   0        0        0    10227 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/iconprovider/__init__.py
+-rw-r--r--   0        0        0     1387 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/iconprovider/animation.py
+-rw-r--r--   0        0        0     3079 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/iconprovider/awesomefileiconprovider.py
+-rw-r--r--   0        0        0      539 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/iconprovider/awesomequickimageprovider.py
+-rw-r--r--   0        0        0      832 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/iconprovider/chariconengine.py
+-rw-r--r--   0        0        0    10996 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/codicon-charmap.json
+-rw-r--r--   0        0        0    68076 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/codicon.ttf
+-rw-r--r--   0        0        0     7924 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/elusiveicons-webfont-charmap.json
+-rw-r--r--   0        0        0    79556 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/elusiveicons-webfont.ttf
+-rw-r--r--   0        0        0    11206 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont-charmap.json
+-rw-r--r--   0        0        0   134316 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont.ttf
+-rw-r--r--   0        0        0     3947 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont-charmap.json
+-rw-r--r--   0        0        0    33692 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont.ttf
+-rw-r--r--   0        0        0    25663 2023-04-09 22:54:45.737041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont-charmap.json
+-rw-r--r--   0        0        0   203644 2023-04-09 22:54:45.741041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont.ttf
+-rw-r--r--   0        0        0   200215 2023-04-09 22:54:45.741041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont-charmap.json
+-rw-r--r--   0        0        0  1026284 2023-04-09 22:54:45.749041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont.ttf
+-rw-r--r--   0        0        0   216192 2023-04-09 22:54:45.749041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont-charmap.json
+-rw-r--r--   0        0        0  1108672 2023-04-09 22:54:45.753041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont.ttf
+-rw-r--r--   0        0        0   151941 2023-04-09 22:54:45.753041 prettyqt-1.1.0/prettyqt/iconprovider/fonts/phosphor-charmap.json
+-rw-r--r--   0        0        0  1392088 2023-04-09 22:54:45.761042 prettyqt-1.1.0/prettyqt/iconprovider/fonts/phosphor.ttf
+-rw-r--r--   0        0        0    72655 2023-04-09 22:54:45.761042 prettyqt-1.1.0/prettyqt/iconprovider/fonts/remixicon-charmap.json
+-rw-r--r--   0        0        0   403056 2023-04-09 22:54:45.765042 prettyqt-1.1.0/prettyqt/iconprovider/fonts/remixicon.ttf
+-rw-r--r--   0        0        0     8417 2023-04-09 22:54:45.765042 prettyqt-1.1.0/prettyqt/iconprovider/iconic_font.py
+-rw-r--r--   0        0        0     2468 2023-04-09 22:54:45.765042 prettyqt-1.1.0/prettyqt/iconprovider/svgbuffericonengine.py
+-rw-r--r--   0        0        0   154232 2023-04-09 22:54:45.765042 prettyqt-1.1.0/prettyqt/localization/language_ar.qm
+-rw-r--r--   0        0        0   155315 2023-04-09 22:54:45.765042 prettyqt-1.1.0/prettyqt/localization/language_bg.qm
+-rw-r--r--   0        0        0   178552 2023-04-09 22:54:45.765042 prettyqt-1.1.0/prettyqt/localization/language_ca.qm
+-rw-r--r--   0        0        0   151054 2023-04-09 22:54:45.769042 prettyqt-1.1.0/prettyqt/localization/language_cs.qm
+-rw-r--r--   0        0        0   179910 2023-04-09 22:54:45.769042 prettyqt-1.1.0/prettyqt/localization/language_da.qm
+-rw-r--r--   0        0        0   212675 2023-04-09 22:54:45.769042 prettyqt-1.1.0/prettyqt/localization/language_de.qm
+-rw-r--r--   0        0        0   154543 2023-04-09 22:54:45.769042 prettyqt-1.1.0/prettyqt/localization/language_es.qm
+-rw-r--r--   0        0        0    97872 2023-04-09 22:54:45.769042 prettyqt-1.1.0/prettyqt/localization/language_fa.qm
+-rw-r--r--   0        0        0   174500 2023-04-09 22:54:45.773043 prettyqt-1.1.0/prettyqt/localization/language_fi.qm
+-rw-r--r--   0        0        0   154190 2023-04-09 22:54:45.773043 prettyqt-1.1.0/prettyqt/localization/language_fr.qm
+-rw-r--r--   0        0        0   183091 2023-04-09 22:54:45.773043 prettyqt-1.1.0/prettyqt/localization/language_gd.qm
+-rw-r--r--   0        0        0   108600 2023-04-09 22:54:45.773043 prettyqt-1.1.0/prettyqt/localization/language_gl.qm
+-rw-r--r--   0        0        0   130568 2023-04-09 22:54:45.777043 prettyqt-1.1.0/prettyqt/localization/language_he.qm
+-rw-r--r--   0        0        0   150033 2023-04-09 22:54:45.777043 prettyqt-1.1.0/prettyqt/localization/language_hu.qm
+-rw-r--r--   0        0        0   153570 2023-04-09 22:54:45.777043 prettyqt-1.1.0/prettyqt/localization/language_it.qm
+-rw-r--r--   0        0        0   122385 2023-04-09 22:54:45.777043 prettyqt-1.1.0/prettyqt/localization/language_ja.qm
+-rw-r--r--   0        0        0   120318 2023-04-09 22:54:45.777043 prettyqt-1.1.0/prettyqt/localization/language_ko.qm
+-rw-r--r--   0        0        0    90502 2023-04-09 22:54:45.777043 prettyqt-1.1.0/prettyqt/localization/language_lt.qm
+-rw-r--r--   0        0        0   143558 2023-04-09 22:54:45.777043 prettyqt-1.1.0/prettyqt/localization/language_lv.qm
+-rw-r--r--   0        0        0   161318 2023-04-09 22:54:45.781043 prettyqt-1.1.0/prettyqt/localization/language_pl.qm
+-rw-r--r--   0        0        0    50541 2023-04-09 22:54:45.781043 prettyqt-1.1.0/prettyqt/localization/language_pt.qm
+-rw-r--r--   0        0        0   197476 2023-04-09 22:54:45.781043 prettyqt-1.1.0/prettyqt/localization/language_ru.qm
+-rw-r--r--   0        0        0   115250 2023-04-09 22:54:45.781043 prettyqt-1.1.0/prettyqt/localization/language_sk.qm
+-rw-r--r--   0        0        0    96357 2023-04-09 22:54:45.781043 prettyqt-1.1.0/prettyqt/localization/language_sl.qm
+-rw-r--r--   0        0        0    47206 2023-04-09 22:54:45.781043 prettyqt-1.1.0/prettyqt/localization/language_sv.qm
+-rw-r--r--   0        0        0   148437 2023-04-09 22:54:45.781043 prettyqt-1.1.0/prettyqt/localization/language_uk.qm
+-rw-r--r--   0        0        0    61089 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/localization/language_zh_CN.qm
+-rw-r--r--   0        0        0   125250 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/localization/language_zh_TW.qm
+-rw-r--r--   0        0        0     2384 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/__init__.py
+-rw-r--r--   0        0        0      387 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/geocodingmanager.py
+-rw-r--r--   0        0        0     2867 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/geomaneuver.py
+-rw-r--r--   0        0        0     1055 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/georoute.py
+-rw-r--r--   0        0        0     5266 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/georouterequest.py
+-rw-r--r--   0        0        0      657 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/georoutesegment.py
+-rw-r--r--   0        0        0     2021 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/georoutingmanager.py
+-rw-r--r--   0        0        0     5880 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/geoserviceprovider.py
+-rw-r--r--   0        0        0     2387 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/place.py
+-rw-r--r--   0        0        0      864 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placeattribute.py
+-rw-r--r--   0        0        0      737 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placecategory.py
+-rw-r--r--   0        0        0      844 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placecontactdetail.py
+-rw-r--r--   0        0        0     1030 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placecontent.py
+-rw-r--r--   0        0        0     1275 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placecontentreply.py
+-rw-r--r--   0        0        0      947 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placecontentrequest.py
+-rw-r--r--   0        0        0      562 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placedetailsreply.py
+-rw-r--r--   0        0        0      849 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placeicon.py
+-rw-r--r--   0        0        0     1185 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placeidreply.py
+-rw-r--r--   0        0        0     2233 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placemanager.py
+-rw-r--r--   0        0        0     1066 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placematchreply.py
+-rw-r--r--   0        0        0      726 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placematchrequest.py
+-rw-r--r--   0        0        0      223 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placeproposedsearchresult.py
+-rw-r--r--   0        0        0      316 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placeratings.py
+-rw-r--r--   0        0        0     1923 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placereply.py
+-rw-r--r--   0        0        0      267 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placeresult.py
+-rw-r--r--   0        0        0     1651 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placesearchreply.py
+-rw-r--r--   0        0        0     2230 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placesearchrequest.py
+-rw-r--r--   0        0        0      884 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placesearchresult.py
+-rw-r--r--   0        0        0      675 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placesupplier.py
+-rw-r--r--   0        0        0      215 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/placeuser.py
+-rw-r--r--   0        0        0      621 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/location/qlocation.py
+-rw-r--r--   0        0        0      167 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/multimediawidgets/__init__.py
+-rw-r--r--   0        0        0     1353 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/multimediawidgets/graphicsvideoitem.py
+-rw-r--r--   0        0        0      872 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/multimediawidgets/videowidget.py
+-rw-r--r--   0        0        0     1172 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/__init__.py
+-rw-r--r--   0        0        0     8113 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/abstractsocket.py
+-rw-r--r--   0        0        0     1775 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/hostaddress.py
+-rw-r--r--   0        0        0     1465 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/httpmultipart.py
+-rw-r--r--   0        0        0      823 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/httppart.py
+-rw-r--r--   0        0        0     1310 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/localserver.py
+-rw-r--r--   0        0        0     2392 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/localsocket.py
+-rw-r--r--   0        0        0     2313 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/networkaccessmanager.py
+-rw-r--r--   0        0        0     2000 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/networkaddressentry.py
+-rw-r--r--   0        0        0     1551 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/networkcookie.py
+-rw-r--r--   0        0        0      850 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/networkcookiejar.py
+-rw-r--r--   0        0        0      627 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/networkdatagram.py
+-rw-r--r--   0        0        0     3011 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/networkinterface.py
+-rw-r--r--   0        0        0     3361 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/networkproxy.py
+-rw-r--r--   0        0        0     6462 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/networkrequest.py
+-rw-r--r--   0        0        0      779 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/tcpserver.py
+-rw-r--r--   0        0        0      178 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/tcpsocket.py
+-rw-r--r--   0        0        0      671 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/network/udpsocket.py
+-rw-r--r--   0        0        0       26 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/objbrowser/__init__.py
+-rw-r--r--   0        0        0     9193 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/objbrowser/attribute_model.py
+-rw-r--r--   0        0        0    14897 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/objbrowser/objectbrowser.py
+-rw-r--r--   0        0        0    17849 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/objbrowser/objectbrowsertreemodel.py
+-rw-r--r--   0        0        0      356 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/paths.py
+-rw-r--r--   0        0        0     1169 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/__init__.py
+-rw-r--r--   0        0        0      171 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/geoaddress.py
+-rw-r--r--   0        0        0     1149 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/geoareamonitorinfo.py
+-rw-r--r--   0        0        0     1260 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/geoareamonitorsource.py
+-rw-r--r--   0        0        0     1072 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/geocircle.py
+-rw-r--r--   0        0        0     1172 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/geocoordinate.py
+-rw-r--r--   0        0        0      706 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/geolocation.py
+-rw-r--r--   0        0        0     1021 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/geopath.py
+-rw-r--r--   0        0        0     1145 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/geopolygon.py
+-rw-r--r--   0        0        0     1687 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/geopositioninfo.py
+-rw-r--r--   0        0        0     2960 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/geopositioninfosource.py
+-rw-r--r--   0        0        0      769 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/georectangle.py
+-rw-r--r--   0        0        0     1861 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/geosatelliteinfo.py
+-rw-r--r--   0        0        0     1110 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/geosatelliteinfosource.py
+-rw-r--r--   0        0        0      755 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/geoshape.py
+-rw-r--r--   0        0        0     1196 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/positioning/nmeapositioninginfosource.py
+-rw-r--r--   0        0        0        0 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/py.typed
+-rw-r--r--   0        0        0      943 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qml/__init__.py
+-rw-r--r--   0        0        0     1212 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qml/jsengine.py
+-rw-r--r--   0        0        0     2397 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qml/jsvalue.py
+-rw-r--r--   0        0        0      295 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qml/jsvalueiterator.py
+-rw-r--r--   0        0        0      955 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qml/qmlapplicationengine.py
+-rw-r--r--   0        0        0      907 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qml/qmlcomponent.py
+-rw-r--r--   0        0        0     2020 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qml/qmlengine.py
+-rw-r--r--   0        0        0      536 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qml/qmlimageproviderbase.py
+-rw-r--r--   0        0        0      185 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qml/qmlparserstatus.py
+-rw-r--r--   0        0        0      251 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qt/Qsci/__init__.py
+-rw-r--r--   0        0        0      268 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qt/QtBluetooth/__init__.py
+-rw-r--r--   0        0        0      683 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qt/QtCharts/__init__.py
+-rw-r--r--   0        0        0     3505 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qt/QtCore/__init__.py
+-rw-r--r--   0        0        0      808 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qt/QtGui/__init__.py
+-rw-r--r--   0        0        0      303 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qt/QtHelp/__init__.py
+-rw-r--r--   0        0        0      335 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qt/QtLocation/__init__.py
+-rw-r--r--   0        0        0      327 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qt/QtMultimedia/__init__.py
+-rw-r--r--   0        0        0      355 2023-04-09 22:54:45.785043 prettyqt-1.1.0/prettyqt/qt/QtMultimediaWidgets/__init__.py
+-rw-r--r--   0        0        0      331 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/QtNetwork/__init__.py
+-rw-r--r--   0        0        0      331 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/QtPositioning/__init__.py
+-rw-r--r--   0        0        0      315 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/QtQml/__init__.py
+-rw-r--r--   0        0        0      323 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/QtQuick/__init__.py
+-rw-r--r--   0        0        0      307 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/QtScxml/__init__.py
+-rw-r--r--   0        0        0      601 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/QtStateMachine/__init__.py
+-rw-r--r--   0        0        0      381 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/QtSvg/__init__.py
+-rw-r--r--   0        0        0      319 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/QtTest/__init__.py
+-rw-r--r--   0        0        0      213 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/QtTextToSpeech/__init__.py.old
+-rw-r--r--   0        0        0      614 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/QtUiTools/__init__.py
+-rw-r--r--   0        0        0      330 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/QtWebChannel/__init__.py
+-rw-r--r--   0        0        0      715 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/QtWebEngineCore/__init__.py
+-rw-r--r--   0        0        0      351 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/QtWebEngineWidgets/__init__.py
+-rw-r--r--   0        0        0     1408 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/QtWidgets/__init__.py
+-rw-r--r--   0        0        0     1459 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qt/__init__.py
+-rw-r--r--   0        0        0      969 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qthelp/__init__.py
+-rw-r--r--   0        0        0      271 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qthelp/helpcontentitem.py
+-rw-r--r--   0        0        0      183 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qthelp/helpcontentmodel.py
+-rw-r--r--   0        0        0      460 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qthelp/helpcontentwidget.py
+-rw-r--r--   0        0        0      260 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qthelp/helpengine.py
+-rw-r--r--   0        0        0      978 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qthelp/helpenginecore.py
+-rw-r--r--   0        0        0      302 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qthelp/helpfilterengine.py
+-rw-r--r--   0        0        0      177 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qthelp/helpindexmodel.py
+-rw-r--r--   0        0        0      178 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qthelp/helpindexwidget.py
+-rw-r--r--   0        0        0      442 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qthelp/helpsearchengine.py
+-rw-r--r--   0        0        0      188 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qthelp/helpsearchquerywidget.py
+-rw-r--r--   0        0        0      216 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qthelp/helpsearchresult.py
+-rw-r--r--   0        0        0      403 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qthelp/helpsearchresultwidget.py
+-rw-r--r--   0        0        0     8290 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/qtre.py
+-rw-r--r--   0        0        0      868 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/quick/__init__.py
+-rw-r--r--   0        0        0      208 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/quick/quickasyncimageprovider.py
+-rw-r--r--   0        0        0      257 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/quick/quickimageprovider.py
+-rw-r--r--   0        0        0      239 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/quick/quickimageresponse.py
+-rw-r--r--   0        0        0     3753 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/quick/quickitem.py
+-rw-r--r--   0        0        0      519 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/quick/quickitemgrabresult.py
+-rw-r--r--   0        0        0     1495 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/quick/quickpainteditem.py
+-rw-r--r--   0        0        0      239 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/quick/quickrendercontrol.py
+-rw-r--r--   0        0        0      271 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/quick/quicktextdocument.py
+-rw-r--r--   0        0        0     1204 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/quick/quickview.py
+-rw-r--r--   0        0        0     3637 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/quick/quickwindow.py
+-rw-r--r--   0        0        0      123 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/scintilla/__init__.py
+-rw-r--r--   0        0        0     9347 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/scintilla/sciscintilla.py
+-rw-r--r--   0        0        0      193 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/scxml/__init__.py
+-rw-r--r--   0        0        0      362 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/scxml/scxmlcompiler.py
+-rw-r--r--   0        0        0      176 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/scxml/scxmlstatemachine.py
+-rw-r--r--   0        0        0      785 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/statemachine/__init__.py
+-rw-r--r--   0        0        0      361 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/statemachine/abstractstate.py
+-rw-r--r--   0        0        0     1159 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/statemachine/abstracttransition.py
+-rw-r--r--   0        0        0      220 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/statemachine/eventtransition.py
+-rw-r--r--   0        0        0      199 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/statemachine/finalstate.py
+-rw-r--r--   0        0        0     1104 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/statemachine/historystate.py
+-rw-r--r--   0        0        0      223 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/statemachine/keyeventtransition.py
+-rw-r--r--   0        0        0      227 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/statemachine/mouseeventtransition.py
+-rw-r--r--   0        0        0      222 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/statemachine/signaltransition.py
+-rw-r--r--   0        0        0     1276 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/statemachine/state.py
+-rw-r--r--   0        0        0     2222 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/statemachine/statemachine.py
+-rw-r--r--   0        0        0      368 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/svg/__init__.py
+-rw-r--r--   0        0        0      182 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/svg/graphicssvgitem.py
+-rw-r--r--   0        0        0      405 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/svg/svggenerator.py
+-rw-r--r--   0        0        0     1080 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/svg/svgrenderer.py
+-rw-r--r--   0        0        0      279 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/svg/svgwidget.py
+-rw-r--r--   0        0        0      675 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/syntaxhighlighters/__init__.py
+-rw-r--r--   0        0        0     1236 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/syntaxhighlighters/highlightrule.py
+-rw-r--r--   0        0        0     1271 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/syntaxhighlighters/jsonhighlighter.py
+-rw-r--r--   0        0        0     3178 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/syntaxhighlighters/markdownhighlighter.py
+-rw-r--r--   0        0        0      872 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/syntaxhighlighters/pygments/regularexpressionlexer.py
+-rw-r--r--   0        0        0     8585 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/syntaxhighlighters/pygmentshighlighter.py
+-rw-r--r--   0        0        0     4836 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/syntaxhighlighters/pythonhighlighter.py
+-rw-r--r--   0        0        0     2079 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/syntaxhighlighters/regexmatchhighlighter.py
+-rw-r--r--   0        0        0     2192 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/syntaxhighlighters/xmlhighlighter.py
+-rw-r--r--   0        0        0     2106 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/syntaxhighlighters/yamlhighlighter.py
+-rw-r--r--   0        0        0      180 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/texttospeech/__init__.py
+-rw-r--r--   0        0        0     1327 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/texttospeech/texttospeech.py
+-rw-r--r--   0        0        0      903 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/texttospeech/voice.py
+-rw-r--r--   0        0        0    15547 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/themes/darktheme.qss
+-rw-r--r--   0        0        0      845 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/utils/__init__.py
+-rw-r--r--   0        0        0     3561 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/utils/autoslot.py
+-rw-r--r--   0        0        0     3307 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/utils/colors.py
+-rw-r--r--   0        0        0     2337 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/utils/debugging.py
+-rw-r--r--   0        0        0     3598 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/utils/helpers.py
+-rw-r--r--   0        0        0      939 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/utils/mappers.py
+-rw-r--r--   0        0        0     1054 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/utils/prettyprinter.py
+-rw-r--r--   0        0        0     5546 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/utils/searchandreplacemixin.py
+-rw-r--r--   0        0        0      629 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/utils/signallogger.py
+-rw-r--r--   0        0        0     2306 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/utils/singleapplication.py
+-rw-r--r--   0        0        0      493 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/utils/singleton.py
+-rw-r--r--   0        0        0     2110 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/utils/syncedproperty.py
+-rw-r--r--   0        0        0     1887 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/utils/treeitem.py
+-rw-r--r--   0        0        0     3738 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/utils/types.py
+-rw-r--r--   0        0        0      303 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webchannel/__init__.py
+-rw-r--r--   0        0        0      228 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webchannel/webchannel.py
+-rw-r--r--   0        0        0     1337 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginecore/__init__.py
+-rw-r--r--   0        0        0     3315 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginecore/webenginecontextmenurequest.py
+-rw-r--r--   0        0        0     4498 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginecore/webenginedownloadrequest.py
+-rw-r--r--   0        0        0     1299 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginecore/webenginehistory.py
+-rw-r--r--   0        0        0      422 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginecore/webenginehistoryitem.py
+-rw-r--r--   0        0        0     1776 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginecore/webenginehttprequest.py
+-rw-r--r--   0        0        0    14262 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginecore/webenginepage.py
+-rw-r--r--   0        0        0     2461 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginecore/webengineprofile.py
+-rw-r--r--   0        0        0     1574 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginecore/webenginescript.py
+-rw-r--r--   0        0        0     1429 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginecore/webenginescriptcollection.py
+-rw-r--r--   0        0        0     7469 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginecore/webenginesettings.py
+-rw-r--r--   0        0        0     2044 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginecore/webengineurlscheme.py
+-rw-r--r--   0        0        0      282 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginecore/webengineurlschemehandler.py
+-rw-r--r--   0        0        0      330 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginewidgets/__init__.py
+-rw-r--r--   0        0        0     4602 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/webenginewidgets/webengineview.py
+-rw-r--r--   0        0        0    13430 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/widgets/__init__.py
+-rw-r--r--   0        0        0     3797 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/widgets/abstractbutton.py
+-rw-r--r--   0        0        0      406 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/widgets/abstractgraphicsshapeitem.py
+-rw-r--r--   0        0        0      257 2023-04-09 22:54:45.789044 prettyqt-1.1.0/prettyqt/widgets/abstractitemdelegate.py
+-rw-r--r--   0        0        0    11893 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/abstractitemview.py
+-rw-r--r--   0        0        0     5361 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/abstractscrollarea.py
+-rw-r--r--   0        0        0     5560 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/abstractslider.py
+-rw-r--r--   0        0        0     3715 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/abstractspinbox.py
+-rw-r--r--   0        0        0     8410 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/action.py
+-rw-r--r--   0        0        0     2143 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/actiongroup.py
+-rw-r--r--   0        0        0     7998 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/application.py
+-rw-r--r--   0        0        0     2754 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/boxlayout.py
+-rw-r--r--   0        0        0      342 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/buttongroup.py
+-rw-r--r--   0        0        0     2960 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/calendarwidget.py
+-rw-r--r--   0        0        0     1647 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/checkbox.py
+-rw-r--r--   0        0        0     3856 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/colordialog.py
+-rw-r--r--   0        0        0      331 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/columnview.py
+-rw-r--r--   0        0        0     7000 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/combobox.py
+-rw-r--r--   0        0        0      365 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/commandlinkbutton.py
+-rw-r--r--   0        0        0      281 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/commonstyle.py
+-rw-r--r--   0        0        0     3501 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/completer.py
+-rw-r--r--   0        0        0     2700 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/datawidgetmapper.py
+-rw-r--r--   0        0        0     1412 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/dateedit.py
+-rw-r--r--   0        0        0     4324 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/datetimeedit.py
+-rw-r--r--   0        0        0     1079 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/dial.py
+-rw-r--r--   0        0        0     2813 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/dialog.py
+-rw-r--r--   0        0        0     5950 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/dialogbuttonbox.py
+-rw-r--r--   0        0        0     2356 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/dockwidget.py
+-rw-r--r--   0        0        0     1772 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/doublespinbox.py
+-rw-r--r--   0        0        0      328 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/errormessage.py
+-rw-r--r--   0        0        0     7406 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/filedialog.py
+-rw-r--r--   0        0        0     1256 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/fileiconprovider.py
+-rw-r--r--   0        0        0     3513 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/filesystemmodel.py
+-rw-r--r--   0        0        0      289 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/focusframe.py
+-rw-r--r--   0        0        0     2477 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/fontcombobox.py
+-rw-r--r--   0        0        0      363 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/fontdialog.py
+-rw-r--r--   0        0        0     4998 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/formlayout.py
+-rw-r--r--   0        0        0     2540 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/frame.py
+-rw-r--r--   0        0        0     1822 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/gesture.py
+-rw-r--r--   0        0        0     2334 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsanchorlayout.py
+-rw-r--r--   0        0        0     1360 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsblureffect.py
+-rw-r--r--   0        0        0      469 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicscolorizeeffect.py
+-rw-r--r--   0        0        0      435 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsdropshadoweffect.py
+-rw-r--r--   0        0        0      416 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicseffect.py
+-rw-r--r--   0        0        0      559 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsellipseitem.py
+-rw-r--r--   0        0        0     3589 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsgridlayout.py
+-rw-r--r--   0        0        0     4694 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsitem.py
+-rw-r--r--   0        0        0      192 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsitemgroup.py
+-rw-r--r--   0        0        0     1173 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicslayout.py
+-rw-r--r--   0        0        0      262 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicslayoutitem.py
+-rw-r--r--   0        0        0     1098 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicslinearlayout.py
+-rw-r--r--   0        0        0      651 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicslineitem.py
+-rw-r--r--   0        0        0      700 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsobject.py
+-rw-r--r--   0        0        0      538 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsopacityeffect.py
+-rw-r--r--   0        0        0      209 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicspathitem.py
+-rw-r--r--   0        0        0     2241 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicspixmapitem.py
+-rw-r--r--   0        0        0      800 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicspolygonitem.py
+-rw-r--r--   0        0        0      198 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsproxywidget.py
+-rw-r--r--   0        0        0      542 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsrectitem.py
+-rw-r--r--   0        0        0      495 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsrotation.py
+-rw-r--r--   0        0        0      250 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsscale.py
+-rw-r--r--   0        0        0     8525 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsscene.py
+-rw-r--r--   0        0        0      293 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicssimpletextitem.py
+-rw-r--r--   0        0        0      707 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicstextitem.py
+-rw-r--r--   0        0        0      310 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicstransform.py
+-rw-r--r--   0        0        0     8390 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicsview.py
+-rw-r--r--   0        0        0     2770 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/graphicswidget.py
+-rw-r--r--   0        0        0     4159 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/gridlayout.py
+-rw-r--r--   0        0        0     1955 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/groupbox.py
+-rw-r--r--   0        0        0     5318 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/headerview.py
+-rw-r--r--   0        0        0     3755 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/inputdialog.py
+-rw-r--r--   0        0        0      190 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/itemdelegate.py
+-rw-r--r--   0        0        0      144 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/itemeditorcreatorbase.py
+-rw-r--r--   0        0        0     2331 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/itemeditorfactory.py
+-rw-r--r--   0        0        0      846 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/keysequenceedit.py
+-rw-r--r--   0        0        0     8483 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/label.py
+-rw-r--r--   0        0        0     3961 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/layout.py
+-rw-r--r--   0        0        0     1272 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/layoutitem.py
+-rw-r--r--   0        0        0     2416 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/lcdnumber.py
+-rw-r--r--   0        0        0     6525 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/lineedit.py
+-rw-r--r--   0        0        0     5606 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/listview.py
+-rw-r--r--   0        0        0     5823 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/listwidget.py
+-rw-r--r--   0        0        0     2851 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/listwidgetitem.py
+-rw-r--r--   0        0        0     6705 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/mainwindow.py
+-rw-r--r--   0        0        0     4584 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/mdiarea.py
+-rw-r--r--   0        0        0      689 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/mdisubwindow.py
+-rw-r--r--   0        0        0     4397 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/menu.py
+-rw-r--r--   0        0        0     2145 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/menubar.py
+-rw-r--r--   0        0        0     7314 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/messagebox.py
+-rw-r--r--   0        0        0      542 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/pangesture.py
+-rw-r--r--   0        0        0     1902 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/pinchgesture.py
+-rw-r--r--   0        0        0      415 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/plaintextdocumentlayout.py
+-rw-r--r--   0        0        0     9079 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/plaintextedit.py
+-rw-r--r--   0        0        0     3564 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/progressbar.py
+-rw-r--r--   0        0        0     1029 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/progressdialog.py
+-rw-r--r--   0        0        0      231 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/proxystyle.py
+-rw-r--r--   0        0        0      804 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/pushbutton.py
+-rw-r--r--   0        0        0      517 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/radiobutton.py
+-rw-r--r--   0        0        0      758 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/rubberband.py
+-rw-r--r--   0        0        0      611 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/scrollarea.py
+-rw-r--r--   0        0        0      707 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/scrollbar.py
+-rw-r--r--   0        0        0     3060 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/scroller.py
+-rw-r--r--   0        0        0     3937 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/scrollerproperties.py
+-rw-r--r--   0        0        0     1399 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/shortcut.py
+-rw-r--r--   0        0        0      309 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/sizegrip.py
+-rw-r--r--   0        0        0     5373 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/sizepolicy.py
+-rw-r--r--   0        0        0     2654 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/slider.py
+-rw-r--r--   0        0        0     1297 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/spaceritem.py
+-rw-r--r--   0        0        0     1837 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/spinbox.py
+-rw-r--r--   0        0        0     1181 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/splashscreen.py
+-rw-r--r--   0        0        0     3908 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/splitter.py
+-rw-r--r--   0        0        0     1417 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/splitterhandle.py
+-rw-r--r--   0        0        0      983 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/stackedlayout.py
+-rw-r--r--   0        0        0     1372 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/stackedwidget.py
+-rw-r--r--   0        0        0     1677 2023-04-09 22:54:45.793044 prettyqt-1.1.0/prettyqt/widgets/statusbar.py
+-rw-r--r--   0        0        0    19383 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/style.py
+-rw-r--r--   0        0        0      208 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleditemdelegate.py
+-rw-r--r--   0        0        0      126 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/stylefactory.py
+-rw-r--r--   0        0        0      318 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoption.py
+-rw-r--r--   0        0        0      686 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptionbutton.py
+-rw-r--r--   0        0        0      208 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptioncombobox.py
+-rw-r--r--   0        0        0      260 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptioncomplex.py
+-rw-r--r--   0        0        0      199 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptiondockwidget.py
+-rw-r--r--   0        0        0      197 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptionfocusrect.py
+-rw-r--r--   0        0        0      189 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptionframe.py
+-rw-r--r--   0        0        0      209 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptiongraphicsitem.py
+-rw-r--r--   0        0        0      197 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptiongroupbox.py
+-rw-r--r--   0        0        0      911 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptionheader.py
+-rw-r--r--   0        0        0     1032 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptionmenuitem.py
+-rw-r--r--   0        0        0      201 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptionprogressbar.py
+-rw-r--r--   0        0        0      199 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptionrubberband.py
+-rw-r--r--   0        0        0      208 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptionsizegrip.py
+-rw-r--r--   0        0        0     1046 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptionslider.py
+-rw-r--r--   0        0        0      195 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptionspinbox.py
+-rw-r--r--   0        0        0     1135 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptiontab.py
+-rw-r--r--   0        0        0      199 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptiontabbarbase.py
+-rw-r--r--   0        0        0      213 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptiontabwidgetframe.py
+-rw-r--r--   0        0        0      197 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptiontitlebar.py
+-rw-r--r--   0        0        0      397 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptiontoolbar.py
+-rw-r--r--   0        0        0     1176 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptiontoolbox.py
+-rw-r--r--   0        0        0      201 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptiontoolbutton.py
+-rw-r--r--   0        0        0     1344 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/styleoptionviewitem.py
+-rw-r--r--   0        0        0      397 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/stylepainter.py
+-rw-r--r--   0        0        0     1311 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/swipegesture.py
+-rw-r--r--   0        0        0     1732 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/systemtrayicon.py
+-rw-r--r--   0        0        0     5232 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/tabbar.py
+-rw-r--r--   0        0        0     3112 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/tableview.py
+-rw-r--r--   0        0        0     1085 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/tablewidget.py
+-rw-r--r--   0        0        0     3334 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/tablewidgetitem.py
+-rw-r--r--   0        0        0     1920 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/tablewidgetselectionrange.py
+-rw-r--r--   0        0        0    10591 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/tabwidget.py
+-rw-r--r--   0        0        0      392 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/tapandholdgesture.py
+-rw-r--r--   0        0        0      371 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/tapgesture.py
+-rw-r--r--   0        0        0     2400 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/textbrowser.py
+-rw-r--r--   0        0        0     6089 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/textedit.py
+-rw-r--r--   0        0        0     1526 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/timeedit.py
+-rw-r--r--   0        0        0     5008 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/toolbar.py
+-rw-r--r--   0        0        0     2568 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/toolbox.py
+-rw-r--r--   0        0        0     3175 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/toolbutton.py
+-rw-r--r--   0        0        0      710 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/tooltip.py
+-rw-r--r--   0        0        0     2532 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/treeview.py
+-rw-r--r--   0        0        0      630 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/treewidget.py
+-rw-r--r--   0        0        0     4841 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/treewidgetitem.py
+-rw-r--r--   0        0        0     4142 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/treewidgetitemiterator.py
+-rw-r--r--   0        0        0     1003 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/undoview.py
+-rw-r--r--   0        0        0      552 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/whatsthis.py
+-rw-r--r--   0        0        0    19395 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/widget.py
+-rw-r--r--   0        0        0      545 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/widgetaction.py
+-rw-r--r--   0        0        0      248 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/widgetitem.py
+-rw-r--r--   0        0        0     9052 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/wizard.py
+-rw-r--r--   0        0        0     1997 2023-04-09 22:54:45.797044 prettyqt-1.1.0/prettyqt/widgets/wizardpage.py
+-rw-r--r--   0        0        0     4767 2023-04-09 22:54:45.797044 prettyqt-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4515 1970-01-01 00:00:00.000000 prettyqt-1.1.0/PKG-INFO
```

### Comparing `prettyqt-1.0.0/LICENSE` & `prettyqt-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/docs/index.md` & `prettyqt-1.1.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/__init__.py` & `prettyqt-1.1.0/prettyqt/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Top-level package for PrettyQt."""
 
 __author__ = """Philipp Temminghoff"""
 __email__ = "phil65@kodi.tv"
-__version__ = "1.0.0"
+__version__ = "1.1.0"
 
 
 def debug():
     """Print the local variables in the caller's frame."""
     import inspect
 
     frame = inspect.currentframe()
```

### Comparing `prettyqt-1.0.0/prettyqt/__pyinstaller/hook-prettyqt.py` & `prettyqt-1.1.0/prettyqt/__pyinstaller/hook-prettyqt.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/bluetooth/__init__.py` & `prettyqt-1.1.0/prettyqt/bluetooth/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/bluetooth/bluetoothdevicediscoveryagent.py` & `prettyqt-1.1.0/prettyqt/bluetooth/bluetoothdevicediscoveryagent.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/bluetooth/bluetoothservicediscoveryagent.py` & `prettyqt-1.1.0/prettyqt/bluetooth/bluetoothservicediscoveryagent.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/bluetooth/bluetoothserviceinfo.py` & `prettyqt-1.1.0/prettyqt/bluetooth/bluetoothserviceinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/bluetooth/bluetoothuuid.py` & `prettyqt-1.1.0/prettyqt/bluetooth/bluetoothuuid.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/__init__.py` & `prettyqt-1.1.0/prettyqt/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/abstractaxis.py` & `prettyqt-1.1.0/prettyqt/charts/abstractaxis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/abstractbarseries.py` & `prettyqt-1.1.0/prettyqt/charts/abstractbarseries.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/abstractseries.py` & `prettyqt-1.1.0/prettyqt/charts/abstractseries.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/barcategoryaxis.py` & `prettyqt-1.1.0/prettyqt/charts/barcategoryaxis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/barset.py` & `prettyqt-1.1.0/prettyqt/charts/barset.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/boxset.py` & `prettyqt-1.1.0/prettyqt/charts/boxset.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/candlestickset.py` & `prettyqt-1.1.0/prettyqt/charts/candlestickset.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/categoryaxis.py` & `prettyqt-1.1.0/prettyqt/charts/categoryaxis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/chart.py` & `prettyqt-1.1.0/prettyqt/charts/chart.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/chartview.py` & `prettyqt-1.1.0/prettyqt/charts/chartview.py`

 * *Files 14% similar despite different names*

```diff
@@ -30,33 +30,34 @@
         self.setRenderHint(gui.Painter.RenderHint.Antialiasing)
         self.set_rubber_band("rectangle")
         # self.setDragMode(self.RubberBandDrag)
 
     def keyPressEvent(self, event: QtGui.QKeyEvent):
         """Handle keypress events to allow navigation via keyboard."""
         key = event.key()
-        if key == QtCore.Qt.Key.Key_Escape:
-            self.chart().zoomReset()
-        elif key == QtCore.Qt.Key.Key_Plus:
-            self.chart().zoom_by_factor(ZOOM_IN_FACTOR)
-        elif key == QtCore.Qt.Key.Key_Minus:
-            self.chart().zoom_by_factor(ZOOM_OUT_FACTOR)
-        elif key == QtCore.Qt.Key.Key_Left:
-            self.chart().scroll(-SCROLL_STEP_SIZE, 0)
-        elif key == QtCore.Qt.Key.Key_Right:
-            self.chart().scroll(SCROLL_STEP_SIZE, 0)
-        elif key == QtCore.Qt.Key.Key_Up:
-            self.chart().scroll(0, SCROLL_STEP_SIZE)
-        elif key == QtCore.Qt.Key.Key_Down:
-            self.chart().scroll(0, -SCROLL_STEP_SIZE)
-        elif key == QtCore.Qt.Key.Key_0:
-            self.chart().apply_nice_numbers()
-        else:
-            super().keyPressEvent(event)
-            return
+        match key:
+            case QtCore.Qt.Key.Key_Escape:
+                self.chart().zoomReset()
+            case QtCore.Qt.Key.Key_Plus:
+                self.chart().zoom_by_factor(ZOOM_IN_FACTOR)
+            case QtCore.Qt.Key.Key_Minus:
+                self.chart().zoom_by_factor(ZOOM_OUT_FACTOR)
+            case QtCore.Qt.Key.Key_Left:
+                self.chart().scroll(-SCROLL_STEP_SIZE, 0)
+            case QtCore.Qt.Key.Key_Right:
+                self.chart().scroll(SCROLL_STEP_SIZE, 0)
+            case QtCore.Qt.Key.Key_Up:
+                self.chart().scroll(0, SCROLL_STEP_SIZE)
+            case QtCore.Qt.Key.Key_Down:
+                self.chart().scroll(0, -SCROLL_STEP_SIZE)
+            case QtCore.Qt.Key.Key_0:
+                self.chart().apply_nice_numbers()
+            case _:
+                super().keyPressEvent(event)
+                return
         event.accept()
 
     def wheelEvent(self, event: QtGui.QWheelEvent):
         """Handle wheel event for zooming."""
         fct = ZOOM_IN_FACTOR if event.angleDelta().y() > 0 else ZOOM_OUT_FACTOR
         self.chart().zoom_by_factor(fct)
```

### Comparing `prettyqt-1.0.0/prettyqt/charts/legend.py` & `prettyqt-1.1.0/prettyqt/charts/legend.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/lineseries.py` & `prettyqt-1.1.0/prettyqt/charts/lineseries.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/pieslice.py` & `prettyqt-1.1.0/prettyqt/charts/pieslice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/polarchart.py` & `prettyqt-1.1.0/prettyqt/charts/polarchart.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/valueaxis.py` & `prettyqt-1.1.0/prettyqt/charts/valueaxis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/charts/xyseries.py` & `prettyqt-1.1.0/prettyqt/charts/xyseries.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/constants/__init__.py` & `prettyqt-1.1.0/prettyqt/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/__init__.py` & `prettyqt-1.1.0/prettyqt/core/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/_calendar.py` & `prettyqt-1.1.0/prettyqt/core/_calendar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/_datetime.py` & `prettyqt-1.1.0/prettyqt/core/_datetime.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/abstractanimation.py` & `prettyqt-1.1.0/prettyqt/core/abstractanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/abstractitemmodel.py` & `prettyqt-1.1.0/prettyqt/core/abstractitemmodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/animationgroup.py` & `prettyqt-1.1.0/prettyqt/core/animationgroup.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/basictimer.py` & `prettyqt-1.1.0/prettyqt/core/basictimer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/collator.py` & `prettyqt-1.1.0/prettyqt/core/collator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/commandlineparser.py` & `prettyqt-1.1.0/prettyqt/core/commandlineparser.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/coreapplication.py` & `prettyqt-1.1.0/prettyqt/core/coreapplication.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
+from collections.abc import Callable
 import logging
 import os
 import pathlib
 import sys
-from typing import Callable
 
 import prettyqt
 from prettyqt import constants, core
 from prettyqt.qt import QtCore
 from prettyqt.utils import InvalidParamError, types
```

### Comparing `prettyqt-1.0.0/prettyqt/core/cryptographichash.py` & `prettyqt-1.1.0/prettyqt/core/cryptographichash.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/datastream.py` & `prettyqt-1.1.0/prettyqt/core/datastream.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/deadlinetimer.py` & `prettyqt-1.1.0/prettyqt/core/deadlinetimer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/debug.py` & `prettyqt-1.1.0/prettyqt/core/debug.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/dir.py` & `prettyqt-1.1.0/prettyqt/core/dir.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/easingcurve.py` & `prettyqt-1.1.0/prettyqt/core/easingcurve.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
-from typing import Callable, Literal
+from collections.abc import Callable
+from typing import Literal
 
 from prettyqt.qt import QtCore
 from prettyqt.utils import InvalidParamError, bidict
 
 
 TYPE = bidict(
     linear=QtCore.QEasingCurve.Type.Linear,
```

### Comparing `prettyqt-1.0.0/prettyqt/core/elapsedtimer.py` & `prettyqt-1.1.0/prettyqt/core/elapsedtimer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/event.py` & `prettyqt-1.1.0/prettyqt/core/event.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/eventloop.py` & `prettyqt-1.1.0/prettyqt/core/eventloop.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/filedevice.py` & `prettyqt-1.1.0/prettyqt/core/filedevice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/fileinfo.py` & `prettyqt-1.1.0/prettyqt/core/fileinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/fileselector.py` & `prettyqt-1.1.0/prettyqt/core/fileselector.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/filesystemwatcher.py` & `prettyqt-1.1.0/prettyqt/core/filesystemwatcher.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/iodevice.py` & `prettyqt-1.1.0/prettyqt/core/iodevice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/itemselectionrange.py` & `prettyqt-1.1.0/prettyqt/core/itemselectionrange.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/jsondocument.py` & `prettyqt-1.1.0/prettyqt/core/jsondocument.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/jsonvalue.py` & `prettyqt-1.1.0/prettyqt/core/jsonvalue.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/library.py` & `prettyqt-1.1.0/prettyqt/core/library.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/libraryinfo.py` & `prettyqt-1.1.0/prettyqt/core/libraryinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/line.py` & `prettyqt-1.1.0/prettyqt/core/line.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/linef.py` & `prettyqt-1.1.0/prettyqt/core/linef.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/locale.py` & `prettyqt-1.1.0/prettyqt/core/locale.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/lockfile.py` & `prettyqt-1.1.0/prettyqt/core/lockfile.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/margins.py` & `prettyqt-1.1.0/prettyqt/core/margins.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/marginsf.py` & `prettyqt-1.1.0/prettyqt/core/marginsf.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/metaenum.py` & `prettyqt-1.1.0/prettyqt/core/metaenum.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/metamethod.py` & `prettyqt-1.1.0/prettyqt/core/metamethod.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/metaobject.py` & `prettyqt-1.1.0/prettyqt/core/metaobject.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/mimedata.py` & `prettyqt-1.1.0/prettyqt/core/mimedata.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/mimedatabase.py` & `prettyqt-1.1.0/prettyqt/core/mimedatabase.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/object.py` & `prettyqt-1.1.0/prettyqt/core/object.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/operatingsystemversion.py` & `prettyqt-1.1.0/prettyqt/core/operatingsystemversion.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/pluginloader.py` & `prettyqt-1.1.0/prettyqt/core/pluginloader.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/process.py` & `prettyqt-1.1.0/prettyqt/core/process.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/processenvironment.py` & `prettyqt-1.1.0/prettyqt/core/processenvironment.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/propertyanimation.py` & `prettyqt-1.1.0/prettyqt/core/propertyanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/rect.py` & `prettyqt-1.1.0/prettyqt/core/rect.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/regularexpression.py` & `prettyqt-1.1.0/prettyqt/core/regularexpression.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-from collections.abc import Iterator
-from typing import Callable, Literal
+from collections.abc import Callable, Iterator
+from typing import Literal
 
 from prettyqt import core, qt
 from prettyqt.qt import QtCore
 from prettyqt.utils import bidict
 
 
 mod = QtCore.QRegularExpression
```

### Comparing `prettyqt-1.0.0/prettyqt/core/regularexpressionmatch.py` & `prettyqt-1.1.0/prettyqt/core/regularexpressionmatch.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/regularexpressionmatchiterator.py` & `prettyqt-1.1.0/prettyqt/core/regularexpressionmatchiterator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/resource.py` & `prettyqt-1.1.0/prettyqt/core/resource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/settings.py` & `prettyqt-1.1.0/prettyqt/core/settings.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/size.py` & `prettyqt-1.1.0/prettyqt/core/size.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/sizef.py` & `prettyqt-1.1.0/prettyqt/core/sizef.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/socketnotifier.py` & `prettyqt-1.1.0/prettyqt/core/socketnotifier.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/sortfilterproxymodel.py` & `prettyqt-1.1.0/prettyqt/core/sortfilterproxymodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/standardpaths.py` & `prettyqt-1.1.0/prettyqt/core/standardpaths.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/storageinfo.py` & `prettyqt-1.1.0/prettyqt/core/storageinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/temporarydir.py` & `prettyqt-1.1.0/prettyqt/core/temporarydir.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/textboundaryfinder.py` & `prettyqt-1.1.0/prettyqt/core/textboundaryfinder.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/textstream.py` & `prettyqt-1.1.0/prettyqt/core/textstream.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/timeline.py` & `prettyqt-1.1.0/prettyqt/core/timeline.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
-from typing import Callable, Literal
+from collections.abc import Callable
+from typing import Literal
 
 from prettyqt import core
 from prettyqt.qt import QtCore
 from prettyqt.utils import InvalidParamError, bidict
 
 
 DIRECTION = bidict(
```

### Comparing `prettyqt-1.0.0/prettyqt/core/timer.py` & `prettyqt-1.1.0/prettyqt/core/timer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Callable
+from collections.abc import Callable
 
 from prettyqt import constants, core
 from prettyqt.qt import QtCore
 from prettyqt.utils import InvalidParamError, helpers
 
 
 class Timer(core.ObjectMixin, QtCore.QTimer):
```

### Comparing `prettyqt-1.0.0/prettyqt/core/timezone.py` & `prettyqt-1.1.0/prettyqt/core/timezone.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/translator.py` & `prettyqt-1.1.0/prettyqt/core/translator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/url.py` & `prettyqt-1.1.0/prettyqt/core/url.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/urlquery.py` & `prettyqt-1.1.0/prettyqt/core/urlquery.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/uuid.py` & `prettyqt-1.1.0/prettyqt/core/uuid.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/variantanimation.py` & `prettyqt-1.1.0/prettyqt/core/variantanimation.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import annotations
 
-from collections.abc import Iterator
-from typing import Callable
+from collections.abc import Callable, Iterator
 
 from prettyqt import core
 from prettyqt.qt import QtCore
 from prettyqt.utils import types
 
 
 class VariantAnimationMixin(core.AbstractAnimationMixin):
```

### Comparing `prettyqt-1.0.0/prettyqt/core/versionnumber.py` & `prettyqt-1.1.0/prettyqt/core/versionnumber.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/core/xmlstreamreader.py` & `prettyqt-1.1.0/prettyqt/core/xmlstreamreader.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_animations/bounceanimation.py` & `prettyqt-1.1.0/prettyqt/custom_animations/bounceanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_animations/fadeinanimation.py` & `prettyqt-1.1.0/prettyqt/custom_animations/fadeinanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_animations/slideanimation.py` & `prettyqt-1.1.0/prettyqt/custom_animations/slideanimation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_delegates/__init__.py` & `prettyqt-1.1.0/prettyqt/custom_delegates/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_delegates/buttondelegate.py` & `prettyqt-1.1.0/prettyqt/custom_delegates/buttondelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_delegates/checkboxdelegate.py` & `prettyqt-1.1.0/prettyqt/custom_delegates/checkboxdelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_delegates/icondelegate.py` & `prettyqt-1.1.0/prettyqt/custom_delegates/icondelegate.py`

 * *Files 25% similar despite different names*

```diff
@@ -30,33 +30,33 @@
         margin = 10
         mode = gui.Icon.Mode.Normal
 
         if not (option.state & widgets.Style.StateFlag.State_Enabled):
             mode = gui.Icon.Mode.Disabled
         elif option.state & widgets.Style.StateFlag.State_Selected:
             mode = gui.Icon.Mode.Selected
+        match value:
+            case QtGui.QPixmap():
+                icon = QtGui.QIcon(value)
+                option.decorationSize = int(value.size() / value.devicePixelRatio())
 
-        if isinstance(value, QtGui.QPixmap):
-            icon = QtGui.QIcon(value)
-            option.decorationSize = int(value.size() / value.devicePixelRatio())
+            case QtGui.QColor():
+                pixmap = QtGui.QPixmap(option.decorationSize)
+                pixmap.fill(value)
+                icon = QtGui.QIcon(pixmap)
 
-        elif isinstance(value, QtGui.QColor):
-            pixmap = QtGui.QPixmap(option.decorationSize)
-            pixmap.fill(value)
-            icon = QtGui.QIcon(pixmap)
+            case QtGui.QImage():
+                icon = QtGui.QIcon(QtGui.QPixmap.fromImage(value))
+                option.decorationSize = int(value.size() / value.devicePixelRatio())
 
-        elif isinstance(value, QtGui.QImage):
-            icon = QtGui.QIcon(QtGui.QPixmap.fromImage(value))
-            option.decorationSize = int(value.size() / value.devicePixelRatio())
-
-        elif isinstance(value, QtGui.QIcon):
-            is_on = option.state & widgets.Style.StateFlag.State_Open
-            state = gui.Icon.State.On if is_on else gui.Icon.State.Off
-            actual_size = option.icon.actualSize(option.decorationSize, mode, state)
-            option.decorationSize = option.decorationSize & actual_size
+            case QtGui.QIcon():
+                is_on = option.state & widgets.Style.StateFlag.State_Open
+                state = gui.Icon.State.On if is_on else gui.Icon.State.Off
+                actual_size = option.icon.actualSize(option.decorationSize, mode, state)
+                option.decorationSize = option.decorationSize & actual_size
         r = core.Rect(core.Point(), option.decorationSize)
         r.moveCenter(option.rect.center())
         r.setRight(option.rect.right() - margin)
         state = (
             gui.Icon.State.On
             if option.state & widgets.Style.StateFlag.State_Open
             else gui.Icon.State.Off
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_delegates/nofocusdelegate.py` & `prettyqt-1.1.0/prettyqt/custom_delegates/nofocusdelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_delegates/progressbardelegate.py` & `prettyqt-1.1.0/prettyqt/custom_delegates/progressbardelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_delegates/radiodelegate.py` & `prettyqt-1.1.0/prettyqt/custom_delegates/radiodelegate.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,33 +40,34 @@
 
         # set a property that will be used for the mask
         editor.setProperty("offMask", gui.Region(editor.rect()))  # type: ignore
         editor.installEventFilter(self)
         return editor
 
     def eventFilter(self, source: QtWidgets.QWidget, event: QtCore.QEvent) -> bool:
-        if event.type() == core.Event.Type.MouseButtonPress:
-            if isinstance(source, QtWidgets.QRadioButton):
-                if not source.parent().hasFocus():
-                    # the parent has no focus, set it and ignore the click
-                    source.parent().setFocus()
-                    return True
-            elif not source.hasFocus():
-                # the container has been clicked, check
-                source.setFocus()
-        elif event.type() == core.Event.Type.FocusIn:
-            # event received as a consequence of setFocus
-            # clear the mask to show it completely
-            source.clearMask()
-        elif event.type() == core.Event.Type.FocusOut:
-            # another widget has requested focus, set the mask
-            source.setMask(source.property(b"offMask"))
-            # update the table viewport to get rid of possible
-            # grid lines left after masking
-            source.parent().update()
+        match event.type():
+            case core.Event.Type.MouseButtonPress:
+                if isinstance(source, QtWidgets.QRadioButton):
+                    if not source.parent().hasFocus():
+                        # the parent has no focus, set it and ignore the click
+                        source.parent().setFocus()
+                        return True
+                elif not source.hasFocus():
+                    # the container has been clicked, check
+                    source.setFocus()
+            case core.Event.Type.FocusIn:
+                # event received as a consequence of setFocus
+                # clear the mask to show it completely
+                source.clearMask()
+            case core.Event.Type.FocusOut:
+                # another widget has requested focus, set the mask
+                source.setMask(source.property(b"offMask"))
+                # update the table viewport to get rid of possible
+                # grid lines left after masking
+                source.parent().update()
         return super().eventFilter(source, event)
 
     def updateEditorGeometry(
         self,
         editor: QtWidgets.QWidget,
         option: QtWidgets.QStyleOptionViewItem,
         index: QtCore.QModelIndex,
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_delegates/renderlinkdelegate.py` & `prettyqt-1.1.0/prettyqt/custom_delegates/renderlinkdelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_delegates/stardelegate.py` & `prettyqt-1.1.0/prettyqt/custom_delegates/stardelegate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_models/__init__.py` & `prettyqt-1.1.0/prettyqt/custom_models/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_models/columnitemmodel.py` & `prettyqt-1.1.0/prettyqt/custom_models/columnitemmodel.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
+from collections.abc import Callable
 from dataclasses import dataclass
 import logging
-from typing import Callable
 
 from prettyqt import constants, core, gui
 from prettyqt.qt import QtCore, QtGui
 
 
 logger = logging.getLogger(__name__)
 
@@ -133,31 +133,32 @@
         """Return the tree item at the given index and role."""
         if not index.isValid():
             return None
 
         col = index.column()
         tree_item = index.internalPointer()
 
-        if role in [constants.DISPLAY_ROLE, constants.EDIT_ROLE]:
-            val = self._attr_cols[col].get_label(tree_item)
-            return val.replace("\n", " ")
-        elif role == constants.DECORATION_ROLE:
-            return self._attr_cols[col].get_decoration(tree_item)
-        elif role == constants.CHECKSTATE_ROLE:
-            return self._attr_cols[col].get_checkstate(tree_item)
-        elif role == constants.ALIGNMENT_ROLE:
-            return self._attr_cols[col].get_alignment(tree_item)
-        elif role == constants.FOREGROUND_ROLE:
-            return self._attr_cols[col].get_foreground_color(tree_item)
-        elif role == constants.BACKGROUND_ROLE:
-            return self._attr_cols[col].get_background_color(tree_item)
-        elif role == constants.FONT_ROLE:
-            return self._attr_cols[col].get_font(tree_item)
-        else:
-            return None
+        match role:
+            case constants.DISPLAY_ROLE | constants.EDIT_ROLE:
+                val = self._attr_cols[col].get_label(tree_item)
+                return val.replace("\n", " ")
+            case constants.DECORATION_ROLE:
+                return self._attr_cols[col].get_decoration(tree_item)
+            case constants.CHECKSTATE_ROLE:
+                return self._attr_cols[col].get_checkstate(tree_item)
+            case constants.ALIGNMENT_ROLE:
+                return self._attr_cols[col].get_alignment(tree_item)
+            case constants.FOREGROUND_ROLE:
+                return self._attr_cols[col].get_foreground_color(tree_item)
+            case constants.BACKGROUND_ROLE:
+                return self._attr_cols[col].get_background_color(tree_item)
+            case constants.FONT_ROLE:
+                return self._attr_cols[col].get_font(tree_item)
+            case _:
+                return None
 
     def flags(self, index):
         if not index.isValid():
             return constants.NO_CHILDREN
         col = index.column()
         return self._attr_cols[col].get_flag()
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_models/importlibdistributionmodel.py` & `prettyqt-1.1.0/prettyqt/custom_models/importlibdistributionmodel.py`

 * *Files 10% similar despite different names*

```diff
@@ -49,36 +49,32 @@
         if role == constants.DISPLAY_ROLE:
             if orientation == constants.HORIZONTAL:
                 return self.HEADER[offset]
 
     def data(self, index, role=constants.DISPLAY_ROLE):
         if not index.isValid():
             return None
-        if role == constants.DISPLAY_ROLE:
-            if index.column() == 0:
-                dist = self.distributions[index.row()]
-                return dist.metadata["Name"]
-            elif index.column() == 1:
-                dist = self.distributions[index.row()]
-                return dist.version
-            elif index.column() == 2:
-                dist = self.distributions[index.row()]
-                return dist.metadata["Summary"]
-            elif index.column() == 3:
-                dist = self.distributions[index.row()]
-                return dist.metadata["Home-Page"]
-            elif index.column() == 4:
-                dist = self.distributions[index.row()]
-                return dist.metadata["Author"]
-            elif index.column() == 5:
-                dist = self.distributions[index.row()]
-                return dist.metadata["License"]
-        elif role == constants.USER_ROLE:
-            dist = self.distributions[index.row()]
-            return dist
+        dist = self.distributions[index.row()]
+        match role:
+            case constants.DISPLAY_ROLE:
+                match index.column():
+                    case 0:
+                        return dist.metadata["Name"]
+                    case 1:
+                        return dist.version
+                    case 2:
+                        return dist.metadata["Summary"]
+                    case 3:
+                        return dist.metadata["Home-Page"]
+                    case 4:
+                        return dist.metadata["Author"]
+                    case 5:
+                        return dist.metadata["License"]
+            case constants.USER_ROLE:
+                return dist
 
     @classmethod
     def from_system(
         cls, parent: QtCore.QObject | None = None
     ) -> ImportlibDistributionModel:
         distributions = list_system_modules()
         return cls(distributions, parent)
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_models/jsonmodel.py` & `prettyqt-1.1.0/prettyqt/custom_models/jsonmodel.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,27 +88,29 @@
         return True
 
     def data(self, index, role):
         if not index.isValid():
             return None
 
         item = index.internalPointer()
-        if role in [constants.DISPLAY_ROLE, constants.EDIT_ROLE]:
-            if index.column() == 0:
-                return repr(item.key)
-            elif index.column() == 1:
-                if item.type in (dict, list, tuple):
-                    return ""
-                else:
-                    if role == constants.DISPLAY_ROLE:
-                        return repr(item.value)
-                    else:
-                        return item.value
-            elif index.column() == 2:
-                return item.type.__name__
+        match role:
+            case constants.DISPLAY_ROLE | constants.EDIT_ROLE:
+                match index.column():
+                    case 0:
+                        return repr(item.key)
+                    case 1:
+                        if item.type in (dict, list, tuple):
+                            return ""
+                        else:
+                            if role == constants.DISPLAY_ROLE:
+                                return repr(item.value)
+                            else:
+                                return item.value
+                    case 2:
+                        return item.type.__name__
 
     def setData(self, index, value, role):
         if role == constants.EDIT_ROLE:
             if index.column() == 1:
                 item = index.internalPointer()
                 item.value = str(value)
                 self.update_row(index.row())
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_models/listmixin.py` & `prettyqt-1.1.0/prettyqt/custom_models/listmixin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from collections.abc import Iterable
-from typing import Any, Callable, Optional
+from collections.abc import Callable, Iterable
+from typing import Any
 
 from prettyqt import constants
 
 
 class ListMixin:
     remove_rows: Callable
     SORT_METHODS: dict[int, Callable]
@@ -61,20 +61,20 @@
     def sort(self, ncol: int, order):
         """Sort table by given column number."""
         is_asc = order == constants.ASCENDING
         if sorter := self.SORT_METHODS.get(ncol):
             with self.change_layout():
                 self.items.sort(key=sorter, reverse=is_asc)
 
-    def add(self, item: Any, position: Optional[int] = None):
+    def add(self, item: Any, position: int | None = None):
         """Append provided item to the list."""
         self.add_items(items=[item], position=position)
         return item
 
-    def add_items(self, items: Iterable[Any], position: Optional[int] = None):
+    def add_items(self, items: Iterable[Any], position: int | None = None):
         """Append a list of items to the list."""
         if position is None:
             position = len(self.items)
         items = list(items)
         with self.insert_rows(position, position + len(items) - 1):
             for i in range(len(items)):
                 self.items.insert(i + position, items[i])
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_models/modelmixin.py` & `prettyqt-1.1.0/prettyqt/custom_models/modelmixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable
+from collections.abc import Callable
 
 from prettyqt import constants
 
 
 class ModelMixin:
     DATA_ROLE = constants.USER_ROLE
     DTYPE_ROLE = constants.USER_ROLE + 1  # type: ignore
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_models/nesteditem.py` & `prettyqt-1.1.0/prettyqt/custom_models/nesteditem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_models/nestedmodel.py` & `prettyqt-1.1.0/prettyqt/custom_models/nestedmodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_models/regexmatchesmodel.py` & `prettyqt-1.1.0/prettyqt/custom_models/regexmatchesmodel.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,22 +22,23 @@
                 return self.HEADER[section]
 
     def data(self, index, role):
         if not index.isValid():
             return None
         item = self.matches[index.row()]
         if role in [constants.DISPLAY_ROLE]:
-            if index.column() == 0:
-                return str(item.span()[0])
-            if index.column() == 1:
-                return str(item.span()[1])
-            elif index.column() == 2:
-                return repr(item.group())
-            elif index.column() == 3:
-                return str(len(item.groups()))
+            match index.column():
+                case 0:
+                    return str(item.span()[0])
+                case 1:
+                    return str(item.span()[1])
+                case 2:
+                    return repr(item.group())
+                case 3:
+                    return str(len(item.groups()))
         if role in [constants.USER_ROLE]:
             return item.span()
 
     def rowCount(self, parent=None):
         """Override for AbstractitemModel base method."""
         return len(self.matches)
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_models/selectionmixin.py` & `prettyqt-1.1.0/prettyqt/custom_models/selectionmixin.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Callable
+from collections.abc import Callable
 
 from prettyqt import constants
 from prettyqt.qt import QtCore
 
 
 class SelectionMixin:
     CHECKSTATE: dict[int, Callable] = {}  # column: identifier
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_models/storageinfomodel.py` & `prettyqt-1.1.0/prettyqt/custom_models/storageinfomodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,28 +74,29 @@
 
     def rowCount(self, parent):
         return 0 if parent.isValid() else len(self.volumes)
 
     def data(self, index, role):
         if not index.isValid():
             return None
-        if role == constants.DISPLAY_ROLE:
-            volume = self.volumes[index.row()]
-            func = self.columnFuncMap.get(index.column())
-            if func is not None:
-                return func(volume)
+        match role:
+            case constants.DISPLAY_ROLE:
+                volume = self.volumes[index.row()]
+                func = self.columnFuncMap.get(index.column())
+                if func is not None:
+                    return func(volume)
 
-        elif role == constants.TOOLTIP_ROLE:
-            volume = self.volumes[index.row()]
-            tooltip = []
-            for column in range(self.ColumnCount):
-                label = self.columnNameMap.get(column)
-                value = self.columnFuncMap[column](volume)
-                tooltip.append(f"{label}: {value}")
-            return "\n".join(tooltip)
+            case constants.TOOLTIP_ROLE:
+                volume = self.volumes[index.row()]
+                tooltip = []
+                for column in range(self.ColumnCount):
+                    label = self.columnNameMap.get(column)
+                    value = self.columnFuncMap[column](volume)
+                    tooltip.append(f"{label}: {value}")
+                return "\n".join(tooltip)
 
     def headerData(self, section, orientation, role):
         if orientation != constants.HORIZONTAL:
             return None
         if role != constants.DISPLAY_ROLE:
             return None
         return self.columnNameMap.get(section)
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_models/subsequencesortfilterproxymodel.py` & `prettyqt-1.1.0/prettyqt/custom_models/subsequencesortfilterproxymodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_validators/__init__.py` & `prettyqt-1.1.0/prettyqt/custom_validators/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_validators/compositevalidator.py` & `prettyqt-1.1.0/prettyqt/custom_validators/compositevalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_validators/integervalidator.py` & `prettyqt-1.1.0/prettyqt/custom_validators/integervalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_validators/notemptyvalidator.py` & `prettyqt-1.1.0/prettyqt/custom_validators/notemptyvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_validators/notzerovalidator.py` & `prettyqt-1.1.0/prettyqt/custom_validators/notzerovalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_validators/pathvalidator.py` & `prettyqt-1.1.0/prettyqt/custom_validators/pathvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_validators/regexpatternvalidator.py` & `prettyqt-1.1.0/prettyqt/custom_validators/regexpatternvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_validators/regexvalidators.py` & `prettyqt-1.1.0/prettyqt/custom_validators/regexvalidators.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/__init__.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/booldicttoolbutton.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/booldicttoolbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/borderlayout.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/borderlayout.py`

 * *Files 5% similar despite different names*

```diff
@@ -76,80 +76,78 @@
         north_height = 0
         south_height = 0
 
         super().setGeometry(rect)
 
         for wrapper in self.items:
             item = wrapper.item
-            position = wrapper.position
+            match wrapper.position:
+                case BorderLayout.Position.North:
+                    geom = core.Rect(
+                        rect.x(), north_height, rect.width(), item.sizeHint().height()
+                    )
+                    item.setGeometry(geom)
+
+                    north_height += item.geometry().height() + self.spacing()
+
+                case BorderLayout.Position.South:
+                    geom = core.Rect(
+                        item.geometry().x(),
+                        item.geometry().y(),
+                        rect.width(),
+                        item.sizeHint().height(),
+                    )
+                    item.setGeometry(geom)
+
+                    south_height += item.geometry().height() + self.spacing()
+                    geom = core.Rect(
+                        rect.x(),
+                        rect.y() + rect.height() - south_height + self.spacing(),
+                        item.geometry().width(),
+                        item.geometry().height(),
+                    )
+                    item.setGeometry(geom)
 
-            if position == BorderLayout.Position.North:
-                geom = core.Rect(
-                    rect.x(), north_height, rect.width(), item.sizeHint().height()
-                )
-                item.setGeometry(geom)
-
-                north_height += item.geometry().height() + self.spacing()
-
-            elif position == BorderLayout.Position.South:
-                geom = core.Rect(
-                    item.geometry().x(),
-                    item.geometry().y(),
-                    rect.width(),
-                    item.sizeHint().height(),
-                )
-                item.setGeometry(geom)
-
-                south_height += item.geometry().height() + self.spacing()
-                geom = core.Rect(
-                    rect.x(),
-                    rect.y() + rect.height() - south_height + self.spacing(),
-                    item.geometry().width(),
-                    item.geometry().height(),
-                )
-                item.setGeometry(geom)
-
-            elif position == BorderLayout.Position.Center:
-                center = wrapper
+                case BorderLayout.Position.Center:
+                    center = wrapper
 
         center_height = rect.height() - north_height - south_height
 
         for wrapper in self.items:
             item = wrapper.item
-            position = wrapper.position
-
-            if position == BorderLayout.Position.West:
-                geom = core.Rect(
-                    rect.x() + west_width,
-                    north_height,
-                    item.sizeHint().width(),
-                    center_height,
-                )
-                item.setGeometry(geom)
-
-                west_width += item.geometry().width() + self.spacing()
-
-            elif position == BorderLayout.Position.East:
-                geom = core.Rect(
-                    item.geometry().x(),
-                    item.geometry().y(),
-                    item.sizeHint().width(),
-                    center_height,
-                )
-                item.setGeometry(geom)
-
-                east_width += item.geometry().width() + self.spacing()
-
-                geom = core.Rect(
-                    rect.x() + rect.width() - east_width + self.spacing(),
-                    north_height,
-                    item.geometry().width(),
-                    item.geometry().height(),
-                )
-                item.setGeometry(geom)
+            match wrapper.position:
+                case BorderLayout.Position.West:
+                    geom = core.Rect(
+                        rect.x() + west_width,
+                        north_height,
+                        item.sizeHint().width(),
+                        center_height,
+                    )
+                    item.setGeometry(geom)
+
+                    west_width += item.geometry().width() + self.spacing()
+
+                case BorderLayout.Position.East:
+                    geom = core.Rect(
+                        item.geometry().x(),
+                        item.geometry().y(),
+                        item.sizeHint().width(),
+                        center_height,
+                    )
+                    item.setGeometry(geom)
+
+                    east_width += item.geometry().width() + self.spacing()
+
+                    geom = core.Rect(
+                        rect.x() + rect.width() - east_width + self.spacing(),
+                        north_height,
+                        item.geometry().width(),
+                        item.geometry().height(),
+                    )
+                    item.setGeometry(geom)
 
         if center:
             rect = core.Rect(
                 west_width,
                 north_height,
                 rect.width() - east_width - west_width,
                 center_height,
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/codeeditor.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/codeeditor.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/collapsibleframe.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/collapsibleframe.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/colorchooserbutton.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/colorchooserbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/completionwidget.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/completionwidget.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,33 +46,32 @@
                 else:
                     self.cancel_completion()
 
         return super().eventFilter(obj, event)
 
     def keyPressEvent(self, event):
         key = event.key()
-        if key in (
-            QtCore.Qt.Key.Key_Return,
-            QtCore.Qt.Key.Key_Enter,
-            QtCore.Qt.Key.Key_Tab,
-        ):
-            self._complete_current()
-        elif key == QtCore.Qt.Key.Key_Escape:
-            self.hide()
-        elif key in (
-            QtCore.Qt.Key.Key_Up,
-            QtCore.Qt.Key.Key_Down,
-            QtCore.Qt.Key.Key_PageUp,
-            QtCore.Qt.Key.Key_PageDown,
-            QtCore.Qt.Key.Key_Home,
-            QtCore.Qt.Key.Key_End,
-        ):
-            return super().keyPressEvent(event)
-        else:
-            QtWidgets.QApplication.sendEvent(self._text_edit, event)
+        match key:
+            case (
+                QtCore.Qt.Key.Key_Return | QtCore.Qt.Key.Key_Enter | QtCore.Qt.Key.Key_Tab
+            ):
+                self._complete_current()
+            case QtCore.Qt.Key.Key_Escape:
+                self.hide()
+            case (
+                QtCore.Qt.Key.Key_Up
+                | QtCore.Qt.Key.Key_Down
+                | QtCore.Qt.Key.Key_PageUp
+                | QtCore.Qt.Key.Key_PageDown
+                | QtCore.Qt.Key.Key_Home
+                | QtCore.Qt.Key.Key_End
+            ):
+                return super().keyPressEvent(event)
+            case _:
+                QtWidgets.QApplication.sendEvent(self._text_edit, event)
 
     # 'QWidget' interface
 
     def hideEvent(self, event):
         """Disconnect signal handlers and event filter."""
         super().hideEvent(event)
         try:
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/dataset.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
-from collections.abc import Iterable, Mapping
+from collections.abc import Callable, Iterable, Mapping
 import functools
 import pathlib
-from typing import Any, Callable
+from typing import Any
 
 from prettyqt import custom_validators, custom_widgets, gui, widgets
 from prettyqt.utils import types
 
 
 class DataItem:
     def __init__(
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/elidedlabel.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/elidedlabel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/expandableline.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/expandableline.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/filechooserbutton.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/filechooserbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/flagselectionwidget.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/flagselectionwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/flowlayout.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/flowlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/fontchooserbutton.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/fontchooserbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/framelesswindow.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/framelesswindow.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/iconbrowser.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/iconbrowser.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/iconlabel.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/iconlabel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/iconwidget.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/iconwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/image.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/image.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/imageviewer.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/imageviewer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/inputandslider.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/inputandslider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/joystickbutton.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/joystickbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/labeledslider.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/labeledslider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/listinput.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/listinput.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/logtextedit.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/logtextedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/mappedcheckbox.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/mappedcheckbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/markdownwidget.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/markdownwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/menurecentfiles.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/menurecentfiles.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/notification.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/notification.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
+from collections.abc import Callable
 from queue import Empty, Queue
-from typing import Callable, Literal
+from typing import Literal
 
 from prettyqt import core, gui, widgets
 from prettyqt.qt import QtWidgets
 
 
 CURSOR_MARGIN_TOP = 10
 CURSOR_MARGIN_BOTTOM = 50
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/optionalwidget.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/optionalwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/popupinfo.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/popupinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/regexeditor/quick_ref.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/regexeditor/quick_ref.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/regexeditor/ref.html` & `prettyqt-1.1.0/prettyqt/custom_widgets/regexeditor/ref.html`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/regexeditor/regexeditorwidget.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/regexeditor/regexeditorwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/regexinput.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/regexinput.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/roundprogressbar.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/roundprogressbar.py`

 * *Files 10% similar despite different names*

```diff
@@ -133,70 +133,73 @@
             self._draw_base(painter, rect)
             self._draw_value(painter, rect, self.current_value)
             inner_rect, inner_radius = self._calculate_inner_rect(outer_radius)
             self._draw_inner_background(painter, inner_rect)
             self._draw_text(painter, inner_rect, inner_radius, self.current_value)
 
     def _draw_base(self, painter: gui.Painter, rect: core.RectF):
-        if self.bar_style == "donut":
-            color = self.palette().shadow().color()
-            painter.set_pen(color=color, width=self.outline_pen_width)
-            painter.setBrush(self.palette().base())
-            painter.drawEllipse(rect)
-        elif self.bar_style == "line":
-            base_color = self.palette().base().color()
-            painter.set_pen(color=base_color, width=self.outline_pen_width)
-            painter.setBrush(QtCore.Qt.BrushStyle.NoBrush)
-            width = self.outline_pen_width / 2
-            adjusted = rect.adjusted(width, width, -width, -width)
-            painter.drawEllipse(adjusted)
-        elif self.bar_style in ("pie", "expand"):
-            base_color = self.palette().base().color()
-            painter.set_pen(color=base_color, width=self.outline_pen_width)
-            painter.setBrush(self.palette().base())
-            painter.drawEllipse(rect)
+        match self.bar_style:
+            case "donut":
+                color = self.palette().shadow().color()
+                painter.set_pen(color=color, width=self.outline_pen_width)
+                painter.setBrush(self.palette().base())
+                painter.drawEllipse(rect)
+            case "line":
+                base_color = self.palette().base().color()
+                painter.set_pen(color=base_color, width=self.outline_pen_width)
+                painter.setBrush(QtCore.Qt.BrushStyle.NoBrush)
+                width = self.outline_pen_width / 2
+                adjusted = rect.adjusted(width, width, -width, -width)
+                painter.drawEllipse(adjusted)
+            case "pie" | "expand":
+                base_color = self.palette().base().color()
+                painter.set_pen(color=base_color, width=self.outline_pen_width)
+                painter.setBrush(self.palette().base())
+                painter.drawEllipse(rect)
 
     def _draw_value(self, painter: gui.Painter, rect: core.RectF, value: float):
         if value == self._min_value:
             return
         diff = self.current_value - self._min_value
         value_range = self._max_value - self._min_value
         delta = max(value_range / diff, 0)
-        if self.bar_style == "expand":
-            painter.setBrush(self.palette().highlight())
-            color = self.palette().shadow().color()
-            painter.set_pen(color=color, width=self.data_pen_width)
-            radius = (rect.height() / 2) / delta
-            painter.drawEllipse(rect.center(), radius, radius)
-        elif self.bar_style == "line":
-            color = self.palette().highlight().color()
-            painter.set_pen(color=color, width=self.data_pen_width)
-            painter.setBrush(QtCore.Qt.BrushStyle.NoBrush)
-            pen_width = self.outline_pen_width / 2
-            adjusted = rect.adjusted(pen_width, pen_width, -pen_width, -pen_width)
-            if value == self._max_value:
-                painter.drawEllipse(adjusted)
-            else:
-                arc_length = 360 / delta
-                painter.drawArc(adjusted, int(self.null_pos * 16), int(-arc_length * 16))
-        elif self.bar_style in ["donut", "pie"]:
-            data_path = gui.PainterPath()
-            data_path.set_fill_rule("winding")
-            if value == self._max_value:
-                data_path.addEllipse(rect)
-            else:
-                arc_length = 360 / delta
-                center_point = rect.center()
-                data_path.moveTo(center_point)
-                data_path.arcTo(rect, self.null_pos, -arc_length)
-                data_path.lineTo(center_point)
-            painter.setBrush(self.palette().highlight())
-            shadow_color = self.palette().shadow().color()
-            painter.set_pen(color=shadow_color, width=self.data_pen_width)
-            painter.drawPath(data_path)
+        match self.bar_style:
+            case "expand":
+                painter.setBrush(self.palette().highlight())
+                color = self.palette().shadow().color()
+                painter.set_pen(color=color, width=self.data_pen_width)
+                radius = (rect.height() / 2) / delta
+                painter.drawEllipse(rect.center(), radius, radius)
+            case "line":
+                color = self.palette().highlight().color()
+                painter.set_pen(color=color, width=self.data_pen_width)
+                painter.setBrush(QtCore.Qt.BrushStyle.NoBrush)
+                pen_width = self.outline_pen_width / 2
+                adjusted = rect.adjusted(pen_width, pen_width, -pen_width, -pen_width)
+                if value == self._max_value:
+                    painter.drawEllipse(adjusted)
+                else:
+                    arc_length = 360 / delta
+                    arc_length = int(-arc_length * 16)
+                    painter.drawArc(adjusted, int(self.null_pos * 16), arc_length)
+            case "donut" | "pie":
+                data_path = gui.PainterPath()
+                data_path.set_fill_rule("winding")
+                if value == self._max_value:
+                    data_path.addEllipse(rect)
+                else:
+                    arc_length = 360 / delta
+                    center_point = rect.center()
+                    data_path.moveTo(center_point)
+                    data_path.arcTo(rect, self.null_pos, -arc_length)
+                    data_path.lineTo(center_point)
+                painter.setBrush(self.palette().highlight())
+                shadow_color = self.palette().shadow().color()
+                painter.set_pen(color=shadow_color, width=self.data_pen_width)
+                painter.drawPath(data_path)
 
     def _calculate_inner_rect(self, outer_radius: float) -> tuple[core.RectF, float]:
         if self.bar_style in ("line", "expand"):
             inner_radius = outer_radius - self.outline_pen_width
         else:
             inner_radius = outer_radius * 0.75
         delta = (outer_radius - inner_radius) / 2
@@ -227,26 +230,28 @@
         painter.setFont(font)
         painter.setPen(self.palette().text().color())
         text = self._value_to_text(value)
         painter.drawText(inner_rect, constants.ALIGN_CENTER, text)  # type: ignore
 
     def _value_to_text(self, value: float) -> str:
         text_to_draw = self.number_format
-        if self._update_flags == "value":
-            val = round(value, self.decimals)
-            return text_to_draw.replace(r"%v", str(val))
-        elif self._update_flags == "percent":
-            pct = (value - self._min_value) / (self._max_value - self._min_value) * 100
-            val = round(pct, self.decimals)
-            return text_to_draw.replace(r"%p", str(val))
-        elif self._update_flags == "max":
-            val = round(self._max_value - self._min_value + 1, self.decimals)
-            return text_to_draw.replace(r"%m", str(val))
-        else:
-            return ValueError()
+        match self._update_flags:
+            case "value":
+                val = round(value, self.decimals)
+                return text_to_draw.replace(r"%v", str(val))
+            case "percent":
+                diff = self._max_value - self._min_value
+                pct = (value - self._min_value) / diff * 100
+                val = round(pct, self.decimals)
+                return text_to_draw.replace(r"%p", str(val))
+            case "max":
+                val = round(self._max_value - self._min_value + 1, self.decimals)
+                return text_to_draw.replace(r"%m", str(val))
+            case _:
+                return ValueError()
 
     def _value_format_changed(self):
         for k, v in VALUE_MAP.items():
             if k in self.number_format:
                 self._update_flags = v
         self.update()
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/selectionwidget.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/selectionwidget.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,22 +68,23 @@
     def add_custom(
         self,
         label: str = "Other",
         typ: TypeStr = "string",
         default: None | float | str = None,
         regex: str | None = None,
     ):
-        if typ == "string":
-            self.widget_custom = widgets.LineEdit()
-        elif typ == "int":
-            self.widget_custom = widgets.SpinBox()
-        elif typ == "float":
-            self.widget_custom = widgets.DoubleSpinBox()
-        else:
-            raise ValueError(typ)
+        match typ:
+            case "string":
+                self.widget_custom = widgets.LineEdit()
+            case "int":
+                self.widget_custom = widgets.SpinBox()
+            case "float":
+                self.widget_custom = widgets.DoubleSpinBox()
+            case _:
+                raise ValueError(typ)
         # TODO: Enable this or add BAR radio and option.
         self.widget_custom.set_disabled()  # type: ignore
         if default is not None:
             self.widget_custom.set_value(default)  # type: ignore
         self.rb_other.setText(label)
         self.rb_other.toggled.connect(self.widget_custom.set_enabled)  # type: ignore
         self.widget_custom.value_changed.connect(  # type: ignore
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/sidebarwidget.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/sidebarwidget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
-from typing import Callable, Literal
+from collections.abc import Callable
+from typing import Literal
 
 from prettyqt import constants, gui, iconprovider, widgets
 from prettyqt.qt import QtCore, QtWidgets
 from prettyqt.utils import types
 
 
 AreaStr = Literal["top", "bottom"]
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/singlelinetextedit.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/singlelinetextedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/spanslider.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/spanslider.py`

 * *Files 4% similar despite different names*

```diff
@@ -103,48 +103,45 @@
         m = self.style().pixelMetric(
             widgets.Style.PixelMetric.PM_MaximumDragDistance, opt, self
         )
         pixel_pos = self.pick(event.position()) - self.offset
         new_pos = float(self._pixel_pos_to_value(pixel_pos))
         if m >= 0:
             r = self.rect().adjusted(-m, -m, m, m)
-            if not r.contains(event.position()):
+            if not r.contains(event.position().toPoint()):
                 new_pos = self.position
 
         # pick the preferred handle on the first movement
         if self._first_movement:
             if self.lower_val == self.upper_val:
                 if new_pos < self.lower_value:
                     self._swap_controls()
                     self._first_movement = False
             else:
                 self._first_movement = False
 
-        if self.lower_pressed == HANDLE_STYLE:
-            if self.movement == "no_crossing":
+        match HANDLE_STYLE, self.movement:
+            case self.lower_pressed, "no_crossing":
                 new_pos = min(new_pos, self.upper_val)
-            elif self.movement == "no_overlap":
+                self.set_lower_pos(new_pos)
+            case self.lower_pressed, "no_overlap":
                 new_pos = min(new_pos, self.upper_val - 1)
-
-            if self.movement == "free" and new_pos > self.upper_val:
+                self.set_lower_pos(new_pos)
+            case self.lower_pressed, "free" if new_pos > self.upper_val:
                 self._swap_controls()
                 self.set_upper_pos(new_pos)
-            else:  # movement "none"
-                self.set_lower_pos(new_pos)
-        elif self.upper_pressed == HANDLE_STYLE:
-            if self.movement == "no_crossing":
+            case self.upper_pressed, "no_crossing":
                 new_pos = max(new_pos, self.lower_value)
-            elif self.movement == "no_overlap":
+                self.set_upper_pos(new_pos)
+            case self.upper_pressed, "no_overlap":
                 new_pos = max(new_pos, self.lower_value + 1)
-
-            if self.movement == "free" and new_pos < self.lower_val:
+                self.set_upper_pos(new_pos)
+            case self.upper_pressed, "free" if new_pos < self.lower_val:
                 self._swap_controls()
                 self.set_lower_pos(new_pos)
-            else:  # movement "none"
-                self.set_upper_pos(new_pos)
         event.accept()
 
     def mouseReleaseEvent(self, event):
         super().mouseReleaseEvent(event)
         self.setSliderDown(False)
         self.lower_pressed = self.upper_pressed = widgets.Style.SubControl.SC_None
         self.update()
@@ -301,54 +298,57 @@
         my_min = self.minimum()
         my_max = self.maximum()
         self._block_tracking = True
         main_control = main and self._main_control == "upper"
         alt_control = not main and self._main_control == "lower"
         is_upper_handle = main_control or alt_control
         val = self.upper_val if is_upper_handle else self.lower_val
-        if action == "single_step_add":
-            up = is_upper_handle
-            value = clamp(val + self.singleStep(), my_min, my_max)
-        elif action == "single_step_sub":
-            up = is_upper_handle
-            value = clamp(val - self.singleStep(), my_min, my_max)
-        elif action == "to_minimum":
-            up = is_upper_handle
-            value = my_min
-        elif action == "to_maximum":
-            up = is_upper_handle
-            value = my_max
-        elif action == "move":
-            up = is_upper_handle
-            no = True
-        elif action == "none":
-            no = True
+        match action:
+            case "single_step_add":
+                up = is_upper_handle
+                value = clamp(val + self.singleStep(), my_min, my_max)
+            case "single_step_sub":
+                up = is_upper_handle
+                value = clamp(val - self.singleStep(), my_min, my_max)
+            case "to_minimum":
+                up = is_upper_handle
+                value = my_min
+            case "to_maximum":
+                up = is_upper_handle
+                value = my_max
+            case "move":
+                up = is_upper_handle
+                no = True
+            case "none":
+                no = True
 
         if not no and not up:
-            if self.movement == "no_crossing":
-                value = min(value, self.upper_val)
-            elif self.movement == "no_overlap":
-                value = min(value, self.upper_val - 1)
+            match self.movement:
+                case "no_crossing":
+                    value = min(value, self.upper_val)
+                case "no_overlap":
+                    value = min(value, self.upper_val - 1)
 
-            if self.movement == "free" and value > self.upper_val:
-                self._swap_controls()
-                self.set_upper_pos(value)
-            else:
-                self.set_lower_pos(value)
+                case "free" if value > self.upper_val:
+                    self._swap_controls()
+                    self.set_upper_pos(value)
+                case "free":
+                    self.set_lower_pos(value)
         elif not no:
-            if self.movement == "no_crossing":
-                value = max(value, self.lower_val)
-            elif self.movement == "no_overlap":
-                value = max(value, self.lower_val + 1)
+            match self.movement:
+                case "no_crossing":
+                    value = max(value, self.lower_val)
+                case "no_overlap":
+                    value = max(value, self.lower_val + 1)
 
-            if self.movement == "free" and value < self.lower_val:
-                self._swap_controls()
-                self.set_lower_pos(value)
-            else:
-                self.set_upper_pos(value)
+                case "free" if value < self.lower_val:
+                    self._swap_controls()
+                    self.set_lower_pos(value)
+                case "free":
+                    self.set_upper_pos(value)
 
         self._block_tracking = False
         self.set_lower_value(self.lower_pos)
         self.set_upper_value(self.upper_pos)
 
     def _swap_controls(self):
         self.lower_val, self.upper_val = self.upper_val, self.lower_val
@@ -435,15 +435,17 @@
         return option
 
     def _handle_mouse_press(
         self, pos: QtCore.QPoint, control, value: float, handle: HandleStr
     ):
         opt = self.get_style_option(handle)
         old_control = control
-        control = self.style().hitTestComplexControl(SLIDER_STYLE, opt, pos, self)
+        control = self.style().hitTestComplexControl(
+            SLIDER_STYLE, opt, pos.toPoint(), self
+        )
         sr = self.style().subControlRect(SLIDER_STYLE, opt, HANDLE_STYLE, self)
         if control == HANDLE_STYLE:
             self.position = value
             self.offset = self.pick(pos - sr.topLeft())
             self.last_pressed = handle
             self.setSliderDown(True)
             self.slider_pressed.emit(handle)
@@ -494,14 +496,15 @@
         self.label_upper.set_text(str(self.slider.upper_pos))
 
 
 if __name__ == "__main__":
     app = widgets.app()
     layout = widgets.BoxLayout("horizontal")
     slider = SpanSliderWidget()
+    # slider.set_movement_mode("free")
     slider.set_span(30, 70)
     slider.setRange(0, 100)
     slider.value_changed.connect(print)
     # color = gui.Color("blue").lighter(150)
     # slider.set_left_color(color)
     # slider.set_right_color(color)
     slider.show()
```

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/standardiconswidget.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/standardiconswidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/stringornumberwidget.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/stringornumberwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/subsequencecompleter.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/subsequencecompleter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/timeline.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/timeline.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/custom_widgets/waitingspinner.py` & `prettyqt-1.1.0/prettyqt/custom_widgets/waitingspinner.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/eventfilters/animatedtooltipeventfilter.py` & `prettyqt-1.1.0/prettyqt/eventfilters/animatedtooltipeventfilter.py`

 * *Files 9% similar despite different names*

```diff
@@ -18,42 +18,44 @@
         self.slide_anim = custom_animations.SlideAnimation(duration=1000)
         self.slide_anim.apply_to(self.tool_tip)
         self.fade_anim = custom_animations.FadeInAnimation(duration=1000)
         self.fade_anim.apply_to(self.tool_tip)
         self.animation = self.slide_anim | self.fade_anim
 
     def eventFilter(self, obj: QtWidgets.QAbstractButton, event: QtCore.QEvent):
-        if event.type() == QtCore.QEvent.Type.Enter:
-            # self.tool_tip.adjustSize()
-            self.tool_tip.setText(obj.toolTip())
-            self.tool_tip.show()
-            position = "bottom"
-            distance = 100
-            center = obj.rect().center()
-            if position == "top":
-                center.setY(obj.rect().bottom())
-                delta = core.Point(0, distance)
-            elif position == "bottom":
-                center.setY(obj.rect().top())
-                delta = core.Point(0, -distance)
-            elif position == "left":
-                center.setX(obj.rect().right())
-                delta = core.Point(distance, 0)
-            elif position == "right":
-                center.setX(obj.rect().left())
-                delta = core.Point(-distance, 0)
-            center = obj.mapToGlobal(center)
-            self.slide_anim.set_start_value(center + delta)
-            self.slide_anim.set_end_value(center)
-            self.animation.start_animation()
-        elif event.type() == QtCore.QEvent.Type.Leave:
-            self.tool_tip.hide()
-            self.animation.stop()
-        elif event.type() == QtCore.QEvent.Type.ToolTip:
-            return True
+        match event.type():
+            case QtCore.QEvent.Type.Enter:
+                # self.tool_tip.adjustSize()
+                self.tool_tip.setText(obj.toolTip())
+                self.tool_tip.show()
+                position = "bottom"
+                distance = 100
+                center = obj.rect().center()
+                match position:
+                    case "top":
+                        center.setY(obj.rect().bottom())
+                        delta = core.Point(0, distance)
+                    case "bottom":
+                        center.setY(obj.rect().top())
+                        delta = core.Point(0, -distance)
+                    case "left":
+                        center.setX(obj.rect().right())
+                        delta = core.Point(distance, 0)
+                    case "right":
+                        center.setX(obj.rect().left())
+                        delta = core.Point(-distance, 0)
+                center = obj.mapToGlobal(center)
+                self.slide_anim.set_start_value(center + delta)
+                self.slide_anim.set_end_value(center)
+                self.animation.start_animation()
+            case QtCore.QEvent.Type.Leave:
+                self.tool_tip.hide()
+                self.animation.stop()
+            case QtCore.QEvent.Type.ToolTip:
+                return True
         return super().eventFilter(obj, event)
 
 
 if __name__ == "__main__":
     app = widgets.app()
     w = widgets.ToolButton()
     ef = AnimatedToolTipEventFilter()
```

### Comparing `prettyqt-1.0.0/prettyqt/eventfilters/hovericoneventfilter.py` & `prettyqt-1.1.0/prettyqt/eventfilters/hovericoneventfilter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/__init__.py` & `prettyqt-1.1.0/prettyqt/gui/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -126,15 +126,17 @@
 from .textblockgroup import TextBlockGroup
 from .textframe import TextFrame
 from .abstracttextdocumentlayout import (
     AbstractTextDocumentLayout,
     AbstractTextDocumentLayoutMixin,
 )
 from .syntaxhighlighter import SyntaxHighlighter
-
+from .undocommand import UndoCommand
+from .undostack import UndoStack
+from .undogroup import UndoGroup
 from .colorspace import ColorSpace
 
 
 def app(args: list[str] | None = None) -> GuiApplication:
     instance = GuiApplication.instance()
     if instance is not None:
         return instance
@@ -243,14 +245,17 @@
     "TextCharFormat",
     "TextCharFormatMixin",
     "TextImageFormat",
     "TextListFormat",
     "TextTableCellFormat",
     "TextCursor",
     "SyntaxHighlighter",
+    "UndoCommand",
+    "UndoStack",
+    "UndoGroup",
     "PdfWriter",
     "KeySequence",
     "Surface",
     "SurfaceMixin",
     "Window",
     "WindowMixin",
     "DesktopServices",
```

### Comparing `prettyqt-1.0.0/prettyqt/gui/abstracttextdocumentlayout.py` & `prettyqt-1.1.0/prettyqt/gui/abstracttextdocumentlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/brush.py` & `prettyqt-1.1.0/prettyqt/gui/brush.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/clipboard.py` & `prettyqt-1.1.0/prettyqt/gui/clipboard.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/color.py` & `prettyqt-1.1.0/prettyqt/gui/color.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,54 +112,58 @@
             if percent == 100:
                 return cls(*end.getRgb())
             else:
                 return cls(*start.getRgb())
         if colorspace not in SPEC:
             raise InvalidParamError(colorspace, SPEC)
         out = cls()
-        if colorspace == "rgb":
-            components = helpers.get_color_percentage(
-                start.getRgb(), end.getRgb(), percent  # type: ignore
-            )
-            out.setRgb(*components)
-        elif colorspace == "hsv":
-            components = helpers.get_color_percentage(
-                start.getHsv(), end.getHsv(), percent  # type: ignore
-            )
-            out.setHsv(*components)
-        elif colorspace == "hsl":
-            components = helpers.get_color_percentage(
-                start.getHsl(), end.getHsl(), percent  # type: ignore
-            )
-            out.setHsl(*components)
-        else:
-            raise ValueError("Invalid colorspace!")
+        match colorspace:
+            case "rgb":
+                components = helpers.get_color_percentage(
+                    start.getRgb(), end.getRgb(), percent  # type: ignore
+                )
+                out.setRgb(*components)
+            case "hsv":
+                components = helpers.get_color_percentage(
+                    start.getHsv(), end.getHsv(), percent  # type: ignore
+                )
+                out.setHsv(*components)
+            case "hsl":
+                components = helpers.get_color_percentage(
+                    start.getHsl(), end.getHsl(), percent  # type: ignore
+                )
+                out.setHsl(*components)
+            case _:
+                raise ValueError("Invalid colorspace!")
         out = out.convertTo(start.spec())
         return out
 
     def is_dark(self) -> bool:
         """Check whether a color is 'dark'."""
         return self.lightness() < 128
 
     def get_name(self, name_format: NameStr = "hex_argb") -> str:
-        if name_format == "svg_rgb":
-            if not self.isValid():
-                return 'fill=""'
-            return f'fill="rgb({self.red()}, {self.green()}, {self.blue()})"'
-        elif name_format == "svg_argb":
-            if not self.isValid():
-                return 'fill=""'
-            fill_str = f"rgb({self.red()}, {self.green()}, {self.blue()})"
-            return f'fill="{fill_str}" fill-opacity="{self.alpha()}"'
-        elif name_format == "qcss_argb":
-            return f"rgba({self.red()}, {self.green()}, {self.blue()}, {self.alpha()})"
-        elif name_format == "qcss_rgb":
-            return f"rgb({self.red()}, {self.green()}, {self.blue()})"
-        else:
-            return self.name(NAME_FORMAT[name_format])
+        match name_format:
+            case "svg_rgb":
+                if not self.isValid():
+                    return 'fill=""'
+                return f'fill="rgb({self.red()}, {self.green()}, {self.blue()})"'
+            case "svg_argb":
+                if not self.isValid():
+                    return 'fill=""'
+                fill_str = f"rgb({self.red()}, {self.green()}, {self.blue()})"
+                return f'fill="{fill_str}" fill-opacity="{self.alpha()}"'
+            case "qcss_argb":
+                return (
+                    f"rgba({self.red()}, {self.green()}, {self.blue()}, {self.alpha()})"
+                )
+            case "qcss_rgb":
+                return f"rgb({self.red()}, {self.green()}, {self.blue()})"
+            case _:
+                return self.name(NAME_FORMAT[name_format])
 
     @deprecated(reason="This method is deprecated, use Color.get_name instead.")
     def to_qsscolor(self) -> str:
         """Convert Color to a string that can be used in a QStyleSheet."""
         return f"rgba({self.red()}, {self.green()}, {self.blue()}, {self.alpha()})"
 
     def as_qt(self) -> QtGui.QColor:
```

### Comparing `prettyqt-1.0.0/prettyqt/gui/colorspace.py` & `prettyqt-1.1.0/prettyqt/gui/colorspace.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/cursor.py` & `prettyqt-1.1.0/prettyqt/gui/cursor.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/doublevalidator.py` & `prettyqt-1.1.0/prettyqt/gui/doublevalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/drag.py` & `prettyqt-1.1.0/prettyqt/gui/drag.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/font.py` & `prettyqt-1.1.0/prettyqt/gui/font.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/fontdatabase.py` & `prettyqt-1.1.0/prettyqt/gui/fontdatabase.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/fontmetrics.py` & `prettyqt-1.1.0/prettyqt/gui/fontmetrics.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/fontmetricsf.py` & `prettyqt-1.1.0/prettyqt/gui/fontmetricsf.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/gradient.py` & `prettyqt-1.1.0/prettyqt/gui/gradient.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/guiapplication.py` & `prettyqt-1.1.0/prettyqt/gui/guiapplication.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/icon.py` & `prettyqt-1.1.0/prettyqt/gui/icon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/iconengine.py` & `prettyqt-1.1.0/prettyqt/gui/iconengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/image.py` & `prettyqt-1.1.0/prettyqt/gui/image.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
 from prettyqt import core, gui
-from prettyqt.qt import QtGui
+from prettyqt.qt import API, QtGui
 
 
 class Image(gui.PaintDeviceMixin, QtGui.QImage):
     def __getstate__(self):
         return bytes(self)
 
     def __setstate__(self, ba):
@@ -35,11 +35,25 @@
         return cls(arr.data, width, height, channel * width, cls.Format.Format_RGB888)
 
     def invert_pixels(self, invert_alpha: bool = False):
         self.invertPixels(
             self.InvertMode.InvertRgba if invert_alpha else self.InvertMode.InvertRgb
         )
 
+    def as_bytes(self) -> bytes | None:
+        bits = self.bits()
+        if bits is None:
+            return None
+        match API:
+            case "pyqt5":
+                return bits.asstring(self.byteCount())
+            case "pyqt6":
+                return bits.asstring(self.sizeInBytes())
+            case "pyside6":
+                return bits.tobytes()
+
 
 if __name__ == "__main__":
-    image = Image()
-    bytes(image)
+    app = gui.app()
+    image = gui.Pixmap(100, 100).toImage()
+    image = Image(image)
+    print(len(bytes(image)))
```

### Comparing `prettyqt-1.0.0/prettyqt/gui/imageiohandler.py` & `prettyqt-1.1.0/prettyqt/gui/imageiohandler.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/imagereader.py` & `prettyqt-1.1.0/prettyqt/gui/imagereader.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/imagewriter.py` & `prettyqt-1.1.0/prettyqt/gui/imagewriter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/inputmethod.py` & `prettyqt-1.1.0/prettyqt/gui/inputmethod.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/intvalidator.py` & `prettyqt-1.1.0/prettyqt/gui/intvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/keysequence.py` & `prettyqt-1.1.0/prettyqt/gui/keysequence.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/lineargradient.py` & `prettyqt-1.1.0/prettyqt/gui/lineargradient.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/movie.py` & `prettyqt-1.1.0/prettyqt/gui/movie.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/pagelayout.py` & `prettyqt-1.1.0/prettyqt/gui/pagelayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/pagesize.py` & `prettyqt-1.1.0/prettyqt/gui/pagesize.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/paintdevice.py` & `prettyqt-1.1.0/prettyqt/gui/paintdevice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/painter.py` & `prettyqt-1.1.0/prettyqt/gui/painter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/painterpath.py` & `prettyqt-1.1.0/prettyqt/gui/painterpath.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/painterpathstroker.py` & `prettyqt-1.1.0/prettyqt/gui/painterpathstroker.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/palette.py` & `prettyqt-1.1.0/prettyqt/gui/palette.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/pdfwriter.py` & `prettyqt-1.1.0/prettyqt/gui/pdfwriter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/pen.py` & `prettyqt-1.1.0/prettyqt/gui/pen.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/pixmap.py` & `prettyqt-1.1.0/prettyqt/gui/pixmap.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/pixmapcache.py` & `prettyqt-1.1.0/prettyqt/gui/pixmapcache.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/polygon.py` & `prettyqt-1.1.0/prettyqt/gui/polygon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/polygonf.py` & `prettyqt-1.1.0/prettyqt/gui/polygonf.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/radialgradient.py` & `prettyqt-1.1.0/prettyqt/gui/radialgradient.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/region.py` & `prettyqt-1.1.0/prettyqt/gui/region.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/regularexpressionvalidator.py` & `prettyqt-1.1.0/prettyqt/gui/regularexpressionvalidator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/screen.py` & `prettyqt-1.1.0/prettyqt/gui/screen.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/sessionmanager.py` & `prettyqt-1.1.0/prettyqt/gui/sessionmanager.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/standarditem.py` & `prettyqt-1.1.0/prettyqt/gui/standarditem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/standarditemmodel.py` & `prettyqt-1.1.0/prettyqt/gui/standarditemmodel.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/statictext.py` & `prettyqt-1.1.0/prettyqt/gui/statictext.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/surface.py` & `prettyqt-1.1.0/prettyqt/gui/surface.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/syntaxhighlighter.py` & `prettyqt-1.1.0/prettyqt/gui/syntaxhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textblock.py` & `prettyqt-1.1.0/prettyqt/gui/textblock.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textblockgroup.py` & `prettyqt-1.1.0/prettyqt/gui/textblockgroup.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textblockuserdata.py` & `prettyqt-1.1.0/prettyqt/gui/textblockuserdata.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textcharformat.py` & `prettyqt-1.1.0/prettyqt/gui/textcharformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textcursor.py` & `prettyqt-1.1.0/prettyqt/gui/textcursor.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textdocument.py` & `prettyqt-1.1.0/prettyqt/gui/textdocument.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textdocumentfragment.py` & `prettyqt-1.1.0/prettyqt/gui/textdocumentfragment.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textdocumentwriter.py` & `prettyqt-1.1.0/prettyqt/gui/textdocumentwriter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textformat.py` & `prettyqt-1.1.0/prettyqt/gui/textformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textframe.py` & `prettyqt-1.1.0/prettyqt/gui/textframe.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textframeformat.py` & `prettyqt-1.1.0/prettyqt/gui/textframeformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textlayout.py` & `prettyqt-1.1.0/prettyqt/gui/textlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textlength.py` & `prettyqt-1.1.0/prettyqt/gui/textlength.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textline.py` & `prettyqt-1.1.0/prettyqt/gui/textline.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textlistformat.py` & `prettyqt-1.1.0/prettyqt/gui/textlistformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/textoption.py` & `prettyqt-1.1.0/prettyqt/gui/textoption.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/texttablecellformat.py` & `prettyqt-1.1.0/prettyqt/gui/texttablecellformat.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/transform.py` & `prettyqt-1.1.0/prettyqt/gui/transform.py`

 * *Files 10% similar despite different names*

```diff
@@ -36,34 +36,37 @@
         return type(self), (), self.__getstate__()
 
     def __setstate__(self, ba):
         core.DataStream.write_bytearray(ba, self)
 
     def __getitem__(self, value: tuple[int, int]) -> float:
         if value[0] == 0:
-            if value[1] == 0:
-                return self.m11()
-            elif value[1] == 1:
-                return self.m12()
-            elif value[1] == 2:
-                return self.m13()
+            match value[1]:
+                case 0:
+                    return self.m11()
+                case 1:
+                    return self.m12()
+                case 2:
+                    return self.m13()
         elif value[0] == 1:
-            if value[1] == 0:
-                return self.m21()
-            elif value[1] == 1:
-                return self.m22()
-            elif value[1] == 2:
-                return self.m23()
+            match value[1]:
+                case 0:
+                    return self.m21()
+                case 1:
+                    return self.m22()
+                case 2:
+                    return self.m23()
         elif value[0] == 2:
-            if value[1] == 0:
-                return self.m31()
-            elif value[1] == 1:
-                return self.m32()
-            elif value[1] == 2:
-                return self.m33()
+            match value[1]:
+                case 0:
+                    return self.m31()
+                case 1:
+                    return self.m32()
+                case 2:
+                    return self.m33()
         raise ValueError(f"Wrong value {value}")
 
     def __bytes__(self):
         ba = core.DataStream.create_bytearray(self)
         return bytes(ba)
 
     @classmethod
```

### Comparing `prettyqt-1.0.0/prettyqt/gui/validator.py` & `prettyqt-1.1.0/prettyqt/gui/validator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/vector3d.py` & `prettyqt-1.1.0/prettyqt/gui/vector3d.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/vector4d.py` & `prettyqt-1.1.0/prettyqt/gui/vector4d.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/gui/window.py` & `prettyqt-1.1.0/prettyqt/gui/window.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/__init__.py` & `prettyqt-1.1.0/prettyqt/iconprovider/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/animation.py` & `prettyqt-1.1.0/prettyqt/iconprovider/animation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/awesomequickimageprovider.py` & `prettyqt-1.1.0/prettyqt/iconprovider/awesomequickimageprovider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/chariconengine.py` & `prettyqt-1.1.0/prettyqt/iconprovider/chariconengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/codicon-charmap.json` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/codicon-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/codicon.ttf` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/codicon.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/elusiveicons-webfont-charmap.json` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/elusiveicons-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/elusiveicons-webfont.ttf` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/elusiveicons-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont-charmap.json` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont.ttf` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/fontawesome5-brands-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont-charmap.json` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont.ttf` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/fontawesome5-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont-charmap.json` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont.ttf` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/fontawesome5-solid-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont-charmap.json` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont.ttf` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/materialdesignicons5-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont-charmap.json` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont.ttf` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/materialdesignicons6-webfont.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/phosphor-charmap.json` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/phosphor-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/phosphor.ttf` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/phosphor.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/remixicon-charmap.json` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/remixicon-charmap.json`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/fonts/remixicon.ttf` & `prettyqt-1.1.0/prettyqt/iconprovider/fonts/remixicon.ttf`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/iconic_font.py` & `prettyqt-1.1.0/prettyqt/iconprovider/iconic_font.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/iconprovider/svgbuffericonengine.py` & `prettyqt-1.1.0/prettyqt/iconprovider/svgbuffericonengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_ar.qm` & `prettyqt-1.1.0/prettyqt/localization/language_ar.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_bg.qm` & `prettyqt-1.1.0/prettyqt/localization/language_bg.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_ca.qm` & `prettyqt-1.1.0/prettyqt/localization/language_ca.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_cs.qm` & `prettyqt-1.1.0/prettyqt/localization/language_cs.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_da.qm` & `prettyqt-1.1.0/prettyqt/localization/language_da.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_de.qm` & `prettyqt-1.1.0/prettyqt/localization/language_de.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_es.qm` & `prettyqt-1.1.0/prettyqt/localization/language_es.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_fa.qm` & `prettyqt-1.1.0/prettyqt/localization/language_fa.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_fi.qm` & `prettyqt-1.1.0/prettyqt/localization/language_fi.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_fr.qm` & `prettyqt-1.1.0/prettyqt/localization/language_fr.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_gd.qm` & `prettyqt-1.1.0/prettyqt/localization/language_gd.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_gl.qm` & `prettyqt-1.1.0/prettyqt/localization/language_gl.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_he.qm` & `prettyqt-1.1.0/prettyqt/localization/language_he.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_hu.qm` & `prettyqt-1.1.0/prettyqt/localization/language_hu.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_it.qm` & `prettyqt-1.1.0/prettyqt/localization/language_it.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_ja.qm` & `prettyqt-1.1.0/prettyqt/localization/language_ja.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_ko.qm` & `prettyqt-1.1.0/prettyqt/localization/language_ko.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_lt.qm` & `prettyqt-1.1.0/prettyqt/localization/language_lt.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_lv.qm` & `prettyqt-1.1.0/prettyqt/localization/language_lv.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_pl.qm` & `prettyqt-1.1.0/prettyqt/localization/language_pl.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_pt.qm` & `prettyqt-1.1.0/prettyqt/localization/language_pt.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_ru.qm` & `prettyqt-1.1.0/prettyqt/localization/language_ru.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_sk.qm` & `prettyqt-1.1.0/prettyqt/localization/language_sk.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_sl.qm` & `prettyqt-1.1.0/prettyqt/localization/language_sl.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_sv.qm` & `prettyqt-1.1.0/prettyqt/localization/language_sv.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_uk.qm` & `prettyqt-1.1.0/prettyqt/localization/language_uk.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_zh_CN.qm` & `prettyqt-1.1.0/prettyqt/localization/language_zh_CN.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/localization/language_zh_TW.qm` & `prettyqt-1.1.0/prettyqt/localization/language_zh_TW.qm`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/__init__.py` & `prettyqt-1.1.0/prettyqt/location/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/geomaneuver.py` & `prettyqt-1.1.0/prettyqt/location/geomaneuver.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/georoute.py` & `prettyqt-1.1.0/prettyqt/location/georoute.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/georouterequest.py` & `prettyqt-1.1.0/prettyqt/location/georouterequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/georoutesegment.py` & `prettyqt-1.1.0/prettyqt/location/georoutesegment.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/georoutingmanager.py` & `prettyqt-1.1.0/prettyqt/location/georoutingmanager.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/geoserviceprovider.py` & `prettyqt-1.1.0/prettyqt/location/geoserviceprovider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/place.py` & `prettyqt-1.1.0/prettyqt/location/place.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placeattribute.py` & `prettyqt-1.1.0/prettyqt/location/placeattribute.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placecategory.py` & `prettyqt-1.1.0/prettyqt/location/placecategory.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placecontactdetail.py` & `prettyqt-1.1.0/prettyqt/location/placecontactdetail.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placecontent.py` & `prettyqt-1.1.0/prettyqt/location/placecontent.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placecontentreply.py` & `prettyqt-1.1.0/prettyqt/location/placecontentreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placecontentrequest.py` & `prettyqt-1.1.0/prettyqt/location/placecontentrequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placedetailsreply.py` & `prettyqt-1.1.0/prettyqt/location/placedetailsreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placeicon.py` & `prettyqt-1.1.0/prettyqt/location/placeicon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placeidreply.py` & `prettyqt-1.1.0/prettyqt/location/placeidreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placemanager.py` & `prettyqt-1.1.0/prettyqt/location/placemanager.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placematchreply.py` & `prettyqt-1.1.0/prettyqt/location/placematchreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placematchrequest.py` & `prettyqt-1.1.0/prettyqt/location/placematchrequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placereply.py` & `prettyqt-1.1.0/prettyqt/location/placereply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placesearchreply.py` & `prettyqt-1.1.0/prettyqt/location/placesearchreply.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placesearchrequest.py` & `prettyqt-1.1.0/prettyqt/location/placesearchrequest.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,24 +26,25 @@
         return location.VISIBILITY.inverse[self.visibilityScope()]
 
     def get_categories(self) -> list[location.PlaceCategory]:
         return [location.PlaceCategory(i) for i in self.categories()]
 
     def get_search_area(self) -> positioning.GeoShape:
         area = self.searchArea()
-        if isinstance(area, QtPositioning.QGeoCircle):
-            return positioning.GeoCircle(area)
-        elif isinstance(area, QtPositioning.QGeoPath):
-            return positioning.GeoPath(area)
-        elif isinstance(area, QtPositioning.QGeoPolygon):
-            return positioning.GeoPolygon(area)
-        elif isinstance(area, QtPositioning.QGeoRectangle):
-            return positioning.GeoRectangle(area)
-        else:
-            return positioning.GeoShape(area)
+        match area:
+            case QtPositioning.QGeoCircle():
+                return positioning.GeoCircle(area)
+            case QtPositioning.QGeoPath():
+                return positioning.GeoPath(area)
+            case QtPositioning.QGeoPolygon():
+                return positioning.GeoPolygon(area)
+            case QtPositioning.QGeoRectangle():
+                return positioning.GeoRectangle(area)
+            case _:
+                return positioning.GeoShape(area)
 
     def set_relevance_hint(self, hint: RelevanceHintStr):
         """Set the relevance hint.
 
         Args:
             hint: Relevance hint
```

### Comparing `prettyqt-1.0.0/prettyqt/location/placesearchresult.py` & `prettyqt-1.1.0/prettyqt/location/placesearchresult.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/placesupplier.py` & `prettyqt-1.1.0/prettyqt/location/placesupplier.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/location/qlocation.py` & `prettyqt-1.1.0/prettyqt/location/qlocation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/multimediawidgets/graphicsvideoitem.py` & `prettyqt-1.1.0/prettyqt/multimediawidgets/graphicsvideoitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/multimediawidgets/videowidget.py` & `prettyqt-1.1.0/prettyqt/multimediawidgets/videowidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/__init__.py` & `prettyqt-1.1.0/prettyqt/network/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/abstractsocket.py` & `prettyqt-1.1.0/prettyqt/network/abstractsocket.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/hostaddress.py` & `prettyqt-1.1.0/prettyqt/network/hostaddress.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/httpmultipart.py` & `prettyqt-1.1.0/prettyqt/network/httpmultipart.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/httppart.py` & `prettyqt-1.1.0/prettyqt/network/httppart.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/localserver.py` & `prettyqt-1.1.0/prettyqt/network/localserver.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/localsocket.py` & `prettyqt-1.1.0/prettyqt/network/localsocket.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/networkaccessmanager.py` & `prettyqt-1.1.0/prettyqt/network/networkaccessmanager.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/networkaddressentry.py` & `prettyqt-1.1.0/prettyqt/network/networkaddressentry.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/networkcookie.py` & `prettyqt-1.1.0/prettyqt/network/networkcookie.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/networkcookiejar.py` & `prettyqt-1.1.0/prettyqt/network/networkcookiejar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/networkdatagram.py` & `prettyqt-1.1.0/prettyqt/network/networkdatagram.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/networkinterface.py` & `prettyqt-1.1.0/prettyqt/network/networkinterface.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/networkproxy.py` & `prettyqt-1.1.0/prettyqt/network/networkproxy.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/networkrequest.py` & `prettyqt-1.1.0/prettyqt/network/networkrequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/tcpserver.py` & `prettyqt-1.1.0/prettyqt/network/tcpserver.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/network/udpsocket.py` & `prettyqt-1.1.0/prettyqt/network/udpsocket.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/objbrowser/attribute_model.py` & `prettyqt-1.1.0/prettyqt/objbrowser/attribute_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Module that defines AttributeModel."""
 
 from __future__ import annotations
 
+from collections.abc import Callable
 import inspect
 import logging
 import pprint
-from typing import Callable
 
 from prettyqt import constants, custom_models, gui
 from prettyqt.qt import QtGui
 from prettyqt.utils import treeitem
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `prettyqt-1.0.0/prettyqt/objbrowser/objectbrowser.py` & `prettyqt-1.1.0/prettyqt/objbrowser/objectbrowser.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/objbrowser/objectbrowsertreemodel.py` & `prettyqt-1.1.0/prettyqt/objbrowser/objectbrowsertreemodel.py`

 * *Files 1% similar despite different names*

```diff
@@ -308,57 +308,57 @@
         for tag, i1, i2, j1, j2 in reversed(opcodes):
             if 1 or tag != "equal":
                 logger.debug(
                     "  {:7s}, a[{}:{}] ({}), b[{}:{}] ({})".format(
                         tag, i1, i2, old_item_names[i1:i2], j1, j2, new_item_names[j1:j2]
                     )
                 )
-
-            if tag == "equal":
-                # Only when node names are equal is _aux_refresh_tree called recursively.
-                assert (
-                    i2 - i1 == j2 - j1
-                ), f"equal sanity check failed {i2 - i1} != {j2 - j1}"
-                for old_row, new_row in zip(range(i1, i2), range(j1, j2)):
-                    old_items[old_row].obj = new_items[new_row].obj
-                    child_index = self.index(old_row, 0, parent=tree_index)
-                    self._aux_refresh_tree(child_index)
-
-            elif tag == "replace":
-                # Explicitly remove the old item and insert the new. The old item may have
-                # child nodes which indices must be removed by Qt, otherwise it crashes.
-                assert (
-                    i2 - i1 == j2 - j1
-                ), f"replace sanity check failed {i2 - i1} != {j2 - j1}"
-
-                first = i1  # row number of first that will be removed
-                last = i1 + i2 - 1  # row number of last element after insertion
-                with self.remove_rows(first, last, tree_index):
-                    del tree_item.child_items[i1:i2]
-
-                first = i1  # row number of first element after insertion
-                last = i1 + j2 - j1 - 1  # row number of last element after insertion
-                with self.insert_rows(first, last, tree_index):
-                    tree_item.insert_children(i1, new_items[j1:j2])
-
-            elif tag == "delete":
-                assert j1 == j2, f"delete sanity check failed. {j1} != {j2}"
-                first = i1  # row number of first that will be removed
-                last = i1 + i2 - 1  # row number of last element after insertion
-                with self.remove_rows(first, last, tree_index):
-                    del tree_item.child_items[i1:i2]
-
-            elif tag == "insert":
-                assert i1 == i2, f"insert sanity check failed. {i1} != {i2}"
-                first = i1
-                last = i1 + j2 - j1 - 1
-                with self.insert_rows(first, last, tree_index):
-                    tree_item.insert_children(i1, new_items[j1:j2])
-            else:
-                raise ValueError(f"Invalid tag: {tag}")
+            match tag:
+                case "equal":
+                    # Only when node names are equal is aux_refresh_tree called recursively.
+                    assert (
+                        i2 - i1 == j2 - j1
+                    ), f"equal sanity check failed {i2 - i1} != {j2 - j1}"
+                    for old_row, new_row in zip(range(i1, i2), range(j1, j2)):
+                        old_items[old_row].obj = new_items[new_row].obj
+                        child_index = self.index(old_row, 0, parent=tree_index)
+                        self._aux_refresh_tree(child_index)
+
+                case "replace":
+                    # Explicitly remove the old item and insert the new. The old item may have
+                    # child nodes which indices must be removed by Qt, otherwise it crashes.
+                    assert (
+                        i2 - i1 == j2 - j1
+                    ), f"replace sanity check failed {i2 - i1} != {j2 - j1}"
+
+                    first = i1  # row number of first that will be removed
+                    last = i1 + i2 - 1  # row number of last element after insertion
+                    with self.remove_rows(first, last, tree_index):
+                        del tree_item.child_items[i1:i2]
+
+                    first = i1  # row number of first element after insertion
+                    last = i1 + j2 - j1 - 1  # row number of last element after insertion
+                    with self.insert_rows(first, last, tree_index):
+                        tree_item.insert_children(i1, new_items[j1:j2])
+
+                case "delete":
+                    assert j1 == j2, f"delete sanity check failed. {j1} != {j2}"
+                    first = i1  # row number of first that will be removed
+                    last = i1 + i2 - 1  # row number of last element after insertion
+                    with self.remove_rows(first, last, tree_index):
+                        del tree_item.child_items[i1:i2]
+
+                case "insert":
+                    assert i1 == i2, f"insert sanity check failed. {i1} != {i2}"
+                    first = i1
+                    last = i1 + j2 - j1 - 1
+                    with self.insert_rows(first, last, tree_index):
+                        tree_item.insert_children(i1, new_items[j1:j2])
+                case _:
+                    raise ValueError(f"Invalid tag: {tag}")
 
     def refresh_tree(self):
         """Refresh the tree model from the underlying root object."""
         logger.info("")
         logger.info("refresh_tree: %s", self.root_item)
 
         root_item = self.tree_item(self.root_index())
```

### Comparing `prettyqt-1.0.0/prettyqt/positioning/__init__.py` & `prettyqt-1.1.0/prettyqt/positioning/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/positioning/geoareamonitorinfo.py` & `prettyqt-1.1.0/prettyqt/positioning/geoareamonitorinfo.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,26 +9,27 @@
         return self.name()
 
     def __repr__(self):
         return f"{type(self).__name__}({self.name()!r})"
 
     def get_area(self) -> positioning.GeoShape:
         area = self.area()
-        if isinstance(area, QtPositioning.QGeoCircle):
-            return positioning.GeoCircle(area)
-        elif isinstance(area, QtPositioning.QGeoRectangle):
-            return positioning.GeoRectangle(area)
-        elif isinstance(area, QtPositioning.QGeoPath):
-            return positioning.GeoPath(area)
-        elif isinstance(area, QtPositioning.QGeoPolygon):
-            return positioning.GeoPolygon(area)
-        elif isinstance(area, QtPositioning.QGeoShape):
-            return positioning.GeoShape(area)
-        else:
-            raise RuntimeError()
+        match area:
+            case QtPositioning.QGeoCircle():
+                return positioning.GeoCircle(area)
+            case QtPositioning.QGeoRectangle():
+                return positioning.GeoRectangle(area)
+            case QtPositioning.QGeoPath():
+                return positioning.GeoPath(area)
+            case QtPositioning.QGeoPolygon():
+                return positioning.GeoPolygon(area)
+            case QtPositioning.QGeoShape():
+                return positioning.GeoShape(area)
+            case _:
+                raise RuntimeError()
 
     def get_expiration(self) -> core.DateTime:
         return core.DateTime(self.expiration())
 
 
 if __name__ == "__main__":
     info = GeoAreaMonitorInfo("test")
```

### Comparing `prettyqt-1.0.0/prettyqt/positioning/geoareamonitorsource.py` & `prettyqt-1.1.0/prettyqt/positioning/geoareamonitorsource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/positioning/geocircle.py` & `prettyqt-1.1.0/prettyqt/positioning/geocircle.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/positioning/geocoordinate.py` & `prettyqt-1.1.0/prettyqt/positioning/geocoordinate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/positioning/geolocation.py` & `prettyqt-1.1.0/prettyqt/positioning/geolocation.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/positioning/geopath.py` & `prettyqt-1.1.0/prettyqt/positioning/geopath.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/positioning/geopolygon.py` & `prettyqt-1.1.0/prettyqt/positioning/geopolygon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/positioning/geopositioninfo.py` & `prettyqt-1.1.0/prettyqt/positioning/geopositioninfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/positioning/geopositioninfosource.py` & `prettyqt-1.1.0/prettyqt/positioning/geopositioninfosource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/positioning/georectangle.py` & `prettyqt-1.1.0/prettyqt/positioning/georectangle.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/positioning/geosatelliteinfo.py` & `prettyqt-1.1.0/prettyqt/positioning/geosatelliteinfo.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/positioning/geosatelliteinfosource.py` & `prettyqt-1.1.0/prettyqt/positioning/geosatelliteinfosource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/positioning/geoshape.py` & `prettyqt-1.1.0/prettyqt/positioning/geoshape.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/positioning/nmeapositioninginfosource.py` & `prettyqt-1.1.0/prettyqt/positioning/nmeapositioninginfosource.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qml/__init__.py` & `prettyqt-1.1.0/prettyqt/qml/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qml/jsengine.py` & `prettyqt-1.1.0/prettyqt/qml/jsengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qml/jsvalue.py` & `prettyqt-1.1.0/prettyqt/qml/jsvalue.py`

 * *Files 14% similar despite different names*

```diff
@@ -52,30 +52,31 @@
     def get_error_type(self) -> str | None:
         error_type = self.errorType()
         return ERROR_TYPES.inverse.get(error_type)
 
     @classmethod
     def from_object(cls, obj, jsengine) -> JSValue:
         """Convert any python object into a QJSValue (must happen in GUI thread)."""
-        if obj is None:
-            return cls()
-        elif isinstance(obj, list) or isinstance(obj, tuple):
-            length = len(obj)
-            array = JSValue(jsengine.newArray(length))
-            for i, v in enumerate(obj):
-                array.setProperty(i, cls.from_object(v, jsengine))
-            return array
-        elif isinstance(obj, dict):
-            array = JSValue(jsengine.newArray())
-            for k, v in obj.items():
-                array.setProperty(k, cls.from_object(v, jsengine))
-            return array
-        else:
-            try:
-                return cls(obj)
-            except TypeError:
-                logger.debug("unknown type: " + str(obj))
+        match obj:
+            case None:
                 return cls()
+            case list() | tuple():
+                length = len(obj)
+                array = JSValue(jsengine.newArray(length))
+                for i, v in enumerate(obj):
+                    array.setProperty(i, cls.from_object(v, jsengine))
+                return array
+            case dict():
+                array = JSValue(jsengine.newArray())
+                for k, v in obj.items():
+                    array.setProperty(k, cls.from_object(v, jsengine))
+                return array
+            case _:
+                try:
+                    return cls(obj)
+                except TypeError:
+                    logger.debug("unknown type: " + str(obj))
+                    return cls()
 
 
 if __name__ == "__main__":
     val = JSValue()
```

### Comparing `prettyqt-1.0.0/prettyqt/qml/qmlapplicationengine.py` & `prettyqt-1.1.0/prettyqt/qml/qmlapplicationengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qml/qmlcomponent.py` & `prettyqt-1.1.0/prettyqt/qml/qmlcomponent.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qml/qmlengine.py` & `prettyqt-1.1.0/prettyqt/qml/qmlengine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qml/qmlimageproviderbase.py` & `prettyqt-1.1.0/prettyqt/qml/qmlimageproviderbase.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qt/QtCharts/__init__.py` & `prettyqt-1.1.0/prettyqt/qt/QtCharts/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qt/QtCore/__init__.py` & `prettyqt-1.1.0/prettyqt/qt/QtCore/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qt/QtGui/__init__.py` & `prettyqt-1.1.0/prettyqt/qt/QtGui/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Provides QtGui classes and functions."""
 
 from prettyqt.qt import PYQT5, PYQT6, PYSIDE6, PythonQtError
 
 
 if PYQT5:
     from PyQt5.QtGui import *
+    from PyQt5.QtWidgets import QUndoStack, QUndoGroup, QUndoCommand
 elif PYQT6:
     from PyQt6.QtGui import *
 
     for cls in (QPalette,):
         for attr in dir(cls):
             if not attr[0].isupper():
                 continue
```

### Comparing `prettyqt-1.0.0/prettyqt/qt/QtStateMachine/__init__.py` & `prettyqt-1.1.0/prettyqt/qt/QtStateMachine/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qt/QtUiTools/__init__.py` & `prettyqt-1.1.0/prettyqt/qt/QtUiTools/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qt/QtWebEngineCore/__init__.py` & `prettyqt-1.1.0/prettyqt/qt/QtWebEngineCore/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qt/QtWidgets/__init__.py` & `prettyqt-1.1.0/prettyqt/qt/QtWidgets/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qt/__init__.py` & `prettyqt-1.1.0/prettyqt/qt/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Provides Qt init stuff."""
 
-from typing import Callable, Literal
+from typing import Literal
+
+from collections.abc import Callable
 import operator
 import os
 import importlib
 
 
 class PythonQtError(ImportError):
     pass
```

### Comparing `prettyqt-1.0.0/prettyqt/qthelp/__init__.py` & `prettyqt-1.1.0/prettyqt/qthelp/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qthelp/helpenginecore.py` & `prettyqt-1.1.0/prettyqt/qthelp/helpenginecore.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/qtre.py` & `prettyqt-1.1.0/prettyqt/qtre.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
-from collections.abc import Iterator
+from collections.abc import Callable, Iterator
 import re
-from typing import Any, Callable
+from typing import Any
 
 from prettyqt import core
 from prettyqt.qt import QtCore
 from prettyqt.utils import bidict
 
 
 # IGNORECASE = QtCore.QRegularExpression.CaseInsensitiveOption
```

### Comparing `prettyqt-1.0.0/prettyqt/quick/__init__.py` & `prettyqt-1.1.0/prettyqt/quick/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/quick/quickitem.py` & `prettyqt-1.1.0/prettyqt/quick/quickitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/quick/quickitemgrabresult.py` & `prettyqt-1.1.0/prettyqt/quick/quickitemgrabresult.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/quick/quickpainteditem.py` & `prettyqt-1.1.0/prettyqt/quick/quickpainteditem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/quick/quickview.py` & `prettyqt-1.1.0/prettyqt/quick/quickview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/quick/quickwindow.py` & `prettyqt-1.1.0/prettyqt/quick/quickwindow.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/scintilla/sciscintilla.py` & `prettyqt-1.1.0/prettyqt/scintilla/sciscintilla.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/statemachine/__init__.py` & `prettyqt-1.1.0/prettyqt/statemachine/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/statemachine/abstracttransition.py` & `prettyqt-1.1.0/prettyqt/statemachine/abstracttransition.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/statemachine/historystate.py` & `prettyqt-1.1.0/prettyqt/statemachine/historystate.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/statemachine/state.py` & `prettyqt-1.1.0/prettyqt/statemachine/state.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/statemachine/statemachine.py` & `prettyqt-1.1.0/prettyqt/statemachine/statemachine.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/svg/svgrenderer.py` & `prettyqt-1.1.0/prettyqt/svg/svgrenderer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/syntaxhighlighters/__init__.py` & `prettyqt-1.1.0/prettyqt/syntaxhighlighters/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/syntaxhighlighters/highlightrule.py` & `prettyqt-1.1.0/prettyqt/syntaxhighlighters/highlightrule.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/syntaxhighlighters/jsonhighlighter.py` & `prettyqt-1.1.0/prettyqt/syntaxhighlighters/jsonhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/syntaxhighlighters/markdownhighlighter.py` & `prettyqt-1.1.0/prettyqt/syntaxhighlighters/markdownhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/syntaxhighlighters/pygments/regularexpressionlexer.py` & `prettyqt-1.1.0/prettyqt/syntaxhighlighters/pygments/regularexpressionlexer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/syntaxhighlighters/pygmentshighlighter.py` & `prettyqt-1.1.0/prettyqt/syntaxhighlighters/pygmentshighlighter.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,32 +51,32 @@
                 continue
             if action is not None:
                 if isinstance(action, _TokenType):
                     yield pos, action, m.group()
                 else:
                     yield from action(self, m)
             pos = m.end()
-            if new_state is None:
-                break
-            # state transition
-            if isinstance(new_state, tuple):
-                for state in new_state:
-                    if state == "#pop":
-                        statestack.pop()
-                    elif state == "#push":
-                        statestack.append(statestack[-1])
-                    else:
-                        statestack.append(state)
-            elif isinstance(new_state, int):
-                # pop
-                del statestack[new_state:]
-            elif new_state == "#push":
-                statestack.append(statestack[-1])
-            else:
-                assert False, f"wrong state def: {new_state!r}"
+            match new_state:
+                case None:
+                    break
+                case tuple():
+                    for state in new_state:
+                        match state:
+                            case "#pop":
+                                statestack.pop()
+                            case "#push":
+                                statestack.append(statestack[-1])
+                            case _:
+                                statestack.append(state)
+                case int():
+                    del statestack[new_state:]
+                case "#push":
+                    statestack.append(statestack[-1])
+                case _:
+                    assert False, f"wrong state def: {new_state!r}"
             statetokens = tokendefs[statestack[-1]]
             break
         else:
             try:
                 if text[pos] == "\n":
                     # at EOL, reset state to "root"
                     statestack = ["root"]
@@ -191,30 +191,31 @@
         result = gui.TextCharFormat()
         try:
             token_style = style.style_for_token(token)
         except KeyError:
             return result
         for key, value in token_style.items():
             if value:
-                if key == "color":
-                    result.set_foreground_color(self._get_brush(value))
-                elif key == "bgcolor":
-                    result.set_background_color(self._get_brush(value))
-                elif key == "bold":
-                    result.set_font_weight("bold")
-                elif key == "italic":
-                    result.setFontItalic(True)
-                elif key == "underline":
-                    result.set_underline_style("single")
-                elif key == "sans":
-                    result.set_font_style_hint("sans_serif")
-                elif key == "roman":
-                    result.set_font_style_hint("serif")
-                elif key == "mono":
-                    result.set_font_style_hint("typewriter")
+                match key:
+                    case "color":
+                        result.set_foreground_color(self._get_brush(value))
+                    case "bgcolor":
+                        result.set_background_color(self._get_brush(value))
+                    case "bold":
+                        result.set_font_weight("bold")
+                    case "italic":
+                        result.setFontItalic(True)
+                    case "underline":
+                        result.set_underline_style("single")
+                    case "sans":
+                        result.set_font_style_hint("sans_serif")
+                    case "roman":
+                        result.set_font_style_hint("serif")
+                    case "mono":
+                        result.set_font_style_hint("typewriter")
         return result
 
     @functools.cache
     def _get_brush(self, color: str) -> gui.Brush:
         """Return a brush for the color."""
         qcolor = gui.Color(f"#{color[:6]}")
         return gui.Brush(qcolor)
```

### Comparing `prettyqt-1.0.0/prettyqt/syntaxhighlighters/pythonhighlighter.py` & `prettyqt-1.1.0/prettyqt/syntaxhighlighters/pythonhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/syntaxhighlighters/regexmatchhighlighter.py` & `prettyqt-1.1.0/prettyqt/syntaxhighlighters/regexmatchhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/syntaxhighlighters/xmlhighlighter.py` & `prettyqt-1.1.0/prettyqt/syntaxhighlighters/xmlhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/syntaxhighlighters/yamlhighlighter.py` & `prettyqt-1.1.0/prettyqt/syntaxhighlighters/yamlhighlighter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/texttospeech/texttospeech.py` & `prettyqt-1.1.0/prettyqt/texttospeech/texttospeech.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/texttospeech/voice.py` & `prettyqt-1.1.0/prettyqt/texttospeech/voice.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/themes/darktheme.qss` & `prettyqt-1.1.0/prettyqt/themes/darktheme.qss`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/utils/__init__.py` & `prettyqt-1.1.0/prettyqt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/utils/autoslot.py` & `prettyqt-1.1.0/prettyqt/utils/autoslot.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Functions for the Qt meta-object system (like signal, slot, etc)
 # credits to Empyrical
 # https://gist.github.com/empyrical/a103c46f454a433e8798#file-decorator-py
 
 from __future__ import annotations
 
+from collections.abc import Callable
 import inspect
 import logging
-from typing import Callable, get_type_hints
+from typing import get_type_hints
 
 from prettyqt import core
 
 
 logger = logging.getLogger(__name__)
```

### Comparing `prettyqt-1.0.0/prettyqt/utils/colors.py` & `prettyqt-1.1.0/prettyqt/utils/colors.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/utils/debugging.py` & `prettyqt-1.1.0/prettyqt/utils/debugging.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/utils/helpers.py` & `prettyqt-1.1.0/prettyqt/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/utils/mappers.py` & `prettyqt-1.1.0/prettyqt/utils/mappers.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/utils/prettyprinter.py` & `prettyqt-1.1.0/prettyqt/utils/prettyprinter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-from collections.abc import Generator
-from typing import Any, Callable
+from collections.abc import Callable, Generator
+from typing import Any
 
 
 class PrettyPrinter:
     serialize: Callable
 
     def __pretty__(
         self, fmt: Callable[[Any], Any], **kwargs: Any
```

### Comparing `prettyqt-1.0.0/prettyqt/utils/searchandreplacemixin.py` & `prettyqt-1.1.0/prettyqt/utils/searchandreplacemixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
+from collections.abc import Callable
 import logging
 import re
-from typing import Callable
 
 from prettyqt import gui
 
 
 logger = logging.getLogger(__name__)
 
 SEARCH_REGEX = re.compile(r"([^/]|\\/)+$")
```

### Comparing `prettyqt-1.0.0/prettyqt/utils/signallogger.py` & `prettyqt-1.1.0/prettyqt/utils/signallogger.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/utils/singleapplication.py` & `prettyqt-1.1.0/prettyqt/utils/singleapplication.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/utils/syncedproperty.py` & `prettyqt-1.1.0/prettyqt/utils/syncedproperty.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Optional
-
 from prettyqt import core
 from prettyqt.qt import QtCore
 
 
 class PropertyMeta(type(QtCore.QObject)):  # type: ignore
     def __new__(cls, name, bases, attrs):
         for key in list(attrs.keys()):
@@ -31,15 +29,15 @@
         self.name = name
 
 
 class PropertyImpl(core.Property):
     """Actual property implementation using a signal to notify any change."""
 
     def __init__(
-        self, initial_value, name: str = "", type_: Optional[type] = None, notify=None
+        self, initial_value, name: str = "", type_: type | None = None, notify=None
     ):
         super().__init__(type_, self.getter, self.setter, notify=notify)
         self.initial_value = initial_value
         self.name = name
 
     def getter(self, inst):
         return getattr(inst, value_attribute_name(self.name), self.initial_value)
```

### Comparing `prettyqt-1.0.0/prettyqt/utils/treeitem.py` & `prettyqt-1.1.0/prettyqt/utils/treeitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/utils/types.py` & `prettyqt-1.1.0/prettyqt/utils/types.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/webenginecore/__init__.py` & `prettyqt-1.1.0/prettyqt/webenginecore/__init__.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/webenginecore/webenginecontextmenurequest.py` & `prettyqt-1.1.0/prettyqt/webenginecore/webenginecontextmenurequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/webenginecore/webenginedownloadrequest.py` & `prettyqt-1.1.0/prettyqt/webenginecore/webenginedownloadrequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/webenginecore/webenginehistory.py` & `prettyqt-1.1.0/prettyqt/webenginecore/webenginehistory.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/webenginecore/webenginehttprequest.py` & `prettyqt-1.1.0/prettyqt/webenginecore/webenginehttprequest.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/webenginecore/webenginepage.py` & `prettyqt-1.1.0/prettyqt/webenginecore/webenginepage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
+from collections.abc import Callable
 import logging
 import os
-from typing import Callable, Literal
+from typing import Literal
 import webbrowser
 
 from prettyqt import core, gui, webenginecore
 from prettyqt.qt import QtWebEngineCore
 from prettyqt.utils import InvalidParamError, bidict, types
```

### Comparing `prettyqt-1.0.0/prettyqt/webenginecore/webengineprofile.py` & `prettyqt-1.1.0/prettyqt/webenginecore/webengineprofile.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/webenginecore/webenginescript.py` & `prettyqt-1.1.0/prettyqt/webenginecore/webenginescript.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/webenginecore/webenginescriptcollection.py` & `prettyqt-1.1.0/prettyqt/webenginecore/webenginescriptcollection.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/webenginecore/webenginesettings.py` & `prettyqt-1.1.0/prettyqt/webenginecore/webenginesettings.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/webenginecore/webengineurlscheme.py` & `prettyqt-1.1.0/prettyqt/webenginecore/webengineurlscheme.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/webenginewidgets/webengineview.py` & `prettyqt-1.1.0/prettyqt/webenginewidgets/webengineview.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
+from collections.abc import Callable
 import os
-from typing import Callable
 import webbrowser
 
 from prettyqt import core, webenginecore, widgets
 from prettyqt.qt import QtWebEngineWidgets
 from prettyqt.utils import types
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/__init__.py` & `prettyqt-1.1.0/prettyqt/widgets/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,17 +107,14 @@
 from .dial import Dial
 
 from .dockwidget import DockWidget
 
 from .action import Action, ActionMixin
 from .actiongroup import ActionGroup
 from .shortcut import Shortcut
-from .undocommand import UndoCommand
-from .undostack import UndoStack
-from .undogroup import UndoGroup
 from .widgetaction import WidgetAction
 from .menu import Menu
 from .mainwindow import MainWindow
 from .whatsthis import WhatsThis
 from .listwidgetitem import ListWidgetItem
 from .treewidgetitem import TreeWidgetItem
 from .toolbutton import ToolButton
@@ -406,17 +403,14 @@
     "Shortcut",
     "WhatsThis",
     "AbstractItemDelegate",
     "AbstractItemDelegateMixin",
     "ItemDelegate",
     "StyledItemDelegate",
     "SystemTrayIcon",
-    "UndoCommand",
-    "UndoStack",
-    "UndoGroup",
     "UndoView",
     "DataWidgetMapper",
     "SizeGrip",
     "KeyEventTransition",
     "MouseEventTransition",
     "GraphicsSceneHoverEvent",
     "GraphicsSceneMouseEvent",
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/abstractbutton.py` & `prettyqt-1.1.0/prettyqt/widgets/abstractbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/abstractitemview.py` & `prettyqt-1.1.0/prettyqt/widgets/abstractitemview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/abstractscrollarea.py` & `prettyqt-1.1.0/prettyqt/widgets/abstractscrollarea.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/abstractslider.py` & `prettyqt-1.1.0/prettyqt/widgets/abstractslider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/abstractspinbox.py` & `prettyqt-1.1.0/prettyqt/widgets/abstractspinbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/action.py` & `prettyqt-1.1.0/prettyqt/widgets/action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
+from collections.abc import Callable
 import os
-from typing import Callable, Literal
+from typing import Literal
 
 from prettyqt import constants, core, gui, iconprovider
 from prettyqt.qt import QtCore, QtGui, QtWidgets
 from prettyqt.utils import InvalidParamError, bidict, helpers, prettyprinter, types
 
 
 PRIORITIES = bidict(
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/actiongroup.py` & `prettyqt-1.1.0/prettyqt/widgets/actiongroup.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/application.py` & `prettyqt-1.1.0/prettyqt/widgets/application.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/boxlayout.py` & `prettyqt-1.1.0/prettyqt/widgets/boxlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/calendarwidget.py` & `prettyqt-1.1.0/prettyqt/widgets/calendarwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/checkbox.py` & `prettyqt-1.1.0/prettyqt/widgets/checkbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/colordialog.py` & `prettyqt-1.1.0/prettyqt/widgets/colordialog.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/combobox.py` & `prettyqt-1.1.0/prettyqt/widgets/combobox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/completer.py` & `prettyqt-1.1.0/prettyqt/widgets/completer.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/datawidgetmapper.py` & `prettyqt-1.1.0/prettyqt/widgets/datawidgetmapper.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/dateedit.py` & `prettyqt-1.1.0/prettyqt/widgets/dateedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/datetimeedit.py` & `prettyqt-1.1.0/prettyqt/widgets/datetimeedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/dial.py` & `prettyqt-1.1.0/prettyqt/widgets/dial.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/dialog.py` & `prettyqt-1.1.0/prettyqt/widgets/dialog.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/dialogbuttonbox.py` & `prettyqt-1.1.0/prettyqt/widgets/dialogbuttonbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-from collections.abc import Iterator, Sequence
-from typing import Callable, Literal
+from collections.abc import Callable, Iterator, Sequence
+from typing import Literal
 
 from prettyqt import constants, core, widgets
 from prettyqt.qt import QtCore, QtWidgets
 from prettyqt.utils import InvalidParamError, bidict
 
 
 BUTTONS = bidict(
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/dockwidget.py` & `prettyqt-1.1.0/prettyqt/widgets/dockwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/doublespinbox.py` & `prettyqt-1.1.0/prettyqt/widgets/doublespinbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/filedialog.py` & `prettyqt-1.1.0/prettyqt/widgets/filedialog.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/fileiconprovider.py` & `prettyqt-1.1.0/prettyqt/widgets/fileiconprovider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/filesystemmodel.py` & `prettyqt-1.1.0/prettyqt/widgets/filesystemmodel.py`

 * *Files 6% similar despite different names*

```diff
@@ -55,22 +55,23 @@
         self.setOption(OPTIONS["dont_watch_changes"], not watch)
 
     def use_custom_icons(self, use: bool):
         self.setOption(OPTIONS["no_custom_icons"], not use)
 
     def set_root_path(self, path: types.PathType) -> QtCore.QModelIndex:
         path = os.fspath(path)
-        if path in ["/", "root"]:
-            path = core.Dir.rootPath()
-        elif path == "home":
-            path = core.Dir.homePath()
-        elif path == "temp":
-            path = core.Dir.tempPath()
-        elif path == "current":
-            path = core.Dir.currentPath()
+        match path:
+            case "/" | "root":
+                path = core.Dir.rootPath()
+            case "home":
+                path = core.Dir.homePath()
+            case "temp":
+                path = core.Dir.tempPath()
+            case "current":
+                path = core.Dir.currentPath()
         return self.setRootPath(path)
 
     def set_name_filters(self, filters, hide: bool = False):
         self.setNameFilters(filters)
         self.setNameFilterDisables(not hide)
 
     def set_filter(self, filter_mode: core.dir.FilterStr):
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/fontcombobox.py` & `prettyqt-1.1.0/prettyqt/widgets/fontcombobox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/formlayout.py` & `prettyqt-1.1.0/prettyqt/widgets/formlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/frame.py` & `prettyqt-1.1.0/prettyqt/widgets/frame.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/gesture.py` & `prettyqt-1.1.0/prettyqt/widgets/gesture.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicsanchorlayout.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicsanchorlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicsblureffect.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicsblureffect.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicsellipseitem.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicsellipseitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicsgridlayout.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicsgridlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicsitem.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicsitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicslayout.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicslayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicslinearlayout.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicslinearlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicslineitem.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicslineitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicsobject.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicsobject.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicsopacityeffect.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicsopacityeffect.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicspixmapitem.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicspixmapitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicspolygonitem.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicspolygonitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicsrectitem.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicsrectitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicsscene.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicsscene.py`

 * *Files 7% similar despite different names*

```diff
@@ -65,33 +65,34 @@
     def get_background_brush(self) -> gui.Brush:
         return gui.Brush(self.backgroundBrush())
 
     def get_foreground_brush(self) -> gui.Brush:
         return gui.Brush(self.foregroundBrush())
 
     def add(self, item) -> QtWidgets.QGraphicsItem:
-        if isinstance(item, QtWidgets.QGraphicsItem):
-            self.addItem(item)
-            return item
-        elif isinstance(item, QtGui.QPixmap):
-            return self.add_pixmap(item)
-        elif isinstance(item, QtGui.QPainterPath):
-            return self.add_path(item)
-        elif isinstance(item, QtGui.QPolygonF):
-            return self.add_polygon(item)
-        elif isinstance(item, QtCore.QRectF):
-            return self.add_rect(item)
-        elif isinstance(item, QtCore.QLine):
-            return self.add_line(item)
-        elif isinstance(item, str):
-            return self.add_text(item)
-        elif isinstance(item, QtWidgets.QWidget):
-            return self.add_widget(item)
-        else:
-            raise TypeError(item)
+        match item:
+            case QtWidgets.QGraphicsItem():
+                self.addItem(item)
+                return item
+            case QtGui.QPixmap():
+                return self.add_pixmap(item)
+            case QtGui.QPainterPath():
+                return self.add_path(item)
+            case QtGui.QPolygonF():
+                return self.add_polygon(item)
+            case QtCore.QRectF():
+                return self.add_rect(item)
+            case QtCore.QLine():
+                return self.add_line(item)
+            case str():
+                return self.add_text(item)
+            case QtWidgets.QWidget():
+                return self.add_widget(item)
+            case _:
+                raise TypeError(item)
 
     def add_pixmap(self, pixmap: QtGui.QPixmap) -> widgets.GraphicsPixmapItem:
         g_item = widgets.GraphicsPixmapItem()
         g_item.setPixmap(pixmap)
         self.addItem(g_item)
         return g_item
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicstextitem.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicstextitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicsview.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicsview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/graphicswidget.py` & `prettyqt-1.1.0/prettyqt/widgets/graphicswidget.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,26 +19,27 @@
             preferred_size=self.preferredSize(),
             maximum_size=self.maximumSize(),
             palette=self.get_palette(),
             focus_policy=self.get_focus_policy(),
         )
 
     def set_layout(self, layout: LayoutStr | QtWidgets.QGraphicsLayout | None):
-        if layout is None:
-            return
-        if isinstance(layout, QtWidgets.QGraphicsLayout):
-            self.box = layout
-        elif layout == "grid":
-            self.box = widgets.GraphicsGridLayout()
-        elif layout == "anchor":
-            self.box = widgets.GraphicsAnchorLayout()
-        elif layout in ("horizontal", "vertical"):
-            self.box = widgets.GraphicsLinearLayout(layout)
-        else:
-            raise ValueError("Invalid Layout")
+        match layout:
+            case None:
+                return
+            case QtWidgets.QGraphicsLayout():
+                self.box = layout
+            case "grid":
+                self.box = widgets.GraphicsGridLayout()
+            case "anchor":
+                self.box = widgets.GraphicsAnchorLayout()
+            case "horizontal" | "vertical":
+                self.box = widgets.GraphicsLinearLayout(layout)
+            case _:
+                raise ValueError("Invalid Layout")
         self.setLayout(self.box)
 
     def set_focus_policy(self, policy: constants.FocusPolicyStr) -> None:
         """Set the way the widget accepts keyboard focus.
 
         Args:
             policy: Focus policy
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/gridlayout.py` & `prettyqt-1.1.0/prettyqt/widgets/gridlayout.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,20 +70,21 @@
         self,
         item: QtWidgets.QWidget | QtWidgets.QLayout | QtWidgets.QLayoutItem,
         rowstart: int,
         colstart: int,
         rowspan: int = 1,
         colspan: int = 1,
     ):
-        if isinstance(item, QtWidgets.QWidget):
-            self.addWidget(item, rowstart, colstart, rowspan, colspan)
-        elif isinstance(item, QtWidgets.QLayout):
-            self.addLayout(item, rowstart, colstart, rowspan, colspan)
-        else:
-            self.addItem(item, rowstart, colstart, rowspan, colspan)
+        match item:
+            case QtWidgets.QWidget():
+                self.addWidget(item, rowstart, colstart, rowspan, colspan)
+            case QtWidgets.QLayout():
+                self.addLayout(item, rowstart, colstart, rowspan, colspan)
+            case QtWidgets.QLayoutItem():
+                self.addItem(item, rowstart, colstart, rowspan, colspan)
 
     def append(self, item: QtWidgets.QWidget | QtWidgets.QLayout | QtWidgets.QLayoutItem):
         self[self.rowCount(), 0 : self.columnCount() - 1] = item
 
     def set_origin_corner(self, corner: constants.CornerStr):
         """Set the origin corner.
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/groupbox.py` & `prettyqt-1.1.0/prettyqt/widgets/groupbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/headerview.py` & `prettyqt-1.1.0/prettyqt/widgets/headerview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/inputdialog.py` & `prettyqt-1.1.0/prettyqt/widgets/inputdialog.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/itemeditorfactory.py` & `prettyqt-1.1.0/prettyqt/widgets/itemeditorfactory.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/keysequenceedit.py` & `prettyqt-1.1.0/prettyqt/widgets/keysequenceedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/label.py` & `prettyqt-1.1.0/prettyqt/widgets/label.py`

 * *Files 4% similar despite different names*

```diff
@@ -92,22 +92,23 @@
 
     def set_alignment(
         self,
         horizontal: constants.HorizontalAlignmentStr | None = None,
         vertical: constants.VerticalAlignmentStr | None = None,
     ):
         """Set the alignment of the label's contents."""
-        if horizontal is None and vertical is not None:
-            flag = constants.V_ALIGNMENT[vertical]
-        elif vertical is None and horizontal is not None:
-            flag = constants.H_ALIGNMENT[horizontal]
-        elif vertical is not None and horizontal is not None:
-            flag = constants.V_ALIGNMENT[vertical] | constants.H_ALIGNMENT[horizontal]
-        else:
-            return
+        match horizontal, vertical:
+            case None, None:
+                return self
+            case None, _:
+                flag = constants.V_ALIGNMENT[vertical]
+            case _, None:
+                flag = constants.H_ALIGNMENT[horizontal]
+            case _, _:
+                flag = constants.V_ALIGNMENT[vertical] | constants.H_ALIGNMENT[horizontal]
         self.setAlignment(flag)
         return self
 
     def get_horizontal_alignment(self) -> constants.HorizontalAlignmentStr:
         align = self.alignment()
         if align & constants.ALIGN_RIGHT:  # type: ignore
             return "right"
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/layout.py` & `prettyqt-1.1.0/prettyqt/widgets/layout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/layoutitem.py` & `prettyqt-1.1.0/prettyqt/widgets/layoutitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/lcdnumber.py` & `prettyqt-1.1.0/prettyqt/widgets/lcdnumber.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/lineedit.py` & `prettyqt-1.1.0/prettyqt/widgets/lineedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/listview.py` & `prettyqt-1.1.0/prettyqt/widgets/listview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/listwidget.py` & `prettyqt-1.1.0/prettyqt/widgets/listwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/listwidgetitem.py` & `prettyqt-1.1.0/prettyqt/widgets/listwidgetitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/mainwindow.py` & `prettyqt-1.1.0/prettyqt/widgets/mainwindow.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/mdiarea.py` & `prettyqt-1.1.0/prettyqt/widgets/mdiarea.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/mdisubwindow.py` & `prettyqt-1.1.0/prettyqt/widgets/mdisubwindow.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/menu.py` & `prettyqt-1.1.0/prettyqt/widgets/menu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations
 
-from collections.abc import Iterator
-from typing import Any, Callable
+from collections.abc import Callable, Iterator
+from typing import Any
 
 from prettyqt import core, gui, iconprovider, widgets
 from prettyqt.qt import QtWidgets
 from prettyqt.utils import types
 
 
 class MenuMixin(widgets.WidgetMixin):
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/menubar.py` & `prettyqt-1.1.0/prettyqt/widgets/menubar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/messagebox.py` & `prettyqt-1.1.0/prettyqt/widgets/messagebox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/pangesture.py` & `prettyqt-1.1.0/prettyqt/widgets/pangesture.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/pinchgesture.py` & `prettyqt-1.1.0/prettyqt/widgets/pinchgesture.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/plaintextedit.py` & `prettyqt-1.1.0/prettyqt/widgets/plaintextedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/progressbar.py` & `prettyqt-1.1.0/prettyqt/widgets/progressbar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/progressdialog.py` & `prettyqt-1.1.0/prettyqt/widgets/progressdialog.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/pushbutton.py` & `prettyqt-1.1.0/prettyqt/widgets/pushbutton.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from typing import Callable
+from collections.abc import Callable
 
 from prettyqt import core, widgets
 from prettyqt.qt import QtWidgets
 
 
 class PushButtonMixin(widgets.AbstractButtonMixin):
     value_changed = core.Signal(bool)
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/radiobutton.py` & `prettyqt-1.1.0/prettyqt/widgets/radiobutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/rubberband.py` & `prettyqt-1.1.0/prettyqt/widgets/rubberband.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/scrollarea.py` & `prettyqt-1.1.0/prettyqt/widgets/scrollarea.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/scrollbar.py` & `prettyqt-1.1.0/prettyqt/widgets/scrollbar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/scroller.py` & `prettyqt-1.1.0/prettyqt/widgets/scroller.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/scrollerproperties.py` & `prettyqt-1.1.0/prettyqt/widgets/scrollerproperties.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/shortcut.py` & `prettyqt-1.1.0/prettyqt/widgets/shortcut.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/sizepolicy.py` & `prettyqt-1.1.0/prettyqt/widgets/sizepolicy.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/slider.py` & `prettyqt-1.1.0/prettyqt/widgets/slider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/spaceritem.py` & `prettyqt-1.1.0/prettyqt/widgets/spaceritem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/spinbox.py` & `prettyqt-1.1.0/prettyqt/widgets/spinbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/splashscreen.py` & `prettyqt-1.1.0/prettyqt/widgets/splashscreen.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/splitter.py` & `prettyqt-1.1.0/prettyqt/widgets/splitter.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/splitterhandle.py` & `prettyqt-1.1.0/prettyqt/widgets/splitterhandle.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/stackedlayout.py` & `prettyqt-1.1.0/prettyqt/widgets/stackedlayout.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/stackedwidget.py` & `prettyqt-1.1.0/prettyqt/widgets/stackedwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/statusbar.py` & `prettyqt-1.1.0/prettyqt/widgets/statusbar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/style.py` & `prettyqt-1.1.0/prettyqt/widgets/style.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/styleoptionbutton.py` & `prettyqt-1.1.0/prettyqt/widgets/styleoptionbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/styleoptionheader.py` & `prettyqt-1.1.0/prettyqt/widgets/styleoptionheader.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,10 +24,9 @@
 SORT_INDICATOR = bidict(
     none=mod.SortIndicator(0),  # type: ignore
     sort_up=mod.SortIndicator.SortUp,
     sort_down=mod.SortIndicator.SortDown,
 )
 
 
-
 class StyleOptionHeader(widgets.StyleOptionMixin, QtWidgets.QStyleOptionHeader):
     pass
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/styleoptionmenuitem.py` & `prettyqt-1.1.0/prettyqt/widgets/styleoptionmenuitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/styleoptionslider.py` & `prettyqt-1.1.0/prettyqt/widgets/styleoptionslider.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/styleoptiontab.py` & `prettyqt-1.1.0/prettyqt/widgets/styleoptiontab.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/styleoptiontoolbox.py` & `prettyqt-1.1.0/prettyqt/widgets/styleoptiontoolbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/styleoptionviewitem.py` & `prettyqt-1.1.0/prettyqt/widgets/styleoptionviewitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/swipegesture.py` & `prettyqt-1.1.0/prettyqt/widgets/swipegesture.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/systemtrayicon.py` & `prettyqt-1.1.0/prettyqt/widgets/systemtrayicon.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/tabbar.py` & `prettyqt-1.1.0/prettyqt/widgets/tabbar.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/tableview.py` & `prettyqt-1.1.0/prettyqt/widgets/tableview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/tablewidget.py` & `prettyqt-1.1.0/prettyqt/widgets/tablewidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/tablewidgetitem.py` & `prettyqt-1.1.0/prettyqt/widgets/tablewidgetitem.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,22 +64,23 @@
         Args:
             horizontal: horizontal text alignment to use
             vertical: vertical text alignment to use
 
         Raises:
             InvalidParamError: invalid text alignment
         """
-        if horizontal is None and vertical is not None:
-            flag = constants.V_ALIGNMENT[vertical]
-        elif vertical is None and horizontal is not None:
-            flag = constants.H_ALIGNMENT[horizontal]
-        elif vertical is not None and horizontal is not None:
-            flag = constants.V_ALIGNMENT[vertical] | constants.H_ALIGNMENT[horizontal]
-        else:
-            return
+        match horizontal, vertical:
+            case None, None:
+                return
+            case None, _:
+                flag = constants.V_ALIGNMENT[vertical]
+            case _, None:
+                flag = constants.H_ALIGNMENT[horizontal]
+            case _, _:
+                flag = constants.V_ALIGNMENT[vertical] | constants.H_ALIGNMENT[horizontal]
         self.setTextAlignment(flag)
 
     def get_background(self) -> gui.Brush:
         return gui.Brush(self.background())
 
     def get_foreground(self) -> gui.Brush:
         return gui.Brush(self.foreground())
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/tablewidgetselectionrange.py` & `prettyqt-1.1.0/prettyqt/widgets/tablewidgetselectionrange.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/tabwidget.py` & `prettyqt-1.1.0/prettyqt/widgets/tabwidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/textbrowser.py` & `prettyqt-1.1.0/prettyqt/widgets/textbrowser.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/textedit.py` & `prettyqt-1.1.0/prettyqt/widgets/textedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/timeedit.py` & `prettyqt-1.1.0/prettyqt/widgets/timeedit.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/toolbar.py` & `prettyqt-1.1.0/prettyqt/widgets/toolbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
-from typing import Any, Callable
+from collections.abc import Callable
+from typing import Any
 
 from prettyqt import constants, core, iconprovider, widgets
 from prettyqt.qt import QtWidgets
 from prettyqt.utils import InvalidParamError, helpers, types
 
 
 class ToolBarMixin(widgets.WidgetMixin):
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/toolbox.py` & `prettyqt-1.1.0/prettyqt/widgets/toolbox.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/toolbutton.py` & `prettyqt-1.1.0/prettyqt/widgets/toolbutton.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/tooltip.py` & `prettyqt-1.1.0/prettyqt/widgets/tooltip.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/treeview.py` & `prettyqt-1.1.0/prettyqt/widgets/treeview.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/treewidget.py` & `prettyqt-1.1.0/prettyqt/widgets/treewidget.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/treewidgetitem.py` & `prettyqt-1.1.0/prettyqt/widgets/treewidgetitem.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/treewidgetitemiterator.py` & `prettyqt-1.1.0/prettyqt/widgets/treewidgetitemiterator.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/undocommand.py` & `prettyqt-1.1.0/prettyqt/gui/undocommand.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from __future__ import annotations
 
-from prettyqt.qt import QtWidgets
+from prettyqt.qt import QtGui
 
 
-class UndoCommand(QtWidgets.QUndoCommand):
+class UndoCommand(QtGui.QUndoCommand):
     def __len__(self) -> int:
         return self.childCount()
 
-    def __getitem__(self, index: int) -> QtWidgets.QUndoCommand:
+    def __getitem__(self, index: int) -> QtGui.QUndoCommand:
         child = self.child(index)
         if child is None:
             raise KeyError(index)
         return child
 
     def serialize_fields(self):
         return dict(children=[self.child(i) for i in range(self.childCount())])
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/undostack.py` & `prettyqt-1.1.0/prettyqt/gui/undostack.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 from __future__ import annotations
 
+from collections.abc import Callable
 import contextlib
-from typing import Callable
 
-from prettyqt import core, widgets
-from prettyqt.qt import QtWidgets
+from prettyqt import core, gui
+from prettyqt.qt import QtGui
 
 
 class UndoStackMixin(core.ObjectMixin):
     def __len__(self) -> int:
         return self.count()
 
-    def __getitem__(self, index: int) -> QtWidgets.QUndoCommand:
+    def __getitem__(self, index: int) -> QtGui.QUndoCommand:
         cmd = self.command(index)
         if cmd is None:
             return KeyError(index)
         return cmd
 
     @contextlib.contextmanager
     def create_macro(self, text: str):
         self.beginMacro(text)
         yield None
         self.endMacro()
 
     def add_command(
         self, title: str, redo: Callable, undo: Callable
-    ) -> widgets.UndoCommand:
-        class MyCommand(widgets.UndoCommand):
+    ) -> gui.UndoCommand:
+        class MyCommand(gui.UndoCommand):
             def redo(self):
                 return redo()
 
             def undo(self):
                 return undo()
 
         cmd = MyCommand(title)
         self.push(cmd)
         return cmd
 
 
-class UndoStack(UndoStackMixin, QtWidgets.QUndoStack):
+class UndoStack(UndoStackMixin, QtGui.QUndoStack):
     pass
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/whatsthis.py` & `prettyqt-1.1.0/prettyqt/widgets/whatsthis.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/widget.py` & `prettyqt-1.1.0/prettyqt/widgets/widget.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
-from collections.abc import Iterator
+from collections.abc import Callable, Iterator
 import contextlib
 import os
 import pathlib
 import sys
-from typing import Any, Callable, Literal
+from typing import Any, Literal
 
 from deprecated import deprecated
 import qstylizer.parser
 import qstylizer.style
 
 from prettyqt import constants, core, gui, iconprovider, widgets
 from prettyqt.qt import QtCore, QtGui, QtWidgets
```

### Comparing `prettyqt-1.0.0/prettyqt/widgets/widgetaction.py` & `prettyqt-1.1.0/prettyqt/widgets/widgetaction.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/wizard.py` & `prettyqt-1.1.0/prettyqt/widgets/wizard.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/prettyqt/widgets/wizardpage.py` & `prettyqt-1.1.0/prettyqt/widgets/wizardpage.py`

 * *Files identical despite different names*

### Comparing `prettyqt-1.0.0/pyproject.toml` & `prettyqt-1.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "PrettyQt"
-version = "1.0.0"
+version = "1.1.0"
 description = "A pythonic layer on top of PyQt5 / PyQt6 / PySide6"
 readme = 'docs/index.md'
 repository = "https://github.com/phil65/prettyqt"
 homepage = "https://github.com/phil65/prettyqt"
 authors = ["phil65 <philipptemminghoff@googlemail.com>"]
 packages = [
     { include = "prettyqt" },
@@ -46,15 +46,15 @@
 types-Deprecated = "^1.2"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7"
 pip = "^23"
 pytest-cov = "^4"
 pytest-qt = {version = "^4.1"}
-mypy = "^0"
+mypy = "^1"
 types-Deprecated = "^1.2"
 types-docutils = "^0"
 types-orjson = "^3.6"
 pylint = "^2.5"
 pytest-xvfb = {version = "^2", markers = "sys_platform == 'linux'"}
 codecov = "^2.1"
 coverage = "^7"
@@ -180,15 +180,15 @@
   | build
   | dist
   | tests/.*/setup.py
 )/
 '''
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.0"
+version = "1.1.0"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_start_rev = "v0.100.0"
 changelog_file = "docs/changelog.md"
 version_files = [
     "prettyqt/__init__.py:__version__",
     "pyproject.toml:version",
```

### Comparing `prettyqt-1.0.0/PKG-INFO` & `prettyqt-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prettyqt
-Version: 1.0.0
+Version: 1.1.0
 Summary: A pythonic layer on top of PyQt5 / PyQt6 / PySide6
 Home-page: https://github.com/phil65/prettyqt
 Author: phil65
 Author-email: philipptemminghoff@googlemail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

