# Comparing `tmp/plantuml_sequence-0.1.1.tar.gz` & `tmp/plantuml_sequence-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plantuml_sequence-0.1.1.tar", max compression
+gzip compressed data, was "plantuml_sequence-0.2.0.tar", max compression
```

## Comparing `plantuml_sequence-0.1.1.tar` & `plantuml_sequence-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1069 2023-04-06 10:03:16.416578 plantuml_sequence-0.1.1/LICENSE
--rw-r--r--   0        0        0     2410 2023-04-10 15:28:49.331488 plantuml_sequence-0.1.1/README.md
--rw-r--r--   0        0        0       52 2023-04-10 15:36:43.909170 plantuml_sequence-0.1.1/plantuml_sequence/__init__.py
--rw-r--r--   0        0        0    13860 2023-04-10 15:28:49.337755 plantuml_sequence-0.1.1/plantuml_sequence/diagram.py
--rw-r--r--   0        0        0        0 2023-04-10 10:02:31.709709 plantuml_sequence-0.1.1/plantuml_sequence/py.typed
--rw-r--r--   0        0        0     4783 2023-04-10 10:12:37.459284 plantuml_sequence-0.1.1/plantuml_sequence/utils.py
--rw-r--r--   0        0        0     2280 2023-04-10 15:37:45.576156 plantuml_sequence-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     3119 1970-01-01 00:00:00.000000 plantuml_sequence-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-04-06 10:03:16.416578 plantuml_sequence-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2410 2023-04-10 15:28:49.331488 plantuml_sequence-0.2.0/README.md
+-rw-r--r--   0        0        0       52 2023-04-10 15:36:43.909170 plantuml_sequence-0.2.0/plantuml_sequence/__init__.py
+-rw-r--r--   0        0        0    15464 2023-04-10 17:07:01.248505 plantuml_sequence-0.2.0/plantuml_sequence/diagram.py
+-rw-r--r--   0        0        0        0 2023-04-10 10:02:31.709709 plantuml_sequence-0.2.0/plantuml_sequence/py.typed
+-rw-r--r--   0        0        0     4783 2023-04-10 10:12:37.459284 plantuml_sequence-0.2.0/plantuml_sequence/utils.py
+-rw-r--r--   0        0        0     2280 2023-04-10 17:07:39.827583 plantuml_sequence-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3119 1970-01-01 00:00:00.000000 plantuml_sequence-0.2.0/PKG-INFO
```

### Comparing `plantuml_sequence-0.1.1/LICENSE` & `plantuml_sequence-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plantuml_sequence-0.1.1/README.md` & `plantuml_sequence-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `plantuml_sequence-0.1.1/plantuml_sequence/diagram.py` & `plantuml_sequence-0.2.0/plantuml_sequence/diagram.py`

 * *Files 4% similar despite different names*

```diff
@@ -288,36 +288,82 @@
         :rtype: Self
         """
         title = utils.escape_newlines(title) if title is not None else ""
         self._line_writer.writeline(f"newpage {title}")
         return self
 
     @contextlib.contextmanager
-    def activate_lifeline(
+    def active_lifeline(
         self, participant: Participant | str, color: str = "", destroy: bool = False
     ) -> collections.abc.Generator[Self, None, None]:
         """
         Contextmanager to activate the lifeline of a participant
 
         :param participant: Participant to activate
         :type participant: Participant | str
         :param color: Color of the active lifeline, defaults to ""
         :type color: str, optional
         :param destroy: Whether to destroy or deactivate the lifeline at the end of the context, defaults to False
         :type destroy: bool, optional
         :yield: Sequence diagram instance
         :rtype: Iterator[collections.abc.Generator[Self, None, None]]
         """
-        alias = participant_to_string(participant)
-        self._line_writer.writeline(f"activate {alias} {color}")
+        self.activate_lifeline(participant, color)
         try:
             yield self
         finally:
-            action = "destroy" if destroy else "deactivate"
-            self._line_writer.writeline(f"{action} {alias}")
+            if destroy:
+                self.destroy_lifeline(participant)
+            else:
+                self.deactivate_lifeline(participant)
+
+    def activate_lifeline(self, participant: Participant | str, color: str = "") -> Self:
+        """
+        Activate the lifeline of `participant`
+
+        :param participant: Participant to activate
+        :type participant: Participant | str
+        :param color: Color of the active lifeline, defaults to ""
+        :type color: str, optional
+        :return: Sequence diagram instance
+        :rtype: Self
+        """
+        alias = participant_to_string(participant)
+        self._line_writer.writeline(f"activate {alias} {color}")
+        return self
+
+    def deactivate_lifeline(self, participant: Participant | str) -> Self:
+        """
+        Deactivate the lifeline of `participant`
+
+        :param participant: Participant to activate
+        :type participant: Participant | str
+        :param color: Color of the active lifeline, defaults to ""
+        :type color: str, optional
+        :return: Sequence diagram instance
+        :rtype: Self
+        """
+        alias = participant_to_string(participant)
+        self._line_writer.writeline(f"deactivate {alias}")
+        return self
+
+    def destroy_lifeline(self, participant: Participant | str) -> Self:
+        """
+        Deactivate the lifeline of `participant`
+
+        :param participant: Participant to activate
+        :type participant: Participant | str
+        :param color: Color of the active lifeline, defaults to ""
+        :type color: str, optional
+        :return: Sequence diagram instance
+        :rtype: Self
+        """
+        alias = participant_to_string(participant)
+        self._line_writer.writeline(f"deactivate {alias}")
+        return self
 
     def delay(self, msg: str | None = None) -> Self:
         """
         Indicate a delay in the diagram
 
         :param msg: Message to add to the delay, defaults to None
         :type msg: str | None, optional
```

### Comparing `plantuml_sequence-0.1.1/plantuml_sequence/utils.py` & `plantuml_sequence-0.2.0/plantuml_sequence/utils.py`

 * *Files identical despite different names*

### Comparing `plantuml_sequence-0.1.1/pyproject.toml` & `plantuml_sequence-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "plantuml-sequence"
-version = "0.1.1"
+version = "0.2.0"
 description = "Create PlantUML sequence charts programmatically from Python"
 authors = ["Jonas Ehrlich <jonas.ehrlich@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/jonasehrlich/plantuml-sequence"
 repository = "https://github.com/jonasehrlich/plantuml-sequence"
 keywords = ["plantuml", "charts"]
```

### Comparing `plantuml_sequence-0.1.1/PKG-INFO` & `plantuml_sequence-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plantuml-sequence
-Version: 0.1.1
+Version: 0.2.0
 Summary: Create PlantUML sequence charts programmatically from Python
 Home-page: https://github.com/jonasehrlich/plantuml-sequence
 License: MIT
 Keywords: plantuml,charts
 Author: Jonas Ehrlich
 Author-email: jonas.ehrlich@gmail.com
 Requires-Python: >=3.10
```

