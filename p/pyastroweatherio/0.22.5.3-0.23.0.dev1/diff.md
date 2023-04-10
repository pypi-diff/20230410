# Comparing `tmp/pyastroweatherio-0.22.5.3.tar.gz` & `tmp/pyastroweatherio-0.23.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyastroweatherio-0.22.5.3.tar", last modified: Wed Mar 22 09:02:02 2023, max compression
+gzip compressed data, was "pyastroweatherio-0.23.0.dev1.tar", last modified: Mon Apr 10 15:32:10 2023, max compression
```

## Comparing `pyastroweatherio-0.22.5.3.tar` & `pyastroweatherio-0.23.0.dev1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-22 09:02:02.572265 pyastroweatherio-0.22.5.3/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1071 2022-02-18 09:50:43.000000 pyastroweatherio-0.22.5.3/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)      863 2023-03-22 09:02:02.573265 pyastroweatherio-0.22.5.3/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3076 2022-07-20 14:26:18.000000 pyastroweatherio-0.22.5.3/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-22 09:02:02.572265 pyastroweatherio-0.22.5.3/pyastroweatherio/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      285 2022-07-20 14:19:32.000000 pyastroweatherio-0.22.5.3/pyastroweatherio/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    15968 2022-07-22 12:30:08.000000 pyastroweatherio-0.22.5.3/pyastroweatherio/client.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     4385 2023-03-22 08:51:06.000000 pyastroweatherio-0.22.5.3/pyastroweatherio/const.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    16312 2023-03-22 09:01:48.000000 pyastroweatherio-0.22.5.3/pyastroweatherio/dataclasses.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      337 2022-02-18 09:50:43.000000 pyastroweatherio-0.22.5.3/pyastroweatherio/errors.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)    14814 2022-07-20 14:24:20.000000 pyastroweatherio-0.22.5.3/pyastroweatherio/helper_functions.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-03-22 09:02:02.572265 pyastroweatherio-0.22.5.3/pyastroweatherio.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      863 2023-03-22 09:02:02.000000 pyastroweatherio-0.22.5.3/pyastroweatherio.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      413 2023-03-22 09:02:02.000000 pyastroweatherio-0.22.5.3/pyastroweatherio.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-03-22 09:02:02.000000 pyastroweatherio-0.22.5.3/pyastroweatherio.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       16 2023-03-22 09:02:02.000000 pyastroweatherio-0.22.5.3/pyastroweatherio.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       17 2023-03-22 09:02:02.000000 pyastroweatherio-0.22.5.3/pyastroweatherio.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       79 2023-03-22 09:02:02.573265 pyastroweatherio-0.22.5.3/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1171 2023-03-22 09:02:00.000000 pyastroweatherio-0.22.5.3/setup.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-10 15:32:10.449692 pyastroweatherio-0.23.0.dev1/
+-rw-r--r--   0 markus    (1000) markus    (1000)     1071 2021-04-12 14:01:42.000000 pyastroweatherio-0.23.0.dev1/LICENSE
+-rw-rw-r--   0 markus    (1000) markus    (1000)      866 2023-04-10 15:32:10.449692 pyastroweatherio-0.23.0.dev1/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)     3076 2023-03-21 16:46:28.000000 pyastroweatherio-0.23.0.dev1/README.md
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-10 15:32:10.449692 pyastroweatherio-0.23.0.dev1/pyastroweatherio/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      285 2023-03-21 16:46:28.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio/__init__.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    24579 2023-04-10 15:28:51.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio/client.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)     4473 2023-04-08 14:28:26.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio/const.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    16844 2023-04-10 15:29:18.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio/dataclasses.py
+-rw-r--r--   0 markus    (1000) markus    (1000)      337 2021-04-12 14:01:42.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio/errors.py
+-rw-rw-r--   0 markus    (1000) markus    (1000)    14814 2023-03-21 16:46:28.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio/helper_functions.py
+drwxrwxr-x   0 markus    (1000) markus    (1000)        0 2023-04-10 15:32:10.449692 pyastroweatherio-0.23.0.dev1/pyastroweatherio.egg-info/
+-rw-rw-r--   0 markus    (1000) markus    (1000)      866 2023-04-10 15:32:10.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio.egg-info/PKG-INFO
+-rw-rw-r--   0 markus    (1000) markus    (1000)      413 2023-04-10 15:32:10.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio.egg-info/SOURCES.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)        1 2023-04-10 15:32:10.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio.egg-info/dependency_links.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       16 2023-04-10 15:32:10.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio.egg-info/requires.txt
+-rw-rw-r--   0 markus    (1000) markus    (1000)       17 2023-04-10 15:32:10.000000 pyastroweatherio-0.23.0.dev1/pyastroweatherio.egg-info/top_level.txt
+-rw-r--r--   0 markus    (1000) markus    (1000)       79 2023-04-10 15:32:10.449692 pyastroweatherio-0.23.0.dev1/setup.cfg
+-rw-rw-r--   0 markus    (1000) markus    (1000)     1174 2023-04-10 15:32:07.000000 pyastroweatherio-0.23.0.dev1/setup.py
```

### Comparing `pyastroweatherio-0.22.5.3/LICENSE` & `pyastroweatherio-0.23.0.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.22.5.3/PKG-INFO` & `pyastroweatherio-0.23.0.dev1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.22.5.3
+Version: 0.23.0.dev1
 Summary: Python Wrapper for 7Timer REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyastroweatherio-0.22.5.3/README.md` & `pyastroweatherio-0.23.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.22.5.3/pyastroweatherio/client.py` & `pyastroweatherio-0.23.0.dev1/pyastroweatherio/client.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 from datetime import datetime, timedelta
 from typing import Optional
 from aiohttp import ClientSession, ClientTimeout
 from aiohttp.client_exceptions import ClientError
 from decimal import Decimal
 
 from pyastroweatherio.const import (
-    BASE_URL,
+    BASE_URL_SEVENTIMER,
+    BASE_URL_MET,
     DEFAULT_TIMEOUT,
     DEFAULT_CACHE_TIMEOUT,
     DEFAULT_ELEVATION,
     DEFAULT_TIMEZONE,
     DEFAULT_CONDITION_CLOUDCOVER_WEIGHT,
     DEFAULT_CONDITION_SEEING_WEIGHT,
     DEFAULT_CONDITION_TRANSPARENCY_WEIGHT,
@@ -29,15 +30,14 @@
     ForecastData,
     LocationData,
     NightlyConditionsData,
 )
 from pyastroweatherio.errors import RequestError
 from pyastroweatherio.helper_functions import ConversionFunctions, AstronomicalRoutines
 
-
 _LOGGER = logging.getLogger(__name__)
 
 
 class AstroWeather:
     """AstroWeather Communication Client."""
 
     def __init__(
@@ -52,19 +52,20 @@
         transparency_weight=DEFAULT_CONDITION_TRANSPARENCY_WEIGHT,
     ):
         self._session: ClientSession = session
         self._latitude = latitude
         self._longitude = longitude
         self._elevation = elevation
         self._timezone_info = timezone_info
-        self._weather_data = []
-        self._weather_data_init = ""
-        self._weather_data_timestamp = datetime.now() - timedelta(
-            seconds=(DEFAULT_CACHE_TIMEOUT + 1)
-        )
+        self._weather_data_seventimer = []
+        self._weather_data_seventimer_init = ""
+        self._weather_data_met = []
+        self._weather_data_met_init = ""
+        self._weather_data_seventimer_timestamp = datetime.now() - timedelta(seconds=(DEFAULT_CACHE_TIMEOUT + 1))
+        self._weather_data_met_timestamp = datetime.now() - timedelta(seconds=(DEFAULT_CACHE_TIMEOUT + 1))
         self._cloudcover_weight = cloudcover_weight
         self._seeing_weight = seeing_weight
         self._transparency_weight = transparency_weight
         self.req = session
 
     # Public functions
     async def get_location_data(
@@ -93,51 +94,63 @@
     # Private functions
     async def _get_location_data(self) -> None:
         """Return Forecast data"""
 
         cnv = ConversionFunctions()
         items = []
 
-        await self.retrieve_data()
+        await self.retrieve_data_seventimer()
+        await self.retrieve_data_met()
         now = datetime.utcnow()
 
         # Anchor timestamp
-        init_ts = await cnv.anchor_timestamp(self._weather_data_init)
+        init_ts = await cnv.anchor_timestamp(self._weather_data_seventimer_init)
 
+        # met.no
+        met_index = -1
         forecast_skipped = 0
-        for row in self._weather_data:
+        for row in self._weather_data_seventimer:
             # Skip over past forecasts
             forecast_time = init_ts + timedelta(hours=row["timepoint"])
             if now > forecast_time:
                 forecast_skipped += 1
                 continue
 
+            _LOGGER.debug("forecast_time: %s", str(forecast_time))
+
+            # met.no
+            for datapoint in self._weather_data_met:
+                met_index = met_index + 1
+                if forecast_time == datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
+                    break
+            _LOGGER.debug("met start index: %s", str(met_index))
+
             # Astro Routines
             astro_routines = AstronomicalRoutines(
                 self._latitude,
                 self._longitude,
                 self._elevation,
                 self._timezone_info,
                 now,
             )
 
             item = {
                 "init": init_ts,
                 "timepoint": row["timepoint"],
                 "timestamp": forecast_time,
-                "forecast_length": (len(self._weather_data) - forecast_skipped) * 3,
+                "forecast_length": (len(self._weather_data_seventimer) - forecast_skipped) * 3,
                 "latitude": self._latitude,
                 "longitude": self._longitude,
                 "elevation": self._elevation,
                 "cloudcover": row["cloudcover"],
                 "seeing": row["seeing"],
                 "transparency": row["transparency"],
-                "condition_percentage": await self.calc_condition_percentage(
-                    row["cloudcover"], row["seeing"], row["transparency"]
-                ),
+                # "condition_percentage": await self.calc_condition_percentage(
+                #     row["cloudcover"], row["seeing"], row["transparency"]
+                # ),
                 "lifted_index": row["lifted_index"],
                 "rh2m": row["rh2m"],
                 "wind10m": row["wind10m"],
                 "temp2m": row["temp2m"],
                 "dewpoint2m": await self.calc_dewpoint2m(row["rh2m"], row["temp2m"]),
                 "prec_type": row["prec_type"],
                 "sun_next_rising": await astro_routines.sun_next_rising(),
@@ -152,48 +165,84 @@
                 "moon_next_setting": await astro_routines.moon_next_setting(),
                 "moon_phase": await astro_routines.moon_phase(),
                 "moon_altitude": await astro_routines.moon_altitude(),
                 "moon_azimuth": await astro_routines.moon_azimuth(),
                 "weather": row.get("weather", ""),
                 "deepsky_forecast": await self._deepsky_forecast(),
             }
+            # met.no
+            if datetime.strptime(self._weather_data_met[met_index].get("time"), "%Y-%m-%dT%H:%M:%SZ") == forecast_time:
+                _LOGGER.debug("Cloud Area Fraction timestamp match: %s", str(forecast_time))
+                datails = self._weather_data_met[met_index].get("data", {}).get("instant", {}).get("details", {})
+                # Overwrite cloudcover
+                item["cloudcover"] = datails.get("cloud_area_fraction", -1) / 12.5 + 1
+
+                item["cloud_area_fraction"] = datails.get("cloud_area_fraction", -1)
+                item["cloud_area_fraction_high"] = datails.get("cloud_area_fraction_high", -1)
+                item["cloud_area_fraction_low"] = datails.get("cloud_area_fraction_low", -1)
+                item["cloud_area_fraction_medium"] = datails.get("cloud_area_fraction_medium", -1)
+                item["condition_percentage"] = await self.calc_condition_percentage(
+                    item["cloud_area_fraction"] / 12.5 + 1,
+                    row["seeing"],
+                    row["transparency"],
+                )
+            else:
+                _LOGGER.debug("No Cloud Area Fraction for: %s", str(forecast_time))
+                item["cloud_area_fraction"] = None
+                item["cloud_area_fraction_high"] = None
+                item["cloud_area_fraction_low"] = None
+                item["cloud_area_fraction_medium"] = None
+                item["condition_percentage"] = await self.calc_condition_percentage(
+                    row["cloudcover"], row["seeing"], row["transparency"]
+                )
+
             items.append(LocationData(item))
             break
 
         return items
 
     async def _forecast_data(self, forecast_type, hours_to_show) -> None:
         """Return Forecast data for the Station."""
 
         cnv = ConversionFunctions()
         items = []
 
-        await self.retrieve_data()
+        await self.retrieve_data_seventimer()
+        await self.retrieve_data_met()
         now = datetime.utcnow()
 
         # Create items
         cnt = 0
 
         # Anchor timestamp
-        init_ts = await cnv.anchor_timestamp(self._weather_data_init)
+        init_ts = await cnv.anchor_timestamp(self._weather_data_seventimer_init)
 
         # Astro Routines
         astro_routines = AstronomicalRoutines(
             self._latitude, self._longitude, self._elevation, self._timezone_info, now
         )
         utc_to_local_diff = astro_routines.utc_to_local_diff()
         _LOGGER.debug("UTC to local diff: %s", str(utc_to_local_diff))
-        _LOGGER.debug("Forecast length: %s", str(len(self._weather_data)))
+        _LOGGER.debug("Forecast length: %s", str(len(self._weather_data_seventimer)))
 
-        for row in self._weather_data:
+        met_index = -1
+        for row in self._weather_data_seventimer:
             # Skip over past forecasts
             forecast_time = init_ts + timedelta(hours=row["timepoint"])
             if now > forecast_time:
                 continue
 
+            # met.no
+            if met_index == -1:
+                for datapoint in self._weather_data_met:
+                    met_index = met_index + 1
+                    if forecast_time == datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
+                        break
+                _LOGGER.debug("met start index: %s", str(met_index))
+
             # Hour of day needs to be in local time
             hour_of_day = (forecast_time.hour + utc_to_local_diff) % 24
 
             cloudcover = row["cloudcover"]
             seeing = row["seeing"]
             transparency = row["transparency"]
 
@@ -202,91 +251,152 @@
                 "timepoint": row["timepoint"],
                 "timestamp": forecast_time,
                 # "timestamp": astro_routines.utc_to_local(forecast_time),
                 "hour": hour_of_day,
                 "cloudcover": cloudcover,
                 "seeing": seeing,
                 "transparency": transparency,
-                "condition_percentage": await self.calc_condition_percentage(
-                    row["cloudcover"], row["seeing"], row["transparency"]
-                ),
+                # "condition_percentage": await self.calc_condition_percentage(
+                #     row["cloudcover"], row["seeing"], row["transparency"]
+                # ),
                 "lifted_index": row["lifted_index"],
                 "rh2m": row["rh2m"],
                 "wind10m": row["wind10m"],
                 "temp2m": row["temp2m"],
                 "dewpoint2m": await self.calc_dewpoint2m(row["rh2m"], row["temp2m"]),
                 "prec_type": row["prec_type"],
                 "weather": row.get("weather", ""),
             }
+            # met.no
+            if (
+                datetime.strptime(
+                    self._weather_data_met[met_index + cnt].get("time"),
+                    "%Y-%m-%dT%H:%M:%SZ",
+                )
+                == forecast_time
+            ):
+                _LOGGER.debug("Cloud Area Fraction timestamp match: %s", str(forecast_time))
+                datails = self._weather_data_met[met_index + cnt].get("data", {}).get("instant", {}).get("details", {})
+                # Overwrite cloudcover
+                item["cloudcover"] = datails.get("cloud_area_fraction", -1) / 12.5 + 1
+
+                item["cloud_area_fraction"] = datails.get("cloud_area_fraction", -1)
+                item["cloud_area_fraction_high"] = datails.get("cloud_area_fraction_high", -1)
+                item["cloud_area_fraction_low"] = datails.get("cloud_area_fraction_low", -1)
+                item["cloud_area_fraction_medium"] = datails.get("cloud_area_fraction_medium", -1)
+                item["condition_percentage"] = await self.calc_condition_percentage(
+                    item["cloud_area_fraction"] / 12.5 + 1,
+                    row["seeing"],
+                    row["transparency"],
+                )
+            else:
+                _LOGGER.debug("No Cloud Area Fraction for: %s", str(forecast_time))
+                item["cloud_area_fraction"] = None
+                item["cloud_area_fraction_high"] = None
+                item["cloud_area_fraction_low"] = None
+                item["cloud_area_fraction_medium"] = None
+                item["condition_percentage"] = await self.calc_condition_percentage(
+                    row["cloudcover"], row["seeing"], row["transparency"]
+                )
             items.append(ForecastData(item))
             # Limit number of Hours
             cnt += 3
             if cnt >= hours_to_show:
                 break
 
         return items
 
     async def _deepsky_forecast(self):
         """Return Deepsky Forecast data"""
 
         cnv = ConversionFunctions()
         items = []
 
-        await self.retrieve_data()
+        await self.retrieve_data_seventimer()
+        await self.retrieve_data_met()
         now = datetime.utcnow()
 
+        # Create items
+        cnt = 0
+
         # Anchor timestamp
-        init_ts = await cnv.anchor_timestamp(self._weather_data_init)
+        init_ts = await cnv.anchor_timestamp(self._weather_data_seventimer_init)
 
         # Astro Routines
         astro_routines = AstronomicalRoutines(
             self._latitude, self._longitude, self._elevation, self._timezone_info, now
         )
         utc_to_local_diff = astro_routines.utc_to_local_diff()
 
         # Create forecast
         forecast_dayname = ""
         start_forecast_hour = 0
         start_weather = ""
         interval_points = []
 
-        for row in self._weather_data:
+        met_index = -1
+        for row in self._weather_data_seventimer:
             # Skip over past forecasts
             forecast_time = init_ts + timedelta(hours=row["timepoint"])
             if now > forecast_time:
                 continue
 
+            # met.no
+            if met_index == -1:
+                for datapoint in self._weather_data_met:
+                    met_index = met_index + 1
+                    if forecast_time == datetime.strptime(datapoint.get("time"), "%Y-%m-%dT%H:%M:%SZ"):
+                        break
+
             # Hour of day needs to be in local time
             hour_of_day = (forecast_time.hour + utc_to_local_diff) % 24
 
             # Skip daytime, we're only interested in the forecasts in
             # between 9pm to 3am.
             # Possible timestamps within the data:
             # 15 18 (21 00 03) 06 09 12
             # 16 (19 22 01) 04 07 10 13
             # 17 (20 23 02) 05 08 11 14
             # Relevant ones in brackets
             if hour_of_day < 19 and hour_of_day > 3:
                 start_forecast_hour = 0
                 start_weather = ""
                 interval_points = []
+                cnt += 3
                 continue
 
             cloudcover = row["cloudcover"]
             seeing = row["seeing"]
             transparency = row["transparency"]
+            cloud_area_fraction = 0
+            # met.no
+            if (
+                datetime.strptime(
+                    self._weather_data_met[met_index + cnt].get("time"),
+                    "%Y-%m-%dT%H:%M:%SZ",
+                )
+                == forecast_time
+            ):
+                # met.no
+                _LOGGER.debug("Cloud Area Fraction timestamp match: %s", str(forecast_time))
+                datails = self._weather_data_met[met_index + cnt].get("data", {}).get("instant", {}).get("details", {})
+                cloud_area_fraction = datails.get("cloud_area_fraction") / 12.5 + 1
+            else:
+                _LOGGER.debug("No Cloud Area Fraction for: %s", str(forecast_time))
+
             if len(interval_points) == 0:
                 forecast_dayname = forecast_time.strftime("%A")
                 start_forecast_hour = hour_of_day
                 start_weather = row.get("weather", "")
 
             # Calculate Condition
-            interval_points.append(
-                await self.calc_condition_percentage(cloudcover, seeing, transparency)
-            )
+            if cloud_area_fraction > 0:
+                interval_points.append(await self.calc_condition_percentage(cloud_area_fraction, seeing, transparency))
+            else:
+                interval_points.append(await self.calc_condition_percentage(cloudcover, seeing, transparency))
 
             if len(interval_points) == 3:
                 item = {
                     "init": init_ts,
                     "dayname": forecast_dayname,
                     "hour": start_forecast_hour,
                     "nightly_conditions": interval_points,
@@ -295,14 +405,15 @@
                 items.append(NightlyConditionsData(item))
                 _LOGGER.debug(
                     "Nightly conditions day: %s, start hour: %s, condition percentages: %s",
                     str(forecast_dayname),
                     str(start_forecast_hour),
                     str(interval_points),
                 )
+            cnt += 3
             if len(items) == 2:
                 break
 
         return items
 
     async def calc_condition_percentage(self, cloudcover, seeing, transparency):
         """Return condition based on cloud cover, seeing and transparency"""
@@ -342,70 +453,66 @@
         )
         return condition
 
     async def calc_dewpoint2m(self, rh2m, temp2m):
         """Calculate 2m Dew Point."""
         # α(T,RH) = ln(RH/100) + aT/(b+T)
         # Ts = (b × α(T,RH)) / (a - α(T,RH))
-        alpha = float(Decimal(str(rh2m / 100)).ln()) + MAGNUS_COEFFICIENT_A * temp2m / (
-            MAGNUS_COEFFICIENT_B + temp2m
-        )
+        alpha = float(Decimal(str(rh2m / 100)).ln()) + MAGNUS_COEFFICIENT_A * temp2m / (MAGNUS_COEFFICIENT_B + temp2m)
         dewpoint = (MAGNUS_COEFFICIENT_B * alpha) / (MAGNUS_COEFFICIENT_A - alpha)
 
         return dewpoint
 
-    async def retrieve_data(self):
+    async def retrieve_data_seventimer(self):
         """Retrieves current data from 7timer"""
 
-        if (
-            (datetime.now() - self._weather_data_timestamp).total_seconds()
-        ) > DEFAULT_CACHE_TIMEOUT:
-            self._weather_data_timestamp = datetime.now()
+        if ((datetime.now() - self._weather_data_seventimer_timestamp).total_seconds()) > DEFAULT_CACHE_TIMEOUT:
+            self._weather_data_seventimer_timestamp = datetime.now()
             _LOGGER.debug("Updating data")
 
             # Testing
             # json_data_astro = {"init": "2022060906"}
             # with open("astro.json") as json_file:
             #     astro_dataseries = json.load(json_file).get("dataseries", {})
             # with open("civil.json") as json_file:
             #     civil_dataseries = json.load(json_file).get("dataseries", {})
             # -Testing
-            json_data_astro = await self.async_request("astro", "get")
-            json_data_civil = await self.async_request("civil", "get")
+            json_data_astro = await self.async_request_seventimer("astro", "get")
+            json_data_civil = await self.async_request_seventimer("civil", "get")
 
             astro_dataseries = json_data_astro.get("dataseries", {})
             civil_dataseries = json_data_civil.get("dataseries", {})
             # /Testing
 
             for astro, civil in zip(astro_dataseries, civil_dataseries):
                 if astro["timepoint"] == civil["timepoint"]:
                     astro["weather"] = civil["weather"]
                     astro["rh2m"] = int(civil["rh2m"].replace("%", ""))
 
-            self._weather_data = astro_dataseries
-            self._weather_data_init = json_data_astro.get("init")
+            self._weather_data_seventimer = astro_dataseries
+            self._weather_data_seventimer_init = json_data_astro.get("init")
         else:
             _LOGGER.debug("Using cached data")
 
-    async def async_request(self, product="astro", method="get") -> dict:
+    async def async_request_seventimer(self, product="astro", method="get") -> dict:
         """Make a request against the 7timer API."""
 
         use_running_session = self._session and not self._session.closed
 
         if use_running_session:
             session = self._session
         else:
             session = ClientSession(
                 timeout=ClientTimeout(total=DEFAULT_TIMEOUT),
             )
 
-        # BASE_URL = "http://www.7timer.info/bin/api.pl?lon=XX.XX&lat=YY.YY&product=astro&output=json"
+        # BASE_URL_SEVENTIMER = "http://www.7timer.info/bin/api.pl?lon=XX.XX&lat=YY.YY&product=astro&output=json"
         # STIMER_OUTPUT = "json"
         url = (
-            str(f"{BASE_URL}")
+            str(f"{BASE_URL_SEVENTIMER}")
             + "?lon="
             + str("%.1f" % round(self._longitude, 2))
             + "&lat="
             + str("%.1f" % round(self._latitude, 2))
             + "&product="
             + str(product)
             + "&output="
@@ -420,14 +527,85 @@
 
                 # Testing
                 # json_string = json.dumps(data)
                 # with open(product + ".json", "w") as outfile:
                 #     outfile.write(json_string)
                 # /Testing
 
+                return data
+        except asyncio.TimeoutError:
+            raise RequestError("Request to endpoint timed out")
+        except ClientError as err:
+            raise RequestError(f"Error requesting data: {err}") from None
+
+        finally:
+            if not use_running_session:
+                await session.close()
+
+    async def retrieve_data_met(self):
+        """Retrieves current data from met"""
+
+        if ((datetime.now() - self._weather_data_met_timestamp).total_seconds()) > DEFAULT_CACHE_TIMEOUT:
+            self._weather_data_met_timestamp = datetime.now()
+            _LOGGER.debug("Updating data")
+
+            # Testing
+            # json_data_astro = {"init": "2022060906"}
+            # with open("astro.json") as json_file:
+            #     astro_dataseries = json.load(json_file).get("dataseries", {})
+            # with open("civil.json") as json_file:
+            #     civil_dataseries = json.load(json_file).get("dataseries", {})
+            # -Testing
+            json_data_met = await self.async_request_met("met", "get")
+
+            dataseries = json_data_met.get("properties", {}).get("timeseries", [])
+            # /Testing
+
+            self._weather_data_met = dataseries
+            self._weather_data_met_init = dataseries[0].get("time", None)
+        else:
+            _LOGGER.debug("Using cached data")
+
+    async def async_request_met(self, product="met", method="get") -> dict:
+        """Make a request against the 7timer API."""
+
+        use_running_session = self._session and not self._session.closed
+
+        if use_running_session:
+            session = self._session
+        else:
+            session = ClientSession(
+                timeout=ClientTimeout(total=DEFAULT_TIMEOUT),
+            )
+
+        # BASE_URL_MET = "https://api.met.no/weatherapi/locationforecast/2.0/complete?altitude=XX&lat=XX.XX&lon=XX.XX"
+        # STIMER_OUTPUT = "json"
+        url = (
+            str(f"{BASE_URL_MET}")
+            + "?lon="
+            + str("%.1f" % round(self._longitude, 2))
+            + "&lat="
+            + str("%.1f" % round(self._latitude, 2))
+            + "&altitude="
+            + str(self._elevation)
+        )
+        try:
+            _LOGGER.debug(f"Query url: {url}")
+            async with session.request(method, url) as resp:
+                resp.raise_for_status()
+                # plain = str(await resp.text()).replace("\n", " ")
+                # data = json.loads(plain)
+                data = await resp.json()
+
+                # Testing
+                # json_string = json.dumps(data)
+                # with open(product + ".json", "w") as outfile:
+                #     outfile.write(json_string)
+                # /Testing
+
                 return data
         except asyncio.TimeoutError:
             raise RequestError("Request to endpoint timed out")
         except ClientError as err:
             raise RequestError(f"Error requesting data: {err}") from None
 
         finally:
```

### Comparing `pyastroweatherio-0.22.5.3/pyastroweatherio/const.py` & `pyastroweatherio-0.23.0.dev1/pyastroweatherio/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Constant Definitions for AstroWeather."""
 
-BASE_URL = "http://www.7timer.info/bin/api.pl"
+BASE_URL_SEVENTIMER = "http://www.7timer.info/bin/api.pl"
+BASE_URL_MET = "https://api.met.no/weatherapi/locationforecast/2.0/complete"
 STIMER_OUTPUT = "json"
 
 DEFAULT_TIMEOUT = 10
 DEFAULT_CACHE_TIMEOUT = 1770
 DEFAULT_ELEVATION = 0
 DEFAULT_TIMEZONE = "Etc/UTC"
 DEFAULT_CONDITION_CLOUDCOVER_WEIGHT = 3
```

### Comparing `pyastroweatherio-0.22.5.3/pyastroweatherio/dataclasses.py` & `pyastroweatherio-0.23.0.dev1/pyastroweatherio/dataclasses.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,18 @@
     """A representation of the base class for AstroWeather Data."""
 
     def __init__(self, data):
         self._init = data["init"]
         self._timepoint = data["timepoint"]
         self._timestamp = data["timestamp"]
         self._cloudcover = data["cloudcover"]
+        self._cloud_area_fraction = data["cloud_area_fraction"]
+        self._cloud_area_fraction_high = data["cloud_area_fraction_high"]
+        self._cloud_area_fraction_low = data["cloud_area_fraction_low"]
+        self._cloud_area_fraction_medium = data["cloud_area_fraction_medium"]
         self._seeing = data["seeing"]
         self._transparency = data["transparency"]
         self._condition_percentage = data["condition_percentage"]
         self._lifted_index = data["lifted_index"]
         self._rh2m = data["rh2m"]
         self._wind10m = data["wind10m"]
         self._temp2m = data["temp2m"]
@@ -67,14 +71,34 @@
 
     @property
     def cloudless_percentage(self) -> int:
         """Return Cloudless Percentage."""
         return int(100 + 100 * (1 - self._cloudcover) / 8)
 
     @property
+    def cloud_area_fraction_percentage(self) -> int:
+        """Return Cloud Cover Percentage."""
+        return self._cloud_area_fraction
+
+    @property
+    def cloud_area_fraction_high_percentage(self) -> int:
+        """Return Cloud Cover Percentage."""
+        return self._cloud_area_fraction_high
+
+    @property
+    def cloud_area_fraction_low_percentage(self) -> int:
+        """Return Cloud Cover Percentage."""
+        return self._cloud_area_fraction_low
+
+    @property
+    def cloud_area_fraction_medium_percentage(self) -> int:
+        """Return Cloud Cover Percentage."""
+        return self._cloud_area_fraction_medium
+
+    @property
     def seeing(self) -> int:
         """Return Seeing."""
         return self._seeing
 
     @property
     def seeing_percentage(self) -> int:
         """Return Seeing."""
@@ -368,29 +392,17 @@
 
     @property
     def deepsky_forecast_today_plain(self):
         """Return Forecast Today."""
         if len(self._deepsky_forecast) > 0:
             nightly_conditions = self._deepsky_forecast[0]
             out = ""
-            out += (
-                CONDITION[
-                    4 - math.floor(nightly_conditions.nightly_conditions[0] / 20)
-                ].capitalize()
-                + "-"
-            )
-            out += (
-                CONDITION[
-                    4 - math.floor(nightly_conditions.nightly_conditions[1] / 20)
-                ].capitalize()
-                + "-"
-            )
-            out += CONDITION[
-                4 - math.floor(nightly_conditions.nightly_conditions[2] / 20)
-            ].capitalize()
+            out += CONDITION[4 - math.floor(nightly_conditions.nightly_conditions[0] / 20)].capitalize() + "-"
+            out += CONDITION[4 - math.floor(nightly_conditions.nightly_conditions[1] / 20)].capitalize() + "-"
+            out += CONDITION[4 - math.floor(nightly_conditions.nightly_conditions[2] / 20)].capitalize()
             return out
         return None
 
     @property
     def deepsky_forecast_today_desc(self):
         """Return Forecast Today Description."""
         if len(self._deepsky_forecast) > 0:
@@ -426,29 +438,17 @@
 
     @property
     def deepsky_forecast_tomorrow_plain(self):
         """Return Forecast Tomorrow."""
         if len(self._deepsky_forecast) > 1:
             nightly_conditions = self._deepsky_forecast[1]
             out = ""
-            out += (
-                CONDITION[
-                    4 - math.floor(nightly_conditions.nightly_conditions[0] / 20)
-                ].capitalize()
-                + "-"
-            )
-            out += (
-                CONDITION[
-                    4 - math.floor(nightly_conditions.nightly_conditions[1] / 20)
-                ].capitalize()
-                + "-"
-            )
-            out += CONDITION[
-                4 - math.floor(nightly_conditions.nightly_conditions[2] / 20)
-            ].capitalize()
+            out += CONDITION[4 - math.floor(nightly_conditions.nightly_conditions[0] / 20)].capitalize() + "-"
+            out += CONDITION[4 - math.floor(nightly_conditions.nightly_conditions[1] / 20)].capitalize() + "-"
+            out += CONDITION[4 - math.floor(nightly_conditions.nightly_conditions[2] / 20)].capitalize()
             return out
         return None
 
     @property
     def deepsky_forecast_tomorrow_desc(self):
         """Return Forecast Tomorrow Description."""
         if len(self._deepsky_forecast) > 1:
```

### Comparing `pyastroweatherio-0.22.5.3/pyastroweatherio/helper_functions.py` & `pyastroweatherio-0.23.0.dev1/pyastroweatherio/helper_functions.py`

 * *Files identical despite different names*

### Comparing `pyastroweatherio-0.22.5.3/pyastroweatherio.egg-info/PKG-INFO` & `pyastroweatherio-0.23.0.dev1/pyastroweatherio.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyastroweatherio
-Version: 0.22.5.3
+Version: 0.23.0.dev1
 Summary: Python Wrapper for 7Timer REST API
 Home-page: https://github.com/mawinkler/pyastroweatherio
 Author: Markus Winkler
 Author-email: winkler.info@icloud.com
 License: MIT
 Keywords: AstroWeather,7Timer,Python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pyastroweatherio-0.22.5.3/setup.py` & `pyastroweatherio-0.23.0.dev1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 setup(
     name="pyastroweatherio",
     packages=["pyastroweatherio"],
-    version="0.22.5.3",
+    version="0.23.0.dev1",
     license="MIT",
     description="Python Wrapper for 7Timer REST API",
     long_description=" ".join(
         ["Lightweight Python 3 module to receive data via", "REST API from 7Timer."],
     ),
     author="Markus Winkler",
     author_email="winkler.info@icloud.com",
```

