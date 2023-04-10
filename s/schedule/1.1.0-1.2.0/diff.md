# Comparing `tmp/schedule-1.1.0.tar.gz` & `tmp/schedule-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schedule-1.1.0.tar", last modified: Sat Apr 10 10:47:09 2021, max compression
+gzip compressed data, was "schedule-1.2.0.tar", last modified: Mon Apr 10 10:10:20 2023, max compression
```

## Comparing `schedule-1.1.0.tar` & `schedule-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 sijmen    (1000) sijmen    (1000)        0 2021-04-10 10:47:09.282941 schedule-1.1.0/
--rw-r--r--   0 sijmen    (1000) sijmen    (1000)     1539 2021-04-10 10:46:12.000000 schedule-1.1.0/AUTHORS.rst
--rw-r--r--   0 sijmen    (1000) sijmen    (1000)     5719 2021-04-10 10:46:12.000000 schedule-1.1.0/HISTORY.rst
--rw-r--r--   0 sijmen    (1000) sijmen    (1000)     1099 2020-11-14 16:33:21.000000 schedule-1.1.0/LICENSE.txt
--rw-r--r--   0 sijmen    (1000) sijmen    (1000)      147 2020-11-14 16:33:21.000000 schedule-1.1.0/MANIFEST.in
--rw-r--r--   0 sijmen    (1000) sijmen    (1000)     3527 2021-04-10 10:47:09.282941 schedule-1.1.0/PKG-INFO
--rw-r--r--   0 sijmen    (1000) sijmen    (1000)     2078 2021-02-14 16:34:37.000000 schedule-1.1.0/README.rst
-drwxr-xr-x   0 sijmen    (1000) sijmen    (1000)        0 2021-04-10 10:47:09.282941 schedule-1.1.0/schedule/
--rw-r--r--   0 sijmen    (1000) sijmen    (1000)    28680 2021-03-27 14:13:32.000000 schedule-1.1.0/schedule/__init__.py
-drwxr-xr-x   0 sijmen    (1000) sijmen    (1000)        0 2021-04-10 10:47:09.282941 schedule-1.1.0/schedule.egg-info/
--rw-r--r--   0 sijmen    (1000) sijmen    (1000)     3527 2021-04-10 10:47:09.000000 schedule-1.1.0/schedule.egg-info/PKG-INFO
--rw-r--r--   0 sijmen    (1000) sijmen    (1000)      243 2021-04-10 10:47:09.000000 schedule-1.1.0/schedule.egg-info/SOURCES.txt
--rw-r--r--   0 sijmen    (1000) sijmen    (1000)        1 2021-04-10 10:47:09.000000 schedule-1.1.0/schedule.egg-info/dependency_links.txt
--rw-r--r--   0 sijmen    (1000) sijmen    (1000)        9 2021-04-10 10:47:09.000000 schedule-1.1.0/schedule.egg-info/top_level.txt
--rw-r--r--   0 sijmen    (1000) sijmen    (1000)       93 2021-04-10 10:47:09.282941 schedule-1.1.0/setup.cfg
--rw-r--r--   0 sijmen    (1000) sijmen    (1000)     1442 2021-04-10 10:46:12.000000 schedule-1.1.0/setup.py
--rw-r--r--   0 sijmen    (1000) sijmen    (1000)    31857 2021-03-07 10:49:24.000000 schedule-1.1.0/test_schedule.py
+drwxr-xr-x   0 sijmen    (1000) sijmen    (1000)        0 2023-04-10 10:10:19.999968 schedule-1.2.0/
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)     1933 2023-04-10 10:09:26.000000 schedule-1.2.0/AUTHORS.rst
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)     6415 2023-04-10 10:09:26.000000 schedule-1.2.0/HISTORY.rst
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)     1099 2022-10-09 12:03:39.000000 schedule-1.2.0/LICENSE.txt
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)      147 2022-10-09 12:03:39.000000 schedule-1.2.0/MANIFEST.in
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)     3284 2023-04-10 10:10:19.999968 schedule-1.2.0/PKG-INFO
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)     2282 2023-04-09 21:07:47.000000 schedule-1.2.0/README.rst
+drwxr-xr-x   0 sijmen    (1000) sijmen    (1000)        0 2023-04-10 10:10:19.996635 schedule-1.2.0/schedule/
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)    30205 2023-04-09 21:19:45.000000 schedule-1.2.0/schedule/__init__.py
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)        0 2022-10-09 12:03:39.000000 schedule-1.2.0/schedule/py.typed
+drwxr-xr-x   0 sijmen    (1000) sijmen    (1000)        0 2023-04-10 10:10:19.999968 schedule-1.2.0/schedule.egg-info/
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)     3284 2023-04-10 10:10:19.000000 schedule-1.2.0/schedule.egg-info/PKG-INFO
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)      261 2023-04-10 10:10:19.000000 schedule-1.2.0/schedule.egg-info/SOURCES.txt
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)        1 2023-04-10 10:10:19.000000 schedule-1.2.0/schedule.egg-info/dependency_links.txt
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)        9 2023-04-10 10:10:19.000000 schedule-1.2.0/schedule.egg-info/top_level.txt
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)       93 2023-04-10 10:10:19.999968 schedule-1.2.0/setup.cfg
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)     1538 2023-04-10 10:09:26.000000 schedule-1.2.0/setup.py
+-rw-r--r--   0 sijmen    (1000) sijmen    (1000)    35321 2023-04-09 21:19:45.000000 schedule-1.2.0/test_schedule.py
```

### Comparing `schedule-1.1.0/AUTHORS.rst` & `schedule-1.2.0/AUTHORS.rst`

 * *Files 7% similar despite different names*

```diff
@@ -28,8 +28,17 @@
 - rhagenaars <https://github.com/RHagenaars>
 - Skenvy <https://github.com/skenvy>
 - zcking <https://github.com/zcking>
 - Martin Thoma <https://github.com/MartinThoma>
 - ebllg <https://github.com/ebllg>
 - fredthomsen <https://github.com/fredthomsen>
 - biggerfisch <https://github.com/biggerfisch>
-- sosolidkk <https://github.com/sosolidkk>
+- sosolidkk <https://github.com/sosolidkk>
+- rudSarkar <https://github.com/rudSarkar>
+- chrimaho <https://github.com/chrimaho>
+- jweijers <https://github.com/jweijers>
+- Akuli <https://github.com/Akuli>
+- NaelsonDouglas <https://github.com/NaelsonDouglas>
+- SergBobrovsky <https://github.com/SergBobrovsky>
+- CPickens42 <https://github.com/CPickens42>
+- emollier <https://github.com/emollier>
+- sunpro108 <https://github.com/sunpro108>
```

### Comparing `schedule-1.1.0/HISTORY.rst` & `schedule-1.2.0/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,26 @@
 .. :changelog:
 
 History
 -------
 
+1.2.0 (2023-04-10)
+++++++++++++++++++
+
+- Dropped support for Python 3.6, add support for Python 3.10 and 3.11.
+- Add timezone support for .at(). See #517. Thanks @chrimaho!
+- Get next run by tag (#463) Thanks @jweijers!
+- Add py.typed file. See #521. Thanks @Akuli!
+
+- Fix the re pattern of the 'days'. See #506 Thanks @sunpro108!
+- Fix test_until_time failure when run early. See #563. Thanks @emollier!
+- Fix crash repr on partially constructed job. See #569. Thanks @CPickens42!
+- Code cleanup and modernization. See #567, #536. Thanks @masa-08 and @SergBobrovsky!
+- Documentation improvements and fix typos. See #469, #479, #493, #519, #520. Thanks to @NaelsonDouglas, @chrimaho, @rudSarkar
+
 1.1.0 (2021-04-09)
 ++++++++++++++++++
 
 - Added @repeat() decorator. See #148. Thanks @rhagenaars!
 - Added execute .until(). See #195. Thanks @fredthomsen!
 - Added job retrieval filtered by tags using get_jobs('tag'). See #419. Thanks @skenvy!
 - Added type annotations. See #427. Thanks @martinthoma!
```

### Comparing `schedule-1.1.0/LICENSE.txt` & `schedule-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `schedule-1.1.0/PKG-INFO` & `schedule-1.2.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,97 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: schedule
-Version: 1.1.0
+Version: 1.2.0
 Summary: Job scheduling for humans.
 Home-page: https://github.com/dbader/schedule
+Download-URL: https://github.com/dbader/schedule/tarball/1.2.0
 Author: Daniel Bader
 Author-email: mail@dbader.org
 License: MIT
-Download-URL: https://github.com/dbader/schedule/tarball/1.1.0
-Description: `schedule <https://schedule.readthedocs.io/>`__
-        ===============================================
-        
-        
-        .. image:: https://github.com/dbader/schedule/workflows/Tests/badge.svg
-                :target: https://github.com/dbader/schedule/actions?query=workflow%3ATests+branch%3Amaster
-        
-        .. image:: https://coveralls.io/repos/dbader/schedule/badge.svg?branch=master
-                :target: https://coveralls.io/r/dbader/schedule
-        
-        .. image:: https://img.shields.io/pypi/v/schedule.svg
-                :target: https://pypi.python.org/pypi/schedule
-        
-        Python job scheduling for humans. Run Python functions (or any other callable) periodically using a friendly syntax.
-        
-        - A simple to use API for scheduling jobs, made for humans.
-        - In-process scheduler for periodic jobs. No extra processes needed!
-        - Very lightweight and no external dependencies.
-        - Excellent test coverage.
-        - Tested on Python and 3.6, 3.7, 3.8, 3.9
-        
-        Usage
-        -----
-        
-        .. code-block:: bash
-        
-            $ pip install schedule
-        
-        .. code-block:: python
-        
-            import schedule
-            import time
-        
-            def job():
-                print("I'm working...")
-        
-            schedule.every(10).seconds.do(job)
-            schedule.every(10).minutes.do(job)
-            schedule.every().hour.do(job)
-            schedule.every().day.at("10:30").do(job)
-            schedule.every(5).to(10).minutes.do(job)
-            schedule.every().monday.do(job)
-            schedule.every().wednesday.at("13:15").do(job)
-            schedule.every().minute.at(":17").do(job)
-        
-            while True:
-                schedule.run_pending()
-                time.sleep(1)
-        
-        Documentation
-        -------------
-        
-        Schedule's documentation lives at `schedule.readthedocs.io <https://schedule.readthedocs.io/>`_.
-        
-        
-        Meta
-        ----
-        
-        Daniel Bader - `@dbader_org <https://twitter.com/dbader_org>`_ - mail@dbader.org
-        
-        Inspired by `Adam Wiggins' <https://github.com/adamwiggins>`_ article `"Rethinking Cron" <https://adam.herokuapp.com/past/2010/4/13/rethinking_cron/>`_ and the `clockwork <https://github.com/Rykian/clockwork>`_ Ruby module.
-        
-        Distributed under the MIT license. See `LICENSE.txt <https://github.com/dbader/schedule/blob/master/LICENSE.txt>`_ for more information.
-        
-        https://github.com/dbader/schedule
-        
 Keywords: schedule,periodic,jobs,scheduling,clockwork,cron,scheduler,job scheduling
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
-Requires-Python: >=3.6
+Requires-Python: >=3.7
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+`schedule <https://schedule.readthedocs.io/>`__
+===============================================
+
+
+.. image:: https://github.com/dbader/schedule/workflows/Tests/badge.svg
+        :target: https://github.com/dbader/schedule/actions?query=workflow%3ATests+branch%3Amaster
+
+.. image:: https://coveralls.io/repos/dbader/schedule/badge.svg?branch=master
+        :target: https://coveralls.io/r/dbader/schedule
+
+.. image:: https://img.shields.io/pypi/v/schedule.svg
+        :target: https://pypi.python.org/pypi/schedule
+
+Python job scheduling for humans. Run Python functions (or any other callable) periodically using a friendly syntax.
+
+- A simple to use API for scheduling jobs, made for humans.
+- In-process scheduler for periodic jobs. No extra processes needed!
+- Very lightweight and no external dependencies.
+- Excellent test coverage.
+- Tested on Python and 3.7, 3.8, 3.9, 3.10, 3.11
+
+Usage
+-----
+
+.. code-block:: bash
+
+    $ pip install schedule
+
+.. code-block:: python
+
+    import schedule
+    import time
+
+    def job():
+        print("I'm working...")
+
+    schedule.every(10).seconds.do(job)
+    schedule.every(10).minutes.do(job)
+    schedule.every().hour.do(job)
+    schedule.every().day.at("10:30").do(job)
+    schedule.every(5).to(10).minutes.do(job)
+    schedule.every().monday.do(job)
+    schedule.every().wednesday.at("13:15").do(job)
+    schedule.every().day.at("12:42", "Europe/Amsterdam").do(job)
+    schedule.every().minute.at(":17").do(job)
+
+    def job_with_argument(name):
+        print(f"I am {name}")
+
+    schedule.every(10).seconds.do(job_with_argument, name="Peter")
+
+    while True:
+        schedule.run_pending()
+        time.sleep(1)
+
+Documentation
+-------------
+
+Schedule's documentation lives at `schedule.readthedocs.io <https://schedule.readthedocs.io/>`_.
+
+
+Meta
+----
+
+Daniel Bader - `@dbader_org <https://twitter.com/dbader_org>`_ - mail@dbader.org
+
+Inspired by `Adam Wiggins' <https://github.com/adamwiggins>`_ article `"Rethinking Cron" <https://adam.herokuapp.com/past/2010/4/13/rethinking_cron/>`_ and the `clockwork <https://github.com/Rykian/clockwork>`_ Ruby module.
+
+Distributed under the MIT license. See `LICENSE.txt <https://github.com/dbader/schedule/blob/master/LICENSE.txt>`_ for more information.
+
+https://github.com/dbader/schedule
```

### Comparing `schedule-1.1.0/README.rst` & `schedule-1.2.0/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 Python job scheduling for humans. Run Python functions (or any other callable) periodically using a friendly syntax.
 
 - A simple to use API for scheduling jobs, made for humans.
 - In-process scheduler for periodic jobs. No extra processes needed!
 - Very lightweight and no external dependencies.
 - Excellent test coverage.
-- Tested on Python and 3.6, 3.7, 3.8, 3.9
+- Tested on Python and 3.7, 3.8, 3.9, 3.10, 3.11
 
 Usage
 -----
 
 .. code-block:: bash
 
     $ pip install schedule
@@ -37,16 +37,22 @@
     schedule.every(10).seconds.do(job)
     schedule.every(10).minutes.do(job)
     schedule.every().hour.do(job)
     schedule.every().day.at("10:30").do(job)
     schedule.every(5).to(10).minutes.do(job)
     schedule.every().monday.do(job)
     schedule.every().wednesday.at("13:15").do(job)
+    schedule.every().day.at("12:42", "Europe/Amsterdam").do(job)
     schedule.every().minute.at(":17").do(job)
 
+    def job_with_argument(name):
+        print(f"I am {name}")
+
+    schedule.every(10).seconds.do(job_with_argument, name="Peter")
+
     while True:
         schedule.run_pending()
         time.sleep(1)
 
 Documentation
 -------------
```

### Comparing `schedule-1.1.0/schedule/__init__.py` & `schedule-1.2.0/schedule/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 Inspired by Addam Wiggins' article "Rethinking Cron" [1] and the
 "clockwork" Ruby module [2][3].
 
 Features:
     - A simple to use API for scheduling jobs.
     - Very lightweight and no external dependencies.
     - Excellent test coverage.
-    - Tested on Python 3.6, 3.7, 3.8, 3.9
+    - Tested on Python 3.7, 3.8, 3.9, 3.10 and 3.11
 
 Usage:
     >>> import schedule
     >>> import time
 
     >>> def job(message='stuff'):
     >>>     print("I'm working on:", message)
@@ -63,23 +63,23 @@
 
 class IntervalError(ScheduleValueError):
     """An improper interval was used"""
 
     pass
 
 
-class CancelJob(object):
+class CancelJob:
     """
     Can be returned from a job to unschedule itself.
     """
 
     pass
 
 
-class Scheduler(object):
+class Scheduler:
     """
     Objects instantiated by the :class:`Scheduler <Scheduler>` are
     factories to create jobs, keep record of scheduled jobs and
     handle their execution.
     """
 
     def __init__(self) -> None:
@@ -169,39 +169,47 @@
         return job
 
     def _run_job(self, job: "Job") -> None:
         ret = job.run()
         if isinstance(ret, CancelJob) or ret is CancelJob:
             self.cancel_job(job)
 
-    @property
-    def next_run(self) -> Optional[datetime.datetime]:
+    def get_next_run(
+        self, tag: Optional[Hashable] = None
+    ) -> Optional[datetime.datetime]:
         """
         Datetime when the next job should run.
 
+        :param tag: Filter the next run for the given tag parameter
+
         :return: A :class:`~datetime.datetime` object
                  or None if no jobs scheduled
         """
         if not self.jobs:
             return None
-        return min(self.jobs).next_run
+        jobs_filtered = self.get_jobs(tag)
+        if not jobs_filtered:
+            return None
+        return min(jobs_filtered).next_run
+
+    next_run = property(get_next_run)
 
     @property
     def idle_seconds(self) -> Optional[float]:
         """
         :return: Number of seconds until
                  :meth:`next_run <Scheduler.next_run>`
                  or None if no jobs are scheduled
         """
         if not self.next_run:
             return None
         return (self.next_run - datetime.datetime.now()).total_seconds()
 
 
-class Job(object):
+class Job:
     """
     A periodic job as used by :class:`Scheduler`.
 
     :param interval: A quantity of a certain time unit
     :param scheduler: The :class:`Scheduler <Scheduler>` instance that
                       this job will register itself with once it has
                       been fully configured in :meth:`Job.do()`.
@@ -211,25 +219,28 @@
     * a :meth:`time unit <Job.second>`
     * a quantity of `time units` defined by `interval`
 
     A job is usually created and returned by :meth:`Scheduler.every`
     method, which also defines its `interval`.
     """
 
-    def __init__(self, interval: int, scheduler: Scheduler = None):
+    def __init__(self, interval: int, scheduler: Optional[Scheduler] = None):
         self.interval: int = interval  # pause interval * unit between runs
         self.latest: Optional[int] = None  # upper limit to the interval
         self.job_func: Optional[functools.partial] = None  # the job job_func to run
 
         # time units, e.g. 'minutes', 'hours', ...
         self.unit: Optional[str] = None
 
         # optional time at which this job runs
         self.at_time: Optional[datetime.time] = None
 
+        # optional time zone of the self.at_time field. Only relevant when at_time is not None
+        self.at_time_zone = None
+
         # datetime of the last run
         self.last_run: Optional[datetime.datetime] = None
 
         # datetime of the next run
         self.next_run: Optional[datetime.datetime] = None
 
         # timedelta between runs, only valid for
@@ -277,17 +288,21 @@
             format_time(self.next_run),
         )
 
         if hasattr(self.job_func, "__name__"):
             job_func_name = self.job_func.__name__
         else:
             job_func_name = repr(self.job_func)
-        args = [repr(x) if is_repr(x) else str(x) for x in self.job_func.args]
-        kwargs = ["%s=%s" % (k, repr(v)) for k, v in self.job_func.keywords.items()]
-        call_repr = job_func_name + "(" + ", ".join(args + kwargs) + ")"
+
+        if self.job_func is not None:
+            args = [repr(x) if is_repr(x) else str(x) for x in self.job_func.args]
+            kwargs = ["%s=%s" % (k, repr(v)) for k, v in self.job_func.keywords.items()]
+            call_repr = job_func_name + "(" + ", ".join(args + kwargs) + ")"
+        else:
+            call_repr = "[None]"
 
         if self.at_time is not None:
             return "Every %s %s at %s do %s %s" % (
                 self.interval,
                 self.unit[:-1] if self.interval == 1 else self.unit,
                 self.at_time,
                 call_repr,
@@ -450,42 +465,58 @@
         :return: The invoked job instance
         """
         if not all(isinstance(tag, Hashable) for tag in tags):
             raise TypeError("Tags must be hashable")
         self.tags.update(tags)
         return self
 
-    def at(self, time_str):
+    def at(self, time_str: str, tz: Optional[str] = None):
 
         """
         Specify a particular time that the job should be run at.
 
         :param time_str: A string in one of the following formats:
 
             - For daily jobs -> `HH:MM:SS` or `HH:MM`
             - For hourly jobs -> `MM:SS` or `:MM`
             - For minute jobs -> `:SS`
 
             The format must make sense given how often the job is
             repeating; for example, a job that repeats every minute
             should not be given a string in the form `HH:MM:SS`. The
-            difference between `:MM` and :SS` is inferred from the
+            difference between `:MM` and `:SS` is inferred from the
             selected time-unit (e.g. `every().hour.at(':30')` vs.
             `every().minute.at(':30')`).
 
+        :param tz: The timezone that this timestamp refers to. Can be
+            a string that can be parsed by pytz.timezone(), or a pytz.BaseTzInfo object
+
         :return: The invoked job instance
         """
         if self.unit not in ("days", "hours", "minutes") and not self.start_day:
             raise ScheduleValueError(
                 "Invalid unit (valid units are `days`, `hours`, and `minutes`)"
             )
+
+        if tz is not None:
+            import pytz
+
+            if isinstance(tz, str):
+                self.at_time_zone = pytz.timezone(tz)  # type: ignore
+            elif isinstance(tz, pytz.BaseTzInfo):
+                self.at_time_zone = tz
+            else:
+                raise ScheduleValueError(
+                    "Timezone must be string or pytz.timezone object"
+                )
+
         if not isinstance(time_str, str):
             raise TypeError("at() should be passed a string")
         if self.unit == "days" or self.start_day:
-            if not re.match(r"^([0-2]\d:)?[0-5]\d:[0-5]\d$", time_str):
+            if not re.match(r"^[0-2]\d:[0-5]\d(:[0-5]\d)?$", time_str):
                 raise ScheduleValueError(
                     "Invalid time format for a daily job (valid format is HH:MM(:SS)?)"
                 )
         if self.unit == "hours":
             if not re.match(r"^([0-5]\d)?:[0-5]\d$", time_str):
                 raise ScheduleValueError(
                     "Invalid time format for an hourly job (valid format is (MM)?:SS)"
@@ -519,14 +550,15 @@
                     "Invalid number of hours ({} is not between 0 and 23)"
                 )
         elif self.unit == "hours":
             hour = 0
         elif self.unit == "minutes":
             hour = 0
             minute = 0
+        hour = int(hour)
         minute = int(minute)
         second = int(second)
         self.at_time = datetime.time(hour, minute, second)
         return self
 
     def to(self, latest: int):
         """
@@ -558,15 +590,15 @@
         If until_time is a moment in the past, ScheduleValueError is thrown.
 
         :param until_time: A moment in the future representing the latest time a job can
            be run. If only a time is supplied, the date is set to today.
            The following formats are accepted:
 
            - datetime.datetime
-           -  datetime.timedelta
+           - datetime.timedelta
            - datetime.time
            - String in one of the following formats: "%Y-%m-%d %H:%M:%S",
              "%Y-%m-%d %H:%M", "%Y-%m-%d", "%H:%M:%S", "%H:%M"
              as defined by strptime() behaviour. If an invalid string format is passed,
              ScheduleValueError is thrown.
 
         :return: The invoked job instance
@@ -712,14 +744,24 @@
                 raise ScheduleValueError("Invalid unit without specifying start day")
             kwargs = {"second": self.at_time.second, "microsecond": 0}
             if self.unit == "days" or self.start_day is not None:
                 kwargs["hour"] = self.at_time.hour
             if self.unit in ["days", "hours"] or self.start_day is not None:
                 kwargs["minute"] = self.at_time.minute
             self.next_run = self.next_run.replace(**kwargs)  # type: ignore
+
+            if self.at_time_zone is not None:
+                # Convert next_run from the expected timezone into the local time
+                # self.next_run is a naive datetime so after conversion remove tzinfo
+                self.next_run = (
+                    self.at_time_zone.localize(self.next_run)
+                    .astimezone()
+                    .replace(tzinfo=None)
+                )
+
             # Make sure we run at the specified time *today* (or *this hour*)
             # as well. This accounts for when a job takes so long it finished
             # in the next period.
             if not self.last_run or (self.next_run - self.last_run) > self.period:
                 now = datetime.datetime.now()
                 if (
                     self.unit == "days"
@@ -804,19 +846,19 @@
 def cancel_job(job: Job) -> None:
     """Calls :meth:`cancel_job <Scheduler.cancel_job>` on the
     :data:`default scheduler instance <default_scheduler>`.
     """
     default_scheduler.cancel_job(job)
 
 
-def next_run() -> Optional[datetime.datetime]:
+def next_run(tag: Optional[Hashable] = None) -> Optional[datetime.datetime]:
     """Calls :meth:`next_run <Scheduler.next_run>` on the
     :data:`default scheduler instance <default_scheduler>`.
     """
-    return default_scheduler.next_run
+    return default_scheduler.get_next_run(tag)
 
 
 def idle_seconds() -> Optional[float]:
     """Calls :meth:`idle_seconds <Scheduler.idle_seconds>` on the
     :data:`default scheduler instance <default_scheduler>`.
     """
     return default_scheduler.idle_seconds
```

### Comparing `schedule-1.1.0/schedule.egg-info/PKG-INFO` & `schedule-1.2.0/schedule.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,89 +1,97 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: schedule
-Version: 1.1.0
+Version: 1.2.0
 Summary: Job scheduling for humans.
 Home-page: https://github.com/dbader/schedule
+Download-URL: https://github.com/dbader/schedule/tarball/1.2.0
 Author: Daniel Bader
 Author-email: mail@dbader.org
 License: MIT
-Download-URL: https://github.com/dbader/schedule/tarball/1.1.0
-Description: `schedule <https://schedule.readthedocs.io/>`__
-        ===============================================
-        
-        
-        .. image:: https://github.com/dbader/schedule/workflows/Tests/badge.svg
-                :target: https://github.com/dbader/schedule/actions?query=workflow%3ATests+branch%3Amaster
-        
-        .. image:: https://coveralls.io/repos/dbader/schedule/badge.svg?branch=master
-                :target: https://coveralls.io/r/dbader/schedule
-        
-        .. image:: https://img.shields.io/pypi/v/schedule.svg
-                :target: https://pypi.python.org/pypi/schedule
-        
-        Python job scheduling for humans. Run Python functions (or any other callable) periodically using a friendly syntax.
-        
-        - A simple to use API for scheduling jobs, made for humans.
-        - In-process scheduler for periodic jobs. No extra processes needed!
-        - Very lightweight and no external dependencies.
-        - Excellent test coverage.
-        - Tested on Python and 3.6, 3.7, 3.8, 3.9
-        
-        Usage
-        -----
-        
-        .. code-block:: bash
-        
-            $ pip install schedule
-        
-        .. code-block:: python
-        
-            import schedule
-            import time
-        
-            def job():
-                print("I'm working...")
-        
-            schedule.every(10).seconds.do(job)
-            schedule.every(10).minutes.do(job)
-            schedule.every().hour.do(job)
-            schedule.every().day.at("10:30").do(job)
-            schedule.every(5).to(10).minutes.do(job)
-            schedule.every().monday.do(job)
-            schedule.every().wednesday.at("13:15").do(job)
-            schedule.every().minute.at(":17").do(job)
-        
-            while True:
-                schedule.run_pending()
-                time.sleep(1)
-        
-        Documentation
-        -------------
-        
-        Schedule's documentation lives at `schedule.readthedocs.io <https://schedule.readthedocs.io/>`_.
-        
-        
-        Meta
-        ----
-        
-        Daniel Bader - `@dbader_org <https://twitter.com/dbader_org>`_ - mail@dbader.org
-        
-        Inspired by `Adam Wiggins' <https://github.com/adamwiggins>`_ article `"Rethinking Cron" <https://adam.herokuapp.com/past/2010/4/13/rethinking_cron/>`_ and the `clockwork <https://github.com/Rykian/clockwork>`_ Ruby module.
-        
-        Distributed under the MIT license. See `LICENSE.txt <https://github.com/dbader/schedule/blob/master/LICENSE.txt>`_ for more information.
-        
-        https://github.com/dbader/schedule
-        
 Keywords: schedule,periodic,jobs,scheduling,clockwork,cron,scheduler,job scheduling
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Natural Language :: English
-Requires-Python: >=3.6
+Requires-Python: >=3.7
+License-File: LICENSE.txt
+License-File: AUTHORS.rst
+
+`schedule <https://schedule.readthedocs.io/>`__
+===============================================
+
+
+.. image:: https://github.com/dbader/schedule/workflows/Tests/badge.svg
+        :target: https://github.com/dbader/schedule/actions?query=workflow%3ATests+branch%3Amaster
+
+.. image:: https://coveralls.io/repos/dbader/schedule/badge.svg?branch=master
+        :target: https://coveralls.io/r/dbader/schedule
+
+.. image:: https://img.shields.io/pypi/v/schedule.svg
+        :target: https://pypi.python.org/pypi/schedule
+
+Python job scheduling for humans. Run Python functions (or any other callable) periodically using a friendly syntax.
+
+- A simple to use API for scheduling jobs, made for humans.
+- In-process scheduler for periodic jobs. No extra processes needed!
+- Very lightweight and no external dependencies.
+- Excellent test coverage.
+- Tested on Python and 3.7, 3.8, 3.9, 3.10, 3.11
+
+Usage
+-----
+
+.. code-block:: bash
+
+    $ pip install schedule
+
+.. code-block:: python
+
+    import schedule
+    import time
+
+    def job():
+        print("I'm working...")
+
+    schedule.every(10).seconds.do(job)
+    schedule.every(10).minutes.do(job)
+    schedule.every().hour.do(job)
+    schedule.every().day.at("10:30").do(job)
+    schedule.every(5).to(10).minutes.do(job)
+    schedule.every().monday.do(job)
+    schedule.every().wednesday.at("13:15").do(job)
+    schedule.every().day.at("12:42", "Europe/Amsterdam").do(job)
+    schedule.every().minute.at(":17").do(job)
+
+    def job_with_argument(name):
+        print(f"I am {name}")
+
+    schedule.every(10).seconds.do(job_with_argument, name="Peter")
+
+    while True:
+        schedule.run_pending()
+        time.sleep(1)
+
+Documentation
+-------------
+
+Schedule's documentation lives at `schedule.readthedocs.io <https://schedule.readthedocs.io/>`_.
+
+
+Meta
+----
+
+Daniel Bader - `@dbader_org <https://twitter.com/dbader_org>`_ - mail@dbader.org
+
+Inspired by `Adam Wiggins' <https://github.com/adamwiggins>`_ article `"Rethinking Cron" <https://adam.herokuapp.com/past/2010/4/13/rethinking_cron/>`_ and the `clockwork <https://github.com/Rykian/clockwork>`_ Ruby module.
+
+Distributed under the MIT license. See `LICENSE.txt <https://github.com/dbader/schedule/blob/master/LICENSE.txt>`_ for more information.
+
+https://github.com/dbader/schedule
```

### Comparing `schedule-1.1.0/setup.py` & `schedule-1.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import codecs
 from setuptools import setup
 
 
-SCHEDULE_VERSION = "1.1.0"
+SCHEDULE_VERSION = "1.2.0"
 SCHEDULE_DOWNLOAD_URL = "https://github.com/dbader/schedule/tarball/" + SCHEDULE_VERSION
 
 
 def read_file(filename):
     """
     Read a utf8 encoded text file and return its contents.
     """
     with codecs.open(filename, "r", "utf8") as f:
         return f.read()
 
 
 setup(
     name="schedule",
     packages=["schedule"],
+    package_data={"schedule": ["py.typed"]},
     version=SCHEDULE_VERSION,
     description="Job scheduling for humans.",
     long_description=read_file("README.rst"),
     license="MIT",
     author="Daniel Bader",
     author_email="mail@dbader.org",
     url="https://github.com/dbader/schedule",
@@ -38,15 +39,16 @@
     classifiers=[
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Development Status :: 5 - Production/Stable",
         "Operating System :: OS Independent",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Natural Language :: English",
     ],
-    python_requires=">=3.6",
+    python_requires=">=3.7",
 )
```

### Comparing `schedule-1.1.0/test_schedule.py` & `schedule-1.2.0/test_schedule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,52 @@
 """Unit tests for schedule.py"""
 import datetime
 import functools
 import mock
 import unittest
+import os
+import time
 
 # Silence "missing docstring", "method could be a function",
 # "class already defined", and "too many public methods" messages:
 # pylint: disable-msg=R0201,C0111,E0102,R0904,R0901
 
 import schedule
 from schedule import (
     every,
     repeat,
     ScheduleError,
     ScheduleValueError,
     IntervalError,
 )
 
+# Set timezone to Europe/Berlin (CEST) to ensure global reproducibility
+os.environ["TZ"] = "CET-1CEST,M3.5.0,M10.5.0"
+time.tzset()
+
 
 def make_mock_job(name=None):
     job = mock.Mock()
     job.__name__ = name or "job"
     return job
 
 
-class mock_datetime(object):
+class mock_datetime:
     """
     Monkey-patch datetime for predictable results
     """
 
     def __init__(self, year, month, day, hour, minute, second=0):
         self.year = year
         self.month = month
         self.day = day
         self.hour = hour
         self.minute = minute
         self.second = second
+        self.original_datetime = None
 
     def __enter__(self):
         class MockDate(datetime.datetime):
             @classmethod
             def today(cls):
                 return cls(self.year, self.month, self.day)
 
@@ -185,14 +192,28 @@
 
         # test self.latest >= self.interval
         job_instance.latest = 1
         self.assertRaises(ScheduleError, job_instance._schedule_next_run)
         job_instance.latest = 3
         self.assertRaises(ScheduleError, job_instance._schedule_next_run)
 
+    def test_next_run_with_tag(self):
+        with mock_datetime(2014, 6, 28, 12, 0):
+            job1 = every(5).seconds.do(make_mock_job(name="job1")).tag("tag1")
+            job2 = every(2).hours.do(make_mock_job(name="job2")).tag("tag1", "tag2")
+            job3 = (
+                every(1)
+                .minutes.do(make_mock_job(name="job3"))
+                .tag("tag1", "tag3", "tag2")
+            )
+            assert schedule.next_run("tag1") == job1.next_run
+            assert schedule.default_scheduler.get_next_run("tag2") == job3.next_run
+            assert schedule.next_run("tag3") == job3.next_run
+            assert schedule.next_run("tag4") is None
+
     def test_singular_time_units_match_plural_units(self):
         assert every().second.unit == every().seconds.unit
         assert every().minute.unit == every().minutes.unit
         assert every().hour.unit == every().hours.unit
         assert every().day.unit == every().days.unit
         assert every().week.unit == every().weeks.unit
 
@@ -221,22 +242,24 @@
 
         assert job_repr.startswith("Every 5 to 30 minutes do job()")
 
     def test_at_time(self):
         mock_job = make_mock_job()
         assert every().day.at("10:30").do(mock_job).next_run.hour == 10
         assert every().day.at("10:30").do(mock_job).next_run.minute == 30
+        assert every().day.at("20:59").do(mock_job).next_run.minute == 59
         assert every().day.at("10:30:50").do(mock_job).next_run.second == 50
 
         self.assertRaises(ScheduleValueError, every().day.at, "2:30:000001")
         self.assertRaises(ScheduleValueError, every().day.at, "::2")
         self.assertRaises(ScheduleValueError, every().day.at, ".2")
         self.assertRaises(ScheduleValueError, every().day.at, "2")
         self.assertRaises(ScheduleValueError, every().day.at, ":2")
         self.assertRaises(ScheduleValueError, every().day.at, " 2:30:00")
+        self.assertRaises(ScheduleValueError, every().day.at, "59:59")
         self.assertRaises(ScheduleValueError, every().do, lambda: 0)
         self.assertRaises(TypeError, every().day.at, 2)
 
         # without a context manager, it incorrectly raises an error because
         # it is not callable
         with self.assertRaises(IntervalError):
             every(interval=2).second
@@ -310,15 +333,16 @@
             ScheduleValueError,
             every().day.until,
             datetime.datetime(2019, 12, 31, 23, 59),
         )
         self.assertRaises(
             ScheduleValueError, every().day.until, datetime.timedelta(minutes=-1)
         )
-        self.assertRaises(ScheduleValueError, every().day.until, datetime.time(hour=5))
+        one_hour_ago = datetime.datetime.now() - datetime.timedelta(hours=1)
+        self.assertRaises(ScheduleValueError, every().day.until, one_hour_ago)
 
         # Unschedule job after next_run passes the deadline
         schedule.clear()
         with mock_datetime(2020, 1, 1, 11, 35, 10):
             mock_job.reset_mock()
             every(5).seconds.until(datetime.time(11, 35, 20)).do(mock_job)
             with mock_datetime(2020, 1, 1, 11, 35, 15):
@@ -495,14 +519,66 @@
             assert job.next_run.second == 15
 
         with mock_datetime(2010, 10, 10, 10, 12, 16):
             job.run()
             assert job.next_run.minute == 13
             assert job.next_run.second == 15
 
+    def test_at_timezone(self):
+        mock_job = make_mock_job()
+        try:
+            import pytz
+        except ModuleNotFoundError:
+            self.skipTest("pytz unavailable")
+            return
+
+        with mock_datetime(2022, 2, 1, 23, 15):
+            # Current Berlin time: feb-1 23:15 (local)
+            # Current India time: feb-2 03:45
+            # Expected to run India time: feb-2 06:30
+            # Next run Berlin time: feb-2 02:00
+            next = every().day.at("06:30", "Asia/Kolkata").do(mock_job).next_run
+            assert next.hour == 2
+            assert next.minute == 0
+
+        with mock_datetime(2022, 4, 8, 10, 0):
+            # Current Berlin time: 10:00 (local) (during daylight saving)
+            # Current NY time: 04:00
+            # Expected to run NY time: 10:30
+            # Next run Berlin time: 16:30
+            next = every().day.at("10:30", "America/New_York").do(mock_job).next_run
+            assert next.hour == 16
+            assert next.minute == 30
+
+        with mock_datetime(2022, 3, 20, 10, 0):
+            # Current Berlin time: 10:00 (local) (NOT during daylight saving)
+            # Current NY time: 04:00 (during daylight saving)
+            # Expected to run NY time: 10:30
+            # Next run Berlin time: 15:30
+            tz = pytz.timezone("America/New_York")
+            next = every().day.at("10:30", tz).do(mock_job).next_run
+            assert next.hour == 15
+            assert next.minute == 30
+
+        with self.assertRaises(pytz.exceptions.UnknownTimeZoneError):
+            every().day.at("10:30", "FakeZone").do(mock_job)
+
+        with self.assertRaises(ScheduleValueError):
+            every().day.at("10:30", 43).do(mock_job)
+
+    def test_daylight_saving_time(self):
+        mock_job = make_mock_job()
+        # 27 March 2022, 02:00:00 clocks were turned forward 1 hour
+        with mock_datetime(2022, 3, 27, 0, 0):
+            assert every(4).hours.do(mock_job).next_run.hour == 4
+
+        # Sunday, 30 October 2022, 03:00:00 clocks were turned backward 1 hour
+        with mock_datetime(2022, 10, 30, 0, 0):
+            assert every(4).hours.do(mock_job).next_run.hour == 4
+
     def test_run_all(self):
         mock_job = make_mock_job()
         every().minute.do(mock_job)
         every().hour.do(mock_job)
         every().day.at("11:00").do(mock_job)
         schedule.run_all()
         assert mock_job.call_count == 3
@@ -581,14 +657,18 @@
         assert s2.startswith(
             (
                 "Every 1 day at 00:00:00 do job_fun('foo', "
                 "bar=23) (last run: [never], next run: "
             )
         )
 
+        # Ensure Job.__repr__ does not throw exception on a partially-composed Job
+        s3 = repr(schedule.every(10))
+        assert s3 == "Every 10 None do [None] (last run: [never], next run: [never])"
+
     def test_to_string_lambda_job_func(self):
         assert len(str(every().minute.do(lambda: 1))) > 1
         assert len(str(every().day.at("10:30").do(lambda: 1))) > 1
 
     def test_repr_functools_partial_job_func(self):
         def job_fun(arg):
             pass
@@ -710,15 +790,15 @@
             every().day.do(daily_job)
             every().hour.do(hourly_job)
             assert len(schedule.jobs) == 2
             # Make sure the hourly job is first
             assert schedule.next_run() == original_datetime(2010, 1, 6, 14, 16)
 
     def test_idle_seconds(self):
-        assert schedule.next_run() is None
+        assert schedule.default_scheduler.next_run is None
         assert schedule.idle_seconds() is None
 
         mock_job = make_mock_job()
         with mock_datetime(2020, 12, 9, 21, 46):
             job = every().hour.do(mock_job)
             assert schedule.idle_seconds() == 60 * 60
             schedule.cancel_job(job)
```

