# Comparing `tmp/motion_python-0.1.27.tar.gz` & `tmp/motion_python-0.1.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "motion_python-0.1.27.tar", max compression
+gzip compressed data, was "motion_python-0.1.28.tar", max compression
```

## Comparing `motion_python-0.1.27.tar` & `motion_python-0.1.28.tar`

### file list

```diff
@@ -1,29 +1,29 @@
--rw-r--r--   0        0        0     2819 2023-04-07 23:27:00.723290 motion_python-0.1.27/README.md
--rw-r--r--   0        0        0      641 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/__init__.py
--rw-r--r--   0        0        0       80 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/api/__init__.py
--rw-r--r--   0        0        0     6702 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/api/api.py
--rw-r--r--   0        0        0      616 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/api/models.py
--rw-r--r--   0        0        0     2582 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/cli.py
--rw-r--r--   0        0        0     6675 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/client.py
--rw-r--r--   0        0        0    21748 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/cursor.py
--rw-r--r--   0        0        0     8099 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/entry.py
--rw-r--r--   0        0        0      214 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/examples/basic/mconfig.py
--rw-r--r--   0        0        0        0 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/examples/basic/schemas/__init__.py
--rw-r--r--   0        0        0        0 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/examples/basic/triggers/__init__.py
--rw-r--r--   0        0        0     1796 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/examples/cooking/dashboard.py
--rw-r--r--   0        0        0      388 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/examples/cooking/mconfig.py
--rw-r--r--   0        0        0       63 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/examples/cooking/requirements.txt
--rw-r--r--   0        0        0       73 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/examples/cooking/schemas/__init__.py
--rw-r--r--   0        0        0      421 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/examples/cooking/schemas/all.py
--rw-r--r--   0        0        0     1351 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/examples/cooking/test.py
--rw-r--r--   0        0        0      134 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/examples/cooking/triggers/__init__.py
--rw-r--r--   0        0        0     4564 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/examples/cooking/triggers/scrape.py
--rw-r--r--   0        0        0     4820 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/examples/cooking/triggers/search.py
--rw-r--r--   0        0        0     1771 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/routing.py
--rw-r--r--   0        0        0     2671 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/schema.py
--rw-r--r--   0        0        0    14188 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/store.py
--rw-r--r--   0        0        0     3741 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/task.py
--rw-r--r--   0        0        0     5010 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/trigger.py
--rw-r--r--   0        0        0     1092 2023-04-07 23:27:00.727290 motion_python-0.1.27/motion/utils.py
--rw-r--r--   0        0        0     1416 2023-04-07 23:27:25.743520 motion_python-0.1.27/pyproject.toml
--rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 motion_python-0.1.27/PKG-INFO
+-rw-r--r--   0        0        0     2819 2023-04-10 04:39:54.759126 motion_python-0.1.28/README.md
+-rw-r--r--   0        0        0      641 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/__init__.py
+-rw-r--r--   0        0        0       80 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/api/__init__.py
+-rw-r--r--   0        0        0     6702 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/api/api.py
+-rw-r--r--   0        0        0      616 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/api/models.py
+-rw-r--r--   0        0        0     2582 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/cli.py
+-rw-r--r--   0        0        0     9885 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/client.py
+-rw-r--r--   0        0        0    21544 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/cursor.py
+-rw-r--r--   0        0        0     8664 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/entry.py
+-rw-r--r--   0        0        0      214 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/examples/basic/mconfig.py
+-rw-r--r--   0        0        0        0 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/examples/basic/schemas/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/examples/basic/triggers/__init__.py
+-rw-r--r--   0        0        0     1796 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/examples/cooking/dashboard.py
+-rw-r--r--   0        0        0      388 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/examples/cooking/mconfig.py
+-rw-r--r--   0        0        0       63 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/examples/cooking/requirements.txt
+-rw-r--r--   0        0        0       73 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/examples/cooking/schemas/__init__.py
+-rw-r--r--   0        0        0      398 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/examples/cooking/schemas/all.py
+-rw-r--r--   0        0        0     1348 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/examples/cooking/test.py
+-rw-r--r--   0        0        0      134 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/examples/cooking/triggers/__init__.py
+-rw-r--r--   0        0        0     4617 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/examples/cooking/triggers/scrape.py
+-rw-r--r--   0        0        0     5003 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/examples/cooking/triggers/search.py
+-rw-r--r--   0        0        0     2975 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/routing.py
+-rw-r--r--   0        0        0     3477 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/schema.py
+-rw-r--r--   0        0        0    14188 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/store.py
+-rw-r--r--   0        0        0     3741 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/task.py
+-rw-r--r--   0        0        0     5977 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/trigger.py
+-rw-r--r--   0        0        0     1092 2023-04-10 04:39:54.763126 motion_python-0.1.28/motion/utils.py
+-rw-r--r--   0        0        0     1416 2023-04-10 04:40:19.209039 motion_python-0.1.28/pyproject.toml
+-rw-r--r--   0        0        0     3915 1970-01-01 00:00:00.000000 motion_python-0.1.28/PKG-INFO
```

### Comparing `motion_python-0.1.27/README.md` & `motion_python-0.1.28/README.md`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.27/motion/__init__.py` & `motion_python-0.1.28/motion/__init__.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.27/motion/api/api.py` & `motion_python-0.1.28/motion/api/api.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.27/motion/api/models.py` & `motion_python-0.1.28/motion/api/models.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.27/motion/cli.py` & `motion_python-0.1.28/motion/cli.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.27/motion/cursor.py` & `motion_python-0.1.28/motion/cursor.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 import pyarrow as pa
 import pyarrow.compute as pc
 
 from motion.utils import TriggerElement, TriggerFn, logger
 
 
 class Cursor:
+    """A connection to a Motion data store, only accessible within Motion triggers."""
+
     def __init__(
         self,
         *,
         name: str,
         relations: typing.Dict[str, pa.Table],
         log_table: pa.Table,
         table_columns: typing.Dict[str, list[str]],
@@ -52,15 +54,15 @@
     def waitForResults(self) -> None:
         """Waits for all fit events to finish."""
         for t in self.fit_events:
             t.wait()
         self.fit_events = []
 
     def getNewId(self, relation: str, key: str = "identifier") -> str:
-        """Get a new id for a relation.
+        """Gets a new id for a relation.
 
         Args:
             relation (str): The relation to get the new id for.
             key (str, optional): The key to get the new id for. Defaults to "id".
 
         Returns:
             str: The new id.
@@ -74,19 +76,19 @@
         return new_id
 
     def exists(
         self,
         relation: str,
         identifier: str,
     ) -> bool:
-        """Determine if a record exists in a relation.
+        """Determines if a record exists in a relation.
 
         Args:
             relation (str): The relation to check.
-            identifier (str): The primary key of the record.
+            identifier (str): The record's identifier.
 
         Returns:
             bool: True if the record exists, False otherwise.
         """
         if relation not in self.relations.keys():
             raise KeyError(f"Relation {relation} does not exist.")
 
@@ -210,15 +212,15 @@
     def logTriggerExecution(
         self,
         trigger_name: str,
         trigger_version: int,
         trigger_action: str,
         trigger_context: TriggerElement,
     ) -> None:
-        """Logs a trigger execution.
+        """Logs the execution of a trigger.
 
         Args:
             trigger_name (str): The name of the trigger.
             trigger_version (int): The version of the trigger.
             trigger_action (str): The action of the trigger.
             trigger_context (TriggerElement): The element that triggered the trigger.
         """
@@ -244,15 +246,15 @@
     def executeTrigger(
         self,
         *,
         trigger: TriggerFn,
         trigger_context: TriggerElement,
         triggers_to_run_on_duplicate: typing.Dict[TriggerFn, TriggerElement] = {},
     ) -> None:
-        """Execute a trigger.
+        """Executes a trigger, logging completion of infer and fit methods.
 
         Args:
             trigger (TriggerFn): The trigger to execute.
             trigger_context (TriggerElement): The element that triggered the trigger.
             triggers_to_run (typing.Dict[TriggerFn, TriggerElement], optional): The triggers to run whenever duplicate is called within a trigger. Defaults to {}.
         """
         try:
@@ -329,27 +331,23 @@
 
         Returns:
             str: The new identifier of the duplicated record.
         """
         new_id = self.getNewId(relation)
 
         with self.write_lock:
-            # self.cur.execute(
-            #     f"INSERT INTO {self.name}.{relation} SELECT '{new_id}' AS identifier, '{identifier}' AS derived_id, {', '.join(self.table_columns[relation])} FROM {self.name}.{relation} WHERE identifier = '{identifier}'"
-            # )
             table = self.relations[relation]
             condition = pc.equal(table["identifier"], identifier)
 
             row = pc.filter(table, condition).to_pandas()
             row.at[0, "identifier"] = new_id
             row.at[0, "derived_id"] = identifier
 
             new_row = pa.Table.from_pandas(row, schema=table.schema)
 
-            # filtered_table = pc.filter(table, pc.invert(condition))
             final_table = pa.concat_tables([table, new_row])
             self.relations[relation] = final_table
 
         # Run triggers on duplicate if it was from element that spawned
         # the trigger in the first place
         if (
             self.spawned_by is not None
```

### Comparing `motion_python-0.1.27/motion/entry.py` & `motion_python-0.1.28/motion/entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from motion.api import create_fastapi_app
 from motion.client import ClientConnection
 from motion.store import Store
 from motion.utils import PRODUCTION_SESSION_ID
 
 
 def create_token() -> str:
-    """Create a token for the API.
+    """Creates a token for the API.
 
     Returns:
         str: The token.
     """
     return str(os.urandom(20).hex())
 
 
@@ -75,15 +75,15 @@
             .replace("{1}", author)
         )
 
 
 def init(
     mconfig: dict, disable_cron_triggers: bool = False, session_id: str = ""
 ) -> Store:
-    """Initialize the motion store.
+    """Initializes a motion application by creating a data store and adding relations and triggers.
 
     Args:
         mconfig (dict): The motion configuration.
         disable_cron_triggers (bool, optional): Whether to disable cron triggers. Used during testing. Defaults to False.
         prod (bool, optional): Whether to run in production mode. Defaults to False.
 
     Returns:
@@ -135,21 +135,21 @@
 
 def serve(
     mconfig: dict,
     host: str = "0.0.0.0",
     port: int = 5000,
     motion_logging_level: str = "INFO",
 ) -> None:
-    """Serve a Motion application.
+    """Serves a Motion application. Uses the MOTION_API_TOKEN environment variable to authenticate API requests.
 
     Args:
-        mconfig (dict): The motion configuration.
+        mconfig (dict): The motion config, found in the mconfig.py file.
         host (str, optional): The host to serve on. Defaults to "0.0.0.0".
         port (int, optional): The port to serve on. Defaults to 5000.
-        motion_logging_level (str, optional): The logging level for motion.
+        motion_logging_level (str, optional): The logging level for motion. Can be one of "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL". Defaults to "INFO".
     """
     configureLogging(motion_logging_level)
     store = init(mconfig, session_id=PRODUCTION_SESSION_ID)
     serve_store(store, host, port)
 
 
 def serve_store(store: Store, host: str, port: int) -> None:
@@ -180,26 +180,25 @@
 def test(
     mconfig: dict,
     wait_for_triggers: typing.List[str] = [],
     disable_cron_triggers: bool = False,
     motion_logging_level: str = "WARNING",
     session_id: str = "",
 ) -> ClientConnection:
-    """Creates a test connection to a Motion application, defined by a mconfig. This will run the application
-    and then shut it down.
+    """Creates a test connection to a Motion application, defined by a mconfig. This will run the application and then shut it down when the connection goes out of scope. Uses the MOTION_API_TOKEN environment variable to authenticate.
 
     Args:
-        mconfig (dict): Config for the Motion application.
+        mconfig (dict): Config for the Motion application, found in the mconfig.py file.
         wait_for_triggers (typing.List[str], optional): List of cron-scheduled trigger names to wait for a first completion of. Typically used to wait for a first scrape of data.
-        disable_cron_triggers (bool, optional): Whether cron triggers should be disabled for this session (can speed up testing some non-cron triggers). Defaults to False.
-        motion_logging_level (str, optional): Logging level for motion. Use "INFO" if you want to see all trigger execution logs.
+        disable_cron_triggers (bool, optional): Whether cron triggers should be disabled for this session (can speed up testing some non-cron triggers). Defaults to False. Cannot be True if wait_for_triggers is not empty.
+        motion_logging_level (str, optional): Logging level for motion. Can be one of "DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL". Defaults to "WARNING". Use "INFO" if you want to see all trigger execution logs.
         session_id (str, optional): Session ID to use for this connection. Defaults to a random UUID if empty.
 
     Returns:
-        connection: A cannection to the Motion application.
+        connection (motion.ClientConnection): A cannection to the Motion application.
     """
     if wait_for_triggers and disable_cron_triggers:
         raise ValueError("Cannot wait for triggers if cron triggers are disabled.")
 
     configureLogging(motion_logging_level)
     store = init(
         mconfig,
@@ -234,15 +233,15 @@
         name (str): The name of the Motion application.
         host (str, optional): The host of the Motion application. Defaults to localhost.
         port (int, optional): The port of the Motion application. Defaults to 5000.
         wait_for_triggers (typing.List[str], optional): List of cron-scheduled trigger names to wait for a first completion of. Typically used to wait for a first scrape of data.
         motion_api_token (str, optional): API token set as the environment variable on the host serving the Motion application. If not provided as an argument, the token will be read from environment (possibly throwing an error if the environment doesn't have an API token defined).
 
     Returns:
-        connection: A connection to the Motion application.
+        connection (motion.ClientConnection): A connection to the Motion application.
     """
     #  Check logs
     MOTION_API_TOKEN = (
         motion_api_token if motion_api_token else os.environ.get("MOTION_API_TOKEN", "")
     )
 
     server = "http://" + host + ":" + str(port)
```

### Comparing `motion_python-0.1.27/motion/examples/cooking/dashboard.py` & `motion_python-0.1.28/motion/examples/cooking/dashboard.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.27/motion/examples/cooking/test.py` & `motion_python-0.1.28/motion/examples/cooking/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Test that for simple queries, the results make some sense
 
 
 def test_scrape() -> None:
     connection = motion.test(
         MCONFIG,
         wait_for_triggers=["ScrapeBonAppetit"],
-        motion_logging_level="WARNING",  # Can be "INFO" or "DEBUG" for more verbose logging
+        motion_logging_level="INFO",  # Can be "INFO" or "DEBUG" for more verbose logging
         session_id="EXAMPLE_SESSION_ID",  # Can comment this out to generate a new session ID
     )
     print(f"Session ID: {connection.session_id}")
 
     # Must specify kw for every arg in .set and .get
     ingredients = "pasta;tomatoes;garlic;cheese"
     new_id = connection.set(
```

### Comparing `motion_python-0.1.27/motion/examples/cooking/triggers/scrape.py` & `motion_python-0.1.28/motion/examples/cooking/triggers/scrape.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,20 +24,20 @@
 
     def setUp(self, cursor: motion.Cursor) -> Dict:
         return {}
 
     def scrape(
         self, cursor: motion.Cursor, trigger_context: motion.TriggerElement
     ) -> None:
-        # Set lower bound
+        # Set lower time bound to avoid scraping recipes we've already scraped
         lower_bound = cursor.sql(
             "SELECT MAX(create_at) AS lower_bound FROM Recipe WHERE src='Bon Appetit'"
         )["lower_bound"].values[0]
         if pd.isnull(lower_bound):
-            lower_bound = "2020-01-01"
+            lower_bound = "2019-01-01"
         else:
             lower_bound = str(lower_bound)
 
         url_list = asyncio.run(
             fetch_all_urls("https://www.bonappetit.com/sitemap.xml", lower_bound)
         )
```

### Comparing `motion_python-0.1.27/motion/examples/cooking/triggers/search.py` & `motion_python-0.1.28/motion/examples/cooking/triggers/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
                 key="ingredients",
                 infer=self.findNearestRecipes,
                 fit=None,
             ),
         ]
 
     def setUp(self, cursor: motion.Cursor) -> Dict:
-        # Set up the embedding store
+        # Set up the recipe index and cohere client
         co = cohere.Client(os.environ["COHERE_API_KEY"])
         recipe_index = faiss.IndexFlatIP(4096)
         recipe_index_to_id: Dict[int, str] = {}
 
         ingredients_df = cursor.sql("SELECT identifier, ingredients FROM Recipe")
 
         if len(ingredients_df) > 0:
@@ -82,15 +82,17 @@
 
     def addRecipeToIndex(
         self,
         cursor: motion.Cursor,
         trigger_context: motion.TriggerElement,
         infer_context: typing.Any,
     ) -> Dict:
-        # Keep a stream of the last 20 recipes
+        # Keep a stream of the last 20 recipes,
+        # adding them to the index every 20 iterations.
+        # This is to speed up the process of adding recipes
 
         recipe_stream = self.state["recipe_stream"]
         recipe_stream.append(
             IngredientsList(trigger_context.identifier, trigger_context.value)
         )
         new_state = {"recipe_stream": recipe_stream}
 
@@ -132,14 +134,15 @@
         ingredients = trigger_context.value
         response = self.state["cohere"].embed(texts=[ingredients])
         embedding = np.array(response.embeddings[0]).reshape(1, -1)
 
         scores, recipe_ids = self._searchIndex(embedding)
         for score, recipe_id in zip(scores, recipe_ids):
             duplicate_id = cursor.duplicate(
-                relation="Query", identifier=trigger_context.identifier
+                relation=trigger_context.relation,
+                identifier=trigger_context.identifier,
             )
             cursor.set(
-                relation="Query",
+                relation=trigger_context.relation,
                 identifier=duplicate_id,
                 key_values={"recipe_id": recipe_id, "recipe_score": score},
             )
```

### Comparing `motion_python-0.1.27/motion/schema.py` & `motion_python-0.1.28/motion/schema.py`

 * *Files 20% similar despite different names*

```diff
@@ -48,22 +48,43 @@
         return pa.from_numpy_dtype(t)
 
     # TODO: Add support for other types
     raise TypeError(f"Type {t} not supported.")
 
 
 class Schema(BaseModel, extra=Extra.allow):
+    """Schema for a Motion relation. Read more about relations in Motion [here](/concepts/relation).
+
+    Example:
+
+    ```python
+    class User(Schema):
+        name: str
+        dob: date
+        hometown: str
+    ```
+
+    All schemas also have the following fields, by default:
+    - `identifier` (str): A unique identifier for each record in the relation.
+    - `create_at` (datetime): The time at which the record was created.
+    - `derived_id` (str): The identifier of the record that was derived from, if any.
+    - `session_id` (str): The identifier of the session that created the record.
+
+    Raises:
+        TypeError: If a type is not supported. Supported types are: int, str, float, bool, date, datetime, bytes, list, dict, numpy types, and enums.
+    """
+
     identifier: str
     derived_id: str
     create_at: datetime
     session_id: str
 
     @classmethod
     def formatPaSchema(cls, relation: str) -> pa.Schema:
-        """Formats a pyarrow schema for the given relation.
+        """Formats a pyarrow schema for the given relation. This is used internally by Motion.
 
         Returns:
             pa.Schema: Schema for table based on annotations.
         """
 
         fields = [Field(key, val) for key, val in cls.__annotations__.items()]
         user_defined_fields = [
```

### Comparing `motion_python-0.1.27/motion/store.py` & `motion_python-0.1.28/motion/store.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.27/motion/task.py` & `motion_python-0.1.28/motion/task.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.27/motion/trigger.py` & `motion_python-0.1.28/motion/trigger.py`

 * *Files 26% similar despite different names*

```diff
@@ -27,14 +27,16 @@
         except KeyError:
             raise KeyError(
                 f"Key `{key}` not found in {self.dict_type} for trigger {self.trigger_name}."
             )
 
 
 class Trigger(ABC):
+    """A trigger is a class that defines the logic for a particular type of inference. Triggers are instantiated once per project and are responsible for maintaining their own state. Triggers are responsible for defining their setup, routes that they respond to, and the logic for infer and fit. See the [trigger life cycle](/concepts/trigger) for more information."""
+
     def __init__(
         self,
         cursor: Cursor,
         name: str,
         version: int,
         params: dict = {},
         routes_only: bool = False,
@@ -97,19 +99,34 @@
     def getRouteKeys(cls) -> list:
         obj: Trigger = cls(None, "", 0, routes_only=True)  # type: ignore
 
         return list(obj.route_map.keys())
 
     @abstractmethod
     def routes(self) -> list:
+        """Specifies mappings from trigger keys to lifecycle functions (i.e., infer, fit methods).
+        Returns:
+            list: List of routes that this trigger responds to. Each route is a motion.Route object.
+        """
         pass
 
     @abstractmethod
     def setUp(self, cursor: Cursor) -> dict:
-        raise TypeError(f"Please implement setUp() for trigger {self.name}.")
+        """Sets up the initial state of the trigger. Called only when the application is started.
+
+        Args:
+            cursor (Cursor): Cursor object to access the Motion data store.
+
+        Raises:
+            NotImplementedError: Error if this method is not implemented.
+
+        Returns:
+            dict: Initial state of the trigger.
+        """
+        raise NotImplementedError(f"Please implement setUp() for trigger {self.name}.")
 
     @property
     def params(self) -> dict:
         return self._params
 
     @property
     def state(self) -> dict:
```

### Comparing `motion_python-0.1.27/motion/utils.py` & `motion_python-0.1.28/motion/utils.py`

 * *Files identical despite different names*

### Comparing `motion_python-0.1.27/pyproject.toml` & `motion_python-0.1.28/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "motion-python"
-version = "0.1.27"
+version = "0.1.28"
 description = "A trigger-based framework for creating and executing ML pipelines."
 authors = ["Shreya Shankar <shreyashankar@berkeley.edu>"]
 readme = "README.md"
 packages = [{include = "motion"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `motion_python-0.1.27/PKG-INFO` & `motion_python-0.1.28/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: motion-python
-Version: 0.1.27
+Version: 0.1.28
 Summary: A trigger-based framework for creating and executing ML pipelines.
 Author: Shreya Shankar
 Author-email: shreyashankar@berkeley.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

