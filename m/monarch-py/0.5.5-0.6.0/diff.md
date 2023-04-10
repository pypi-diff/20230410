# Comparing `tmp/monarch_py-0.5.5.tar.gz` & `tmp/monarch_py-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monarch_py-0.5.5.tar", max compression
+gzip compressed data, was "monarch_py-0.6.0.tar", max compression
```

## Comparing `monarch_py-0.5.5.tar` & `monarch_py-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      955 2023-04-04 23:25:44.608829 monarch_py-0.5.5/pyproject.toml
--rw-r--r--   0        0        0       77 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/__init__.py
--rw-r--r--   0        0        0     5589 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/cli.py
--rw-r--r--   0        0        0        0 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/datamodels/__init__.py
--rw-r--r--   0        0        0     6087 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/datamodels/model.py
--rw-r--r--   0        0        0     4290 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/datamodels/model.yaml
--rw-r--r--   0        0        0     3300 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/datamodels/solr.py
--rw-r--r--   0        0        0        0 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/implementations/solr/__init__.py
--rw-r--r--   0        0        0    15020 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/implementations/solr/solr_implementation.py
--rw-r--r--   0        0        0        0 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/implementations/sql/__init__.py
--rw-r--r--   0        0        0     7664 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/implementations/sql/sql_implementation.py
--rw-r--r--   0        0        0        0 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/interfaces/__init__.py
--rw-r--r--   0        0        0     2171 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/interfaces/association_interface.py
--rw-r--r--   0        0        0      985 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/interfaces/entity_interface.py
--rw-r--r--   0        0        0      890 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/interfaces/query_interface.py
--rw-r--r--   0        0        0     3254 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/interfaces/search_interface.py
--rw-r--r--   0        0        0        0 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/service/__init__.py
--rw-r--r--   0        0        0     2051 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/service/solr_service.py
--rw-r--r--   0        0        0     7952 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/solr_cli.py
--rw-r--r--   0        0        0     3661 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/sql_cli.py
--rw-r--r--   0        0        0        0 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/utils/__init__.py
--rw-r--r--   0        0        0     3657 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/utils/solr_cli_utils.py
--rw-r--r--   0        0        0     4262 2023-04-04 23:25:44.608829 monarch_py-0.5.5/src/monarch_py/utils/utils.py
--rw-r--r--   0        0        0      894 1970-01-01 00:00:00.000000 monarch_py-0.5.5/PKG-INFO
+-rw-r--r--   0        0        0      955 2023-04-10 15:50:37.713391 monarch_py-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       77 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/__init__.py
+-rw-r--r--   0        0        0     5764 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/cli.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/datamodels/__init__.py
+-rw-r--r--   0        0        0     6595 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/datamodels/model.py
+-rw-r--r--   0        0        0     6272 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/datamodels/model.yaml
+-rw-r--r--   0        0        0     3300 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/datamodels/solr.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/implementations/solr/__init__.py
+-rw-r--r--   0        0        0    16877 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/implementations/solr/solr_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/implementations/sql/__init__.py
+-rw-r--r--   0        0        0     8913 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/implementations/sql/sql_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/interfaces/__init__.py
+-rw-r--r--   0        0        0     2345 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/interfaces/association_interface.py
+-rw-r--r--   0        0        0      985 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/interfaces/entity_interface.py
+-rw-r--r--   0        0        0      890 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/interfaces/query_interface.py
+-rw-r--r--   0        0        0     3732 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/interfaces/search_interface.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/service/__init__.py
+-rw-r--r--   0        0        0     2051 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/service/solr_service.py
+-rw-r--r--   0        0        0     8096 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/solr_cli.py
+-rw-r--r--   0        0        0     3794 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/sql_cli.py
+-rw-r--r--   0        0        0        0 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/utils/__init__.py
+-rw-r--r--   0        0        0     3657 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/utils/solr_cli_utils.py
+-rw-r--r--   0        0        0     4262 2023-04-10 15:50:37.713391 monarch_py-0.6.0/src/monarch_py/utils/utils.py
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 monarch_py-0.6.0/PKG-INFO
```

### Comparing `monarch_py-0.5.5/pyproject.toml` & `monarch_py-0.6.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 [tool.poetry]
 name = "monarch-py"
-version = "0.5.5"
+version = "0.6.0"
 description = "Monarch Initiative data access library"
 authors = [
     "Kevin Schaper <kevin@tislab.org>",
     "Glass Elsarboukh <glass@tislab.org>",
     "The Monarch Initiative <info@monarchinitiative.org>"
 ]
 packages = [
     { include = "monarch_py", from = "src"}
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "^2.28.1"
 pydantic = "^1.9.1"
-linkml = "^1.3.14"
 typer = "^0.7.0"
 typer-cli = "^0.0.13"
-mkdocs = "^1.4.2"
-mkdocs-material = "^8.5.10"
-mkdocstrings = {extras = ["python"], version = "^0.19.0"}
 rich = "*"
 docker = "^6.0.1"
 pystow = ">=0.5.0"
 loguru = "*"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.1.3"
 black = "^22.10.0"
 isort = "^5.10.1"
 flake8 = "^5.0.4"
 autoflake = "^1.7.7"
+mkdocs = "^1.4.2"
+mkdocs-material = "^8.5.10"
+mkdocstrings = {extras = ["python"], version = "^0.19.0"}
+linkml = "^1.3.14"
 
 [tool.poetry.scripts]
 monarch = "monarch_py.cli:app"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `monarch_py-0.5.5/src/monarch_py/cli.py` & `monarch_py-0.6.0/src/monarch_py/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,14 +67,15 @@
 def associations(
     category: str = typer.Option(None, "--category", "-c"),
     subject: str = typer.Option(None, "--subject", "-s"),
     predicate: str = typer.Option(None, "--predicate", "-p"),
     object: str = typer.Option(None, "--object", "-o"),
     entity: str = typer.Option(None, "--entity", "-e"),
     between: str = typer.Option(None, "--between"),
+    association_label: str = typer.Option(None, "--label"),
     limit: int = typer.Option(20, "--limit", "-l"),
     offset: int = typer.Option(0, "--offset"),
     update: bool = typer.Option(
         False, "--update", "-u", help="Whether to re-download the Monarch KG"
     ),
     fmt: str = typer.Option(
         "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
@@ -88,14 +89,16 @@
 
     Args:
         category: The category of the association
         predicate: The predicate of the association
         subject: The subject of the association
         object: The object of the association
         entity: The subject or object of the association
+        between: The subject and object of the association
+        association_label: The label of the association
         limit: The number of associations to return
         offset: The offset of the first association to be retrieved
         fmt: The format of the output (TSV, YAML, JSON)
         output: The path to the output file (stdout if not specified)
     """
     solr_cli.associations(**locals())
```

### Comparing `monarch_py-0.5.5/src/monarch_py/datamodels/model.py` & `monarch_py-0.6.0/src/monarch_py/datamodels/model.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from enum import Enum
 from typing import Dict, List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
 metamodel_version = "None"
 version = "None"
@@ -20,14 +21,28 @@
     underscore_attrs_are_private=True,
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
+class AssociationLabel(str, Enum):
+
+    disease_phenotype = "disease_phenotype"
+    gene_phenotype = "gene_phenotype"
+    gene_interaction = "gene_interaction"
+    gene_pathway = "gene_pathway"
+    gene_expression = "gene_expression"
+    gene_orthology = "gene_orthology"
+    chemical_pathway = "chemical_pathway"
+    gene_function = "gene_function"
+    gene_associated_with_disease = "gene_associated_with_disease"
+    gene_affects_risk_for_disease = "gene_affects_risk_for_disease"
+
+
 class Association(ConfiguredBaseModel):
 
     aggregator_knowledge_source: Optional[List[str]] = Field(default_factory=list)
     id: Optional[str] = Field(None)
     subject: Optional[str] = Field(None)
     original_subject: Optional[str] = Field(None)
     subject_namespace: Optional[str] = Field(None)
```

### Comparing `monarch_py-0.5.5/src/monarch_py/datamodels/solr.py` & `monarch_py-0.6.0/src/monarch_py/datamodels/solr.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.5.5/src/monarch_py/implementations/solr/solr_implementation.py` & `monarch_py-0.6.0/src/monarch_py/implementations/solr/solr_implementation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import os
 from dataclasses import dataclass
+from enum import Enum
 from typing import Dict, List, Tuple
 
 from loguru import logger
 from pydantic import ValidationError
 
 from monarch_py.datamodels.model import (
     Association,
     AssociationCount,
+    AssociationLabel,
     AssociationResults,
     Entity,
     FacetField,
     FacetValue,
     HistoPheno,
     SearchResult,
     SearchResults,
@@ -20,14 +22,29 @@
 from monarch_py.interfaces.association_interface import AssociationInterface
 from monarch_py.interfaces.entity_interface import EntityInterface
 from monarch_py.interfaces.search_interface import SearchInterface
 from monarch_py.service.solr_service import SolrService
 from monarch_py.utils.utils import escape
 
 
+class AssociationLabelQuery(Enum):
+    disease_phenotype = 'category:"biolink:DiseaseToPhenotypicFeatureAssociation"'
+    gene_phenotype = 'category:"biolink:GeneToPhenotypicFeatureAssociation"'
+    gene_interaction = 'category:"biolink:PairwiseGeneToGeneInteraction"'
+    gene_pathway = 'category:"biolink:GeneToPathwayAssociation"'
+    gene_expression = 'category:"biolink:GeneToExpressionSiteAssociation"'
+    gene_orthology = 'category:"biolink:GeneToGeneHomologyAssociation"'
+    chemical_pathway = 'category:"biolink:ChemicalToPathwayAssociation"'
+    gene_function = (
+        'category:"biolink:MacromolecularMachineToMolecularActivityAssociation"'
+    )
+    gene_associated_with_disease = 'category:"biolink:GeneToDiseaseAssociation" AND predicate:"biolink:gene_associated_with_condition"'
+    gene_affects_risk_for_disease = 'category:"biolink:GeneToDiseaseAssociation" AND predicate:"biolink:affects_risk_for"'
+
+
 @dataclass
 class SolrImplementation(EntityInterface, AssociationInterface, SearchInterface):
     """Implementation of Monarch Interfaces for Solr endpoint"""
 
     base_url: str = os.getenv("MONARCH_SOLR_URL", "http://localhost:8983/solr")
 
     ###############################
@@ -62,14 +79,15 @@
         predicate: str = None,
         subject: str = None,
         subject_closure: str = None,
         object: str = None,
         object_closure: str = None,
         entity: str = None,
         between: str = None,
+        association_label: AssociationLabel = None,
         offset: int = 0,
         limit: int = 20,
     ) -> AssociationResults:
         """Retrieve paginated association records, with filter options
 
         Args:
             category (str, optional): Filter to only associations matching the specified category. Defaults to None.
@@ -94,14 +112,15 @@
             predicate=predicate,
             subject=subject,
             subject_closure=subject_closure,
             object=object,
             object_closure=object_closure,
             entity=entity,
             between=between,
+            association_label=association_label,
             offset=offset,
             limit=limit,
         )
 
         query_result = solr.query(query)
         total = query_result.response.num_found
 
@@ -126,14 +145,15 @@
         predicate: str = None,
         subject: str = None,
         subject_closure: str = None,
         object: str = None,
         object_closure: str = None,
         entity: str = None,
         between: str = None,
+        association_label: AssociationLabel = None,
         offset: int = 0,
         limit: int = 20,
     ) -> SolrQuery:
         """
         Populate a SolrQuery object with association filters
         Args:
             category (str, optional): Filter to only associations matching the specified category. Defaults to None.
@@ -172,14 +192,16 @@
             query.add_filter_query(
                 f'(subject:"{e1}" AND object:"{e2}") OR (subject:"{e2}" AND object:"{e1}")'
             )
         if entity:
             query.add_filter_query(
                 f'subject:"{escape(entity)}" OR object:"{escape(entity)}"'
             )
+        if association_label:
+            query.add_filter_query(AssociationLabelQuery[association_label].value)
 
         return query
 
     ###############################
     # Implements: SearchInterface #
     ###############################
 
@@ -371,14 +393,29 @@
         hp = HistoPheno(
             id=subject_closure,
             items=association_counts,
         )
 
         return hp
 
+    def get_association_counts(self, entity: str) -> List[FacetValue]:
+
+        query = self._populate_association_query(entity=entity)
+        query.facet_queries = [alq.value for alq in AssociationLabelQuery]
+
+        solr = SolrService(base_url=self.base_url, core=core.ASSOCIATION)
+        query_result = solr.query(query)
+        facet_values: List[FacetValue] = []
+        for k, v in query_result.facet_counts.facet_queries.items():
+            if v > 0:
+                facet_values.append(
+                    FacetValue(label=AssociationLabelQuery(k).name, count=v)
+                )
+        return facet_values
+
     def _convert_facet_fields(self, solr_facet_fields: Dict) -> Dict[str, FacetField]:
         """
         Converts a list of raw solr facet fields from the solr response to a list of
         FacetField instances
 
         Args:
             facet_fields (Dict): A list of facet fields from the solr response
```

### Comparing `monarch_py-0.5.5/src/monarch_py/implementations/sql/sql_implementation.py` & `monarch_py-0.6.0/src/monarch_py/implementations/sql/sql_implementation.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 from dataclasses import dataclass
+from enum import Enum
 
 import pystow
 from loguru import logger
 from pydantic import ValidationError
 
 from monarch_py.datamodels.model import Association, AssociationResults, Entity
 from monarch_py.interfaces.association_interface import AssociationInterface
 from monarch_py.interfaces.entity_interface import EntityInterface
 from monarch_py.utils.utils import SQL_DATA_URL, dict_factory
 
 monarchstow = pystow.module("monarch")
 
 
+class AssociationLabelQuery(Enum):
+    disease_phenotype = 'category = "biolink:DiseaseToPhenotypicFeatureAssociation"'
+    gene_phenotype = 'category = "biolink:GeneToPhenotypicFeatureAssociation"'
+    gene_interaction = 'category = "biolink:PairwiseGeneToGeneInteraction"'
+    gene_pathway = 'category = "biolink:GeneToPathwayAssociation"'
+    gene_expression = 'category = "biolink:GeneToExpressionSiteAssociation"'
+    gene_orthology = 'category = "biolink:GeneToGeneHomologyAssociation"'
+    chemical_pathway = 'category = "biolink:ChemicalToPathwayAssociation"'
+    gene_function = (
+        'category = "biolink:MacromolecularMachineToMolecularActivityAssociation"'
+    )
+    gene_associated_with_disease = 'category = "biolink:GeneToDiseaseAssociation" AND predicate = "biolink:gene_associated_with_condition"'
+    gene_affects_risk_for_disease = 'category = "biolink:GeneToDiseaseAssociation" AND predicate = "biolink:affects_risk_for"'
+
+
 @dataclass
 class SQLImplementation(EntityInterface, AssociationInterface):
     """Implementation of Monarch Interfaces for SQL endpoint"""
 
     ###############################
     # Implements: EntityInterface #
     ###############################
@@ -78,14 +94,15 @@
         predicate: str = None,
         subject: str = None,
         subject_closure: str = None,
         object: str = None,
         object_closure: str = None,
         entity: str = None,
         between: str = None,
+        association_label: str = None,
         offset: int = 0,
         limit: int = 20,
         update: bool = False,
     ) -> AssociationResults:
         """Retrieve paginated association records, with filter options
 
         Args:
@@ -93,14 +110,15 @@
             predicate (str, optional): Filter to only associations matching the specified predicate. Defaults to None.
             subject (str, optional): Filter to only associations matching the specified subject. Defaults to None.
             subject_closure (str, optional): Filter to only associations with the specified term ID as an ancestor of the subject. Defaults to None.
             object (str, optional): Filter to only associations matching the specified object. Defaults to None.
             object_closure (str, optional): Filter to only associations the specified term ID as an ancestor of the object. Defaults to None.
             entity (str, optional): Filter to only associations where the specified entity is the subject or the object. Defaults to None.
             between (Tuple[str, str], optional): Filter to bi-directional associations between two entities.
+            association_label (str, optional): Filter to only associations matching the specified association label. Defaults to None.
             offset (int, optional): Result offset, for pagination. Defaults to 0.
             limit (int, optional): Limit results to specified number. Defaults to 20.
 
         Returns:
             AssociationResults: Dataclass representing results of an association search.
         """
 
@@ -123,14 +141,16 @@
             # todo: handle error reporting / parsing, think about another way to pass this?
             b = between.split(",")
             e1 = b[0]
             e2 = b[1]
             clauses.append(
                 f"subject = '{e1}' AND object = '{e2}' OR subject = '{e2}' AND object = '{e1}'"
             )
+        if association_label:
+            clauses.append(AssociationLabelQuery[association_label].value)
 
         query = f"SELECT * FROM denormalized_edges "
         if clauses:
             query += "WHERE " + " AND ".join(clauses)
         if limit:
             query += f" LIMIT {limit} OFFSET {offset}"
```

### Comparing `monarch_py-0.5.5/src/monarch_py/interfaces/association_interface.py` & `monarch_py-0.6.0/src/monarch_py/interfaces/association_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,28 +14,30 @@
         predicate: str = None,
         subject: str = None,
         subject_closure: str = None,
         object: str = None,
         object_closure: str = None,
         entity: str = None,
         between: Tuple[str, str] = None,
+        association_label: str = None,
         offset: int = 0,
         limit: int = 20,
     ) -> AssociationResults:
         """Retrieve paginated association records, with filter options
 
         Args:
             category (str, optional): Filter to only associations matching the specified category. Defaults to None.
             predicate (str, optional): Filter to only associations matching the specified predicate. Defaults to None.
             subject (str, optional): Filter to only associations matching the specified subject. Defaults to None.
             subject_closure (str, optional): Filter to only associations with the specified term ID as an ancestor of the subject. Defaults to None
             object (str, optional): Filter to only associations matching the specified object. Defaults to None.
             object_closure (str, optional): Filter to only associations with the specified term ID as an ancestor of the object. Defaults to None
             entity (str, optional): Filter to only associations where the specified entity is the subject or the object. Defaults to None.
             between (Tuple[str, str], optional): Filter to bi-directional associations between two entities.
+            association_label (str, optional): Filter to only associations matching the specified association label. Defaults to None.
             offset (int, optional): Result offset, for pagination. Defaults to 0.
             limit (int, optional): Limit results to specified number. Defaults to 20.
 
         Raises:
             NotImplementedError: Use a specific implementation (see the documentation for a list of implementations)
 
         Returns:
```

### Comparing `monarch_py-0.5.5/src/monarch_py/interfaces/entity_interface.py` & `monarch_py-0.6.0/src/monarch_py/interfaces/entity_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.5.5/src/monarch_py/interfaces/query_interface.py` & `monarch_py-0.6.0/src/monarch_py/interfaces/query_interface.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.5.5/src/monarch_py/interfaces/search_interface.py` & `monarch_py-0.6.0/src/monarch_py/interfaces/search_interface.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from abc import ABC, abstractmethod
 from typing import List, Tuple
 
-from monarch_py.datamodels.model import SearchResults
+from monarch_py.datamodels.model import AssociationLabel, FacetValue, SearchResults
 
 
 class SearchInterface(ABC):
     """Abstract interface for searching the Monarch KG in a Lucene way"""
 
     @abstractmethod
     def search(
@@ -58,14 +58,15 @@
         predicate: str = None,
         subject: str = None,
         subject_closure: str = None,
         object: str = None,
         object_closure: str = None,
         entity: str = None,
         between: Tuple[str, str] = None,
+        association_label: AssociationLabel = None,
     ) -> SearchResults:
         """
         Get facet counts and facet query counts for associations
         Args:
             facet_fields (List[str]): Facet fields to return counts for
             facet_queries (List[str]): Facet queries to return counts for
             category (str): Filter to only associations matching the specified category
@@ -77,7 +78,17 @@
             entity (str): Filter to only associations where the specified entity is the subject or the object
             between (Tuple[str, str]): Filter to bi-directional associations between two entities
         Returns:
             SearchResults: Dataclass representing results of a search, with zero rows returned but total count
             and faceting information populated
         """
         raise NotImplementedError
+
+    def get_association_counts(self, entity: str) -> List[FacetValue]:
+        """
+        Get counts of associations for a given entity
+        Args:
+            entity (str): Entity to get association counts for
+        Returns:
+            List[FacetValue]: List of FacetValue objects representing the counts of associations for the given entity
+        """
+        raise NotImplementedError
```

### Comparing `monarch_py-0.5.5/src/monarch_py/service/solr_service.py` & `monarch_py-0.6.0/src/monarch_py/service/solr_service.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.5.5/src/monarch_py/solr_cli.py` & `monarch_py-0.6.0/src/monarch_py/solr_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 def associations(
     category: str = typer.Option(None, "--category"),
     subject: str = typer.Option(None, "--subject"),
     predicate: str = typer.Option(None, "--predicate"),
     object: str = typer.Option(None, "--object"),
     entity: str = typer.Option(None, "--entity"),
     between: str = typer.Option(None, "--between"),
+    association_label: str = typer.Option(None, "--label"),
     limit: int = typer.Option(20, "--limit"),
     offset: int = typer.Option(0, "--offset"),
     update: bool = typer.Option(
         False, "--update", "-u", help="Whether to re-download the Monarch KG"
     ),
     fmt: str = typer.Option(
         "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
@@ -108,14 +109,15 @@
     Args:
         category (str, optional): The category of the association.
         subject (str, optional): The subject of the association.
         predicate (str, optional): The predicate of the association.
         object (str, optional): The object of the association.
         entity (str, optional): The subject or object of the association.
         between (str, optional): Two comma-separated entities to get bi-directional associations.
+        association_label (str, optional): The association label of the association
         limit (int, optional): The number of associations to return. Default 20
         offset (int, optional): The offset of the first association to be retrieved. Default 0
         update (bool, optional): Whether to re-download the Monarch KG. Default False
         fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
         output (str): The path to the output file. Default stdout
     """
     args = locals()
```

### Comparing `monarch_py-0.5.5/src/monarch_py/sql_cli.py` & `monarch_py-0.6.0/src/monarch_py/sql_cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 def associations(
     category: str = typer.Option(None, "--category"),
     subject: str = typer.Option(None, "--subject"),
     predicate: str = typer.Option(None, "--predicate"),
     object: str = typer.Option(None, "--object"),
     entity: str = typer.Option(None, "--entity"),
     between: str = typer.Option(None, "--between"),
+    association_label: str = typer.Option(None, "--label"),
     limit: int = typer.Option(20, "--limit"),
     offset: int = typer.Option(0, "--offset"),
     update: bool = typer.Option(False, "--update"),
     fmt: str = typer.Option(
         "json", "--format", "-f", help="The format of the output (TSV, YAML, JSON)"
     ),
     output: str = typer.Option(
@@ -74,14 +75,15 @@
     Args:
         category (str, optional): The category of the association.
         subject (str, optional): The subject of the association.
         predicate (str, optional): The predicate of the association.
         object (str, optional): The object of the association.
         entity (str, optional): The subject or object of the association.
         between (str, optional): Two comma-separated entities to get bi-directional associations.
+        association_label (str, optional): The label of the association.
         limit (int, optional): The number of associations to return. Default 20
         offset (int, optional): The offset of the first association to be retrieved. Default 0
         update (bool, optional): Whether to re-download the Monarch KG. Default False
         fmt (str): The format of the output (TSV, YAML, JSON). Default JSON
         output (str): The path to the output file. Default stdout
     """
     args = locals()
```

### Comparing `monarch_py-0.5.5/src/monarch_py/utils/solr_cli_utils.py` & `monarch_py-0.6.0/src/monarch_py/utils/solr_cli_utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.5.5/src/monarch_py/utils/utils.py` & `monarch_py-0.6.0/src/monarch_py/utils/utils.py`

 * *Files identical despite different names*

### Comparing `monarch_py-0.5.5/PKG-INFO` & `monarch_py-0.6.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,24 +1,20 @@
 Metadata-Version: 2.1
 Name: monarch-py
-Version: 0.5.5
+Version: 0.6.0
 Summary: Monarch Initiative data access library
 Author: Kevin Schaper
 Author-email: kevin@tislab.org
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: docker (>=6.0.1,<7.0.0)
-Requires-Dist: linkml (>=1.3.14,<2.0.0)
 Requires-Dist: loguru
-Requires-Dist: mkdocs (>=1.4.2,<2.0.0)
-Requires-Dist: mkdocs-material (>=8.5.10,<9.0.0)
-Requires-Dist: mkdocstrings[python] (>=0.19.0,<0.20.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Requires-Dist: pystow (>=0.5.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: rich
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Requires-Dist: typer-cli (>=0.0.13,<0.0.14)
```

