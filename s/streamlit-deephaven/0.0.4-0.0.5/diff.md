# Comparing `tmp/streamlit-deephaven-0.0.4.tar.gz` & `tmp/streamlit-deephaven-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-deephaven-0.0.4.tar", last modified: Thu Apr  6 17:17:19 2023, max compression
+gzip compressed data, was "streamlit-deephaven-0.0.5.tar", last modified: Mon Apr 10 16:32:55 2023, max compression
```

## Comparing `streamlit-deephaven-0.0.4.tar` & `streamlit-deephaven-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bender     (501) staff       (20)        0 2023-04-06 17:17:19.677280 streamlit-deephaven-0.0.4/
--rw-r--r--   0 bender     (501) staff       (20)     1063 2023-04-02 02:44:37.000000 streamlit-deephaven-0.0.4/LICENSE
--rw-r--r--   0 bender     (501) staff       (20)      359 2023-04-06 17:17:19.677132 streamlit-deephaven-0.0.4/PKG-INFO
--rw-r--r--   0 bender     (501) staff       (20)     1329 2023-04-06 16:47:13.000000 streamlit-deephaven-0.0.4/README.md
--rw-r--r--   0 bender     (501) staff       (20)       38 2023-04-06 17:17:19.677322 streamlit-deephaven-0.0.4/setup.cfg
--rw-r--r--   0 bender     (501) staff       (20)      768 2023-04-06 17:12:40.000000 streamlit-deephaven-0.0.4/setup.py
-drwxr-xr-x   0 bender     (501) staff       (20)        0 2023-04-06 17:17:19.676237 streamlit-deephaven-0.0.4/streamlit_deephaven/
--rw-r--r--   0 bender     (501) staff       (20)     4504 2023-04-06 17:11:59.000000 streamlit-deephaven-0.0.4/streamlit_deephaven/__init__.py
-drwxr-xr-x   0 bender     (501) staff       (20)        0 2023-04-06 17:17:19.676932 streamlit-deephaven-0.0.4/streamlit_deephaven.egg-info/
--rw-r--r--   0 bender     (501) staff       (20)      359 2023-04-06 17:17:19.000000 streamlit-deephaven-0.0.4/streamlit_deephaven.egg-info/PKG-INFO
--rw-r--r--   0 bender     (501) staff       (20)      272 2023-04-06 17:17:19.000000 streamlit-deephaven-0.0.4/streamlit_deephaven.egg-info/SOURCES.txt
--rw-r--r--   0 bender     (501) staff       (20)        1 2023-04-06 17:17:19.000000 streamlit-deephaven-0.0.4/streamlit_deephaven.egg-info/dependency_links.txt
--rw-r--r--   0 bender     (501) staff       (20)       41 2023-04-06 17:17:19.000000 streamlit-deephaven-0.0.4/streamlit_deephaven.egg-info/requires.txt
--rw-r--r--   0 bender     (501) staff       (20)       20 2023-04-06 17:17:19.000000 streamlit-deephaven-0.0.4/streamlit_deephaven.egg-info/top_level.txt
+drwxr-xr-x   0 bender     (501) staff       (20)        0 2023-04-10 16:32:55.492190 streamlit-deephaven-0.0.5/
+-rw-r--r--   0 bender     (501) staff       (20)     1063 2023-04-02 02:44:37.000000 streamlit-deephaven-0.0.5/LICENSE
+-rw-r--r--   0 bender     (501) staff       (20)      359 2023-04-10 16:32:55.492052 streamlit-deephaven-0.0.5/PKG-INFO
+-rw-r--r--   0 bender     (501) staff       (20)     1105 2023-04-10 16:31:53.000000 streamlit-deephaven-0.0.5/README.md
+-rw-r--r--   0 bender     (501) staff       (20)       38 2023-04-10 16:32:55.492230 streamlit-deephaven-0.0.5/setup.cfg
+-rw-r--r--   0 bender     (501) staff       (20)      768 2023-04-10 16:32:30.000000 streamlit-deephaven-0.0.5/setup.py
+drwxr-xr-x   0 bender     (501) staff       (20)        0 2023-04-10 16:32:55.491183 streamlit-deephaven-0.0.5/streamlit_deephaven/
+-rw-r--r--   0 bender     (501) staff       (20)     5048 2023-04-10 16:31:53.000000 streamlit-deephaven-0.0.5/streamlit_deephaven/__init__.py
+drwxr-xr-x   0 bender     (501) staff       (20)        0 2023-04-10 16:32:55.491860 streamlit-deephaven-0.0.5/streamlit_deephaven.egg-info/
+-rw-r--r--   0 bender     (501) staff       (20)      359 2023-04-10 16:32:55.000000 streamlit-deephaven-0.0.5/streamlit_deephaven.egg-info/PKG-INFO
+-rw-r--r--   0 bender     (501) staff       (20)      272 2023-04-10 16:32:55.000000 streamlit-deephaven-0.0.5/streamlit_deephaven.egg-info/SOURCES.txt
+-rw-r--r--   0 bender     (501) staff       (20)        1 2023-04-10 16:32:55.000000 streamlit-deephaven-0.0.5/streamlit_deephaven.egg-info/dependency_links.txt
+-rw-r--r--   0 bender     (501) staff       (20)       41 2023-04-10 16:32:55.000000 streamlit-deephaven-0.0.5/streamlit_deephaven.egg-info/requires.txt
+-rw-r--r--   0 bender     (501) staff       (20)       20 2023-04-10 16:32:55.000000 streamlit-deephaven-0.0.5/streamlit_deephaven.egg-info/top_level.txt
```

### Comparing `streamlit-deephaven-0.0.4/LICENSE` & `streamlit-deephaven-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit-deephaven-0.0.4/setup.py` & `streamlit-deephaven-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="streamlit-deephaven",
-    version="0.0.4",
+    version="0.0.5",
     author="Deephaven Data Labs",
     author_email="support@deephaven.io",
     description="Streamlit Deephaven Component",
     long_description="Use Deephaven within Streamlit and display widgets",
     long_description_content_type="text/plain",
     url="https://github.com/deephaven/streamlit-deephaven",
     packages=setuptools.find_packages(),
```

### Comparing `streamlit-deephaven-0.0.4/streamlit_deephaven/__init__.py` & `streamlit-deephaven-0.0.5/streamlit_deephaven/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import __main__
 import os
 import streamlit.components.v1 as components
 from uuid import uuid4
+import streamlit as st
+from typing import Dict, List, Optional
 
 DEV_MODE = os.environ.get("DH_DEV_MODE", False)
 
 def _str_object_type(obj):
   """Returns the object type as a string value"""
   return f"{obj.__class__.__module__}.{obj.__class__.__name__}"
 
@@ -15,14 +17,39 @@
 
   if name in ('deephaven.table.Table', 'pandas.core.frame.DataFrame'):
     return 'table'
   if name == 'deephaven.plot.figure.Figure':
     return 'chart'
   raise TypeError(f"Unknown object type: {name}")
 
+def open_ctx():
+  """Open the Deephaven execution context. Required before performing any operations on the server."""
+  from deephaven_server import Server
+  # We store the execution context as an attribute on the server instance
+  if not hasattr(Server.instance, '__deephaven_ctx'):
+    print("Initializing Context...")
+
+    from deephaven.execution_context import get_exec_ctx
+    Server.instance.__deephaven_ctx = get_exec_ctx()
+  print("Opening context...")
+  Server.instance.__deephaven_ctx.j_exec_ctx.open()
+  return Server.instance.__deephaven_ctx
+
+def start_server(host: Optional[str] = None, port: Optional[int] = None, jvm_args: Optional[List[str]] = None, dh_args: Dict[str, str] = {}):
+  """Initialize the Deephaven server. This will start the server if it is not already running."""
+  from deephaven_server import Server
+  if Server.instance is None:
+    print("Initializing Deephaven Server...")
+    s = Server(host=host, port=port, jvm_args=jvm_args, dh_args=dh_args)
+    s.start()
+    print("Deephaven Server listening on port", s.port)
+
+  open_ctx()
+  return Server.instance
+
 # Create a wrapper function for the component. This is an optional
 # best practice - we could simply expose the component function returned by
 # `declare_component` and call it done. The wrapper allows us to customize
 # our component's API: we can pre-process its input args, post-process its
 # output value, and add a docstring for users.
 def display_dh(widget, height=600, width=None, object_id=None, key=None):
     """Display a Deephaven widget.
@@ -73,43 +100,25 @@
     # Maybe if we were making a one click widget, that would make sense...
     # component_value = _component_func(iframe_url=iframe_url, object_type=object_type, width=width, height=height, key=key, default=0)
     return components.iframe(iframe_url, height=height, width=width)
 
 
 # Add some test code to play with the component while it's in development.
 # During development, we can run this just as we would any other Streamlit
-# app: `$ streamlit run streamlit_deephaven/__init__.py`
+# app: `$ DH_DEV_MODE=true streamlit run streamlit_deephaven/__init__.py`
 if DEV_MODE:
-    import streamlit as st
-    
-    @st.cache_resource
-    def init_server():
-        print("Starting Deephaven Server...")
-        # Start up the Deephaven Server
-        from deephaven_server import Server
-        s = Server(port=8899)
-        s.start()
-        print("Deephaven Server started!")
-        return s
-    s = init_server()
-
-    @st.cache_resource
-    def init_ctx():
-        # Cache context initiation so that it is only created once
-        from deephaven.execution_context import get_exec_ctx
-        print("Getting Deephaven Context...")
-        return get_exec_ctx()
-    main_exec_ctx = init_ctx()
-
-    st.subheader("Deephaven Component Demo")
-
-    # Create a deephaven component with a simple table
-    # Create a table and display it
-    with main_exec_ctx:
-      from deephaven import time_table
-      from deephaven.plot.figure import Figure
-      t = time_table("00:00:01").update(["x=i", "y=Math.sin(x)", "z=Math.cos(x)"])
-      display_dh(t, height=200)
-
-      f = Figure().plot_xy(series_name="Sine", t=t, x="x", y="y").show()
-      f = f.plot_xy(series_name="Cosine", t=t, x="x", y="z").show()
-      display_dh(f, height=400)
+  import streamlit as st
+  
+  start_server()
+
+  st.subheader("Deephaven Component Demo")
+
+  # Create a deephaven component with a simple table
+  # Create a table and display it
+  from deephaven import time_table
+  from deephaven.plot.figure import Figure
+  t = time_table("00:00:01").update(["x=i", "y=Math.sin(x)", "z=Math.cos(x)"])
+  display_dh(t, height=200)
+
+  f = Figure().plot_xy(series_name="Sine", t=t, x="x", y="y").show()
+  f = f.plot_xy(series_name="Cosine", t=t, x="x", y="z").show()
+  display_dh(f, height=400)
```

