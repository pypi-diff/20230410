# Comparing `tmp/sqlalchemy_easy_softdelete-0.6.2.tar.gz` & `tmp/sqlalchemy_easy_softdelete-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_easy_softdelete-0.6.2.tar", max compression
+gzip compressed data, was "sqlalchemy_easy_softdelete-0.6.4.tar", max compression
```

## Comparing `sqlalchemy_easy_softdelete-0.6.2.tar` & `sqlalchemy_easy_softdelete-0.6.4.tar`

### file list

```diff
@@ -1,20 +1,19 @@
--rw-r--r--   0        0        0     1497 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/LICENSE
--rw-r--r--   0        0        0     2877 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/README.md
--rw-r--r--   0        0        0     2309 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/pyproject.toml
--rw-r--r--   0        0        0      140 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/sqlalchemy_easy_softdelete/__init__.py
--rw-r--r--   0        0        0       65 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/sqlalchemy_easy_softdelete/handler/__init__.py
--rw-r--r--   0        0        0     5787 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py
--rw-r--r--   0        0        0      850 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py
--rw-r--r--   0        0        0     1623 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/sqlalchemy_easy_softdelete/mixin.py
--rw-r--r--   0        0        0       56 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/tests/__init__.py
--rw-r--r--   0        0        0     1781 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/tests/conftest.py
--rw-r--r--   0        0        0     2489 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/tests/model.py
--rw-r--r--   0        0        0      360 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/tests/seed_data/__init__.py
--rw-r--r--   0        0        0     2013 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/tests/seed_data/parent_child_childchild.py
--rw-r--r--   0        0        0        0 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/tests/snapshots/__init__.py
--rw-r--r--   0        0        0     6288 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/tests/snapshots/snap_test_queries.py
--rw-r--r--   0        0        0     9931 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/tests/snapshots/snap_test_seed_data.py
--rw-r--r--   0        0        0     5899 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/tests/test_queries.py
--rw-r--r--   0        0        0      595 2023-01-10 21:15:17.919765 sqlalchemy_easy_softdelete-0.6.2/tests/test_seed_data.py
--rw-r--r--   0        0        0     4353 1970-01-01 00:00:00.000000 sqlalchemy_easy_softdelete-0.6.2/setup.py
--rw-r--r--   0        0        0     4508 1970-01-01 00:00:00.000000 sqlalchemy_easy_softdelete-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1497 2023-04-10 21:45:30.250003 sqlalchemy_easy_softdelete-0.6.4/LICENSE
+-rw-r--r--   0        0        0     2877 2023-04-10 21:45:30.250003 sqlalchemy_easy_softdelete-0.6.4/README.md
+-rw-r--r--   0        0        0     2309 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/pyproject.toml
+-rw-r--r--   0        0        0      140 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/__init__.py
+-rw-r--r--   0        0        0       65 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/handler/__init__.py
+-rw-r--r--   0        0        0     6089 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py
+-rw-r--r--   0        0        0      850 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py
+-rw-r--r--   0        0        0     1623 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/mixin.py
+-rw-r--r--   0        0        0       56 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/__init__.py
+-rw-r--r--   0        0        0     1971 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/conftest.py
+-rw-r--r--   0        0        0     2489 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/model.py
+-rw-r--r--   0        0        0      360 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/seed_data/__init__.py
+-rw-r--r--   0        0        0     2025 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/seed_data/parent_child_childchild.py
+-rw-r--r--   0        0        0        0 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/snapshots/__init__.py
+-rw-r--r--   0        0        0     6518 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/snapshots/snap_test_queries.py
+-rw-r--r--   0        0        0     9931 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/snapshots/snap_test_seed_data.py
+-rw-r--r--   0        0        0     6340 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/test_queries.py
+-rw-r--r--   0        0        0      595 2023-04-10 21:45:30.254003 sqlalchemy_easy_softdelete-0.6.4/tests/test_seed_data.py
+-rw-r--r--   0        0        0     4508 1970-01-01 00:00:00.000000 sqlalchemy_easy_softdelete-0.6.4/PKG-INFO
```

### Comparing `sqlalchemy_easy_softdelete-0.6.2/LICENSE` & `sqlalchemy_easy_softdelete-0.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.2/README.md` & `sqlalchemy_easy_softdelete-0.6.4/README.md`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.2/pyproject.toml` & `sqlalchemy_easy_softdelete-0.6.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "sqlalchemy-easy-softdelete"
-version = "0.6.2"
+version = "0.6.4"
 homepage = "https://github.com/flipbit03/sqlalchemy-easy-softdelete"
 description = "Easily add soft-deletion to your SQLAlchemy Models."
 authors = ["Cadu <cadu.coelho@gmail.com>"]
 readme = "README.md"
 license =  "BSD-3-Clause"
 classifiers=[
     'Development Status :: 5 - Production/Stable',
```

### Comparing `sqlalchemy_easy_softdelete-0.6.2/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py` & `sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/handler/rewriter/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Main query rewriter logic."""
 
 from typing import TypeVar, Union
 
 from sqlalchemy import Table
 from sqlalchemy.orm import FromStatement
 from sqlalchemy.orm.util import _ORMJoin
-from sqlalchemy.sql import Alias, CompoundSelect, Join, Select, Subquery, TableClause
+from sqlalchemy.sql import Alias, CompoundSelect, Executable, Join, Select, Subquery, TableClause
 from sqlalchemy.sql.elements import TextClause
 
-Statement = TypeVar('Statement', bound=Union[Select, FromStatement])
+Statement = TypeVar('Statement', bound=Union[Select, FromStatement, CompoundSelect, Executable])
 
 
 class SoftDeleteQueryRewriter:
     """Rewrites SQL statements based on configuration."""
 
     def __init__(self, deleted_field_name: str, disable_soft_delete_option_name: str):
         """
@@ -33,14 +33,19 @@
         self.disable_soft_delete_option_name = disable_soft_delete_option_name
 
     def rewrite_statement(self, stmt: Statement) -> Statement:
         """Rewrite a single SQL-like Statement."""
         if isinstance(stmt, Select):
             return self.rewrite_select(stmt)
 
+        # Handle CompoundSelect
+        if isinstance(stmt, CompoundSelect):
+            return self.rewrite_compound_select(stmt)
+
+        # Handle FromStatement which is also a Select/Executable
         if isinstance(stmt, FromStatement):
             # Explicitly protect against INSERT with RETURNING
             if not isinstance(stmt.element, Select):
                 return stmt
             stmt.element = self.rewrite_select(stmt.element)
             return stmt
 
@@ -76,14 +81,16 @@
         if isinstance(subquery.element, Select):
             subquery.element = self.rewrite_select(subquery.element)
             return subquery
 
         raise NotImplementedError(f"Unsupported object \"{(type(subquery.element))}\" in subquery.element")
 
     def rewrite_from_orm_join(self, stmt: Select, join_obj: Union[_ORMJoin, Join]) -> Select:
+        """Handle multiple, and potentially recursive joins."""
+
         # Recursive cases (multiple joins)
         if isinstance(join_obj.left, _ORMJoin) or isinstance(join_obj.left, Join):
             stmt = self.rewrite_from_orm_join(stmt, join_obj.left)
 
         if isinstance(join_obj.right, _ORMJoin) or isinstance(join_obj.right, Join):
             stmt = self.rewrite_from_orm_join(stmt, join_obj.right)
```

### Comparing `sqlalchemy_easy_softdelete-0.6.2/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py` & `sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/handler/sqlalchemy_easy_softdelete.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.2/sqlalchemy_easy_softdelete/mixin.py` & `sqlalchemy_easy_softdelete-0.6.4/sqlalchemy_easy_softdelete/mixin.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.2/tests/conftest.py` & `sqlalchemy_easy_softdelete-0.6.4/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,21 +8,26 @@
 from sqlalchemy_easy_softdelete.handler.rewriter import SoftDeleteQueryRewriter
 from tests.model import TestModelBase
 from tests.seed_data import generate_table_with_inheritance_obj
 from tests.seed_data.parent_child_childchild import generate_parent_child_object_hierarchy
 
 env_connection_string = os.environ.get("TEST_CONNECTION_STRING", None)
 
-test_db_url = env_connection_string or "sqlite://"
+
+@pytest.fixture
+def sqla2_warnings() -> Engine:
+    # Enable SQLAlchemy 2.0 Warnings mode to help with 2.0 support
+    os.environ["SQLALCHEMY_WARN_20"] = "1"
 
 
 @pytest.fixture
-def db_engine() -> Engine:
+def db_engine(sqla2_warnings) -> Engine:
+    test_db_url = env_connection_string or "sqlite://"
     print(f"connection_string={test_db_url}")
-    return create_engine(test_db_url)
+    return create_engine(test_db_url, future=True)
 
 
 @pytest.fixture
 def db_connection(db_engine) -> Connection:
     connection = db_engine.connect()
 
     # start a transaction
```

### Comparing `sqlalchemy_easy_softdelete-0.6.2/tests/model.py` & `sqlalchemy_easy_softdelete-0.6.4/tests/model.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.2/tests/seed_data/parent_child_childchild.py` & `sqlalchemy_easy_softdelete-0.6.4/tests/seed_data/parent_child_childchild.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,27 +28,27 @@
     deleted_children = random.randint(min_children, max_children)
 
     children = [False] * active_children + [True] * deleted_children
 
     # Create Children (SDChild)
     for child_no, child_deleted in enumerate(children):
         new_child_id = parent_id * 100 + child_no
-        new_child = SDChild(id=new_child_id, parent=new_parent)
+        new_child = SDChild(id=new_child_id, parent_id=new_parent.id)
         new_child.deleted_at = pseudorandom_date() if child_deleted else None
         s.add(new_child)
         s.flush()
 
         # Create Child's Children (SDChildChild)
         active_child_children = random.randint(min_children, max_children)
         deleted_child_children = random.randint(min_children, max_children)
 
         child_children = [False] * active_child_children + [True] * deleted_child_children
 
         for child_children_no, child_children_deleted in enumerate(child_children):
             sdchild_child_id = new_child_id * 100 + child_children_no
-            new_child_child = SDChildChild(id=sdchild_child_id, child=new_child)
+            new_child_child = SDChildChild(id=sdchild_child_id, child_id=new_child.id)
             child_child_deleted = pseudorandom_date() if child_children_deleted else None
             new_child_child.deleted_at = child_child_deleted
             s.add(new_child_child)
             s.flush()
 
     s.commit()
```

### Comparing `sqlalchemy_easy_softdelete-0.6.2/tests/snapshots/snap_test_queries.py` & `sqlalchemy_easy_softdelete-0.6.4/tests/snapshots/snap_test_queries.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,14 +61,20 @@
     GenericRepr('<SDChild id=100200 deleted=False (parent_id=1002)>'),
     GenericRepr('<SDChild id=100201 deleted=False (parent_id=1002)>'),
     GenericRepr('<SDChild id=100202 deleted=False (parent_id=1002)>'),
     GenericRepr('<SDChild id=100203 deleted=False (parent_id=1002)>'),
     GenericRepr('<SDChild id=100204 deleted=False (parent_id=1002)>')
 ]
 
+snapshots['test_query_union_sdchild_core 1'] = '''SELECT sdchild.id, sdchild.parent_id 
+FROM sdchild 
+WHERE sdchild.deleted_at IS NULL UNION SELECT sdchild.id, sdchild.parent_id 
+FROM sdchild 
+WHERE sdchild.deleted_at IS NULL'''
+
 snapshots['test_query_with_join 1'] = '''SELECT sdchild.id, sdchild.deleted_at, sdchild.parent_id 
 FROM sdchild JOIN sdparent ON sdparent.id = sdchild.parent_id 
 WHERE sdchild.deleted_at IS NULL AND sdparent.deleted_at IS NULL'''
 
 snapshots['test_query_with_join 2'] = [
     GenericRepr('<SDChild id=100000 deleted=False (parent_id=1000)>'),
     GenericRepr('<SDChild id=100001 deleted=False (parent_id=1000)>'),
```

### Comparing `sqlalchemy_easy_softdelete-0.6.2/tests/snapshots/snap_test_seed_data.py` & `sqlalchemy_easy_softdelete-0.6.4/tests/snapshots/snap_test_seed_data.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.2/tests/test_queries.py` & `sqlalchemy_easy_softdelete-0.6.4/tests/test_queries.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,69 +9,80 @@
 from tests.model import SDBaseRequest, SDChild, SDChildChild, SDDerivedRequest, SDParent, SDSimpleTable
 
 
 def test_query_single_table(snapshot, seeded_session, rewriter):
     """Query with one table"""
     test_query: Query = seeded_session.query(SDChild)
 
-    snapshot.assert_match(str(rewriter.rewrite_select(test_query.statement)))
+    snapshot.assert_match(str(rewriter.rewrite_statement(test_query.statement)))
     snapshot.assert_match(sorted(test_query.all(), key=lambda i: i.id))
 
 
 def test_query_with_join(snapshot, seeded_session, rewriter):
     """Query with a simple join"""
     test_query: Query = seeded_session.query(SDChild).join(SDParent)  # noqa -- wrong typing stub in SA
 
-    snapshot.assert_match(str(rewriter.rewrite_select(test_query.statement)))
+    snapshot.assert_match(str(rewriter.rewrite_statement(test_query.statement)))
 
     snapshot.assert_match(sorted(test_query.all(), key=lambda i: i.id))
 
 
 def test_query_union_sdchild(snapshot, seeded_session, rewriter):
     """Two queries joined via UNION"""
     test_query: Query = seeded_session.query(SDChild).union(seeded_session.query(SDChild))
 
-    snapshot.assert_match(str(rewriter.rewrite_select(test_query.statement)))
+    snapshot.assert_match(str(rewriter.rewrite_statement(test_query.statement)))
 
     snapshot.assert_match(sorted(test_query.all(), key=lambda i: i.id))
 
 
+def test_query_union_sdchild_core(snapshot, seeded_session, rewriter):
+    """Two queries joined via UNION, using SQLAlchemy Core"""
+    sdchild = SDChild.__table__
+
+    select_as_core = (select(sdchild.c.id, sdchild.c.parent_id).select_from(sdchild)).union(
+        select(sdchild.c.id, sdchild.c.parent_id).select_from(sdchild)
+    )
+
+    snapshot.assert_match(str(rewriter.rewrite_statement(select_as_core)))
+
+
 def test_query_with_union_but_union_softdelete_disabled(snapshot, seeded_session, rewriter):
     """Two queries joined via UNION but the second one has soft-delete disabled"""
 
     # Two SDChild .all() queries with results joined via UNION
     # the first one has soft delete applied
     # the second one has soft delete DISABLED
     # the second query is a superset of the first one, and results in
     # all objects in the DB being returned
     test_query: Query = seeded_session.query(SDChild).union(
         seeded_session.query(SDChild).execution_options(include_deleted=True)
     )
 
-    snapshot.assert_match(str(rewriter.rewrite_select(test_query.statement)))
+    snapshot.assert_match(str(rewriter.rewrite_statement(test_query.statement)))
 
     all_children: List[SDChild] = seeded_session.query(SDChild).execution_options(include_deleted=True).all()
 
     assert sorted(test_query.all(), key=lambda x: x.id) == sorted(all_children, key=lambda x: x.id)
 
     snapshot.assert_match(sorted(test_query.all(), key=lambda i: i.id))
 
 
 def test_ensure_aggregate_from_multiple_table_deletion_works_active_object_count(snapshot, seeded_session, rewriter):
     """Aggregate function from a query that contains a join"""
     test_query: Query = seeded_session.query(SDChild).join(SDParent).with_entities(func.count())  # noqa
 
-    snapshot.assert_match(str(rewriter.rewrite_select(test_query.statement)))
+    snapshot.assert_match(str(rewriter.rewrite_statement(test_query.statement)))
     snapshot.assert_match(test_query.count())
 
 
 def test_ensure_table_with_inheritance_works(snapshot, seeded_session, rewriter):
     test_query: Query = seeded_session.query(SDDerivedRequest)
 
-    snapshot.assert_match(str(rewriter.rewrite_select(test_query.statement)))
+    snapshot.assert_match(str(rewriter.rewrite_statement(test_query.statement)))
 
     test_query_results = test_query.all()
     assert len(test_query_results) == 2
     snapshot.assert_match(sorted(test_query_results, key=lambda i: i.id))
 
     all_active_and_deleted_derived_requests = (
         seeded_session.query(SDDerivedRequest).execution_options(include_deleted=True).all()
@@ -101,23 +112,23 @@
 
 
 def test_query_with_text_clause_as_table(snapshot, seeded_session, rewriter):
     """We cannot parse information from a literal text table name -- return unchanged"""
 
     # Table as a TextClause
     test_query_text_clause: Select = select(text('id')).select_from(text("sdderivedrequest"))
-    snapshot.assert_match(str(rewriter.rewrite_select(test_query_text_clause)))
+    snapshot.assert_match(str(rewriter.rewrite_statement(test_query_text_clause)))
 
 
 def test_query_with_table_clause_as_table(snapshot, seeded_session, rewriter):
     """We cannot parse information from a literal text table name -- return unchanged"""
 
     # Table as a TableClause
     test_query_table_clause: Select = select(text('id')).select_from(table("sdderivedrequest"))
-    snapshot.assert_match(str(rewriter.rewrite_select(test_query_table_clause)))
+    snapshot.assert_match(str(rewriter.rewrite_statement(test_query_table_clause)))
 
 
 def test_insert_with_returning(snapshot, seeded_session, rewriter, db_connection):
     """Insert with RETURNING is considered a *Select* by SQLAlchemy, since it returns data :dizzy:
     that means we need to actively protect against this case"""
 
     # RETURNING is not supported in SQLite
@@ -140,8 +151,8 @@
         .join(SDChild)
         .join(SDChildChild)
         .filter(
             SDParent.id > 0,
         )
     )
 
-    snapshot.assert_match(str(rewriter.rewrite_select(query.statement)))
+    snapshot.assert_match(str(rewriter.rewrite_statement(query.statement)))
```

### Comparing `sqlalchemy_easy_softdelete-0.6.2/tests/test_seed_data.py` & `sqlalchemy_easy_softdelete-0.6.4/tests/test_seed_data.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_easy_softdelete-0.6.2/PKG-INFO` & `sqlalchemy_easy_softdelete-0.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-easy-softdelete
-Version: 0.6.2
+Version: 0.6.4
 Summary: Easily add soft-deletion to your SQLAlchemy Models.
 Home-page: https://github.com/flipbit03/sqlalchemy-easy-softdelete
 License: BSD-3-Clause
 Author: Cadu
 Author-email: cadu.coelho@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

