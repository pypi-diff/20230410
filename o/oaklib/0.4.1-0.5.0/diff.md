# Comparing `tmp/oaklib-0.4.1.tar.gz` & `tmp/oaklib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaklib-0.4.1.tar", max compression
+gzip compressed data, was "oaklib-0.5.0.tar", max compression
```

## Comparing `oaklib-0.4.1.tar` & `oaklib-0.5.0.tar`

### file list

```diff
@@ -1,246 +1,255 @@
--rw-r--r--   0        0        0    11357 2023-04-06 15:15:58.436868 oaklib-0.4.1/LICENSE
--rw-r--r--   0        0        0     7241 2023-04-06 15:15:58.436868 oaklib-0.4.1/README.md
--rw-r--r--   0        0        0     1728 2023-04-06 15:16:44.705722 oaklib-0.4.1/pyproject.toml
--rw-r--r--   0        0        0      271 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/__init__.py
--rw-r--r--   0        0        0   185955 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/cli.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/conf/__init__.py
--rw-r--r--   0        0        0     1903 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
--rw-r--r--   0        0        0     4537 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/conf/obograph-style.json
--rw-r--r--   0        0        0      256 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/conf/omo-to-skos.sssom.tsv
--rw-r--r--   0        0        0      131 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/conf/value-set-expander.conf.yaml
--rw-r--r--   0        0        0      128 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/constants.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/converters/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/converters/data_model_converter.py
--rw-r--r--   0        0        0     2561 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/converters/logical_definition_flattener.py
--rw-r--r--   0        0        0     2371 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/converters/obo_graph_to_cx_converter.py
--rw-r--r--   0        0        0    12163 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/converters/obo_graph_to_fhir_converter.py
--rw-r--r--   0        0        0     5713 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/converters/obo_graph_to_obo_format_converter.py
--rw-r--r--   0        0        0     5155 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
--rw-r--r--   0        0        0       60 2023-04-06 15:15:58.552870 oaklib-0.4.1/src/oaklib/datamodels/__init__.py
--rw-r--r--   0        0        0     4034 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/association.owl.ttl
--rw-r--r--   0        0        0    10999 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/association.py
--rw-r--r--   0        0        0     2738 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/association.yaml
--rw-r--r--   0        0        0     6165 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/class_enrichment.owl.ttl
--rw-r--r--   0        0        0    10853 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/class_enrichment.py
--rw-r--r--   0        0        0     2648 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/class_enrichment.yaml
--rw-r--r--   0        0        0    19083 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
--rw-r--r--   0        0        0    24246 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/cross_ontology_diff.py
--rw-r--r--   0        0        0    10687 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/cross_ontology_diff.yaml
--rw-r--r--   0        0        0    15826 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/fhir.owl.ttl
--rw-r--r--   0        0        0    35744 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/fhir.py
--rw-r--r--   0        0        0     5064 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/fhir.yaml
--rw-r--r--   0        0        0     8984 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/lexical_index.owl.ttl
--rw-r--r--   0        0        0    17256 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/lexical_index.py
--rw-r--r--   0        0        0     6429 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/lexical_index.schema.json
--rw-r--r--   0        0        0     4016 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/lexical_index.yaml
--rw-r--r--   0        0        0    26434 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/mapping_cluster_datamodel.py
--rw-r--r--   0        0        0     7317 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
--rw-r--r--   0        0        0    17785 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
--rw-r--r--   0        0        0    29752 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/mapping_rules_datamodel.py
--rw-r--r--   0        0        0    11456 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
--rw-r--r--   0        0        0     3220 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/mapping_rules_datamodel.yaml
--rw-r--r--   0        0        0    25354 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/obograph.owl.ttl
--rw-r--r--   0        0        0    45533 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/obograph.py
--rw-r--r--   0        0        0    22375 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/obograph.schema.json
--rw-r--r--   0        0        0    17625 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/obograph.yaml
--rw-r--r--   0        0        0    59793 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/ontology_metadata.owl.ttl
--rw-r--r--   0        0        0   116551 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/ontology_metadata.py
--rw-r--r--   0        0        0    95288 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/ontology_metadata.schema.json
--rw-r--r--   0        0        0    30318 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/ontology_metadata.yaml
--rw-r--r--   0        0        0    14759 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/oxo.owl.ttl
--rw-r--r--   0        0        0    21914 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/oxo.py
--rw-r--r--   0        0        0     4392 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/oxo.yaml
--rw-r--r--   0        0        0     3240 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/search.py
--rw-r--r--   0        0        0    16948 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/search_datamodel.owl.ttl
--rw-r--r--   0        0        0    25145 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/search_datamodel.py
--rw-r--r--   0        0        0     6683 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/search_datamodel.yaml
--rw-r--r--   0        0        0    12767 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/similarity.owl.ttl
--rw-r--r--   0        0        0    22125 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/similarity.py
--rw-r--r--   0        0        0     5512 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/similarity.yaml
--rw-r--r--   0        0        0    31217 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
--rw-r--r--   0        0        0    50746 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/summary_statistics_datamodel.py
--rw-r--r--   0        0        0    21176 2023-04-06 15:15:58.556870 oaklib-0.4.1/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
--rw-r--r--   0        0        0    16249 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/summary_statistics_datamodel.yaml
--rw-r--r--   0        0        0     9909 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/taxon_constraints.owl.ttl
--rw-r--r--   0        0        0    18433 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/taxon_constraints.py
--rw-r--r--   0        0        0     5882 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/taxon_constraints.yaml
--rw-r--r--   0        0        0    11599 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/text_annotator.owl.ttl
--rw-r--r--   0        0        0    20421 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/text_annotator.py
--rw-r--r--   0        0        0     2464 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/text_annotator.schema.json
--rw-r--r--   0        0        0     4222 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/text_annotator.yaml
--rw-r--r--   0        0        0    13670 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/validation_datamodel.owl.ttl
--rw-r--r--   0        0        0    25351 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/validation_datamodel.py
--rw-r--r--   0        0        0    10783 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/validation_datamodel.schema.json
--rw-r--r--   0        0        0     7510 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/validation_datamodel.yaml
--rw-r--r--   0        0        0     6640 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/value_set_configuration.owl.ttl
--rw-r--r--   0        0        0     8458 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/value_set_configuration.py
--rw-r--r--   0        0        0     2276 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/value_set_configuration.yaml
--rw-r--r--   0        0        0     5378 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/datamodels/vocabulary.py
--rw-r--r--   0        0        0     5079 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/aggregator/__init__.py
--rw-r--r--   0        0        0     5454 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/aggregator/aggregator_implementation.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/amigo/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/cx/__init__.py
--rw-r--r--   0        0        0     1985 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/cx/cx_implementation.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/fhir/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/funowl/__init__.py
--rw-r--r--   0        0        0     8331 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/funowl/funowl_implementation.py
--rw-r--r--   0        0        0     2313 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/gilda.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/kgx/__init__.py
--rw-r--r--   0        0        0    30631 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/kgx/kgx_implementation.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/neo4j/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/obograph/__init__.py
--rw-r--r--   0        0        0    15754 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/obograph/obograph_implementation.py
--rw-r--r--   0        0        0      267 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/ols/__init__.py
--rw-r--r--   0        0        0      132 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/ols/constants.py
--rw-r--r--   0        0        0     7942 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/ols/ols_implementation.py
--rw-r--r--   0        0        0      686 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/ols/oxo_utils.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/ontobee/__init__.py
--rw-r--r--   0        0        0     1391 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/ontobee/ontobee_implementation.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/ontoportal/__init__.py
--rw-r--r--   0        0        0      382 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/ontoportal/agroportal_implementation.py
--rw-r--r--   0        0        0      821 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/ontoportal/bioportal_implementation.py
--rw-r--r--   0        0        0      378 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
--rw-r--r--   0        0        0      378 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/ontoportal/matportal_implementation.py
--rw-r--r--   0        0        0    12106 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/owlery/__init__.py
--rw-r--r--   0        0        0      427 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/owlery/owlery_implementation.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/pronto/__init__.py
--rw-r--r--   0        0        0    34424 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/pronto/pronto_implementation.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/robot/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/scigraph/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/simpleobo/__init__.py
--rw-r--r--   0        0        0    33470 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
--rw-r--r--   0        0        0    20498 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/simpleobo/simple_obo_parser.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/skos/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/solor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/solr/__init__.py
--rw-r--r--   0        0        0       96 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/sparql/__init__.py
--rw-r--r--   0        0        0    36179 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
--rw-r--r--   0        0        0      885 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/sparql/lov_implementation.py
--rw-r--r--   0        0        0     1721 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
--rw-r--r--   0        0        0     2525 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/sparql/sparql_implementation.py
--rw-r--r--   0        0        0     2326 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/sparql/sparql_query.py
--rw-r--r--   0        0        0       96 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/sqldb/__init__.py
--rw-r--r--   0        0        0    99520 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/sqldb/sql_implementation.py
--rw-r--r--   0        0        0     1903 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/sqldb/sqlite_utils.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/tccm/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/translator/__init__.py
--rw-r--r--   0        0        0     3111 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/translator/translator_implementation.py
--rw-r--r--   0        0        0      108 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/ubergraph/__init__.py
--rw-r--r--   0        0        0    19393 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.560870 oaklib-0.4.1/src/oaklib/implementations/umls/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/implementations/uniprot/__init__.py
--rw-r--r--   0        0        0     9603 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/implementations/uniprot/uniprot_implementation.py
--rw-r--r--   0        0        0       96 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/implementations/wikidata/__init__.py
--rw-r--r--   0        0        0    17121 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/implementations/wikidata/wikidata_implementation.py
--rw-r--r--   0        0        0      913 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/__init__.py
--rw-r--r--   0        0        0     7725 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/association_provider_interface.py
--rw-r--r--   0        0        0    38972 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/basic_ontology_interface.py
--rw-r--r--   0        0        0     6960 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/class_enrichment_calculation_interface.py
--rw-r--r--   0        0        0    11720 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/differ_interface.py
--rw-r--r--   0        0        0     2649 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/dumper_interface.py
--rw-r--r--   0        0        0     3365 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/mapping_provider_interface.py
--rw-r--r--   0        0        0     3262 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/merge_interface.py
--rw-r--r--   0        0        0     3103 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/metadata_interface.py
--rw-r--r--   0        0        0    17700 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/obograph_interface.py
--rw-r--r--   0        0        0     1003 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/obolegacy_interface.py
--rw-r--r--   0        0        0      784 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/ontology_interface.py
--rw-r--r--   0        0        0    10988 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/owl_interface.py
--rw-r--r--   0        0        0     8236 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/patcher_interface.py
--rw-r--r--   0        0        0     1955 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/rdf_interface.py
--rw-r--r--   0        0        0     2459 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/relation_graph_interface.py
--rw-r--r--   0        0        0     1386 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/search_interface.py
--rw-r--r--   0        0        0    12778 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/semsim_interface.py
--rw-r--r--   0        0        0     1063 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/skos_interface.py
--rw-r--r--   0        0        0     2112 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/subsetter_interface.py
--rw-r--r--   0        0        0    10140 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/summary_statistics_interface.py
--rw-r--r--   0        0        0    18296 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/taxon_constraint_interface.py
--rw-r--r--   0        0        0     7511 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/text_annotator_interface.py
--rw-r--r--   0        0        0     3033 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/interfaces/validator_interface.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/__init__.py
--rw-r--r--   0        0        0     1539 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/heatmap_writer.py
--rw-r--r--   0        0        0     1698 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/html_writer.py
--rw-r--r--   0        0        0     1379 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/obograph_writer.py
--rw-r--r--   0        0        0     3444 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/rollup_report_writer.py
--rw-r--r--   0        0        0      739 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_axiom_writer.py
--rw-r--r--   0        0        0     6519 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_csv_writer.py
--rw-r--r--   0        0        0     1284 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_fhir_writer.py
--rw-r--r--   0        0        0     2353 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_info_writer.py
--rw-r--r--   0        0        0     1231 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_json_lines_writer.py
--rw-r--r--   0        0        0     1806 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_json_writer.py
--rw-r--r--   0        0        0      741 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_kgcl_writer.py
--rw-r--r--   0        0        0     2088 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_markdown_writer.py
--rw-r--r--   0        0        0     1152 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_nl_writer.py
--rw-r--r--   0        0        0     1117 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_obo_json_writer.py
--rw-r--r--   0        0        0     3496 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_obo_writer.py
--rw-r--r--   0        0        0     1270 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_owl_functional_writer.py
--rw-r--r--   0        0        0     2244 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_rdf_writer.py
--rw-r--r--   0        0        0     4438 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_writer.py
--rw-r--r--   0        0        0     1301 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/io/streaming_yaml_writer.py
--rw-r--r--   0        0        0      113 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/mappers/__init__.py
--rw-r--r--   0        0        0     3717 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/mappers/base_mapper.py
--rw-r--r--   0        0        0     1849 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/mappers/ontology_metadata_mapper.py
--rw-r--r--   0        0        0     1742 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/parsers/__init__.py
--rw-r--r--   0        0        0      650 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/parsers/association_parser.py
--rw-r--r--   0        0        0      446 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/parsers/association_parser_factory.py
--rw-r--r--   0        0        0     4731 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/parsers/boomer_parser.py
--rw-r--r--   0        0        0     1178 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/parsers/gaf_association_parser.py
--rw-r--r--   0        0        0      563 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/parsers/hpoa_association_parser.py
--rw-r--r--   0        0        0      602 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/parsers/hpoa_g2p_association_parser.py
--rw-r--r--   0        0        0      653 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/parsers/kgx_association_parser.py
--rw-r--r--   0        0        0      525 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/parsers/pairwise_association_parser.py
--rw-r--r--   0        0        0     1328 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/parsers/parser_base.py
--rw-r--r--   0        0        0      707 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/parsers/phaf_association_parser.py
--rw-r--r--   0        0        0     6128 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/parsers/xaf_association_parser.py
--rw-r--r--   0        0        0     2210 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/resource.py
--rw-r--r--   0        0        0     7867 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/selector.py
--rw-r--r--   0        0        0      177 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/types.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/__init__.py
--rw-r--r--   0        0        0     1613 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/apikey_manager.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/associations/__init__.py
--rw-r--r--   0        0        0     2810 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/associations/association_differ.py
--rw-r--r--   0        0        0     2865 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/associations/association_index.py
--rw-r--r--   0        0        0     1182 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/basic_utils.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/graph/__init__.py
--rw-r--r--   0        0        0     2490 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/graph/networkx_bridge.py
--rw-r--r--   0        0        0     2918 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/graph/relationship_walker.py
--rw-r--r--   0        0        0      993 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/identifier_utils.py
--rw-r--r--   0        0        0      999 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/iterator_utils.py
--rw-r--r--   0        0        0     3345 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/kgcl_utilities.py
--rw-r--r--   0        0        0      850 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/label_utilities.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/lexical/__init__.py
--rw-r--r--   0        0        0    19516 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/lexical/lexical_indexer.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/mapping/__init__.py
--rw-r--r--   0        0        0    14443 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/mapping/boomer_utils.py
--rw-r--r--   0        0        0    15328 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/mapping/cross_ontology_diffs.py
--rw-r--r--   0        0        0      751 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/mapping/mapping_propagator.py
--rw-r--r--   0        0        0     2270 2023-04-06 15:15:58.564870 oaklib-0.4.1/src/oaklib/utilities/mapping/mapping_validation.py
--rw-r--r--   0        0        0     2694 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/mapping/sssom_utils.py
--rw-r--r--   0        0        0      684 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/ner_utilities.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/nlp/__init__.py
--rw-r--r--   0        0        0     3358 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/nlp/natual_language_generation.py
--rw-r--r--   0        0        0      136 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/oboformat_utils.py
--rw-r--r--   0        0        0    22266 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/obograph_utils.py
--rw-r--r--   0        0        0     2275 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/ontology_builder.py
--rw-r--r--   0        0        0      379 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/rate_limiter.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/reasoning/__init__.py
--rw-r--r--   0        0        0      569 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/reasoning/relation_graph.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/semsim/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/semsim/similarity_utils.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/stats/__init__.py
--rw-r--r--   0        0        0     1511 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/stats/hypergeometric.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/subsets/__init__.py
--rw-r--r--   0        0        0     2676 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/subsets/slimmer_utils.py
--rw-r--r--   0        0        0     4701 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/subsets/subset_analysis.py
--rw-r--r--   0        0        0    11592 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/subsets/value_set_expander.py
--rw-r--r--   0        0        0    13212 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/table_filler.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/taxon/__init__.py
--rw-r--r--   0        0        0     1743 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/taxon/taxon_constraint_utils.py
--rw-r--r--   0        0        0        0 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/validation/__init__.py
--rw-r--r--   0        0        0    10097 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/validation/definition_ontology_rule.py
--rw-r--r--   0        0        0     7492 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/validation/disjointness_rule.py
--rw-r--r--   0        0        0     1729 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/validation/lint_utils.py
--rw-r--r--   0        0        0     1402 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/validation/ontology_rule.py
--rw-r--r--   0        0        0     1313 2023-04-06 15:15:58.568870 oaklib-0.4.1/src/oaklib/utilities/validation/rule_runner.py
--rw-r--r--   0        0        0     8923 1970-01-01 00:00:00.000000 oaklib-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-10 18:43:08.756935 oaklib-0.5.0/LICENSE
+-rw-r--r--   0        0        0     7241 2023-04-10 18:43:08.756935 oaklib-0.5.0/README.md
+-rw-r--r--   0        0        0     1728 2023-04-10 18:44:11.231480 oaklib-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      271 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/__init__.py
+-rw-r--r--   0        0        0   188756 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/cli.py
+-rw-r--r--   0        0        0       64 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/conf/__init__.py
+-rw-r--r--   0        0        0      115 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/conf/go-pombase-input-spec.yaml
+-rw-r--r--   0        0        0      106 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/conf/hpoa-input-spec.yaml
+-rw-r--r--   0        0        0     1903 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
+-rw-r--r--   0        0        0     4537 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/conf/obograph-style.json
+-rw-r--r--   0        0        0      256 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/conf/omo-to-skos.sssom.tsv
+-rw-r--r--   0        0        0      131 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/conf/value-set-expander.conf.yaml
+-rw-r--r--   0        0        0      128 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/constants.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/converters/__init__.py
+-rw-r--r--   0        0        0     1456 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/converters/data_model_converter.py
+-rw-r--r--   0        0        0     2561 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/converters/logical_definition_flattener.py
+-rw-r--r--   0        0        0     2371 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/converters/obo_graph_to_cx_converter.py
+-rw-r--r--   0        0        0    12163 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/converters/obo_graph_to_fhir_converter.py
+-rw-r--r--   0        0        0     5713 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/converters/obo_graph_to_obo_format_converter.py
+-rw-r--r--   0        0        0     5155 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
+-rw-r--r--   0        0        0       60 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/__init__.py
+-rw-r--r--   0        0        0     4034 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/association.owl.ttl
+-rw-r--r--   0        0        0    10999 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/association.py
+-rw-r--r--   0        0        0     2738 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/association.yaml
+-rw-r--r--   0        0        0     6165 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/class_enrichment.owl.ttl
+-rw-r--r--   0        0        0    10853 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/class_enrichment.py
+-rw-r--r--   0        0        0     2648 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/class_enrichment.yaml
+-rw-r--r--   0        0        0    19083 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
+-rw-r--r--   0        0        0    24246 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/cross_ontology_diff.py
+-rw-r--r--   0        0        0    10687 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/cross_ontology_diff.yaml
+-rw-r--r--   0        0        0    29418 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/cx.py
+-rw-r--r--   0        0        0     6314 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/cx.yaml
+-rw-r--r--   0        0        0    15826 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/fhir.owl.ttl
+-rw-r--r--   0        0        0    35744 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/fhir.py
+-rw-r--r--   0        0        0     5064 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/fhir.yaml
+-rw-r--r--   0        0        0     7671 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/input_specification.py
+-rw-r--r--   0        0        0     1786 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/input_specification.yaml
+-rw-r--r--   0        0        0    15537 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/item_list.py
+-rw-r--r--   0        0        0     5747 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/item_list.yaml
+-rw-r--r--   0        0        0     8984 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/lexical_index.owl.ttl
+-rw-r--r--   0        0        0    17256 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/lexical_index.py
+-rw-r--r--   0        0        0     6429 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/lexical_index.schema.json
+-rw-r--r--   0        0        0     4016 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/lexical_index.yaml
+-rw-r--r--   0        0        0    26434 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/mapping_cluster_datamodel.py
+-rw-r--r--   0        0        0     7317 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
+-rw-r--r--   0        0        0    17785 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
+-rw-r--r--   0        0        0    30468 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.py
+-rw-r--r--   0        0        0    11456 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
+-rw-r--r--   0        0        0     3220 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.yaml
+-rw-r--r--   0        0        0    25354 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/obograph.owl.ttl
+-rw-r--r--   0        0        0    45533 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/obograph.py
+-rw-r--r--   0        0        0    22375 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/obograph.schema.json
+-rw-r--r--   0        0        0    17625 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/obograph.yaml
+-rw-r--r--   0        0        0    59793 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.owl.ttl
+-rw-r--r--   0        0        0   117175 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.py
+-rw-r--r--   0        0        0    95288 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.schema.json
+-rw-r--r--   0        0        0    30433 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.yaml
+-rw-r--r--   0        0        0    14759 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/oxo.owl.ttl
+-rw-r--r--   0        0        0    21914 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/oxo.py
+-rw-r--r--   0        0        0     4392 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/oxo.yaml
+-rw-r--r--   0        0        0     3240 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/search.py
+-rw-r--r--   0        0        0    16948 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/search_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25145 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/search_datamodel.py
+-rw-r--r--   0        0        0     6683 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/search_datamodel.yaml
+-rw-r--r--   0        0        0      287 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/settings.py
+-rw-r--r--   0        0        0    12767 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/similarity.owl.ttl
+-rw-r--r--   0        0        0    22226 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/similarity.py
+-rw-r--r--   0        0        0     5511 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/similarity.yaml
+-rw-r--r--   0        0        0    31217 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
+-rw-r--r--   0        0        0    50743 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.py
+-rw-r--r--   0        0        0    21176 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
+-rw-r--r--   0        0        0    16246 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.yaml
+-rw-r--r--   0        0        0     9909 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/taxon_constraints.owl.ttl
+-rw-r--r--   0        0        0    18430 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/taxon_constraints.py
+-rw-r--r--   0        0        0     5879 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/taxon_constraints.yaml
+-rw-r--r--   0        0        0    11599 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/text_annotator.owl.ttl
+-rw-r--r--   0        0        0    20418 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/text_annotator.py
+-rw-r--r--   0        0        0     2464 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/text_annotator.schema.json
+-rw-r--r--   0        0        0     4219 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/text_annotator.yaml
+-rw-r--r--   0        0        0    13670 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25351 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.py
+-rw-r--r--   0        0        0    10783 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.schema.json
+-rw-r--r--   0        0        0     7510 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.yaml
+-rw-r--r--   0        0        0     6640 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/value_set_configuration.owl.ttl
+-rw-r--r--   0        0        0     8458 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/value_set_configuration.py
+-rw-r--r--   0        0        0     2276 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/value_set_configuration.yaml
+-rw-r--r--   0        0        0     5588 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/vocabulary.py
+-rw-r--r--   0        0        0     5217 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/aggregator/__init__.py
+-rw-r--r--   0        0        0     5454 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/aggregator/aggregator_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/amigo/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/cx/__init__.py
+-rw-r--r--   0        0        0     1985 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/cx/cx_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/fhir/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/funowl/__init__.py
+-rw-r--r--   0        0        0     8473 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/funowl/funowl_implementation.py
+-rw-r--r--   0        0        0     2313 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/gilda.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/kgx/__init__.py
+-rw-r--r--   0        0        0    30631 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/kgx/kgx_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/neo4j/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/obograph/__init__.py
+-rw-r--r--   0        0        0    16141 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/obograph/obograph_implementation.py
+-rw-r--r--   0        0        0      267 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/ols/__init__.py
+-rw-r--r--   0        0        0      132 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/ols/constants.py
+-rw-r--r--   0        0        0     7942 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/ols/ols_implementation.py
+-rw-r--r--   0        0        0      686 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/ols/oxo_utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontobee/__init__.py
+-rw-r--r--   0        0        0     1391 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontobee/ontobee_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontoportal/__init__.py
+-rw-r--r--   0        0        0      382 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontoportal/agroportal_implementation.py
+-rw-r--r--   0        0        0      821 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontoportal/bioportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontoportal/matportal_implementation.py
+-rw-r--r--   0        0        0    12106 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/owlery/__init__.py
+-rw-r--r--   0        0        0      427 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/owlery/owlery_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/pronto/__init__.py
+-rw-r--r--   0        0        0    34553 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/pronto/pronto_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/robot/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/scigraph/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/simpleobo/__init__.py
+-rw-r--r--   0        0        0    33791 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
+-rw-r--r--   0        0        0    21176 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/simpleobo/simple_obo_parser.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/skos/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/solor/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/solr/__init__.py
+-rw-r--r--   0        0        0       96 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sparql/__init__.py
+-rw-r--r--   0        0        0    36578 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
+-rw-r--r--   0        0        0      885 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sparql/lov_implementation.py
+-rw-r--r--   0        0        0     1721 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
+-rw-r--r--   0        0        0     2525 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sparql/sparql_implementation.py
+-rw-r--r--   0        0        0     2326 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sparql/sparql_query.py
+-rw-r--r--   0        0        0       96 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sqldb/__init__.py
+-rw-r--r--   0        0        0   104382 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sqldb/sql_implementation.py
+-rw-r--r--   0        0        0     1903 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sqldb/sqlite_utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/tccm/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/translator/__init__.py
+-rw-r--r--   0        0        0     3111 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/translator/translator_implementation.py
+-rw-r--r--   0        0        0      108 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ubergraph/__init__.py
+-rw-r--r--   0        0        0    19393 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/umls/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/uniprot/__init__.py
+-rw-r--r--   0        0        0     9603 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/uniprot/uniprot_implementation.py
+-rw-r--r--   0        0        0       96 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/wikidata/__init__.py
+-rw-r--r--   0        0        0    17121 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/wikidata/wikidata_implementation.py
+-rw-r--r--   0        0        0      913 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/__init__.py
+-rw-r--r--   0        0        0     7725 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/association_provider_interface.py
+-rw-r--r--   0        0        0    50981 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/basic_ontology_interface.py
+-rw-r--r--   0        0        0     8022 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/class_enrichment_calculation_interface.py
+-rw-r--r--   0        0        0    11720 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/differ_interface.py
+-rw-r--r--   0        0        0     2649 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/dumper_interface.py
+-rw-r--r--   0        0        0     3365 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/mapping_provider_interface.py
+-rw-r--r--   0        0        0     3262 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/merge_interface.py
+-rw-r--r--   0        0        0     3103 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/metadata_interface.py
+-rw-r--r--   0        0        0    17700 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/obograph_interface.py
+-rw-r--r--   0        0        0     1003 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/obolegacy_interface.py
+-rw-r--r--   0        0        0      784 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/ontology_interface.py
+-rw-r--r--   0        0        0    10988 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/owl_interface.py
+-rw-r--r--   0        0        0     8236 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/patcher_interface.py
+-rw-r--r--   0        0        0     1955 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/rdf_interface.py
+-rw-r--r--   0        0        0     2459 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/relation_graph_interface.py
+-rw-r--r--   0        0        0     1386 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/search_interface.py
+-rw-r--r--   0        0        0    12778 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/semsim_interface.py
+-rw-r--r--   0        0        0     1063 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/skos_interface.py
+-rw-r--r--   0        0        0     2112 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/subsetter_interface.py
+-rw-r--r--   0        0        0    10140 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/summary_statistics_interface.py
+-rw-r--r--   0        0        0    18296 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/interfaces/taxon_constraint_interface.py
+-rw-r--r--   0        0        0     7511 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/interfaces/text_annotator_interface.py
+-rw-r--r--   0        0        0     3033 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/interfaces/validator_interface.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/__init__.py
+-rw-r--r--   0        0        0     1539 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/heatmap_writer.py
+-rw-r--r--   0        0        0     1698 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/html_writer.py
+-rw-r--r--   0        0        0     1379 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/obograph_writer.py
+-rw-r--r--   0        0        0     3444 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/rollup_report_writer.py
+-rw-r--r--   0        0        0      739 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_axiom_writer.py
+-rw-r--r--   0        0        0     7833 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_csv_writer.py
+-rw-r--r--   0        0        0     1284 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_fhir_writer.py
+-rw-r--r--   0        0        0     2524 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_info_writer.py
+-rw-r--r--   0        0        0     1231 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_json_lines_writer.py
+-rw-r--r--   0        0        0     1806 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_json_writer.py
+-rw-r--r--   0        0        0      741 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_kgcl_writer.py
+-rw-r--r--   0        0        0     2088 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_markdown_writer.py
+-rw-r--r--   0        0        0     1152 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_nl_writer.py
+-rw-r--r--   0        0        0     1117 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_obo_json_writer.py
+-rw-r--r--   0        0        0     3496 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_obo_writer.py
+-rw-r--r--   0        0        0     1270 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_owl_functional_writer.py
+-rw-r--r--   0        0        0     2244 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_rdf_writer.py
+-rw-r--r--   0        0        0     5129 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_writer.py
+-rw-r--r--   0        0        0     1301 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_yaml_writer.py
+-rw-r--r--   0        0        0      113 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/mappers/__init__.py
+-rw-r--r--   0        0        0     3717 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/mappers/base_mapper.py
+-rw-r--r--   0        0        0     1849 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/mappers/ontology_metadata_mapper.py
+-rw-r--r--   0        0        0     1742 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/__init__.py
+-rw-r--r--   0        0        0      650 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/association_parser.py
+-rw-r--r--   0        0        0      522 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/association_parser_factory.py
+-rw-r--r--   0        0        0     4731 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/boomer_parser.py
+-rw-r--r--   0        0        0     1178 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/gaf_association_parser.py
+-rw-r--r--   0        0        0      563 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/hpoa_association_parser.py
+-rw-r--r--   0        0        0      602 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/hpoa_g2p_association_parser.py
+-rw-r--r--   0        0        0      653 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/kgx_association_parser.py
+-rw-r--r--   0        0        0      525 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/pairwise_association_parser.py
+-rw-r--r--   0        0        0     1328 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/parser_base.py
+-rw-r--r--   0        0        0      707 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/phaf_association_parser.py
+-rw-r--r--   0        0        0     6194 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/xaf_association_parser.py
+-rw-r--r--   0        0        0     2210 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/resource.py
+-rw-r--r--   0        0        0    12291 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/selector.py
+-rw-r--r--   0        0        0      177 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/types.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/__init__.py
+-rw-r--r--   0        0        0     1613 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/apikey_manager.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/associations/__init__.py
+-rw-r--r--   0        0        0     2810 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/associations/association_differ.py
+-rw-r--r--   0        0        0     2865 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/associations/association_index.py
+-rw-r--r--   0        0        0     1182 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/basic_utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/graph/__init__.py
+-rw-r--r--   0        0        0     2490 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/graph/networkx_bridge.py
+-rw-r--r--   0        0        0     2918 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/graph/relationship_walker.py
+-rw-r--r--   0        0        0      993 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/identifier_utils.py
+-rw-r--r--   0        0        0      999 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/iterator_utils.py
+-rw-r--r--   0        0        0     3345 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/kgcl_utilities.py
+-rw-r--r--   0        0        0      850 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/label_utilities.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/lexical/__init__.py
+-rw-r--r--   0        0        0    19516 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/lexical/lexical_indexer.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/mapping/__init__.py
+-rw-r--r--   0        0        0    14443 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/mapping/boomer_utils.py
+-rw-r--r--   0        0        0    15328 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/mapping/cross_ontology_diffs.py
+-rw-r--r--   0        0        0      751 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/mapping/mapping_propagator.py
+-rw-r--r--   0        0        0     2270 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/mapping/mapping_validation.py
+-rw-r--r--   0        0        0     2694 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/mapping/sssom_utils.py
+-rw-r--r--   0        0        0      684 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/ner_utilities.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/nlp/__init__.py
+-rw-r--r--   0        0        0     3358 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/nlp/natual_language_generation.py
+-rw-r--r--   0        0        0      136 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/oboformat_utils.py
+-rw-r--r--   0        0        0    22266 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/obograph_utils.py
+-rw-r--r--   0        0        0     2275 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/ontology_builder.py
+-rw-r--r--   0        0        0      379 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/rate_limiter.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/reasoning/__init__.py
+-rw-r--r--   0        0        0      569 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/reasoning/relation_graph.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/semsim/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/semsim/similarity_utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/stats/__init__.py
+-rw-r--r--   0        0        0     1511 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/stats/hypergeometric.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/subsets/__init__.py
+-rw-r--r--   0        0        0     2676 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/subsets/slimmer_utils.py
+-rw-r--r--   0        0        0     4701 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/subsets/subset_analysis.py
+-rw-r--r--   0        0        0    11592 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/subsets/value_set_expander.py
+-rw-r--r--   0        0        0    13212 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/table_filler.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/taxon/__init__.py
+-rw-r--r--   0        0        0     1743 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/taxon/taxon_constraint_utils.py
+-rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/validation/__init__.py
+-rw-r--r--   0        0        0    10097 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/validation/definition_ontology_rule.py
+-rw-r--r--   0        0        0     7492 2023-04-10 18:43:08.908941 oaklib-0.5.0/src/oaklib/utilities/validation/disjointness_rule.py
+-rw-r--r--   0        0        0     1729 2023-04-10 18:43:08.908941 oaklib-0.5.0/src/oaklib/utilities/validation/lint_utils.py
+-rw-r--r--   0        0        0     1402 2023-04-10 18:43:08.908941 oaklib-0.5.0/src/oaklib/utilities/validation/ontology_rule.py
+-rw-r--r--   0        0        0     1313 2023-04-10 18:43:08.908941 oaklib-0.5.0/src/oaklib/utilities/validation/rule_runner.py
+-rw-r--r--   0        0        0     8923 1970-01-01 00:00:00.000000 oaklib-0.5.0/PKG-INFO
```

### Comparing `oaklib-0.4.1/LICENSE` & `oaklib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/README.md` & `oaklib-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/pyproject.toml` & `oaklib-0.5.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oaklib"
-version = "v0.4.1"
+version = "v0.5.0"
 description = "Ontology Access Kit: Python library for common ontology operations over a variety of backends"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
```

### Comparing `oaklib-0.4.1/src/oaklib/cli.py` & `oaklib-0.5.0/src/oaklib/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import json
 import logging
 import os
 import re
 import secrets
 import sys
 from collections import defaultdict
-from dataclasses import dataclass
 from enum import Enum, unique
 from itertools import chain
 from pathlib import Path
 from time import time
 from types import ModuleType
 from typing import (
     IO,
@@ -57,14 +56,15 @@
     Edge,
     Graph,
     GraphDocument,
     Meta,
     PrefixDeclaration,
 )
 from oaklib.datamodels.search import create_search_configuration
+from oaklib.datamodels.settings import Settings
 from oaklib.datamodels.summary_statistics_datamodel import (
     GroupedStatistics,
     UngroupedStatistics,
 )
 from oaklib.datamodels.text_annotator import TextAnnotationConfiguration
 from oaklib.datamodels.validation_datamodel import ValidationConfiguration
 from oaklib.datamodels.vocabulary import (
@@ -132,18 +132,15 @@
 from oaklib.io.streaming_owl_functional_writer import StreamingOwlFunctionalWriter
 from oaklib.io.streaming_rdf_writer import StreamingRdfWriter
 from oaklib.io.streaming_writer import StreamingWriter
 from oaklib.io.streaming_yaml_writer import StreamingYamlWriter
 from oaklib.mappers.ontology_metadata_mapper import OntologyMetadataMapper
 from oaklib.parsers.association_parser_factory import get_association_parser
 from oaklib.resource import OntologyResource
-from oaklib.selector import (
-    get_implementation_from_shorthand,
-    get_resource_from_shorthand,
-)
+from oaklib.selector import get_adapter, get_resource_from_shorthand
 from oaklib.types import CURIE, PRED_CURIE
 from oaklib.utilities import table_filler
 from oaklib.utilities.apikey_manager import set_apikey_value
 from oaklib.utilities.associations.association_differ import AssociationDiffer
 from oaklib.utilities.iterator_utils import chunk
 from oaklib.utilities.kgcl_utilities import (
     generate_change_id,
@@ -270,22 +267,22 @@
     intersection = "intersection"
     union = "union"
     difference = "difference"
     symmetric_difference = "symmetric_difference"
     reverse_difference = "reverse_difference"
 
 
-@dataclass
-class Settings:
-    impl: Any = None
-    autosave: bool = False
-    associations_type: str = None
+# TODO: use contexts. See https://stackoverflow.com/questions/64381222/python-click-access-option-values-globally
+settings = Settings()
+
 
+def clear_cli_settings():
+    for k in settings.__dict__:
+        setattr(settings, k, None)
 
-settings = Settings()
 
 input_option = click.option(
     "-i",
     "--input",
     help="input implementation specification. This is either a path to a file, or an ontology selector",
 )
 add_option = click.option(
@@ -394,15 +391,22 @@
     help="a json file to configure visualization. See https://berkeleybop.github.io/kgviz-model/",
 )
 stylemap_configure_option = click.option(
     "-C",
     "--configure",
     help='overrides for stylemap, specified as yaml. E.g. `-C "styles: [filled, rounded]" `',
 )
-
+pivot_languages = click.option(
+    "--pivot-languages/--no-pivot-languages",
+    help="include one column per language",
+)
+all_languages = click.option(
+    "--all-languages/--no-all-languages",
+    help="if source is multi-lingual, show all languages rather than just default",
+)
 group_by_property_option = click.option(
     "--group-by-property",
     help="group summaries by a metadata property, e.g. rdfs:isDefinedBy",
 )
 group_by_obo_namespace_option = click.option(
     "--group-by-obo-namespace/--no-group-by-obo-namespace",
     default=False,
@@ -475,14 +479,15 @@
         if output_type in WRITERS:
             typ = WRITERS[output_type]
         else:
             raise ValueError(f"Unrecognized output type: {output_type}")
     w = typ(ontology_interface=impl)
     if w.uses_schemaview and datamodel is not None:
         w.schemaview = package_schemaview(datamodel.__name__)
+    w.settings = settings
     return w
 
 
 def _apply_changes(impl, changes: List[kgcl.Change]):
     if changes:
         logging.info(f"Applying {len(changes)} changes")
         if not isinstance(impl, PatcherInterface):
@@ -805,14 +810,20 @@
 @click.option(
     "--import-depth",
     type=click.INT,
     help="Maximum depth in the import tree to traverse. Currently this is only used by the pronto adapter",
 )
 @click.option("--associations", "-g", multiple=True, help="Location of ontology associations")
 @click.option("--associations-type", "-G", help="Syntax of associations input")
+@click.option(
+    "--preferred-language", "-l", help="Preferred language for labels and lexical elements"
+)
+@click.option(
+    "--other-languages", multiple=True, help="Additional languages for labels and lexical elements"
+)
 @input_option
 @input_type_option
 @add_option
 @click.option(
     "--merge/--no-merge",
     default=False,
     show_default=True,
@@ -830,14 +841,15 @@
     associations_type: str,
     save_as: str,
     autosave: bool,
     named_prefix_map,
     metamodel_mappings,
     prefix,
     import_depth: Optional[int],
+    **kwargs,
 ):
     """Run the oaklib Command Line.
 
     A subcommand must be passed - for example: ancestors, terms, ...
 
     Most commands require an input ontology to be specified:
 
@@ -857,26 +869,31 @@
     else:
         logger.setLevel(logging.WARNING)
     if quiet:
         logger.setLevel(logging.ERROR)
     resource = OntologyResource()
     resource.slug = input
     settings.autosave = autosave
+    for k, v in kwargs.items():
+        if v is not None:
+            logging.info(f"Setting {k}={v}")
+            setattr(settings, k, v)
     logging.info(f"Settings = {settings}")
     if input:
-        impl_class: Type[OntologyInterface]
-        resource = get_resource_from_shorthand(input, format=input_type, import_depth=import_depth)
-        impl_class = resource.implementation_class
-        logging.info(f"RESOURCE={resource}")
-        settings.impl = impl_class(resource)
+        # impl_class: Type[OntologyInterface]
+        # resource = get_resource_from_shorthand(input, format=input_type, import_depth=import_depth)
+        # impl_class = resource.implementation_class
+        # logging.info(f"RESOURCE={resource}")
+        # settings.impl = impl_class(resource)
+        settings.impl = get_adapter(input)
         settings.impl.autosave = autosave
     if merge and not add:
         raise ValueError("Cannot use --merge without --add")
     if add:
-        impls = [get_implementation_from_shorthand(d) for d in add]
+        impls = [get_adapter(d) for d in add]
         if merge:
             if isinstance(settings.impl, MergeInterface):
                 settings.impl.merge(impls)
             else:
                 raise NotImplementedError(f"{type(settings.impl)} does not implement merging")
         else:
             if settings.impl:
@@ -1214,15 +1231,15 @@
         diff_config.group_by_property = PREFIX_PREDICATE
     diff_stats = None
     if compare_with:
         if branches:
             raise click.UsageError("Cannot specify both branches and compare_with")
         if not isinstance(impl, DifferInterface):
             raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
-        other = get_implementation_from_shorthand(compare_with)
+        other = get_adapter(compare_with)
         logging.info(f"Comparing {impl} with {other} using {diff_config}")
         diff_stats = impl.diff_summary(other, configuration=diff_config)
     if not branches and not group_by_property:
         ssc = impl.branch_summary_statistics(prefixes=prefixes)
     else:
         if branches and group_by_property:
             raise click.UsageError("Cannot specify both branches and predicates")
@@ -2805,21 +2822,49 @@
     logging.info(f"Input Terms={terms}; w={writer}")
     for curie in query_terms_iterator(terms, impl):
         writer.emit(curie)
     writer.finish()
 
 
 @main.command()
+def languages():
+    """
+    Show available languages
+
+    Example:
+
+        runoak languages
+
+    """
+    impl = settings.impl
+    if not isinstance(impl, BasicOntologyInterface):
+        raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
+    for lang in impl.languages():
+        print(lang + ("*" if lang == settings.preferred_language else ""))
+
+
+@main.command()
 @click.argument("terms", nargs=-1)
 @output_option
 @display_option
 @ontological_output_type_option
+@pivot_languages
+@all_languages
 @if_absent_option
 @set_value_option
-def labels(terms, output: TextIO, display: str, output_type: str, if_absent, set_value):
+def labels(
+    terms,
+    output: TextIO,
+    display: str,
+    output_type: str,
+    if_absent,
+    set_value,
+    pivot_languages: bool,
+    all_languages: bool,
+):
     """
     Show labels for term or list of terms
 
     Example:
 
         runoak -i cl.owl labels CL:4023093 CL:4023094
 
@@ -2833,44 +2878,71 @@
 
     You can query for terms that have either no label, or to include only ones with labels:
 
     Nodes with no labels:
 
         runoak -i cl.owl labels .all --if-absent exclude
 
+    Multilingual support: if the adapter supports multilingual querying
+    (currently only SQL) *and* the ontology has multilingual support, you can restrict results to
+    a particular language.
+
+    Example:
+
+        runoak --preferred-language fr -i sqlite:obo:hpinternational labels .ancestors HP:0020110
+
+    You can also query for all languages, and see these pivoted:
+
+    Example:
+
+        runoak  -i sqlite:obo:hpinternational labels .ancestors HP:0020110 --pivot-languages
+
     Python API:
 
        https://incatools.github.io/ontology-access-kit/interfaces/labels
     """
     impl = settings.impl
     writer = _get_writer(output_type, impl, StreamingCsvWriter)
     writer.display_options = display.split(",")
     writer.file = output
     if len(terms) == 0:
         raise ValueError("You must specify a list of terms. Use '.all' for all terms")
     n = 0
+    logging.info(f"Fetching labels; lang={settings.preferred_language}")
     changes = []
+    if pivot_languages:
+        all_languages = True
+        writer.pivot_fields = ["language"]
     for curie_it in chunk(query_terms_iterator(terms, impl)):
         logging.info("** Next chunk:")
         n += 1
-        for curie, label in impl.labels(curie_it):
-            obj = dict(id=curie, label=label)
-            if set_value is not None:
-                obj["new_value"] = set_value
-                if set_value != label:
-                    changes.append(
-                        kgcl.NodeRename(
-                            id="x", about_node=curie, old_value=label, new_value=set_value
+        if all_languages:
+            for curie, label, lang in impl.multilingual_labels(curie_it):
+                obj = dict(id=curie, label=label, language=lang)
+                if set_value is not None:
+                    raise NotImplementedError("Cannot set value for multilingual labels yet")
+                if _skip_if_absent(if_absent, label):
+                    continue
+                writer.emit(obj)
+        else:
+            for curie, label in impl.labels(curie_it, lang=settings.preferred_language):
+                obj = dict(id=curie, label=label)
+                if set_value is not None:
+                    obj["new_value"] = set_value
+                    if set_value != label:
+                        changes.append(
+                            kgcl.NodeRename(
+                                id="x", about_node=curie, old_value=label, new_value=set_value
+                            )
                         )
-                    )
-                else:
-                    logging.info(f"No change for {curie}")
-            if _skip_if_absent(if_absent, label):
-                continue
-            writer.emit(obj)
+                    else:
+                        logging.info(f"No change for {curie}")
+                if _skip_if_absent(if_absent, label):
+                    continue
+                writer.emit(obj)
     if n == 0:
         raise ValueError(f"No results for input: {terms}")
     _apply_changes(impl, changes)
     writer.finish()
 
 
 @main.command()
@@ -3944,19 +4016,30 @@
     terms or term queries, plus the closure predicate(s), e.g.
 
     Example:
 
         runoak -i sqlite:obo:hp -g test.hpoa -G hpoa associations -p i HP:0001392
 
     This shows all annotations either to "Abnormality of the liver" (HP:0001392), or
-    to is-a descendants
+    to is-a descendants.
+
+    Using input specifications:
+
+    It can be awkward to specify both input ontology and association path and format. You
+    can use input specifications to bundle common combinations of inputs together.
+
+    For example, the go-dictybase-input-spec combines go plus dictybase associations.
+
+    Example:
+
+        runoak --i src/oaklib/conf/go-dictybase-input-spec.yaml associations -p i,p GO:0008104
 
     """
     impl = settings.impl
-    writer = _get_writer(output_type, impl, StreamingYamlWriter)
+    writer = _get_writer(output_type, impl, StreamingCsvWriter)
     writer.autolabel = autolabel
     writer.output = output
     actual_predicates = _process_predicates_arg(predicates)
     actual_association_predicates = _process_predicates_arg(association_predicates)
     if isinstance(impl, AssociationProviderInterface):
         curies = list(query_terms_iterator(terms, impl))
         qs_it = impl.associations(
@@ -4761,15 +4844,15 @@
 
     EXPERIMENTAL
     """
     impl = settings.impl
     if other_ontology is None:
         other_impl = impl
     else:
-        other_impl = get_implementation_from_shorthand(other_ontology)
+        other_impl = get_adapter(other_ontology)
     terms = list(query_terms_iterator(terms, impl))
     if len(terms) == 2:
         [term, other_term] = terms
     elif len(terms) == 1:
         (term, other_term) = terms[0], None
     else:
         raise ValueError(f"Must pass one or two terms; got: {terms}")
@@ -4867,15 +4950,15 @@
     use ROBOT.
 
     """
     impl = settings.impl
     writer = _get_writer(output_type, impl, StreamingYamlWriter)
     writer.output = output
     writer.heterogeneous_keys = True
-    other_impl = get_implementation_from_shorthand(other_ontology)
+    other_impl = get_adapter(other_ontology)
     config = DiffConfiguration(simple=simple)
     if group_by_obo_namespace:
         config.group_by_property = HAS_OBO_NAMESPACE
     if group_by_defined_by:
         config.group_by_property = IS_DEFINED_BY
     if group_by_prefix:
         config.group_by_property = PREFIX_PREDICATE
@@ -5212,15 +5295,15 @@
         output_type, oi, StreamingYamlWriter, datamodel=datamodels.cross_ontology_diff
     )
     writer.output = output
     if other_input:
         if intra:
             raise ValueError("No not specify --intra if --other-input is specified")
         else:
-            other_oi = get_implementation_from_shorthand(other_input, format=other_input_type)
+            other_oi = get_adapter(other_input, format=other_input_type)
     else:
         if intra:
             other_oi = oi
         else:
             raise ValueError(
                 "No --other-input specified - specify --intra if mappings are within the main input"
             )
```

### Comparing `oaklib-0.4.1/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml` & `oaklib-0.5.0/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/conf/obograph-style.json` & `oaklib-0.5.0/src/oaklib/conf/obograph-style.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/converters/data_model_converter.py` & `oaklib-0.5.0/src/oaklib/converters/data_model_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/converters/logical_definition_flattener.py` & `oaklib-0.5.0/src/oaklib/converters/logical_definition_flattener.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/converters/obo_graph_to_cx_converter.py` & `oaklib-0.5.0/src/oaklib/converters/obo_graph_to_cx_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/converters/obo_graph_to_fhir_converter.py` & `oaklib-0.5.0/src/oaklib/converters/obo_graph_to_fhir_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/converters/obo_graph_to_obo_format_converter.py` & `oaklib-0.5.0/src/oaklib/converters/obo_graph_to_obo_format_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py` & `oaklib-0.5.0/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/association.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/association.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/association.py` & `oaklib-0.5.0/src/oaklib/datamodels/association.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/association.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/association.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/class_enrichment.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/class_enrichment.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/class_enrichment.py` & `oaklib-0.5.0/src/oaklib/datamodels/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/class_enrichment.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/cross_ontology_diff.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/cross_ontology_diff.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/cross_ontology_diff.py` & `oaklib-0.5.0/src/oaklib/datamodels/cross_ontology_diff.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/cross_ontology_diff.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/cross_ontology_diff.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/fhir.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/fhir.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/fhir.py` & `oaklib-0.5.0/src/oaklib/datamodels/fhir.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/fhir.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/fhir.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/lexical_index.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/lexical_index.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/lexical_index.py` & `oaklib-0.5.0/src/oaklib/datamodels/lexical_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/lexical_index.schema.json` & `oaklib-0.5.0/src/oaklib/datamodels/lexical_index.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/lexical_index.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/lexical_index.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/mapping_cluster_datamodel.py` & `oaklib-0.5.0/src/oaklib/datamodels/mapping_cluster_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/mapping_cluster_datamodel.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/mapping_cluster_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/mapping_rules_datamodel.py` & `oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from mapping_rules_datamodel.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-02-27T09:56:28
+# Generation date: 2023-04-09T14:06:46
 # Schema: mapping-rules-datamodel
 #
 # id: https://w3id.org/oak/mapping-rules-datamodel
 # description: A datamodel for specifying lexical mapping rules.
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
@@ -159,14 +159,15 @@
 
     subject_source_one_of: Optional[Union[str, List[str]]] = empty_list()
     object_source_one_of: Optional[Union[str, List[str]]] = empty_list()
     mapping_source_one_of: Optional[Union[str, List[str]]] = empty_list()
     subject_match_field_one_of: Optional[Union[str, List[str]]] = empty_list()
     object_match_field_one_of: Optional[Union[str, List[str]]] = empty_list()
     transformations_included_in: Optional[Union[str, List[str]]] = empty_list()
+    predicate_id_one_of: Optional[Union[str, List[str]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if not isinstance(self.subject_source_one_of, list):
             self.subject_source_one_of = (
                 [self.subject_source_one_of] if self.subject_source_one_of is not None else []
             )
         self.subject_source_one_of = [
@@ -215,14 +216,22 @@
                 if self.transformations_included_in is not None
                 else []
             )
         self.transformations_included_in = [
             v if isinstance(v, str) else str(v) for v in self.transformations_included_in
         ]
 
+        if not isinstance(self.predicate_id_one_of, list):
+            self.predicate_id_one_of = (
+                [self.predicate_id_one_of] if self.predicate_id_one_of is not None else []
+            )
+        self.predicate_id_one_of = [
+            v if isinstance(v, str) else str(v) for v in self.predicate_id_one_of
+        ]
+
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class Postcondition(YAMLRoot):
     _inherited_slots: ClassVar[List[str]] = []
 
@@ -468,26 +477,26 @@
 
     class_class_uri: ClassVar[URIRef] = ONTOLEXINDEX.LexicalTransformation
     class_class_curie: ClassVar[str] = "ontolexindex:LexicalTransformation"
     class_name: ClassVar[str] = "LexicalTransformation"
     class_model_uri: ClassVar[URIRef] = MAPPINGRULES.LexicalTransformation
 
     type: Optional[Union[str, "TransformationType"]] = None
-    params: Optional[str] = None
+    params: Optional[Union[Union[dict, "Any"], List[Union[dict, "Any"]]]] = empty_list()
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.type is not None and not isinstance(self.type, TransformationType):
             self.type = TransformationType(self.type)
 
-        if self.params is not None and not isinstance(self.params, str):
-            self.params = str(self.params)
-
         super().__post_init__(**kwargs)
 
 
+Any = Any
+
+
 # Enumerations
 class TransformationType(EnumDefinitionImpl):
     """
     A controlled datamodels of the types of transformation that can be applied to
     """
 
     Stemming = PermissibleValue(
@@ -645,14 +654,23 @@
     name="precondition__transformations_included_in",
     curie=MAPPINGRULES.curie("transformations_included_in"),
     model_uri=MAPPINGRULES.precondition__transformations_included_in,
     domain=None,
     range=Optional[Union[str, List[str]]],
 )
 
+slots.precondition__predicate_id_one_of = Slot(
+    uri=MAPPINGRULES.predicate_id_one_of,
+    name="precondition__predicate_id_one_of",
+    curie=MAPPINGRULES.curie("predicate_id_one_of"),
+    model_uri=MAPPINGRULES.precondition__predicate_id_one_of,
+    domain=None,
+    range=Optional[Union[str, List[str]]],
+)
+
 slots.postcondition__predicate_id = Slot(
     uri=MAPPINGRULES.predicate_id,
     name="postcondition__predicate_id",
     curie=MAPPINGRULES.curie("predicate_id"),
     model_uri=MAPPINGRULES.postcondition__predicate_id,
     domain=None,
     range=Optional[str],
@@ -851,9 +869,9 @@
 
 slots.lexicalTransformation__params = Slot(
     uri=ONTOLEXINDEX.params,
     name="lexicalTransformation__params",
     curie=ONTOLEXINDEX.curie("params"),
     model_uri=MAPPINGRULES.lexicalTransformation__params,
     domain=None,
-    range=Optional[str],
+    range=Optional[Union[Union[dict, Any], List[Union[dict, Any]]]],
 )
```

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/mapping_rules_datamodel.schema.json` & `oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/mapping_rules_datamodel.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/obograph.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/obograph.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/obograph.py` & `oaklib-0.5.0/src/oaklib/datamodels/obograph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/obograph.schema.json` & `oaklib-0.5.0/src/oaklib/datamodels/obograph.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/obograph.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/obograph.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/ontology_metadata.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/ontology_metadata.py` & `oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from ontology_metadata.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-01-26T08:32:03
+# Generation date: 2023-04-09T14:06:34
 # Schema: Ontology-Metadata
 #
 # id: http://purl.obolibrary.org/obo/omo/schema
 # description: Schema for ontology metadata
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
@@ -52,14 +52,15 @@
 NCBITAXON = CurieNamespace("NCBITaxon", "http://purl.obolibrary.org/obo/NCBITaxon_")
 NCIT = CurieNamespace("NCIT", "http://purl.obolibrary.org/obo/NCIT_")
 OBI = CurieNamespace("OBI", "http://purl.obolibrary.org/obo/OBI_")
 OIO = CurieNamespace("OIO", "http://www.geneontology.org/formats/oboInOwl#")
 OMO = CurieNamespace("OMO", "http://purl.obolibrary.org/obo/OMO_")
 RO = CurieNamespace("RO", "http://purl.obolibrary.org/obo/RO_")
 BIOLINK = CurieNamespace("biolink", "https://w3id.org/biolink/vocab/")
+DCE = CurieNamespace("dce", "http://example.org/UNKNOWN/dce/")
 DCTERMS = CurieNamespace("dcterms", "http://purl.org/dc/terms/")
 FOAF = CurieNamespace("foaf", "http://xmlns.com/foaf/0.1/")
 LINKML = CurieNamespace("linkml", "https://w3id.org/linkml/")
 OBO = CurieNamespace("obo", "http://purl.obolibrary.org/obo/")
 OIO = CurieNamespace("oio", "http://www.geneontology.org/formats/oboInOwl#")
 OMOSCHEMA = CurieNamespace("omoschema", "http://purl.obolibrary.org/obo/omo/schema/")
 ORCID = CurieNamespace("orcid", "https://orcid.org/")
@@ -2049,14 +2050,32 @@
     name="definition",
     curie=IAO.curie("0000115"),
     model_uri=OMOSCHEMA.definition,
     domain=None,
     range=Optional[Union[Union[str, NarrativeText], List[Union[str, NarrativeText]]]],
 )
 
+slots.predicate = Slot(
+    uri=OMOSCHEMA.predicate,
+    name="predicate",
+    curie=OMOSCHEMA.curie("predicate"),
+    model_uri=OMOSCHEMA.predicate,
+    domain=None,
+    range=Optional[str],
+)
+
+slots.object = Slot(
+    uri=OMOSCHEMA.object,
+    name="object",
+    curie=OMOSCHEMA.curie("object"),
+    model_uri=OMOSCHEMA.object,
+    domain=None,
+    range=Optional[str],
+)
+
 slots.title = Slot(
     uri=DCTERMS.title,
     name="title",
     curie=DCTERMS.curie("title"),
     model_uri=OMOSCHEMA.title,
     domain=None,
     range=Optional[Union[str, NarrativeText]],
@@ -2193,14 +2212,23 @@
     name="defaultLanguage",
     curie=PROTEGE.curie("defaultLanguage"),
     model_uri=OMOSCHEMA.defaultLanguage,
     domain=None,
     range=Optional[str],
 )
 
+slots.language = Slot(
+    uri=DCTERMS.language,
+    name="language",
+    curie=DCTERMS.curie("language"),
+    model_uri=OMOSCHEMA.language,
+    domain=None,
+    range=Optional[str],
+)
+
 slots.has_ontology_root_term = Slot(
     uri=IAO["0000700"],
     name="has_ontology_root_term",
     curie=IAO.curie("0000700"),
     model_uri=OMOSCHEMA.has_ontology_root_term,
     domain=None,
     range=Optional[Union[Union[str, ClassId], List[Union[str, ClassId]]]],
```

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/ontology_metadata.schema.json` & `oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/ontology_metadata.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -626,14 +626,19 @@
       - allotrope permitted profile  ## allotrope uses skos
   has_curation_status:
     is_a: informative_property
     slot_uri: IAO:0000114
   defaultLanguage:
     is_a: informative_property
     slot_uri: protege:defaultLanguage
+  language:
+    is_a: informative_property
+    slot_uri: dcterms:language
+    exact_mappings:
+      - dce:language
   has_ontology_root_term:
     is_a: informative_property
     slot_uri: IAO:0000700
     multivalued: true
     range: Class
     #recommended: true
   # patterns
```

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/oxo.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/oxo.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/oxo.py` & `oaklib-0.5.0/src/oaklib/datamodels/oxo.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/oxo.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/oxo.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/search.py` & `oaklib-0.5.0/src/oaklib/datamodels/search.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/search_datamodel.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/search_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/search_datamodel.py` & `oaklib-0.5.0/src/oaklib/datamodels/search_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/search_datamodel.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/search_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/similarity.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/similarity.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/similarity.py` & `oaklib-0.5.0/src/oaklib/datamodels/similarity.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # Auto generated from similarity.yaml by pythongen.py version: 0.9.0
-# Generation date: 2022-09-07T23:25:27
+# Generation date: 2023-04-10T09:38:53
 # Schema: similarity
 #
-# id: https://w3id.org/linkml/similarity
+# id: https://w3id.org/oak/similarity
 # description: A datamodel for representing semantic similarity between terms or lists of terms.
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
+import re
+import sys
 from dataclasses import dataclass
 from typing import Any, ClassVar, Dict, List, Optional, Union
 
 from jsonasobj2 import JsonObj, as_dict
 from linkml_runtime.linkml_model.meta import (
     EnumDefinition,
     PermissibleValue,
@@ -296,49 +298,53 @@
 
     class_class_uri: ClassVar[URIRef] = SIM.BestMatch
     class_class_curie: ClassVar[str] = "sim:BestMatch"
     class_name: ClassVar[str] = "BestMatch"
     class_model_uri: ClassVar[URIRef] = SIM.BestMatch
 
     match_source: Union[str, BestMatchMatchSource] = None
+    score: float = None
+    similarity: Union[dict, TermPairwiseSimilarity] = None
     match_source_label: Optional[str] = None
     match_target: Optional[str] = None
     match_target_label: Optional[str] = None
-    score: Optional[float] = None
     match_subsumer: Optional[Union[str, URIorCURIE]] = None
     match_subsumer_label: Optional[str] = None
-    similarity: Optional[Union[dict, TermPairwiseSimilarity]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.match_source):
             self.MissingRequiredField("match_source")
         if not isinstance(self.match_source, BestMatchMatchSource):
             self.match_source = BestMatchMatchSource(self.match_source)
 
+        if self._is_empty(self.score):
+            self.MissingRequiredField("score")
+        if not isinstance(self.score, float):
+            self.score = float(self.score)
+
+        if self._is_empty(self.similarity):
+            self.MissingRequiredField("similarity")
+        if not isinstance(self.similarity, TermPairwiseSimilarity):
+            self.similarity = TermPairwiseSimilarity(**as_dict(self.similarity))
+
         if self.match_source_label is not None and not isinstance(self.match_source_label, str):
             self.match_source_label = str(self.match_source_label)
 
         if self.match_target is not None and not isinstance(self.match_target, str):
             self.match_target = str(self.match_target)
 
         if self.match_target_label is not None and not isinstance(self.match_target_label, str):
             self.match_target_label = str(self.match_target_label)
 
-        if self.score is not None and not isinstance(self.score, float):
-            self.score = float(self.score)
-
         if self.match_subsumer is not None and not isinstance(self.match_subsumer, URIorCURIE):
             self.match_subsumer = URIorCURIE(self.match_subsumer)
 
         if self.match_subsumer_label is not None and not isinstance(self.match_subsumer_label, str):
             self.match_subsumer_label = str(self.match_subsumer_label)
 
-        if self.similarity is not None and not isinstance(self.similarity, TermPairwiseSimilarity):
-            self.similarity = TermPairwiseSimilarity(**as_dict(self.similarity))
-
         super().__post_init__(**kwargs)
 
 
 # Enumerations
 
 
 # Slots
@@ -677,15 +683,15 @@
 
 slots.bestMatch__score = Slot(
     uri=SIM.score,
     name="bestMatch__score",
     curie=SIM.curie("score"),
     model_uri=SIM.bestMatch__score,
     domain=None,
-    range=Optional[float],
+    range=float,
 )
 
 slots.bestMatch__match_subsumer = Slot(
     uri=SIM.match_subsumer,
     name="bestMatch__match_subsumer",
     curie=SIM.curie("match_subsumer"),
     model_uri=SIM.bestMatch__match_subsumer,
@@ -704,9 +710,9 @@
 
 slots.bestMatch__similarity = Slot(
     uri=SIM.similarity,
     name="bestMatch__similarity",
     curie=SIM.curie("similarity"),
     model_uri=SIM.bestMatch__similarity,
     domain=None,
-    range=Optional[Union[dict, TermPairwiseSimilarity]],
+    range=Union[dict, TermPairwiseSimilarity],
 )
```

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/similarity.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/similarity.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-id: https://w3id.org/linkml/similarity
+id: https://w3id.org/oak/similarity
 title: Semantic Similarity
 name: similarity
 description: >-
   A datamodel for representing semantic similarity between terms or lists of terms.
 license: https://creativecommons.org/publicdomain/zero/1.0/
 
 prefixes:
@@ -213,12 +213,12 @@
     range: BestMatch
     multivalued: true
     inlined: true
   metric:
     range: uriorcurie
   average_score:
     range: float
-    required: true
+    required: false
   best_score:
     range: float
-    required: true
+    required: false
```

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/summary_statistics_datamodel.py` & `oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Auto generated from summary_statistics_datamodel.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-01-29T12:10:35
+# Generation date: 2023-04-09T15:53:54
 # Schema: summary-statistics
 #
-# id: https://w3id.org/oaklib/summary_statistics
+# id: https://w3id.org/oak/summary_statistics
 # description: A datamodel for reports on data
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
 import re
 import sys
 from dataclasses import dataclass
```

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/summary_statistics_datamodel.schema.json` & `oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/summary_statistics_datamodel.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-id: https://w3id.org/oaklib/summary_statistics
+id: https://w3id.org/oak/summary_statistics
 title: Summary Statistics Datamodel
 name: summary-statistics
 description: A datamodel for reports on data
 license: https://creativecommons.org/publicdomain/zero/1.0/
 
 prefixes:
   linkml: https://w3id.org/linkml/
```

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/taxon_constraints.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/taxon_constraints.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/taxon_constraints.py` & `oaklib-0.5.0/src/oaklib/datamodels/taxon_constraints.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Auto generated from taxon_constraints.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-03-24T10:02:05
+# Generation date: 2023-04-09T15:54:03
 # Schema: taxon-constraints
 #
-# id: https://w3id.org/linkml/taxon_constraints
+# id: https://w3id.org/oak/taxon_constraints
 # description: A datamodel for representing inferred and asserted taxon constraints.
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
 import re
 import sys
 from dataclasses import dataclass
```

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/taxon_constraints.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/taxon_constraints.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-id: https://w3id.org/linkml/taxon_constraints
+id: https://w3id.org/oak/taxon_constraints
 title: Taxon Constraints Reporting Datamodel
 name: taxon-constraints
 description: >-
   A datamodel for representing inferred and asserted taxon constraints.
 license: https://creativecommons.org/publicdomain/zero/1.0/
 
 prefixes:
```

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/text_annotator.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/text_annotator.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/text_annotator.py` & `oaklib-0.5.0/src/oaklib/datamodels/text_annotator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Auto generated from text_annotator.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-01-24T17:05:32
+# Generation date: 2023-04-09T15:53:59
 # Schema: text-annotator
 #
-# id: https://w3id.org/linkml/text_annotator
+# id: https://w3id.org/oak/text_annotator
 # description: A datamodel for representing the results of textual named entity recognition annotation results.
 #              This draws upon both SSSOM and https://www.w3.org/TR/annotation-model/
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
 import re
 import sys
```

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/text_annotator.schema.json` & `oaklib-0.5.0/src/oaklib/datamodels/text_annotator.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/text_annotator.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/text_annotator.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-id: https://w3id.org/linkml/text_annotator
+id: https://w3id.org/oak/text_annotator
 title: Text Annotator Datamodel
 name: text-annotator
 description: >-
   A datamodel for representing the results of textual named entity recognition annotation results.
   This draws upon both SSSOM and https://www.w3.org/TR/annotation-model/
 license: https://creativecommons.org/publicdomain/zero/1.0/
 see_also:
```

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/validation_datamodel.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/validation_datamodel.py` & `oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/validation_datamodel.schema.json` & `oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/validation_datamodel.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/value_set_configuration.owl.ttl` & `oaklib-0.5.0/src/oaklib/datamodels/value_set_configuration.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/value_set_configuration.py` & `oaklib-0.5.0/src/oaklib/datamodels/value_set_configuration.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/value_set_configuration.yaml` & `oaklib-0.5.0/src/oaklib/datamodels/value_set_configuration.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/datamodels/vocabulary.py` & `oaklib-0.5.0/src/oaklib/datamodels/vocabulary.py`

 * *Files 7% similar despite different names*

```diff
@@ -58,14 +58,15 @@
 OWL_DATATYPE_PROPERTY = "owl:DatatypeProperty"
 OWL_ANNOTATION_PROPERTY = "owl:AnnotationProperty"
 OWL_TRANSITIVE_PROPERTY = "owl:TransitiveProperty"
 OWL_SYMMETRIC_PROPERTY = "owl:SymmetricProperty"
 OWL_THING = "owl:Thing"
 OWL_NOTHING = "owl:Nothing"
 IS_DEFINED_BY = "rdfs:isDefinedBy"
+RDFS_COMMENT = "rdfs:comment"
 SUBCLASS_OF = omd.slots.subClassOf.curie
 IS_A = omd.slots.subClassOf.curie
 DISJOINT_WITH = "owl:disjointWith"
 SUBPROPERTY_OF = "rdfs:subPropertyOf"
 RDFS_DOMAIN = "rdfs:domain"
 RDFS_RANGE = "rdfs:range"
 INVERSE_OF = "owl:inverseOf"
@@ -80,14 +81,18 @@
     OWL_NAMED_INDIVIDUAL,
     OWL_DATATYPE_PROPERTY,
     OWL_ANNOTATION_PROPERTY,
     OWL_TRANSITIVE_PROPERTY,
     OWL_SYMMETRIC_PROPERTY,
 ]
 
+DCTERMS_LANGUAGE = "dcterms:language"
+PROTEGE_PREFERRED_LANGUAGE = "protege:preferredLanguage"
+ONTOLOGY_LEVEL_LANGUAGE_INDICATORS = [DCTERMS_LANGUAGE, PROTEGE_PREFERRED_LANGUAGE]
+
 STANDARD_ANNOTATION_PROPERTIES = [
     TERM_REPLACED_BY,
     CONSIDER_REPLACEMENT,
     DEPRECATED_PREDICATE,
     HAS_OBSOLESCENCE_REASON,
     TERMS_MERGED,
     HAS_ONTOLOGY_ROOT_TERM,
```

### Comparing `oaklib-0.4.1/src/oaklib/implementations/__init__.py` & `oaklib-0.5.0/src/oaklib/implementations/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """
 This package serves as the master index for all implementations.
 """
 from functools import cache
 
 from class_resolver import ClassResolver
 
+from oaklib.implementations.aggregator.aggregator_implementation import (
+    AggregatorImplementation,
+)
 from oaklib.implementations.cx.cx_implementation import CXImplementation
 from oaklib.implementations.funowl.funowl_implementation import FunOwlImplementation
 from oaklib.implementations.gilda import GildaImplementation
 from oaklib.implementations.kgx.kgx_implementation import KGXImplementation
 from oaklib.implementations.ols import (
     BaseOlsImplementation,
     OlsImplementation,
@@ -50,14 +53,15 @@
     WikidataImplementation,
 )
 from oaklib.interfaces import OntologyInterface
 
 __all__ = [
     "get_implementation_resolver",
     # Concrete classes
+    "AggregatorImplementation",
     "AgroPortalImplementation",
     "BioPortalImplementation",
     "CXImplementation",
     "EcoPortalImplementation",
     "MatPortalImplementation",
     "OlsImplementation",
     "TIBOlsImplementation",
```

### Comparing `oaklib-0.4.1/src/oaklib/implementations/aggregator/aggregator_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/aggregator/aggregator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/cx/cx_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/cx/cx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/funowl/funowl_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/funowl/funowl_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     DEPRECATED_PREDICATE,
     HAS_DEFINITION_CURIE,
     HAS_EXACT_SYNONYM,
     IS_A,
     LABEL_PREDICATE,
 )
 from oaklib.interfaces import SearchInterface
+from oaklib.interfaces.basic_ontology_interface import LANGUAGE_TAG
 from oaklib.interfaces.owl_interface import OwlInterface, ReasonerConfiguration
 from oaklib.interfaces.patcher_interface import PatcherInterface
 from oaklib.types import CURIE, PRED_CURIE
 
 
 @dataclass
 class FunOwlImplementation(OwlInterface, PatcherInterface, SearchInterface):
@@ -75,18 +76,18 @@
             val = labels[0]
             rdf_v = val.to_rdf(self.functional_writer.g)
             if isinstance(rdf_v, rdflib.Literal):
                 return rdf_v.value
             else:
                 raise ValueError(f"Label must be literal, not {val}")
 
-    def definition(self, curie: CURIE) -> Optional[str]:
+    def definition(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> Optional[str]:
         return self._single_valued_assignment(curie, HAS_DEFINITION_CURIE)
 
-    def label(self, curie: CURIE) -> str:
+    def label(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> str:
         labels = [
             a.value for a in self.annotation_assertion_axioms(curie, property=LABEL_PREDICATE)
         ]
         if labels:
             if len(labels) > 1:
                 logging.warning(f"Multiple labels for {curie} = {labels}")
             label = labels[0]
```

### Comparing `oaklib-0.4.1/src/oaklib/implementations/gilda.py` & `oaklib-0.5.0/src/oaklib/implementations/gilda.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/kgx/kgx_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/kgx/kgx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/obograph/obograph_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/obograph/obograph_implementation.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     LABEL_PREDICATE,
     OWL_CLASS,
     OWL_OBJECT_PROPERTY,
     SUBPROPERTY_OF,
 )
 from oaklib.interfaces.basic_ontology_interface import (
     ALIAS_MAP,
+    LANGUAGE_TAG,
     RELATIONSHIP,
     RELATIONSHIP_MAP,
 )
 from oaklib.interfaces.differ_interface import DifferInterface
 from oaklib.interfaces.dumper_interface import DumperInterface
 from oaklib.interfaces.merge_interface import MergeInterface
 from oaklib.interfaces.obograph_interface import OboGraphInterface
@@ -223,22 +224,26 @@
     def subset_members(self, subset: SUBSET_CURIE) -> Iterable[CURIE]:
         od = self.obograph_document
         for g in od.graphs:
             for n in g.nodes:
                 if subset in self._node_subsets(n):
                     yield n
 
-    def label(self, curie: CURIE) -> Optional[str]:
+    def label(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> Optional[str]:
+        if lang:
+            raise NotImplementedError("Language tags not supported")
         if curie == IS_A:
             return "subClassOf"
         n = self._node(curie)
         if n:
             return n.lbl
 
-    def set_label(self, curie: CURIE, label: str) -> bool:
+    def set_label(self, curie: CURIE, label: str, lang: Optional[LANGUAGE_TAG] = None) -> bool:
+        if lang:
+            raise NotImplementedError("Language tags not supported")
         n = self._node(curie, True)
         n.lbl = label
         return True
 
     def curies_by_label(self, label: str) -> List[CURIE]:
         return [self.uri_to_curie(n.id) for n in self._nodes() if n.lbl == label]
 
@@ -253,15 +258,17 @@
         g = self._entire_graph()
         g.nodes.append(Node(curie, lbl=label, type=type))
         for p, objs in relationships:
             for obj in objs:
                 g.edges.append(Edge(curie, p, obj))
         return curie
 
-    def definition(self, curie: CURIE) -> Optional[str]:
+    def definition(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> Optional[str]:
+        if lang:
+            raise NotImplementedError("Language tags not supported")
         m = self._meta(curie)
         if m:
             return m.definition.val
 
     def comments(self, curies: Iterable[CURIE]) -> Iterable[Tuple[CURIE, str]]:
         for curie in curies:
             m = self._meta(curie)
```

### Comparing `oaklib-0.4.1/src/oaklib/implementations/ols/ols_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/ols/ols_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/ols/oxo_utils.py` & `oaklib-0.5.0/src/oaklib/implementations/ols/oxo_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/ontobee/ontobee_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/ontobee/ontobee_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/ontoportal/bioportal_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/ontoportal/bioportal_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py` & `oaklib-0.5.0/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/pronto/pronto_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/pronto/pronto_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -43,14 +43,15 @@
     SKOS_CLOSE_MATCH,
     TERM_REPLACED_BY,
     TERMS_MERGED,
 )
 from oaklib.interfaces import TextAnnotatorInterface
 from oaklib.interfaces.basic_ontology_interface import (
     ALIAS_MAP,
+    LANGUAGE_TAG,
     METADATA_MAP,
     PRED_CURIE,
     RELATIONSHIP,
     RELATIONSHIP_MAP,
 )
 from oaklib.interfaces.class_enrichment_calculation_interface import (
     ClassEnrichmentCalculationInterface,
@@ -359,25 +360,25 @@
                 yield subset
 
     def subset_members(self, subset: SUBSET_CURIE) -> Iterable[CURIE]:
         for t in self.wrapped_ontology.terms():
             if subset in t.subsets:
                 yield t.id
 
-    def label(self, curie: CURIE) -> str:
+    def label(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> str:
         t = self._entity(curie)
         if t:
             return t.name
         else:
             if curie == IS_A:
                 return "subClassOf"
             else:
                 return None
 
-    def set_label(self, curie: CURIE, label: str) -> bool:
+    def set_label(self, curie: CURIE, label: str, lang: Optional[LANGUAGE_TAG] = None) -> bool:
         t = self._entity(curie)
         if t:
             curr = t.name
             if curr != label:
                 t.name = label
                 return True
             else:
@@ -468,15 +469,15 @@
         if not predicate or predicate == IS_A:
             t.superclasses().remove(filler_term)
         else:
             predicate_term = self._create_pred(predicate)
             t.relationships[predicate_term].remove(filler_term)
         self._clear_relationship_index()
 
-    def definition(self, curie: CURIE) -> Optional[str]:
+    def definition(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> Optional[str]:
         e = self._entity(curie)
         return e.definition if e else None
 
     def comments(self, curies: Iterable[CURIE]) -> Iterable[Tuple[CURIE, str]]:
         for curie in curies:
             e = self._entity(curie)
             if e:
```

### Comparing `oaklib-0.4.1/src/oaklib/implementations/simpleobo/simple_obo_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/simpleobo/simple_obo_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -86,14 +86,15 @@
     Stanza,
     _synonym_scope_pred,
     parse_obo_document,
 )
 from oaklib.interfaces import TextAnnotatorInterface
 from oaklib.interfaces.basic_ontology_interface import (
     ALIAS_MAP,
+    LANGUAGE_TAG,
     METADATA_MAP,
     RELATIONSHIP,
     RELATIONSHIP_MAP,
 )
 from oaklib.interfaces.differ_interface import DifferInterface
 from oaklib.interfaces.dumper_interface import DumperInterface
 from oaklib.interfaces.mapping_provider_interface import MappingProviderInterface
@@ -316,27 +317,32 @@
             alt_curie = self.map_curie_to_shorthand(curie)
             if alt_curie and alt_curie != curie:
                 stanza = self.obo_document.stanzas.get(alt_curie)
         if strict and not stanza:
             raise ValueError(f"No such stanza {curie}")
         return stanza
 
-    def label(self, curie: CURIE) -> Optional[str]:
+    def label(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> Optional[str]:
+        if lang:
+            raise NotImplementedError("Language tags not supported")
         s = self._stanza(curie, False)
         if s:
             return s.singular_value(TAG_NAME)
         else:
             if curie == IS_A:
                 return "subClassOf"
             else:
                 return None
 
-    def set_label(self, curie: CURIE, label: str) -> bool:
+    def set_label(self, curie: CURIE, label: str, lang: Optional[LANGUAGE_TAG] = None) -> bool:
+        if lang:
+            raise NotImplementedError("Language tags not supported")
         s = self._stanza(curie, False)
         s.set_singular_tag(TAG_NAME, label)
+        return True
 
     def curies_by_label(self, label: str) -> List[CURIE]:
         return [
             s.id
             for s in self.obo_document.stanzas.values()
             if s.singular_value(TAG_NAME, False) == label
         ]
@@ -391,15 +397,15 @@
         if not predicate or predicate == IS_A:
             t.remove_simple_tag_value(TAG_IS_A, filler)
         else:
             predicate_code = self.map_curie_to_shorthand(predicate)
             t.remove_pairwise_tag_value(TAG_RELATIONSHIP, predicate_code, filler)
         self._clear_relationship_index()
 
-    def definition(self, curie: CURIE) -> Optional[str]:
+    def definition(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> Optional[str]:
         s = self._stanza(curie, strict=False)
         if s:
             return s.quoted_value(TAG_DEFINITION)
 
     def comments(self, curies: Iterable[CURIE]) -> Iterable[Tuple[CURIE, str]]:
         for curie in curies:
             s = self._stanza(curie)
```

### Comparing `oaklib-0.4.1/src/oaklib/implementations/simpleobo/simple_obo_parser.py` & `oaklib-0.5.0/src/oaklib/implementations/simpleobo/simple_obo_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -90,14 +90,17 @@
     TAG_IS_OBSOLETE,
     TAG_REPLACED_BY,
     TAG_CONSIDER,
     TAG_CREATED_BY,
     TAG_CREATION_DATE,
 ]
 
+OBO_TERM = "Term"
+OBO_TYPEDEF = "Typedef"
+
 
 def _parse_list(as_str: str) -> List[str]:
     if as_str == "":
         return []
     return as_str.split(", ")
 
 
@@ -592,17 +595,33 @@
 
     def order_stanzas(self) -> None:
         """
         Orders stanzas by ID
 
         Does not change tag-value ordering within stanzas
         """
-        stanzas = self.stanzas.values()
-        stanzas = sorted(stanzas, key=lambda x: x.id)
-        self.stanzas = {s.id: s for s in stanzas}
+        term_stanzas = {
+            curie: stanza
+            for curie, stanza in self.stanzas.items()
+            if self.stanzas[curie].type == OBO_TERM
+        }
+        typedef_stanzas = {
+            curie: stanza
+            for curie, stanza in self.stanzas.items()
+            if self.stanzas[curie].type == OBO_TYPEDEF
+        }
+        sorted_term_stanzas = self._sort_stanzas(term_stanzas)
+        sorted_typedef_stanzas = self._sort_stanzas(typedef_stanzas)
+
+        self.stanzas = {s.id: s for s in sorted_term_stanzas}
+        self.stanzas.update({s.id: s for s in sorted_typedef_stanzas})
+
+    def _sort_stanzas(self, stanzas: Mapping[CURIE, Stanza]) -> Mapping[CURIE, Stanza]:
+        values = stanzas.values()
+        return sorted(values, key=lambda x: x.id)
 
     def normalize_line_order(self) -> None:
         """
         Normalizes line order within stanzas
         """
         for s in self.stanzas.values():
             s.normalize_order()
```

### Comparing `oaklib-0.4.1/src/oaklib/implementations/sparql/abstract_sparql_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/sparql/abstract_sparql_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     SEMAPV,
     SYNONYM_PREDICATES,
 )
 from oaklib.implementations.sparql import SEARCH_CONFIG
 from oaklib.implementations.sparql.sparql_query import SparqlQuery, SparqlUpdate
 from oaklib.interfaces.basic_ontology_interface import (
     ALIAS_MAP,
+    LANGUAGE_TAG,
     METADATA_MAP,
     PRED_CURIE,
     PREFIX_MAP,
     RELATIONSHIP,
     RELATIONSHIP_MAP,
 )
 from oaklib.interfaces.dumper_interface import DumperInterface
@@ -384,15 +385,15 @@
             yield self._triple_as_curies(t)
 
     def all_rdflib_triples(self) -> Iterator[RDF_TRIPLE]:
         if not self.graph:
             raise NotImplementedError("Not implemented for SPARQL endpoints")
         yield from self.graph.triples((None, None, None))
 
-    def hierararchical_parents(self, curie: CURIE, isa_only: bool = False) -> List[CURIE]:
+    def hierarchical_parents(self, curie: CURIE, isa_only: bool = False) -> List[CURIE]:
         uri = self.curie_to_uri(curie)
         is_a_pred = (
             self.ontology_metamodel_mapper.is_a_uri()
             if self.ontology_metamodel_mapper
             else RDFS.subClassOf
         )
         query = SparqlQuery(
@@ -421,15 +422,15 @@
             pred_quris = [self.ontology_metamodel_mapper.direct_map_uri(p) for p in pred_quris]
         uri = self.curie_to_uri(curie)
         is_a_pred = (
             self.ontology_metamodel_mapper.is_a_curie() if self.ontology_metamodel_mapper else IS_A
         )
         if not predicates or is_a_pred in predicates:
             # all simple is-a relationships
-            for p in self.hierararchical_parents(curie):
+            for p in self.hierarchical_parents(curie):
                 yield IS_A, p
         if not predicates or predicates != [is_a_pred]:
             # subclassof existential restrictions
             query = SparqlQuery(
                 select=["?p", "?o"],
                 where=[
                     f"<{uri}> <{RDFS.subClassOf}> [owl:onProperty ?p ; owl:someValuesFrom ?o]",
@@ -532,24 +533,30 @@
         pred = self.curie_to_sparql(pred)
         query = SparqlQuery(select=["?v"], where=[f"{uri} {pred} ?v"])
         if self.multilingual:
             query.where.append(f'FILTER (LANG(?v) = "{self.preferred_language}")')
         bindings = self._sparql_query(query)
         return list(set([row[VAL_VAR]["value"] for row in bindings]))
 
-    def label(self, curie: CURIE):
+    def label(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None):
+        if lang:
+            raise NotImplementedError("Language selection not implemented yet")
         labels = list(self.labels([curie]))
         if labels:
             if len(labels) > 1:
                 logging.warning(f"Multiple labels for {curie} = {labels}")
             return labels[0][1]
         else:
             return None
 
-    def labels(self, curies: Iterable[CURIE], allow_none=True) -> Iterable[Tuple[CURIE, str]]:
+    def labels(
+        self, curies: Iterable[CURIE], allow_none=True, lang: Optional[LANGUAGE_TAG] = None
+    ) -> Iterable[Tuple[CURIE, str]]:
+        if lang:
+            raise NotImplementedError("Language selection not implemented yet")
         label_uri = self._label_uri()
         uris = [self.curie_to_sparql(x) for x in curies]
         query = SparqlQuery(
             select=["?s ?label"], where=[f"?s <{label_uri}> ?label", _sparql_values("s", uris)]
         )
         if self.multilingual:
             query.where.append(f'FILTER (LANG(?label) = "{self.preferred_language}")')
@@ -629,22 +636,27 @@
         clauses_j = " UNION ".join([f"{{ {c} }}" for c in clauses])
         query = SparqlQuery(select=["?s"], where=[f"{{ {clauses_j} }}"])
         logging.info(f"Query = {query.query_str()}")
         bindings = self._sparql_query(query)
         return [self.uri_to_curie(row["s"]["value"]) for row in bindings]
 
     def create_entity(
-        self, curie: CURIE, label: str = None, relationships: RELATIONSHIP_MAP = None
+        self,
+        curie: CURIE,
+        label: str = None,
+        relationships: RELATIONSHIP_MAP = None,
+        replace=False,
+        **kwargs,
     ) -> CURIE:
         raise NotImplementedError
 
     def add_relationship(self, curie: CURIE, predicate: PRED_CURIE, filler: CURIE):
         raise NotImplementedError
 
-    def definition(self, curie: CURIE) -> Optional[str]:
+    def definition(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> Optional[str]:
         # TODO: allow this to be configured to use different predicates
         defn_uri = self._definition_uri()
         labels = self._get_anns(curie, defn_uri)
         if labels:
             if len(labels) > 1:
                 logging.error(f"Multiple labels for {curie} = {labels}")
             return labels[0]
```

### Comparing `oaklib-0.4.1/src/oaklib/implementations/sparql/lov_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/sparql/lov_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/sparql/oak_metamodel_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/sparql/oak_metamodel_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/sparql/sparql_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/sparql/sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/sparql/sparql_query.py` & `oaklib-0.5.0/src/oaklib/implementations/sparql/sparql_query.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/sqldb/sql_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/sqldb/sql_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,16 +97,18 @@
     LABEL_PREDICATE,
     OBSOLETION_RELATIONSHIP_PREDICATES,
     OWL_CLASS,
     OWL_META_CLASSES,
     OWL_NAMED_INDIVIDUAL,
     OWL_NOTHING,
     OWL_THING,
+    OWL_VERSION_IRI,
     PREFIX_PREDICATE,
     RDF_TYPE,
+    RDFS_COMMENT,
     RDFS_DOMAIN,
     RDFS_RANGE,
     SEMAPV,
     STANDARD_ANNOTATION_PROPERTIES,
     SUBPROPERTY_OF,
     SYNONYM_PREDICATES,
     TERM_REPLACED_BY,
@@ -114,14 +116,15 @@
     omd_slots,
 )
 from oaklib.implementations.sqldb import SEARCH_CONFIG
 from oaklib.interfaces import SubsetterInterface, TextAnnotatorInterface
 from oaklib.interfaces.basic_ontology_interface import (
     ALIAS_MAP,
     DEFINITION,
+    LANGUAGE_TAG,
     METADATA_MAP,
     PRED_CURIE,
     PREFIX_MAP,
     RELATIONSHIP,
     BasicOntologyInterface,
 )
 from oaklib.interfaces.class_enrichment_calculation_interface import (
@@ -377,14 +380,19 @@
         return has_view
 
     def prefix_map(self) -> PREFIX_MAP:
         if self._prefix_map is None:
             self._prefix_map = {row.prefix: row.base for row in self.session.query(Prefix)}
         return self._prefix_map
 
+    def languages(self) -> Iterable[LANGUAGE_TAG]:
+        for row in self.session.query(Statements.language).distinct():
+            if row.language:
+                yield row.language
+
     def entities(self, filter_obsoletes=True, owl_type=None) -> Iterable[CURIE]:
         # TODO: figure out how to pass through ESCAPE at SQL Alchemy level
         # s = text('SELECT id FROM class_node WHERE id NOT LIKE "\_:%" ESCAPE "\\"')  # noqa W605
         q = self.session.query(Node)
         if owl_type:
             subquery = self.session.query(RdfTypeStatement.subject).filter(
                 RdfTypeStatement.object == owl_type
@@ -427,57 +435,143 @@
         for row in q:
             yield row.subject, row.predicate, row.object if row.object else row.value
 
     def all_relationships(self) -> Iterable[RELATIONSHIP]:
         for row in self.session.query(Edge):
             yield row.subject, row.predicate, row.object
 
-    def label(self, curie: CURIE) -> Optional[str]:
+    def _add_language_filter(self, q, lang, typ: Type[Statements] = Statements):
+        if lang:
+            if not self.multilingual:
+                logging.warning(
+                    f"Source does not appear to be multilingual, filtering by @{lang} may not work"
+                )
+            if lang == self.default_language:
+                q = q.filter(typ.language.is_(None))
+            else:
+                q = q.filter(typ.language == lang)
+        return q
+
+    def label(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> Optional[str]:
         q = self.session.query(RdfsLabelStatement.value).filter(RdfsLabelStatement.subject == curie)
+        q = self._add_language_filter(q, lang, RdfsLabelStatement)
         for (lbl,) in q:
             return lbl
+        if lang and lang != self.default_language:
+            return self.label(curie, lang=self.default_language)
 
-    def labels(self, curies: Iterable[CURIE], allow_none=True) -> Iterable[Tuple[CURIE, str]]:
+    def labels(
+        self, curies: Iterable[CURIE], allow_none=True, lang: LANGUAGE_TAG = None
+    ) -> Iterable[Tuple[CURIE, str]]:
         for curie_it in chunk(curies, self.max_items_for_in_clause):
             curr_curies = list(curie_it)
 
             has_label = set()
-            for row in self.session.query(RdfsLabelStatement).filter(
+            q = self.session.query(RdfsLabelStatement).filter(
                 RdfsLabelStatement.subject.in_(tuple(curr_curies))
-            ):
+            )
+            q = self._add_language_filter(q, lang, RdfsLabelStatement)
+            for row in q:
                 yield row.subject, row.value
-                if allow_none:
-                    has_label.add(row.subject)
+                has_label.add(row.subject)
+            if lang and lang != self.default_language:
+                # fill missing
+                curies_with_no_labels = set(curr_curies) - has_label
+                yield from self.labels(curies_with_no_labels, allow_none=allow_none, lang=None)
+                allow_none = False
             if allow_none:
                 for curie in curr_curies:
                     if curie not in has_label:
                         yield curie, None
 
+    def multilingual_labels(
+        self, curies: Iterable[CURIE], allow_none=True, langs: Optional[List[LANGUAGE_TAG]] = None
+    ) -> Iterable[Tuple[CURIE, str, LANGUAGE_TAG]]:
+        if isinstance(curies, str):
+            logging.warning(f"multilingual_labels called with a single curie: {curies}")
+            curies = [curies]
+        for curie_it in chunk(curies, self.max_items_for_in_clause):
+            curr_curies = list(curie_it)
+
+            has_label = defaultdict(set)
+            q = self.session.query(RdfsLabelStatement).filter(
+                RdfsLabelStatement.subject.in_(tuple(curr_curies))
+            )
+            if langs is not None:
+                if self.default_language in langs:
+                    q = q.filter(
+                        or_(
+                            RdfsLabelStatement.language.is_(None),
+                            RdfsLabelStatement.language.in_(langs),
+                        )
+                    )
+                else:
+                    q = q.filter(RdfsLabelStatement.language.in_(langs))
+            for row in q:
+                yield row.subject, row.value, row.language
+                if allow_none:
+                    has_label[row.subject].add(row.language)
+            if allow_none:
+                for curie in curr_curies:
+                    if curie not in has_label:
+                        yield curie, None, None
+
     def curies_by_label(self, label: str) -> List[CURIE]:
         q = self.session.query(RdfsLabelStatement.subject)
         q = q.filter(RdfsLabelStatement.value == label)
         return list(set([row.subject for row in q]))
 
     def entity_alias_map(self, curie: CURIE) -> ALIAS_MAP:
         m = defaultdict(list)
         m[LABEL_PREDICATE] = [self.label(curie)]
         for row in self.session.query(HasSynonymStatement).filter(
             HasSynonymStatement.subject == curie
         ):
             m[row.predicate].append(row.value)
         return m
 
-    def definition(self, curie: CURIE) -> Optional[str]:
-        for row in self.session.query(HasTextDefinitionStatement).filter(
+    def comments(
+        self, curies: Iterable[CURIE], allow_none=True, lang: LANGUAGE_TAG = None
+    ) -> Iterable[Tuple[CURIE, str]]:
+        for curie_it in chunk(curies, self.max_items_for_in_clause):
+            curr_curies = list(curie_it)
+
+            has_comment = set()
+            q = self.session.query(Statements).filter(Statements.subject.in_(tuple(curr_curies)))
+            q = q.filter(Statements.predicate == RDFS_COMMENT)
+            q = self._add_language_filter(q, lang, Statements)
+            for row in q:
+                yield row.subject, row.value
+                has_comment.add(row.subject)
+            if lang and lang != self.default_language:
+                # fill missing
+                curies_with_no_labels = set(curr_curies) - has_comment
+                yield from self.labels(curies_with_no_labels, allow_none=allow_none, lang=None)
+                allow_none = False
+            if allow_none:
+                for curie in curr_curies:
+                    if curie not in has_comment:
+                        yield curie, None
+
+    def definition(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> Optional[str]:
+        q = self.session.query(HasTextDefinitionStatement.value).filter(
             HasTextDefinitionStatement.subject == curie
-        ):
-            return row.value
+        )
+        q = self._add_language_filter(q, lang, HasTextDefinitionStatement)
+        for (lbl,) in q:
+            return lbl
+        if lang and lang != self.default_language:
+            return self.definition(curie, lang=self.default_language)
 
     def definitions(
-        self, curies: Iterable[CURIE], include_metadata=False, include_missing=False
+        self,
+        curies: Iterable[CURIE],
+        include_metadata=False,
+        include_missing=False,
+        lang: Optional[LANGUAGE_TAG] = None,
     ) -> Iterator[DEFINITION]:
         curies = list(curies)
         has_definition = set()
         metadata_map: Dict[Tuple[str, Optional[str]], METADATA_MAP] = defaultdict(dict)
         if include_metadata:
             # definition metadata may be axiom annotations
             for aa in self._axiom_annotations_multi(curies, predicate=HAS_DEFINITION_CURIE):
@@ -496,22 +590,28 @@
                 # note that direct annotation is unable to distinguish between multiple definitions;
                 # set to match all
                 k = (row.subject, None)
                 metadata = metadata_map[k]
                 if row.predicate not in metadata:
                     metadata[row.predicate] = []
                 metadata[row.predicate].append(row.value if row.value else row.object)
-        for row in self.session.query(HasTextDefinitionStatement).filter(
+        q = self.session.query(HasTextDefinitionStatement).filter(
             HasTextDefinitionStatement.subject.in_(curies)
-        ):
+        )
+        q = self._add_language_filter(q, lang, HasTextDefinitionStatement)
+        curr_curies = list(curies)
+        for row in q:
             reification_metadata = metadata_map.get((row.subject, row.value), {})
             direct_metadata = metadata_map.get((row.subject, None), {})
             yield row.subject, row.value, {**reification_metadata, **direct_metadata}
-            if include_missing:
-                has_definition.add(row.subject)
+            has_definition.add(row.subject)
+        if lang and lang != self.default_language:
+            # fill missing
+            curies_with_no_defs = set(curr_curies) - has_definition
+            yield from self.definitions(curies_with_no_defs, lang=None)
         if include_missing:
             for curie in curies:
                 if curie not in has_definition:
                     yield curie, None, None
 
     def _definitions_with_metadata(
         self, curies: Iterable[CURIE], include_missing=False
@@ -554,14 +654,20 @@
         self.add_missing_property_values(curie, m)
         return dict(m)
 
     def ontologies(self) -> Iterable[CURIE]:
         for row in self.session.query(OntologyNode):
             yield row.id
 
+    def ontology_versions(self, ontology: CURIE) -> Iterable[str]:
+        q = self.session.query(RdfsLabelStatement).filter(RdfsLabelStatement.subject == ontology)
+        q = q.filter(RdfsLabelStatement.predicate == OWL_VERSION_IRI)
+        for row in q:
+            yield row.object
+
     def ontology_metadata_map(self, ontology: CURIE) -> METADATA_MAP:
         return self.entity_metadata_map(ontology, include_all_triples=True)
 
     def _get_subset_curie(self, curie: str) -> str:
         if "#" in curie:
             return curie.split("#")[-1]
         else:
@@ -1263,14 +1369,19 @@
             q = q.filter(EntailedEdge.subject.in_(tuple(start_curies)))
         else:
             q = q.filter(EntailedEdge.subject == start_curies)
         if predicates is not None:
             q = q.filter(EntailedEdge.predicate.in_(tuple(predicates)))
         if not reflexive:
             q = q.filter(EntailedEdge.subject != EntailedEdge.object)
+        if reflexive:
+            if isinstance(start_curies, list):
+                yield from start_curies
+            else:
+                yield start_curies
         logging.debug(f"Ancestors query: {q}")
         for row in q:
             yield row.object
 
     def _multi_ancestors(
         self, start_curies: Union[CURIE, List[CURIE]], predicates: List[PRED_CURIE] = None
     ) -> Iterable[RELATIONSHIP]:
```

### Comparing `oaklib-0.4.1/src/oaklib/implementations/sqldb/sqlite_utils.py` & `oaklib-0.5.0/src/oaklib/implementations/sqldb/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/translator/translator_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/translator/translator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/ubergraph/ubergraph_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/ubergraph/ubergraph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/uniprot/uniprot_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/uniprot/uniprot_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/implementations/wikidata/wikidata_implementation.py` & `oaklib-0.5.0/src/oaklib/implementations/wikidata/wikidata_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/__init__.py` & `oaklib-0.5.0/src/oaklib/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/association_provider_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/association_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/basic_ontology_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/basic_ontology_interface.py`

 * *Files 18% similar despite different names*

```diff
@@ -77,18 +77,19 @@
     is intended to fit the "80% of uses" scenario - for more advanced uses, use one of the
     more specialized subclasses.
 
     For example, BasicOntologyInterface exposes a simple model of synonyms as aliases:
 
     >>> from oaklib import get_adapter
     >>> adapter = get_adapter('tests/input/go-nucleus.db')
-    >>> for alias in adapter.aliases("GO:0005634"):
+    >>> for alias in sorted(adapter.entity_aliases("GO:0005634")):
     ...     print(alias)
     cell nucleus
     horsetail nucleus
+    nucleus
 
     This omits metdata about the synonym, such as the predicate, source, and type.
     For this more granular view, the :ref:`obograph_interface` can be used.
 
     Basic concepts:
 
     - An ontology is a collection of entities
@@ -130,19 +131,15 @@
     in which case URIs may be used
 
     """
 
     strict: bool = False
     """Raise exceptions when entities not found in ID-based lookups"""
 
-    multilingual: bool = None
-    """True if the ontology is multilingual, and may provide alterntive primary labels"""
-
-    preferred_language: LANGUAGE_TAG = field(default_factory=lambda: "en")
-    """The preferred language for labels and other lexical entities"""
+    _multilingual: bool = None
 
     autosave: bool = field(default_factory=lambda: True)
     """For adapters that wrap a transactional source (e.g sqlite), this controls
     whether results should be auto-committed after each operation"""
 
     exclude_owl_top_and_bottom: bool = field(default_factory=lambda: True)
     """Do not include owl:Thing or owl:Nothing"""
@@ -183,14 +180,20 @@
     def get_prefix_map(self) -> PREFIX_MAP:
         return self.prefix_map()
 
     @property
     def converter(self) -> curies.Converter:
         """Get a converter for this ontology interface's prefix map.
 
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> converter = adapter.converter
+        >>> print(converter.compress("http://purl.obolibrary.org/obo/GO_0005634"))
+        GO:0005634
+
         :return: A converter
         """
         if self._converter is None:
             self._converter = curies.Converter.from_prefix_map(self.prefix_map())
         return self._converter
 
     def set_metamodel_mappings(self, mappings: Union[str, Path, List[Mapping]]) -> None:
@@ -210,14 +213,19 @@
             mappings, curie_converter=self.converter
         )
 
     def curie_to_uri(self, curie: CURIE, strict: bool = False) -> Optional[URI]:
         """
         Expands a CURIE to a URI.
 
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> print(adapter.curie_to_uri("GO:0005634"))
+        http://purl.obolibrary.org/obo/GO_0005634
+
         :param curie:
         :param strict: (Default is False) if True, exceptions will be raised if curie cannot be expanded
         :return:
         """
         rv = self.converter.expand(curie)
         if rv is None and strict:
             prefix_map_text = "\n".join(
@@ -232,14 +240,19 @@
 
     def uri_to_curie(
         self, uri: URI, strict: bool = True, use_uri_fallback=False
     ) -> Optional[CURIE]:
         """
         Contracts a URI to a CURIE.
 
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> print(adapter.uri_to_curie("http://purl.obolibrary.org/obo/GO_0005634"))
+        GO:0005634
+
         If strict conditions hold, then no URI can map to more than one CURIE
         (i.e one URI base should not start with another).
 
         :param uri: URI
         :param strict: Boolean [default: True]
         :param use_uri_fallback: if cannot be contracted, use the URI as a CURIE proxy [default: True]
         :return: contracted URI, or original URI if no contraction possible
@@ -279,20 +292,110 @@
 
     def _clear_relationship_index(self):
         self._relationship_index_cache = None
 
     def _all_relationships(self) -> Iterator[RELATIONSHIP]:
         raise NotImplementedError
 
+    @property
+    def multilingual(self) -> bool:
+        """
+        Returns True if this ontology interface supports multilingual annotations.
+
+        This is by default inferred from the content of the ontology, if more than
+        one language tag is present. This is the case for the international version
+        of the HPO:
+
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/hp-international-test.db')
+        >>> adapter.multilingual
+        True
+
+        If no language tags are present, then this will return False:
+
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> adapter.multilingual
+        False
+
+        .. note ::
+
+            currently this is only implemented for the SQL backend.
+
+        :return: True if multilingual
+        """
+        if self._multilingual is None:
+            self._multilingual = len([x for x in self.languages()]) > 1
+        return self._multilingual
+
+    @multilingual.setter
+    def multilingual(self, value: bool):
+        self._multilingual = value
+
+    def languages(self) -> Iterable[LANGUAGE_TAG]:
+        """
+        Returns a list of languages explicitly supported by this ontology interface.
+
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/hp-international-test.db')
+        >>> for lang in sorted(adapter.languages()):
+        ...    print(lang)
+        cs
+        fr
+        nl
+        tr
+
+        :return: iterator of language tags
+        """
+        return iter([])
+
+    @property
+    def default_language(self) -> Optional[LANGUAGE_TAG]:
+        """
+        Returns the default language for this ontology interface.
+
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/hp-international-test.db')
+        >>> adapter.default_language
+        'en'
+
+        Note that here "default" has a particular meaning: it means that lexical elements
+        are MUST NOT be explicitly tagged with this language, and that it MUST be assumed that
+        a blank/empty/null language tag means that the default language is intended.
+
+        :return: language tag
+        """
+        return "en"
+
     def ontologies(self) -> Iterable[CURIE]:
         """
         Yields all known ontology CURIEs.
 
         Many OntologyInterfaces will wrap a single ontology, others will wrap multiple.
-        Even when a single ontology is wrapped, there may be multiple ontologies included as imports
+        Even when a single ontology is wrapped, there may be multiple ontologies included as imports.
+
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.owl.ttl')
+        >>> list(adapter.ontologies())
+        ['go.owl']
+
+        .. note ::
+
+            The payload for this method may change to return normalized ontology names such as 'go'
+
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('bioportal:')
+        >>> for ont in sorted(adapter.ontologies()):
+        ...     print(ont)
+        <BLANKLINE>
+        ...
+        GO
+        ...
+        UBERON
+        ...
 
         :return: iterator
         """
         raise NotImplementedError(
             f"ontologies() method not implemented for {self.__class__.__name__}"
         )
 
@@ -311,14 +414,15 @@
         Example:
 
         >>> from oaklib import get_adapter
         >>> adapter = get_adapter("sqlite:obo:cob")
         >>> for entity in adapter.obsoletes():
         ...     print(entity)
         <BLANKLINE>
+        ...
         COB:0000014
 
         In OWL, obsolete entities (aka deprecated entities) are those
         that have an ``owl:deprecated`` annotation with value "True"
 
         By default, *merged terms* are included. Merged terms are entities
         that are:
@@ -330,31 +434,38 @@
         In OBO Format, merged terms do not get their own stanza, but
         instead show up as ``alt_id`` tags on the replacement term.
 
         To exclude merged terms, set ``include_merged=False``:
 
         Example:
 
-        >>> for entity in ontology.obsoletes(include_merged=False):
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter("sqlite:obo:cob")
+        >>> for entity in adapter.obsoletes(include_merged=False):
         ...     print(entity)
+        <BLANKLINE>
+        ...
+        COB:0000014
 
         :param include_merged: If True, merged terms will be included
         :return: iterator over CURIEs
         """
         raise NotImplementedError
 
     def obsoletes_migration_relationships(
         self, entities: Iterable[CURIE]
     ) -> Iterable[RELATIONSHIP]:
         """
         Yields relationships between an obsolete entity and potential replacements.
 
         Example:
 
-        >>> for rel in ontology.obsoletes_migration_relationships(ontology.obsoletes()):
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter("sqlite:obo:cob")
+        >>> for rel in adapter.obsoletes_migration_relationships(adapter.obsoletes()):
         ...     print(rel)
 
         Obsoletion relationship predicates may be:
 
         - IAO:0100001 (term replaced by)
         - oboInOwl:consider
         - rdfs:seeAlso
@@ -371,48 +482,86 @@
     def all_obsolete_curies(self) -> Iterable[CURIE]:
         return self.obsoletes()
 
     def ontology_versions(self, ontology: CURIE) -> Iterable[str]:
         """
         Yields all version identifiers for an ontology.
 
+        .. warning ::
+
+            This method is not yet implemented for all OntologyInterface implementations.
+
         :param ontology:
         :return: iterator
         """
         raise NotImplementedError
 
     def ontology_metadata_map(self, ontology: CURIE) -> METADATA_MAP:
         """
         Property-values metadata map with metadata about an ontology.
 
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> for ont in adapter.ontologies():
+        ...     m = adapter.ontology_metadata_map(ont)
+        ...     m.get('schema:url')
+        ['http://purl.obolibrary.org/obo/go.owl']
+
         :param ontology:
         :return:
         """
         raise NotImplementedError(
             f"ontology_metadata_map() method not implemented for {self.__class__.__name__}"
         )
 
     def entities(self, filter_obsoletes=True, owl_type=None) -> Iterable[CURIE]:
         """
         Yields all known entity CURIEs.
 
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> for e in adapter.entities():
+        ...     print(e)
+        <BLANKLINE>
+        ...
+        GO:0005634
+        ...
+
+        >>> from oaklib import get_adapter
+        >>> from oaklib.datamodels.vocabulary import OWL_OBJECT_PROPERTY
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> for e in adapter.entities(owl_type=OWL_OBJECT_PROPERTY):
+        ...     print(e)
+        <BLANKLINE>
+        ...
+        BFO:0000051
+        ...
+
         :param filter_obsoletes: if True, exclude any obsolete/deprecated element
         :param owl_type: CURIE for RDF metaclass for the object, e.g. owl:Class
         :return: iterator
         """
         raise NotImplementedError
 
     @deprecated("Replaced by entities")
     def all_entity_curies(self, **kwargs) -> Iterable[CURIE]:
         return self.entities(**kwargs)
 
     def owl_types(self, entities: Iterable[CURIE]) -> Iterable[Tuple[CURIE, CURIE]]:
         """
         Yields all known OWL types for given entities.
 
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> for e, t in sorted(adapter.owl_types(['GO:0005634', 'BFO:0000050'])):
+        ...     print(e, t)
+        BFO:0000050 owl:ObjectProperty
+        BFO:0000050 owl:TransitiveProperty
+        GO:0005634 owl:Class
+
         The OWL type must either be the instantiated type as the RDFS level, e.g.
 
         - owl:Class
         - owl:ObjectProperty
         - owl:DatatypeProperty
         - owl:AnnotationProperty
         - owl:NamedIndividual
@@ -429,28 +578,38 @@
         """
         raise NotImplementedError
 
     def owl_type(self, entity: CURIE) -> List[CURIE]:
         """
         Get the OWL type for a given entity.
 
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> adapter.owl_type('GO:0005634')
+        ['owl:Class']
+
         Typically each entity will have a single OWL type, but in some cases
         an entity may have multiple OWL types. This is called "punning",
         see `Section 8.3<https://www.w3.org/TR/owl2-primer/#Entity_Declarations>` of
         the OWL primer
 
         :param entity:
         :return: CURIE
         """
         return [x[1] for x in self.owl_types([entity]) if x[1] is not None]
 
     def defined_by(self, entity: CURIE) -> Optional[str]:
         """
         Returns the CURIE of the ontology that defines the given entity.
 
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> adapter.defined_by('GO:0005634')
+        'GO'
+
         :param entity:
         :return:
         """
         for _, x in self.defined_bys([entity]):
             return x
 
     def defined_bys(self, entities: Iterable[CURIE]) -> Iterable[str]:
@@ -480,21 +639,43 @@
         filter_obsoletes=True,
         annotated_roots=False,
         id_prefixes: Optional[List[CURIE]] = None,
     ) -> Iterable[CURIE]:
         """
         Yields all entities without a parent.
 
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> for e in sorted(adapter.roots()):
+        ...     print(e)
+        <BLANKLINE>
+        ...
+        BFO:0000003
+        ...
+        OBI:0100026
+        ...
+
         Note that the concept of a "root" in an ontology can be ambiguous:
 
         - is the (trivial) owl:Thing included (OWL tautology)?
         - are we asking for the root of the is-a graph, or a subset of predicates?
         - do we include parents in imported/merged other ontologies (e.g. BFO)?
         - do we include obsolete nodes (which are typically singletons)?
 
+        Note also that the release OWL versions of many OBO ontologies may exhibit a certain
+        level of messiness with multiple roots.
+
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> for e in sorted(adapter.roots(id_prefixes=['GO'])):
+        ...     print(e, adapter.label(e))
+        GO:0003674 molecular_function
+        GO:0005575 cellular_component
+        GO:0008150 biological_process
+
         This method will yield entities that are not the subject of an edge, considering
         only edges with a given set of predicates, optionally ignoring owl:Thing, and
         optionally constraining to a given set of entity CURIE prefixes
 
         :param predicates: predicates to be considered (default: all)
         :param ignore_owl_thing: do not consider artificial/trivial owl:Thing when calculating (default=True)
         :param filter_obsoletes: do not include obsolete/deprecated nodes in results (default=True)
@@ -623,14 +804,25 @@
             if term not in exclusion_list:
                 yield term
 
     def subsets(self) -> Iterable[SUBSET_CURIE]:
         """
         Yields all subsets (slims) defined in the ontology.
 
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> for e in sorted(adapter.subsets()):
+        ...     print(e)
+        <BLANKLINE>
+        ...
+        goslim_drosophila
+        goslim_flybase_ribbon
+        goslim_generic
+        ...
+
         All subsets yielded are contracted to their short form.
 
         :return: iterator
         """
         raise NotImplementedError
 
     @deprecated("Replaced by subsets()")
@@ -641,98 +833,172 @@
     def all_subset_curies(self) -> Iterable[SUBSET_CURIE]:
         return self.subsets()
 
     def subset_members(self, subset: SUBSET_CURIE) -> Iterable[CURIE]:
         """
         Yields all entities belonging to the specified subset.
 
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> for e in sorted(adapter.subset_members('goslim_generic')):
+        ...     print(e, adapter.label(e))
+        <BLANKLINE>
+        ...
+        GO:0005634 nucleus
+        GO:0005635 nuclear envelope
+        GO:0005737 cytoplasm
+        GO:0005773 vacuole
+        ...
+
         :return: iterator
         """
         raise NotImplementedError
 
     def terms_subsets(self, curies: Iterable[CURIE]) -> Iterable[Tuple[CURIE, SUBSET_CURIE]]:
         """
         Yields entity-subset pairs for the given set of entities.
 
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/go-nucleus.db')
+        >>> for e, subset in sorted(adapter.terms_subsets(['GO:0005634', 'GO:0005635'])):
+        ...     print(subset, e, adapter.label(e))
+        <BLANKLINE>
+        ...
+        goslim_yeast GO:0005634 nucleus
+        goslim_chembl GO:0005635 nuclear envelope
+        goslim_generic GO:0005635 nuclear envelope
+        ...
+
         :return: iterator
         """
         # TODO: replace with adaptor-specific
         logging.info("Using naive method for fetching subsets")
         curies = list(curies)
         for s in self.subsets():
             for t in self.subset_members(s):
                 if t in curies:
                     yield t, s
 
     def terms_categories(self, curies: Iterable[CURIE]) -> Iterable[Tuple[CURIE, CATEGORY_CURIE]]:
         """
         Yields all categories an entity or entities belongs to.
 
+        .. note ::
+
+            This method is not implemented for all adapters.
+
         :return: iterator
         """
         raise NotImplementedError
 
     @deprecated("Replaced by subset_members(subset)")
     def curies_by_subset(self, subset: SUBSET_CURIE) -> Iterable[CURIE]:
         return self.subset_members(subset)
 
     def label(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> Optional[str]:
         """
         fetches the unique label for a CURIE.
 
-        The CURIE may be for a class, individual, property, or ontology
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter("tests/input/go-nucleus.owl")
+        >>> adapter.label("GO:0005634")
+        'nucleus'
 
-        :param curie:
-        :param lang: [None] language tag
-        :return:
-        """
-        raise NotImplementedError
+        The CURIE may be for a class, individual, property, or ontology.
 
-    def comments(self, curies: Iterable[CURIE]) -> Iterable[Tuple[CURIE, str]]:
-        """
-        Yields entity-comment pairs for a CURIE or CURIEs.
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter("tests/input/go-nucleus.owl")
+        >>> adapter.label("BFO:0000050")
+        'part of'
 
-        The CURIE may be for a class, individual, property, or ontology
+        For backends that support internationalization, the lang tag can be used:
 
-        :param curies:
-        :return:
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/hp-international-test.db')
+        >>> adapter.label('HP:0000118', lang='fr')
+        'Anomalie phénotypique'
+
+        If the argument matches the default language, and the literal is not
+        explicitly language tagged, it is still returned
+
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/hp-international-test.db')
+        >>> adapter.label('HP:0000118', lang='en')
+        'Phenotypic abnormality'
+
+        :param curie:
+        :param lang: [None] language tag
+        :return: label
         """
         raise NotImplementedError
 
     @deprecated("Use label(curie))")
     def get_label_by_curie(self, curie: CURIE) -> Optional[str]:
         return self.label(curie)
 
-    def labels(self, curies: Iterable[CURIE], allow_none=True) -> Iterable[Tuple[CURIE, str]]:
+    def labels(
+        self, curies: Iterable[CURIE], allow_none=True, lang: LANGUAGE_TAG = None
+    ) -> Iterable[Tuple[CURIE, str]]:
         """
         Yields entity-label pairs for a CURIE or CURIEs.
 
-        The CURIE may be for a class, individual, property, or ontology
+        The CURIE may be for a class, individual, property, or ontology.
+
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter("tests/input/go-nucleus.owl")
+        >>> list(sorted(adapter.labels(["GO:0005634", "GO:0005635"])))
+        [('GO:0005634', 'nucleus'), ('GO:0005635', 'nuclear envelope')]
 
         :param curies: identifiers to be queried
         :param allow_none: [True] use None as value if no label found
-        :return:
+        :return: iterator over tuples of (curie, label)
         """
         # default implementation: may be overridden for efficiency
         for curie in curies:
             label = self.label(curie)
             if label is None and not allow_none:
                 continue
             yield curie, label
 
+    def multilingual_labels(
+        self, curies: Iterable[CURIE], allow_none=True, langs: Optional[List[LANGUAGE_TAG]] = None
+    ) -> Iterable[Tuple[CURIE, str, LANGUAGE_TAG]]:
+        """
+        Yields entity-label-language tuples for a CURIE or CURIEs.
+
+        For example, in the HPO international edition:
+
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter('tests/input/hp-international-test.db')
+        >>> for tuple in sorted(adapter.multilingual_labels(['HP:0000118'], langs=['en', 'nl'])):
+        ...     print(tuple)
+        ('HP:0000118', 'Fenotypische abnormaliteit', 'nl')
+        ('HP:0000118', 'Phenotypic abnormality', None)
+
+        Note that the english label is not explicitly tagged with a language tag, but is returned
+        because it matches the :ref:`default_language`.
+
+        :param curies: identifiers to be queried
+        :param allow_none: [True] use None as value if no label found
+        :param langs: [None] list of languages to be queried (None means all)
+        :return: iterator over tuples of (curie, label, language)
+        """
+        raise NotImplementedError
+
     @deprecated("Use labels(...)")
     def get_labels_for_curies(self, **kwargs) -> Iterable[Tuple[CURIE, str]]:
         return self.labels(**kwargs)
 
-    def set_label(self, curie: CURIE, label: str) -> bool:
+    def set_label(self, curie: CURIE, label: str, lang: LANGUAGE_TAG = None) -> bool:
         """
         Sets the value of a label for a CURIE.
 
         :param curie:
         :param label:
+        :param lang:
         :return:
         """
         raise NotImplementedError
 
     def curies_by_label(self, label: str) -> List[CURIE]:
         """
         Fetches all curies with a given label.
@@ -745,15 +1011,82 @@
         """
         raise NotImplementedError()
 
     @deprecated("Use curies_by_label(label)")
     def get_curies_by_label(self, label: str) -> List[CURIE]:
         return self.curies_by_label(label)
 
-    def hierararchical_parents(self, curie: CURIE, isa_only: bool = False) -> List[CURIE]:
+    def comments(
+        self, curies: Iterable[CURIE], allow_none=True, lang: LANGUAGE_TAG = None
+    ) -> Iterable[Tuple[CURIE, Optional[str]]]:
+        """
+        Yields entity-comment pairs for a CURIE or CURIEs.
+
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter("tests/input/go-nucleus.db")
+        >>> for curie, comment in sorted(adapter.comments(["GO:0016772", "GO:0005634"], allow_none=False)):
+        ...     print(f"{curie} {comment[0:31]}[snip]")
+        GO:0016772 Note that this term encompasses[snip]
+
+        Note in the above query, no tuples for "GO:0005634" were yielded - this is because
+        the test ontology has no comments for this CURIE, and ``allow_none=False``.
+
+        If ``allow_none=True``, then a tuple with a None value in the second position will be yielded.
+
+        The CURIE may be for a class, individual, property, or ontology
+
+        :param curies:
+        :param allow_none: [True] if False, only yield entities with comments
+        :param lang: [None] language tag
+        :return: iterator
+        """
+        raise NotImplementedError
+
+    def relationships(
+        self,
+        subjects: Iterable[CURIE] = None,
+        predicates: Iterable[PRED_CURIE] = None,
+        objects: Iterable[CURIE] = None,
+        include_tbox: bool = True,
+        include_abox: bool = True,
+        include_entailed: bool = False,
+        exclude_blank: bool = True,
+    ) -> Iterator[RELATIONSHIP]:
+        """
+        Yields all relationships matching query constraints.
+
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter("tests/input/go-nucleus.db")
+        >>> for s, p, o in sorted(adapter.relationships(subjects=["GO:0005634"])):
+        ...     print(f"{p} {o} '{adapter.label(o)}'")
+        RO:0002160 NCBITaxon:2759 'Eukaryota'
+        rdfs:subClassOf GO:0043231 'intracellular membrane-bounded organelle'
+
+        :param subjects: constrain search to these subjects (i.e outgoing edges)
+        :param predicates: constrain search to these predicates
+        :param objects: constrain search to these objects (i.e incoming edges)
+        :param include_tbox: if true, include class-class relationships (default True)
+        :param include_abox: if true, include instance-instance/class relationships (default True)
+        :param include_entailed:
+        :param exclude_blank: do not include blank nodes/anonymous expressions
+        :return:
+        """
+        if not subjects:
+            subjects = list(self.entities())
+        logging.info(f"Subjects: {len(subjects)}")
+        for subject in subjects:
+            for this_predicate, this_objects in self.outgoing_relationship_map(subject).items():
+                if predicates and this_predicate not in predicates:
+                    continue
+                for this_object in this_objects:
+                    if objects and this_object not in objects:
+                        continue
+                    yield subject, this_predicate, this_object
+
+    def hierarchical_parents(self, curie: CURIE, isa_only: bool = False) -> List[CURIE]:
         """
         Returns all hierarchical parents.
 
         The definition of hierarchical parent depends on the provider. For example, in OLS,
         this will return part-of parents for GO, as well as is-a
 
         This only returns Named Entities; i.e. if an RDF source is wrapped, this will NOT return blank nodes
@@ -818,79 +1151,65 @@
         :param curie:
         :param predicates: if None, do not filter
         :return:
         """
         for s, p, _ in self.relationships(objects=[curie], predicates=predicates):
             yield p, s
 
-    def relationships(
-        self,
-        subjects: Iterable[CURIE] = None,
-        predicates: Iterable[PRED_CURIE] = None,
-        objects: Iterable[CURIE] = None,
-        include_tbox: bool = True,
-        include_abox: bool = True,
-        include_entailed: bool = False,
-        exclude_blank: bool = True,
-    ) -> Iterator[RELATIONSHIP]:
-        """
-        Yields all relationships matching query constraints.
-
-        :param subjects: constrain search to these subjects (i.e outgoing edges)
-        :param predicates: constrain search to these predicates
-        :param objects: constrain search to these objects (i.e incoming edges)
-        :param include_tbox: if true, include class-class relationships (default True)
-        :param include_abox: if true, include instance-instance/class relationships (default True)
-        :param include_entailed:
-        :param exclude_blank: do not include blank nodes/anonymous expressions
-        :return:
-        """
-        if not subjects:
-            subjects = list(self.entities())
-        logging.info(f"Subjects: {len(subjects)}")
-        for subject in subjects:
-            for this_predicate, this_objects in self.outgoing_relationship_map(subject).items():
-                if predicates and this_predicate not in predicates:
-                    continue
-                for this_object in this_objects:
-                    if objects and this_object not in objects:
-                        continue
-                    yield subject, this_predicate, this_object
-
     @deprecated("Use relationships()")
     def all_relationships(self) -> Iterable[RELATIONSHIP]:
         """
         Yields all known relationships.
 
         :return:
         """
         for curie in self.entities():
             for pred, fillers in self.outgoing_relationship_map(curie).items():
                 for filler in fillers:
                     yield curie, pred, filler
 
-    def definition(self, curie: CURIE) -> Optional[str]:
+    def definition(self, curie: CURIE, lang: Optional[LANGUAGE_TAG] = None) -> Optional[str]:
         """
         Lookup the text definition of an entity.
 
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter("tests/input/go-nucleus.db")
+        >>> for curie, defn, meta in adapter.definitions(["GO:0005634", "GO:0005737"], include_metadata=True):
+        ...     print(f"{curie} {defn[0:30]}[snip] [{meta}]")
+        GO:0005634 A membrane-bounded organelle o[snip] [{'oio:hasDbXref': ['GOC:go_curators']}]
+        GO:0005737 All of the contents of a cell [snip] [{'oio:hasDbXref': ['ISBN:0198547684']}]
+
         :param curie: entity identifier to be looked up
+        :param lang: language tag
         :return:
         """
         raise NotImplementedError()
 
     def definitions(
-        self, curies: Iterable[CURIE], include_metadata=False, include_missing=False
+        self,
+        curies: Iterable[CURIE],
+        include_metadata=False,
+        include_missing=False,
+        lang: Optional[LANGUAGE_TAG] = None,
     ) -> Iterator[DEFINITION]:
         """
         Lookup the text definition plus metadata for a list of entities.
 
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter("tests/input/go-nucleus.db")
+        >>> for curie, defn, meta in adapter.definitions(["GO:0005634", "GO:0005737"], include_metadata=True):
+        ...     print(f"{curie} {defn[0:30]}[snip] [{meta}]")
+        GO:0005634 A membrane-bounded organelle o[snip] [{'oio:hasDbXref': ['GOC:go_curators']}]
+        GO:0005737 All of the contents of a cell [snip] [{'oio:hasDbXref': ['ISBN:0198547684']}]
+
         :param curies: iterable collection of entity identifiers to be looked up
         :param include_metadata: if true, include metadata
         :param include_missing: if true, include curies with no definition
-        :return:
+        :param lang: language tag
+        :return: iterator over definition objects
         """
         if include_metadata:
             raise NotImplementedError()
         for curie in curies:
             defn = self.definition(curie)
             if not defn and not include_missing:
                 continue
@@ -902,14 +1221,18 @@
 
     def simple_mappings_by_curie(self, curie: CURIE) -> Iterable[Tuple[PRED_CURIE, CURIE]]:
         """
         Yields mappings for a given subject.
 
         Here, each mapping is represented as a simple tuple (predicate, object)
 
+        .. note ::
+
+            For a more sophisticated mapping interface, see :ref:`MappingProviderInterface`
+
         :param curie: entity identifier to be looked up
         :return: iterator over predicate-object tuples
         """
         raise NotImplementedError()
 
     def simple_mappings(self, curies: Iterable[CURIE]) -> Iterable[Tuple[CURIE, PRED_CURIE, CURIE]]:
         """
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/class_enrichment_calculation_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/class_enrichment_calculation_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -35,30 +35,42 @@
         cutoff=0.05,
         autolabel=False,
         filter_redundant=False,
         sort_by: str = None,
         direction="greater",
     ) -> Iterator[ClassEnrichmentResult]:
         """
-        Test for overrepresentation of classes in a set of entities.
+        Test for over-representation of classes in a set of entities.
 
-        :param subjects: The set of entities to test for overrepresentation of classes
-        :param background: The set of entities to use as a background for the test
-        :param hypotheses: The set of classes to test for overrepresentation
-        :param cutoff: The threshold to use for significance
-        :param labels: Whether to include labels for the classes
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter("src/oaklib/conf/go-pombase-input-spec.yaml")
+        >>> sample = ["PomBase:SPAC1142.02c", "PomBase:SPAC3H1.05", "PomBase:SPAC1142.06", "PomBase:SPAC4G8.02c"]
+        >>> for result in adapter.enriched_classes(sample, autolabel=True):
+        ...    assert result.p_value < 0.05
+        ...    print(f"{result.class_id} {result.class_label}")
+        <BLANKLINE>
+        GO:0006620 post-translational protein targeting to endoplasmic reticulum membrane
+        ...
+
+        :param subjects: The set of entities to test for over-representation of classes
+        :param background: The set of entities to use as a background for the test (recommended)
+        :param hypotheses: The set of classes to test for over-representation (default is all)
+        :param cutoff: The threshold to use for p-value
+        :param labels: Whether to include labels (names) for the classes
         :param direction: The direction of the test. One of 'greater', 'less', 'two-sided'
         :param filter_redundant: Whether to filter out redundant hypotheses
         :param sort_by: The field to sort by. One of 'p_value', 'sample_count', 'background_count', 'odds_ratio'
         :param direction: The direction of the test. One of 'greater', 'less', 'two-sided'
         :return: An iterator over ClassEnrichmentResult objects
         """
         subjects = list(subjects)
         sample_size = len(subjects)
         logging.info(f"Calculating sample_counts for {sample_size} subjects")
+        if not sample_size:
+            raise ValueError("No subjects provided")
         sample_count = {
             k: v
             for k, v in self.association_subject_counts(
                 subjects, predicates=predicates, object_closure_predicates=object_closure_predicates
             )
         }
         potential_hypotheses = set(sample_count.keys())
@@ -152,21 +164,31 @@
     def create_self_associations(self):
         """
         Create self associations for all terms in the ontology.
 
         >>> from oaklib import get_adapter
         >>> adapter = get_adapter("tests/input/go-nucleus.obo")
         >>> adapter.create_self_associations()
+        >>> assocs = list(adapter.associations(["GO:0005773"]))
+        >>> assert len(assocs) == 1
+        >>> assoc = assocs[0]
+        >>> print(assoc.subject, assoc.predicate, assoc.object)
+        GO:0005773 owl:equivalentClass GO:0005773
+
+        This is useful for simple over-representation tests over term sets without any annotations.
+
+        >>> from oaklib import get_adapter
+        >>> adapter = get_adapter("tests/input/go-nucleus.obo")
+        >>> adapter.create_self_associations()
         >>> terms = ["GO:0034357", "GO:0031965", "GO:0005773"]
         >>> for r in adapter.enriched_classes(terms, autolabel=True, filter_redundant=True):
         ...     print(r.class_id, r.class_label, round(r.p_value_adjusted,3))
         GO:0016020 membrane 0.004
         ...
 
 
-        This is useful for simple over-representation tests over term sets without any annotations.
         """
         assocs = []
         for e in self.entities(filter_obsoletes=True):
             assoc = Association(subject=e, predicate=EQUIVALENT_CLASS, object=e)
             assocs.append(assoc)
         self.add_associations(assocs)
```

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/differ_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/differ_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/dumper_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/dumper_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/mapping_provider_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/mapping_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/merge_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/merge_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/metadata_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/metadata_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/obograph_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/obograph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/obolegacy_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/obolegacy_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/ontology_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/owl_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/owl_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/patcher_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/patcher_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/rdf_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/rdf_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/relation_graph_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/relation_graph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/search_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/semsim_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/semsim_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/skos_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/skos_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/subsetter_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/subsetter_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/summary_statistics_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/summary_statistics_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/taxon_constraint_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/taxon_constraint_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/text_annotator_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/text_annotator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/interfaces/validator_interface.py` & `oaklib-0.5.0/src/oaklib/interfaces/validator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/heatmap_writer.py` & `oaklib-0.5.0/src/oaklib/io/heatmap_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/html_writer.py` & `oaklib-0.5.0/src/oaklib/io/html_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/obograph_writer.py` & `oaklib-0.5.0/src/oaklib/io/obograph_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/rollup_report_writer.py` & `oaklib-0.5.0/src/oaklib/io/rollup_report_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_axiom_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_axiom_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_csv_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_csv_writer.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 import csv
+import logging
 from dataclasses import dataclass, field
 from typing import Any, Dict, List, Mapping, Type, Union
 
 from linkml_runtime import CurieNamespace
 from linkml_runtime.utils.yamlutils import YAMLRoot
 
 import oaklib.datamodels.summary_statistics_datamodel as summary_stats
 from oaklib.datamodels import obograph
 from oaklib.datamodels.vocabulary import HAS_DBXREF, HAS_DEFINITION_CURIE, IS_A, PART_OF
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.interfaces.semsim_interface import SemanticSimilarityInterface
 from oaklib.io.streaming_writer import ID_KEY, LABEL_KEY, StreamingWriter
 from oaklib.types import CURIE
 
+NULL_VALUE = "None"
+
 
 def _keyval(x: Any) -> str:
     if isinstance(x, CurieNamespace):
         return str(x.curie())
     # if isinstance(x, EnumDefinitionImpl):
     #    if x.curie:
     #        return str(x.curie)
@@ -41,15 +44,16 @@
             obj_as_dict = obj
         elif isinstance(obj, CURIE):
             obj_as_dict = self._get_dict(obj)
         else:
             obj_as_dict = vars(obj)
         self._rewrite_dict(obj_as_dict, obj)
         obj_as_dict = self.add_labels(obj_as_dict, label_fields)
-        if not self.heterogeneous_keys:
+        heterogeneous_keys = self.heterogeneous_keys or self.pivot_fields
+        if not heterogeneous_keys:
             if self.writer is None:
                 # TODO: option to delay writing header, as not all keys may be populated in advance
                 self.keys = list(obj_as_dict)
                 self.writer = csv.DictWriter(
                     self.file, delimiter=self.delimiter, fieldnames=self.keys
                 )
                 self.writer.writeheader()
@@ -64,18 +68,48 @@
                     if k not in self.keys:
                         self.keys.append(k)
                     item[k] = _keyval(v)
             self.rows.append(item)
             # self.rows.append({k: _keyval(v) for k, v in obj_as_dict.items()})
 
     def finish(self):
-        if self.heterogeneous_keys:
-            self.writer = csv.DictWriter(self.file, delimiter=self.delimiter, fieldnames=self.keys)
-            self.writer.writeheader()
+        rows = self.rows
+        keys = self.keys
+        heterogeneous_keys = self.heterogeneous_keys or self.pivot_fields
+        if self.pivot_fields:
+            pk = self.primary_key
+            pv_field = self.primary_value_field
+            keys = list(set(keys) - set(self.pivot_fields) - {pv_field})
+            objs = {}
             for row in self.rows:
+                pivoted = False
+                pk_val = row[pk]
+                if pk_val not in objs:
+                    objs[pk_val] = {}
+                obj = objs[pk_val]
+                for k, v in row.items():
+                    if k in self.pivot_fields:
+                        obj[v] = row[pv_field]
+                        pivoted = True
+                        if v not in keys:
+                            keys.append(v)
+                    elif k == pv_field:
+                        pass
+                    else:
+                        obj[k] = row[k]
+                if not pivoted:
+                    obj[NULL_VALUE] = row[pv_field]
+                    if NULL_VALUE not in keys:
+                        keys.append(NULL_VALUE)
+            logging.info(f"Pivoted to make {len(objs)} rows: {objs}")
+            rows = list(objs.values())
+        if heterogeneous_keys:
+            self.writer = csv.DictWriter(self.file, delimiter=self.delimiter, fieldnames=keys)
+            self.writer.writeheader()
+            for row in rows:
                 self.writer.writerow(row)
 
     def _get_dict(self, curie: CURIE):
         oi = self.ontology_interface
         d = dict(
             id=curie,
             label=oi.label(curie),
```

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_fhir_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_fhir_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_info_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_info_writer.py`

 * *Files 15% similar despite different names*

```diff
@@ -25,31 +25,33 @@
     """
     A writer that streams basic line by line reporting info
     """
 
     def emit_curie(self, curie, label=None, **kwargs):
         oi = self.ontology_interface
         if label is None:
-            label = oi.label(curie)
+            label = oi.label(curie, lang=self.settings.preferred_language)
         self.file.write(f"{curie} ! {label}")
         if self.display_options:
             show_all = "all" in self.display_options
             if show_all or "x" in self.display_options:
                 for _, x in oi.simple_mappings_by_curie(curie):
                     self.file.write(f" {x}")
             if show_all or "r" in self.display_options and isinstance(oi, OboGraphInterface):
                 for k, vs in oi.outgoing_relationship_map(curie).items():
                     p = predicate_code_map.get(k, None)
                     if p is None:
-                        p = oi.label(k)
+                        p = oi.label(k, lang=self.settings.preferred_language)
                         if p is None:
                             p = k
                     self.file.write(f" {p}: [")
                     for v in vs:
-                        self.file.write(f' {v} "{oi.label(curie)}"')
+                        self.file.write(
+                            f' {v} "{oi.label(curie, lang=self.settings.preferred_language)}"'
+                        )
                     self.file.write("]")
             if show_all or "d" in self.display_options:
                 defn = oi.definition(curie)
                 if defn:
                     self.file.write(f' "{defn}"')
             if show_all or "db" in self.display_options:
                 self.file.write(f" isDefinedBy: {oi.defined_by(curie)}")
```

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_json_lines_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_json_lines_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_json_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_kgcl_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_kgcl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_markdown_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_markdown_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_nl_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_nl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_obo_json_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_obo_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_obo_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_obo_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_owl_functional_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_owl_functional_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_rdf_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_writer.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from typing import Any, ClassVar, Dict, Iterable, List, Mapping, Optional, Type, Union
 
 from linkml_runtime import SchemaView
 from linkml_runtime.utils.yamlutils import YAMLRoot
 
 from oaklib import BasicOntologyInterface
 from oaklib.datamodels.obograph import Node
+from oaklib.datamodels.settings import Settings
 from oaklib.types import CURIE
 from oaklib.utilities.iterator_utils import chunk
 
 ID_KEY = "id"
 LABEL_KEY = "label"
 
 
@@ -30,14 +31,18 @@
     schemaview: Optional[SchemaView] = None
     index_slot: Optional[str] = None
     uses_schemaview = False
     list_delimiter: ClassVar[str] = None
     heterogeneous_keys: bool = False
     _output: Any = None
     object_count: int = field(default=0)
+    settings: Settings = field(default_factory=lambda: Settings())
+    primary_key: str = field(default="id")
+    primary_value_field: str = field(default="label")
+    pivot_fields: List[str] = field(default_factory=lambda: [])
 
     def __post_init__(self):
         atexit.register(self.close)
 
     def __hash__(self):
         return hash(str(self))
 
@@ -83,15 +88,17 @@
 
         :param entities:
         :param kwargs:
         :return:
         """
         for curie_it in chunk(entities):
             logging.info("** Next chunk:")
-            for curie, label in self.ontology_interface.labels(curie_it):
+            for curie, label in self.ontology_interface.labels(
+                curie_it, lang=self.settings.preferred_language
+            ):
                 self.emit(curie, label)
 
     def emit_curie(self, curie: CURIE, label=None):
         raise NotImplementedError
 
     def emit_obj(self, obj: YAMLRoot):
         raise NotImplementedError
@@ -120,19 +127,28 @@
                 col_name = f"{f}_label"
                 if curie and obj_as_dict.get(col_name, None) is None:
                     # allow for a list of CURIEs flattened using a delimiter
                     delim = self.list_delimiter
                     if delim and isinstance(curie, str) and delim in curie:
                         curie = curie.split("|")
                     if isinstance(curie, list):
-                        label = [str(self.ontology_interface.label(c)) for c in curie]
+                        label = [
+                            str(
+                                self.ontology_interface.label(
+                                    c, lang=self.settings.preferred_language
+                                )
+                            )
+                            for c in curie
+                        ]
                         if delim:
                             label = delim.join(label)
                     else:
-                        label = self.ontology_interface.label(curie)
+                        label = self.ontology_interface.label(
+                            curie, lang=self.settings.preferred_language
+                        )
                     obj_as_dict_new = {}
                     for k, v in obj_as_dict.items():
                         obj_as_dict_new[k] = v
                         if k == f:
                             obj_as_dict_new[col_name] = label
                     obj_as_dict = obj_as_dict_new
         return obj_as_dict
```

### Comparing `oaklib-0.4.1/src/oaklib/io/streaming_yaml_writer.py` & `oaklib-0.5.0/src/oaklib/io/streaming_yaml_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/mappers/base_mapper.py` & `oaklib-0.5.0/src/oaklib/mappers/base_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/mappers/ontology_metadata_mapper.py` & `oaklib-0.5.0/src/oaklib/mappers/ontology_metadata_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/parsers/__init__.py` & `oaklib-0.5.0/src/oaklib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/parsers/association_parser.py` & `oaklib-0.5.0/src/oaklib/parsers/association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/parsers/boomer_parser.py` & `oaklib-0.5.0/src/oaklib/parsers/boomer_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/parsers/gaf_association_parser.py` & `oaklib-0.5.0/src/oaklib/parsers/gaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/parsers/hpoa_association_parser.py` & `oaklib-0.5.0/src/oaklib/parsers/hpoa_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/parsers/hpoa_g2p_association_parser.py` & `oaklib-0.5.0/src/oaklib/parsers/hpoa_g2p_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/parsers/kgx_association_parser.py` & `oaklib-0.5.0/src/oaklib/parsers/kgx_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/parsers/pairwise_association_parser.py` & `oaklib-0.5.0/src/oaklib/parsers/pairwise_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/parsers/parser_base.py` & `oaklib-0.5.0/src/oaklib/parsers/parser_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/parsers/phaf_association_parser.py` & `oaklib-0.5.0/src/oaklib/parsers/phaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/parsers/xaf_association_parser.py` & `oaklib-0.5.0/src/oaklib/parsers/xaf_association_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -135,14 +135,15 @@
         ):
             raise ValueError(f"Unexpected default predicate {self.default_predicate_value} in file")
         for line in file.readlines():
             if line.startswith(self.comment_character):
                 continue
             line = line.rstrip()
             vals = line.split("\t")
+            # logging.debug(f"Processing line: {line} // {vals}")
             s = lookup_subject(vals)
             p = lookup_predicate(vals)
             o = lookup_object(vals)
             if not p:
                 p = self.default_predicate_value
             if self.subject_prefix_column:
                 sp = lookup_subject_prefix(vals)
```

### Comparing `oaklib-0.4.1/src/oaklib/resource.py` & `oaklib-0.5.0/src/oaklib/resource.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/apikey_manager.py` & `oaklib-0.5.0/src/oaklib/utilities/apikey_manager.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/associations/association_differ.py` & `oaklib-0.5.0/src/oaklib/utilities/associations/association_differ.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/associations/association_index.py` & `oaklib-0.5.0/src/oaklib/utilities/associations/association_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/basic_utils.py` & `oaklib-0.5.0/src/oaklib/utilities/basic_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/graph/networkx_bridge.py` & `oaklib-0.5.0/src/oaklib/utilities/graph/networkx_bridge.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/graph/relationship_walker.py` & `oaklib-0.5.0/src/oaklib/utilities/graph/relationship_walker.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/identifier_utils.py` & `oaklib-0.5.0/src/oaklib/utilities/identifier_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/iterator_utils.py` & `oaklib-0.5.0/src/oaklib/utilities/iterator_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/kgcl_utilities.py` & `oaklib-0.5.0/src/oaklib/utilities/kgcl_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/label_utilities.py` & `oaklib-0.5.0/src/oaklib/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/lexical/lexical_indexer.py` & `oaklib-0.5.0/src/oaklib/utilities/lexical/lexical_indexer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/mapping/boomer_utils.py` & `oaklib-0.5.0/src/oaklib/utilities/mapping/boomer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/mapping/cross_ontology_diffs.py` & `oaklib-0.5.0/src/oaklib/utilities/mapping/cross_ontology_diffs.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/mapping/mapping_propagator.py` & `oaklib-0.5.0/src/oaklib/utilities/mapping/mapping_propagator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/mapping/mapping_validation.py` & `oaklib-0.5.0/src/oaklib/utilities/mapping/mapping_validation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/mapping/sssom_utils.py` & `oaklib-0.5.0/src/oaklib/utilities/mapping/sssom_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/ner_utilities.py` & `oaklib-0.5.0/src/oaklib/utilities/ner_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/nlp/natual_language_generation.py` & `oaklib-0.5.0/src/oaklib/utilities/nlp/natual_language_generation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/obograph_utils.py` & `oaklib-0.5.0/src/oaklib/utilities/obograph_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/ontology_builder.py` & `oaklib-0.5.0/src/oaklib/utilities/ontology_builder.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/reasoning/relation_graph.py` & `oaklib-0.5.0/src/oaklib/utilities/reasoning/relation_graph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/semsim/similarity_utils.py` & `oaklib-0.5.0/src/oaklib/utilities/semsim/similarity_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/stats/hypergeometric.py` & `oaklib-0.5.0/src/oaklib/utilities/stats/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/subsets/slimmer_utils.py` & `oaklib-0.5.0/src/oaklib/utilities/subsets/slimmer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/subsets/subset_analysis.py` & `oaklib-0.5.0/src/oaklib/utilities/subsets/subset_analysis.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/subsets/value_set_expander.py` & `oaklib-0.5.0/src/oaklib/utilities/subsets/value_set_expander.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/table_filler.py` & `oaklib-0.5.0/src/oaklib/utilities/table_filler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/taxon/taxon_constraint_utils.py` & `oaklib-0.5.0/src/oaklib/utilities/taxon/taxon_constraint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/validation/definition_ontology_rule.py` & `oaklib-0.5.0/src/oaklib/utilities/validation/definition_ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/validation/disjointness_rule.py` & `oaklib-0.5.0/src/oaklib/utilities/validation/disjointness_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/validation/lint_utils.py` & `oaklib-0.5.0/src/oaklib/utilities/validation/lint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/validation/ontology_rule.py` & `oaklib-0.5.0/src/oaklib/utilities/validation/ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/src/oaklib/utilities/validation/rule_runner.py` & `oaklib-0.5.0/src/oaklib/utilities/validation/rule_runner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.4.1/PKG-INFO` & `oaklib-0.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaklib
-Version: 0.4.1
+Version: 0.5.0
 Summary: Ontology Access Kit: Python library for common ontology operations over a variety of backends
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

