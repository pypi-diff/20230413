# Comparing `tmp/oaklib-0.5.0.tar.gz` & `tmp/oaklib-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaklib-0.5.0.tar", max compression
+gzip compressed data, was "oaklib-0.5.1.tar", max compression
```

## Comparing `oaklib-0.5.0.tar` & `oaklib-0.5.1.tar`

### file list

```diff
@@ -1,255 +1,262 @@
--rw-r--r--   0        0        0    11357 2023-04-10 18:43:08.756935 oaklib-0.5.0/LICENSE
--rw-r--r--   0        0        0     7241 2023-04-10 18:43:08.756935 oaklib-0.5.0/README.md
--rw-r--r--   0        0        0     1728 2023-04-10 18:44:11.231480 oaklib-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      271 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/__init__.py
--rw-r--r--   0        0        0   188756 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/cli.py
--rw-r--r--   0        0        0       64 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/conf/__init__.py
--rw-r--r--   0        0        0      115 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/conf/go-pombase-input-spec.yaml
--rw-r--r--   0        0        0      106 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/conf/hpoa-input-spec.yaml
--rw-r--r--   0        0        0     1903 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
--rw-r--r--   0        0        0     4537 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/conf/obograph-style.json
--rw-r--r--   0        0        0      256 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/conf/omo-to-skos.sssom.tsv
--rw-r--r--   0        0        0      131 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/conf/value-set-expander.conf.yaml
--rw-r--r--   0        0        0      128 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/constants.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/converters/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/converters/data_model_converter.py
--rw-r--r--   0        0        0     2561 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/converters/logical_definition_flattener.py
--rw-r--r--   0        0        0     2371 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/converters/obo_graph_to_cx_converter.py
--rw-r--r--   0        0        0    12163 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/converters/obo_graph_to_fhir_converter.py
--rw-r--r--   0        0        0     5713 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/converters/obo_graph_to_obo_format_converter.py
--rw-r--r--   0        0        0     5155 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
--rw-r--r--   0        0        0       60 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/__init__.py
--rw-r--r--   0        0        0     4034 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/association.owl.ttl
--rw-r--r--   0        0        0    10999 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/association.py
--rw-r--r--   0        0        0     2738 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/association.yaml
--rw-r--r--   0        0        0     6165 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/class_enrichment.owl.ttl
--rw-r--r--   0        0        0    10853 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/class_enrichment.py
--rw-r--r--   0        0        0     2648 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/class_enrichment.yaml
--rw-r--r--   0        0        0    19083 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
--rw-r--r--   0        0        0    24246 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/cross_ontology_diff.py
--rw-r--r--   0        0        0    10687 2023-04-10 18:43:08.888940 oaklib-0.5.0/src/oaklib/datamodels/cross_ontology_diff.yaml
--rw-r--r--   0        0        0    29418 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/cx.py
--rw-r--r--   0        0        0     6314 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/cx.yaml
--rw-r--r--   0        0        0    15826 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/fhir.owl.ttl
--rw-r--r--   0        0        0    35744 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/fhir.py
--rw-r--r--   0        0        0     5064 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/fhir.yaml
--rw-r--r--   0        0        0     7671 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/input_specification.py
--rw-r--r--   0        0        0     1786 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/input_specification.yaml
--rw-r--r--   0        0        0    15537 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/item_list.py
--rw-r--r--   0        0        0     5747 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/item_list.yaml
--rw-r--r--   0        0        0     8984 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/lexical_index.owl.ttl
--rw-r--r--   0        0        0    17256 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/lexical_index.py
--rw-r--r--   0        0        0     6429 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/lexical_index.schema.json
--rw-r--r--   0        0        0     4016 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/lexical_index.yaml
--rw-r--r--   0        0        0    26434 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/mapping_cluster_datamodel.py
--rw-r--r--   0        0        0     7317 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
--rw-r--r--   0        0        0    17785 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
--rw-r--r--   0        0        0    30468 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.py
--rw-r--r--   0        0        0    11456 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
--rw-r--r--   0        0        0     3220 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.yaml
--rw-r--r--   0        0        0    25354 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/obograph.owl.ttl
--rw-r--r--   0        0        0    45533 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/obograph.py
--rw-r--r--   0        0        0    22375 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/obograph.schema.json
--rw-r--r--   0        0        0    17625 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/obograph.yaml
--rw-r--r--   0        0        0    59793 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.owl.ttl
--rw-r--r--   0        0        0   117175 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.py
--rw-r--r--   0        0        0    95288 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.schema.json
--rw-r--r--   0        0        0    30433 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.yaml
--rw-r--r--   0        0        0    14759 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/oxo.owl.ttl
--rw-r--r--   0        0        0    21914 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/oxo.py
--rw-r--r--   0        0        0     4392 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/oxo.yaml
--rw-r--r--   0        0        0     3240 2023-04-10 18:43:08.892940 oaklib-0.5.0/src/oaklib/datamodels/search.py
--rw-r--r--   0        0        0    16948 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/search_datamodel.owl.ttl
--rw-r--r--   0        0        0    25145 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/search_datamodel.py
--rw-r--r--   0        0        0     6683 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/search_datamodel.yaml
--rw-r--r--   0        0        0      287 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/settings.py
--rw-r--r--   0        0        0    12767 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/similarity.owl.ttl
--rw-r--r--   0        0        0    22226 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/similarity.py
--rw-r--r--   0        0        0     5511 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/similarity.yaml
--rw-r--r--   0        0        0    31217 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
--rw-r--r--   0        0        0    50743 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.py
--rw-r--r--   0        0        0    21176 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
--rw-r--r--   0        0        0    16246 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.yaml
--rw-r--r--   0        0        0     9909 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/taxon_constraints.owl.ttl
--rw-r--r--   0        0        0    18430 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/taxon_constraints.py
--rw-r--r--   0        0        0     5879 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/taxon_constraints.yaml
--rw-r--r--   0        0        0    11599 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/text_annotator.owl.ttl
--rw-r--r--   0        0        0    20418 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/text_annotator.py
--rw-r--r--   0        0        0     2464 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/text_annotator.schema.json
--rw-r--r--   0        0        0     4219 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/text_annotator.yaml
--rw-r--r--   0        0        0    13670 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.owl.ttl
--rw-r--r--   0        0        0    25351 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.py
--rw-r--r--   0        0        0    10783 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.schema.json
--rw-r--r--   0        0        0     7510 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.yaml
--rw-r--r--   0        0        0     6640 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/value_set_configuration.owl.ttl
--rw-r--r--   0        0        0     8458 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/value_set_configuration.py
--rw-r--r--   0        0        0     2276 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/value_set_configuration.yaml
--rw-r--r--   0        0        0     5588 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/datamodels/vocabulary.py
--rw-r--r--   0        0        0     5217 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/aggregator/__init__.py
--rw-r--r--   0        0        0     5454 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/aggregator/aggregator_implementation.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/amigo/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/cx/__init__.py
--rw-r--r--   0        0        0     1985 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/cx/cx_implementation.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/fhir/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/funowl/__init__.py
--rw-r--r--   0        0        0     8473 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/funowl/funowl_implementation.py
--rw-r--r--   0        0        0     2313 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/gilda.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/kgx/__init__.py
--rw-r--r--   0        0        0    30631 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/kgx/kgx_implementation.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/neo4j/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/obograph/__init__.py
--rw-r--r--   0        0        0    16141 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/obograph/obograph_implementation.py
--rw-r--r--   0        0        0      267 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/ols/__init__.py
--rw-r--r--   0        0        0      132 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/ols/constants.py
--rw-r--r--   0        0        0     7942 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/ols/ols_implementation.py
--rw-r--r--   0        0        0      686 2023-04-10 18:43:08.896940 oaklib-0.5.0/src/oaklib/implementations/ols/oxo_utils.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontobee/__init__.py
--rw-r--r--   0        0        0     1391 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontobee/ontobee_implementation.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontoportal/__init__.py
--rw-r--r--   0        0        0      382 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontoportal/agroportal_implementation.py
--rw-r--r--   0        0        0      821 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontoportal/bioportal_implementation.py
--rw-r--r--   0        0        0      378 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
--rw-r--r--   0        0        0      378 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontoportal/matportal_implementation.py
--rw-r--r--   0        0        0    12106 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/owlery/__init__.py
--rw-r--r--   0        0        0      427 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/owlery/owlery_implementation.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/pronto/__init__.py
--rw-r--r--   0        0        0    34553 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/pronto/pronto_implementation.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/robot/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/scigraph/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/simpleobo/__init__.py
--rw-r--r--   0        0        0    33791 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
--rw-r--r--   0        0        0    21176 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/simpleobo/simple_obo_parser.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/skos/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/solor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/solr/__init__.py
--rw-r--r--   0        0        0       96 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sparql/__init__.py
--rw-r--r--   0        0        0    36578 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
--rw-r--r--   0        0        0      885 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sparql/lov_implementation.py
--rw-r--r--   0        0        0     1721 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
--rw-r--r--   0        0        0     2525 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sparql/sparql_implementation.py
--rw-r--r--   0        0        0     2326 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sparql/sparql_query.py
--rw-r--r--   0        0        0       96 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sqldb/__init__.py
--rw-r--r--   0        0        0   104382 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sqldb/sql_implementation.py
--rw-r--r--   0        0        0     1903 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/sqldb/sqlite_utils.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/tccm/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/translator/__init__.py
--rw-r--r--   0        0        0     3111 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/translator/translator_implementation.py
--rw-r--r--   0        0        0      108 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ubergraph/__init__.py
--rw-r--r--   0        0        0    19393 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/umls/__init__.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/uniprot/__init__.py
--rw-r--r--   0        0        0     9603 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/uniprot/uniprot_implementation.py
--rw-r--r--   0        0        0       96 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/wikidata/__init__.py
--rw-r--r--   0        0        0    17121 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/implementations/wikidata/wikidata_implementation.py
--rw-r--r--   0        0        0      913 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/__init__.py
--rw-r--r--   0        0        0     7725 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/association_provider_interface.py
--rw-r--r--   0        0        0    50981 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/basic_ontology_interface.py
--rw-r--r--   0        0        0     8022 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/class_enrichment_calculation_interface.py
--rw-r--r--   0        0        0    11720 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/differ_interface.py
--rw-r--r--   0        0        0     2649 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/dumper_interface.py
--rw-r--r--   0        0        0     3365 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/mapping_provider_interface.py
--rw-r--r--   0        0        0     3262 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/merge_interface.py
--rw-r--r--   0        0        0     3103 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/metadata_interface.py
--rw-r--r--   0        0        0    17700 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/obograph_interface.py
--rw-r--r--   0        0        0     1003 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/obolegacy_interface.py
--rw-r--r--   0        0        0      784 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/ontology_interface.py
--rw-r--r--   0        0        0    10988 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/owl_interface.py
--rw-r--r--   0        0        0     8236 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/patcher_interface.py
--rw-r--r--   0        0        0     1955 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/rdf_interface.py
--rw-r--r--   0        0        0     2459 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/relation_graph_interface.py
--rw-r--r--   0        0        0     1386 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/search_interface.py
--rw-r--r--   0        0        0    12778 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/semsim_interface.py
--rw-r--r--   0        0        0     1063 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/skos_interface.py
--rw-r--r--   0        0        0     2112 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/subsetter_interface.py
--rw-r--r--   0        0        0    10140 2023-04-10 18:43:08.900940 oaklib-0.5.0/src/oaklib/interfaces/summary_statistics_interface.py
--rw-r--r--   0        0        0    18296 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/interfaces/taxon_constraint_interface.py
--rw-r--r--   0        0        0     7511 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/interfaces/text_annotator_interface.py
--rw-r--r--   0        0        0     3033 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/interfaces/validator_interface.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/__init__.py
--rw-r--r--   0        0        0     1539 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/heatmap_writer.py
--rw-r--r--   0        0        0     1698 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/html_writer.py
--rw-r--r--   0        0        0     1379 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/obograph_writer.py
--rw-r--r--   0        0        0     3444 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/rollup_report_writer.py
--rw-r--r--   0        0        0      739 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_axiom_writer.py
--rw-r--r--   0        0        0     7833 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_csv_writer.py
--rw-r--r--   0        0        0     1284 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_fhir_writer.py
--rw-r--r--   0        0        0     2524 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_info_writer.py
--rw-r--r--   0        0        0     1231 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_json_lines_writer.py
--rw-r--r--   0        0        0     1806 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_json_writer.py
--rw-r--r--   0        0        0      741 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_kgcl_writer.py
--rw-r--r--   0        0        0     2088 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_markdown_writer.py
--rw-r--r--   0        0        0     1152 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_nl_writer.py
--rw-r--r--   0        0        0     1117 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_obo_json_writer.py
--rw-r--r--   0        0        0     3496 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_obo_writer.py
--rw-r--r--   0        0        0     1270 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_owl_functional_writer.py
--rw-r--r--   0        0        0     2244 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_rdf_writer.py
--rw-r--r--   0        0        0     5129 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_writer.py
--rw-r--r--   0        0        0     1301 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/io/streaming_yaml_writer.py
--rw-r--r--   0        0        0      113 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/mappers/__init__.py
--rw-r--r--   0        0        0     3717 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/mappers/base_mapper.py
--rw-r--r--   0        0        0     1849 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/mappers/ontology_metadata_mapper.py
--rw-r--r--   0        0        0     1742 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/__init__.py
--rw-r--r--   0        0        0      650 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/association_parser.py
--rw-r--r--   0        0        0      522 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/association_parser_factory.py
--rw-r--r--   0        0        0     4731 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/boomer_parser.py
--rw-r--r--   0        0        0     1178 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/gaf_association_parser.py
--rw-r--r--   0        0        0      563 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/hpoa_association_parser.py
--rw-r--r--   0        0        0      602 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/hpoa_g2p_association_parser.py
--rw-r--r--   0        0        0      653 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/kgx_association_parser.py
--rw-r--r--   0        0        0      525 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/pairwise_association_parser.py
--rw-r--r--   0        0        0     1328 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/parser_base.py
--rw-r--r--   0        0        0      707 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/phaf_association_parser.py
--rw-r--r--   0        0        0     6194 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/parsers/xaf_association_parser.py
--rw-r--r--   0        0        0     2210 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/resource.py
--rw-r--r--   0        0        0    12291 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/selector.py
--rw-r--r--   0        0        0      177 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/types.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/__init__.py
--rw-r--r--   0        0        0     1613 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/apikey_manager.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/associations/__init__.py
--rw-r--r--   0        0        0     2810 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/associations/association_differ.py
--rw-r--r--   0        0        0     2865 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/associations/association_index.py
--rw-r--r--   0        0        0     1182 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/basic_utils.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/graph/__init__.py
--rw-r--r--   0        0        0     2490 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/graph/networkx_bridge.py
--rw-r--r--   0        0        0     2918 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/graph/relationship_walker.py
--rw-r--r--   0        0        0      993 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/identifier_utils.py
--rw-r--r--   0        0        0      999 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/iterator_utils.py
--rw-r--r--   0        0        0     3345 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/kgcl_utilities.py
--rw-r--r--   0        0        0      850 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/label_utilities.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/lexical/__init__.py
--rw-r--r--   0        0        0    19516 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/lexical/lexical_indexer.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/mapping/__init__.py
--rw-r--r--   0        0        0    14443 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/mapping/boomer_utils.py
--rw-r--r--   0        0        0    15328 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/mapping/cross_ontology_diffs.py
--rw-r--r--   0        0        0      751 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/mapping/mapping_propagator.py
--rw-r--r--   0        0        0     2270 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/mapping/mapping_validation.py
--rw-r--r--   0        0        0     2694 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/mapping/sssom_utils.py
--rw-r--r--   0        0        0      684 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/ner_utilities.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/nlp/__init__.py
--rw-r--r--   0        0        0     3358 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/nlp/natual_language_generation.py
--rw-r--r--   0        0        0      136 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/oboformat_utils.py
--rw-r--r--   0        0        0    22266 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/obograph_utils.py
--rw-r--r--   0        0        0     2275 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/ontology_builder.py
--rw-r--r--   0        0        0      379 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/rate_limiter.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/reasoning/__init__.py
--rw-r--r--   0        0        0      569 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/reasoning/relation_graph.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/semsim/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/semsim/similarity_utils.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/stats/__init__.py
--rw-r--r--   0        0        0     1511 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/stats/hypergeometric.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/subsets/__init__.py
--rw-r--r--   0        0        0     2676 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/subsets/slimmer_utils.py
--rw-r--r--   0        0        0     4701 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/subsets/subset_analysis.py
--rw-r--r--   0        0        0    11592 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/subsets/value_set_expander.py
--rw-r--r--   0        0        0    13212 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/table_filler.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/taxon/__init__.py
--rw-r--r--   0        0        0     1743 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/taxon/taxon_constraint_utils.py
--rw-r--r--   0        0        0        0 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/validation/__init__.py
--rw-r--r--   0        0        0    10097 2023-04-10 18:43:08.904940 oaklib-0.5.0/src/oaklib/utilities/validation/definition_ontology_rule.py
--rw-r--r--   0        0        0     7492 2023-04-10 18:43:08.908941 oaklib-0.5.0/src/oaklib/utilities/validation/disjointness_rule.py
--rw-r--r--   0        0        0     1729 2023-04-10 18:43:08.908941 oaklib-0.5.0/src/oaklib/utilities/validation/lint_utils.py
--rw-r--r--   0        0        0     1402 2023-04-10 18:43:08.908941 oaklib-0.5.0/src/oaklib/utilities/validation/ontology_rule.py
--rw-r--r--   0        0        0     1313 2023-04-10 18:43:08.908941 oaklib-0.5.0/src/oaklib/utilities/validation/rule_runner.py
--rw-r--r--   0        0        0     8923 1970-01-01 00:00:00.000000 oaklib-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-13 14:49:46.691053 oaklib-0.5.1/LICENSE
+-rw-r--r--   0        0        0     7241 2023-04-13 14:49:46.691053 oaklib-0.5.1/README.md
+-rw-r--r--   0        0        0     1807 2023-04-13 14:50:39.991624 oaklib-0.5.1/pyproject.toml
+-rw-r--r--   0        0        0      271 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/__init__.py
+-rw-r--r--   0        0        0   188779 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/cli.py
+-rw-r--r--   0        0        0       64 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/__init__.py
+-rw-r--r--   0        0        0      117 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/go-human-input-spec.yaml
+-rw-r--r--   0        0        0      115 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/go-pombase-input-spec.yaml
+-rw-r--r--   0        0        0      109 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/hpoa-g2p-input-spec.yaml
+-rw-r--r--   0        0        0      106 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/hpoa-input-spec.yaml
+-rw-r--r--   0        0        0     1903 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
+-rw-r--r--   0        0        0      562 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/mondo-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      109 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/mondo-gencc-input-spec.yaml
+-rw-r--r--   0        0        0      118 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
+-rw-r--r--   0        0        0     4537 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/obograph-style.json
+-rw-r--r--   0        0        0      256 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/omo-to-skos.sssom.tsv
+-rw-r--r--   0        0        0      131 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/value-set-expander.conf.yaml
+-rw-r--r--   0        0        0      128 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/constants.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/converters/__init__.py
+-rw-r--r--   0        0        0     1456 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/converters/data_model_converter.py
+-rw-r--r--   0        0        0     2561 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/converters/logical_definition_flattener.py
+-rw-r--r--   0        0        0     2371 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/converters/obo_graph_to_cx_converter.py
+-rw-r--r--   0        0        0    12163 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/converters/obo_graph_to_fhir_converter.py
+-rw-r--r--   0        0        0     5713 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/converters/obo_graph_to_obo_format_converter.py
+-rw-r--r--   0        0        0     5155 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
+-rw-r--r--   0        0        0       60 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/__init__.py
+-rw-r--r--   0        0        0     4034 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/association.owl.ttl
+-rw-r--r--   0        0        0    13782 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/association.py
+-rw-r--r--   0        0        0     4506 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/association.yaml
+-rw-r--r--   0        0        0     6165 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/class_enrichment.owl.ttl
+-rw-r--r--   0        0        0    10853 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/class_enrichment.py
+-rw-r--r--   0        0        0     2648 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/class_enrichment.yaml
+-rw-r--r--   0        0        0    19083 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
+-rw-r--r--   0        0        0    24246 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/cross_ontology_diff.py
+-rw-r--r--   0        0        0    10687 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/cross_ontology_diff.yaml
+-rw-r--r--   0        0        0    29418 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/cx.py
+-rw-r--r--   0        0        0     6314 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/cx.yaml
+-rw-r--r--   0        0        0    15826 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/fhir.owl.ttl
+-rw-r--r--   0        0        0    35744 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/fhir.py
+-rw-r--r--   0        0        0     5064 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/fhir.yaml
+-rw-r--r--   0        0        0    13217 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/input_specification.py
+-rw-r--r--   0        0        0     3134 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/input_specification.yaml
+-rw-r--r--   0        0        0    15518 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/item_list.py
+-rw-r--r--   0        0        0     5765 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/item_list.yaml
+-rw-r--r--   0        0        0     8984 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/lexical_index.owl.ttl
+-rw-r--r--   0        0        0    17256 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/lexical_index.py
+-rw-r--r--   0        0        0     6429 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/lexical_index.schema.json
+-rw-r--r--   0        0        0     4016 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/lexical_index.yaml
+-rw-r--r--   0        0        0    26434 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/mapping_cluster_datamodel.py
+-rw-r--r--   0        0        0     7317 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
+-rw-r--r--   0        0        0   226115 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
+-rw-r--r--   0        0        0    32727 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.py
+-rw-r--r--   0        0        0    12889 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
+-rw-r--r--   0        0        0     3607 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.yaml
+-rw-r--r--   0        0        0    25354 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/obograph.owl.ttl
+-rw-r--r--   0        0        0    45533 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/obograph.py
+-rw-r--r--   0        0        0    22375 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/obograph.schema.json
+-rw-r--r--   0        0        0    17625 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/obograph.yaml
+-rw-r--r--   0        0        0    59793 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.owl.ttl
+-rw-r--r--   0        0        0   117175 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.py
+-rw-r--r--   0        0        0    95288 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.schema.json
+-rw-r--r--   0        0        0    30433 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.yaml
+-rw-r--r--   0        0        0    14759 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/oxo.owl.ttl
+-rw-r--r--   0        0        0    21914 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/oxo.py
+-rw-r--r--   0        0        0     4392 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/oxo.yaml
+-rw-r--r--   0        0        0     3240 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/search.py
+-rw-r--r--   0        0        0    16948 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/search_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25145 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/search_datamodel.py
+-rw-r--r--   0        0        0     6683 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/search_datamodel.yaml
+-rw-r--r--   0        0        0      287 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/settings.py
+-rw-r--r--   0        0        0    12767 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/similarity.owl.ttl
+-rw-r--r--   0        0        0    22226 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/similarity.py
+-rw-r--r--   0        0        0     5511 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/similarity.yaml
+-rw-r--r--   0        0        0    31217 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
+-rw-r--r--   0        0        0    50743 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.py
+-rw-r--r--   0        0        0    21176 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
+-rw-r--r--   0        0        0    16246 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.yaml
+-rw-r--r--   0        0        0     9909 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/taxon_constraints.owl.ttl
+-rw-r--r--   0        0        0    18430 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/taxon_constraints.py
+-rw-r--r--   0        0        0     5879 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/taxon_constraints.yaml
+-rw-r--r--   0        0        0    11599 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/text_annotator.owl.ttl
+-rw-r--r--   0        0        0    20418 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/text_annotator.py
+-rw-r--r--   0        0        0     2464 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/text_annotator.schema.json
+-rw-r--r--   0        0        0     4219 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/text_annotator.yaml
+-rw-r--r--   0        0        0    13670 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25351 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.py
+-rw-r--r--   0        0        0    10783 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.schema.json
+-rw-r--r--   0        0        0     7510 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.yaml
+-rw-r--r--   0        0        0     6640 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/value_set_configuration.owl.ttl
+-rw-r--r--   0        0        0     8458 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/value_set_configuration.py
+-rw-r--r--   0        0        0     2276 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/value_set_configuration.yaml
+-rw-r--r--   0        0        0     5588 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/vocabulary.py
+-rw-r--r--   0        0        0     5217 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/aggregator/__init__.py
+-rw-r--r--   0        0        0     5454 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/aggregator/aggregator_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/amigo/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/cx/__init__.py
+-rw-r--r--   0        0        0     1985 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/cx/cx_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/fhir/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/funowl/__init__.py
+-rw-r--r--   0        0        0     8473 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/funowl/funowl_implementation.py
+-rw-r--r--   0        0        0     2313 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/gilda.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/kgx/__init__.py
+-rw-r--r--   0        0        0    30631 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/kgx/kgx_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/neo4j/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/obograph/__init__.py
+-rw-r--r--   0        0        0    16141 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/obograph/obograph_implementation.py
+-rw-r--r--   0        0        0      267 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ols/__init__.py
+-rw-r--r--   0        0        0      132 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ols/constants.py
+-rw-r--r--   0        0        0     7942 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ols/ols_implementation.py
+-rw-r--r--   0        0        0      686 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ols/oxo_utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontobee/__init__.py
+-rw-r--r--   0        0        0     1391 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontobee/ontobee_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontoportal/__init__.py
+-rw-r--r--   0        0        0      382 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontoportal/agroportal_implementation.py
+-rw-r--r--   0        0        0      821 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontoportal/bioportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontoportal/matportal_implementation.py
+-rw-r--r--   0        0        0    12106 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/owlery/__init__.py
+-rw-r--r--   0        0        0      427 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/owlery/owlery_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/pronto/__init__.py
+-rw-r--r--   0        0        0    35361 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/pronto/pronto_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/robot/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/scigraph/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/simpleobo/__init__.py
+-rw-r--r--   0        0        0    34101 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
+-rw-r--r--   0        0        0    21451 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/simpleobo/simple_obo_parser.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/skos/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/solor/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/solr/__init__.py
+-rw-r--r--   0        0        0       96 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/sparql/__init__.py
+-rw-r--r--   0        0        0    36699 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
+-rw-r--r--   0        0        0      885 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/sparql/lov_implementation.py
+-rw-r--r--   0        0        0     1721 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
+-rw-r--r--   0        0        0     2658 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/sparql/sparql_implementation.py
+-rw-r--r--   0        0        0     2326 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/sparql/sparql_query.py
+-rw-r--r--   0        0        0       96 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/sqldb/__init__.py
+-rw-r--r--   0        0        0   105245 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/sqldb/sql_implementation.py
+-rw-r--r--   0        0        0     1903 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/sqldb/sqlite_utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/tccm/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/translator/__init__.py
+-rw-r--r--   0        0        0     3283 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/translator/translator_implementation.py
+-rw-r--r--   0        0        0      108 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/ubergraph/__init__.py
+-rw-r--r--   0        0        0    19393 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/umls/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/uniprot/__init__.py
+-rw-r--r--   0        0        0     9603 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/uniprot/uniprot_implementation.py
+-rw-r--r--   0        0        0       96 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/wikidata/__init__.py
+-rw-r--r--   0        0        0    17121 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/wikidata/wikidata_implementation.py
+-rw-r--r--   0        0        0      913 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/__init__.py
+-rw-r--r--   0        0        0    13371 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/association_provider_interface.py
+-rw-r--r--   0        0        0    50981 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/basic_ontology_interface.py
+-rw-r--r--   0        0        0     8640 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/class_enrichment_calculation_interface.py
+-rw-r--r--   0        0        0    11720 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/differ_interface.py
+-rw-r--r--   0        0        0     2649 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/dumper_interface.py
+-rw-r--r--   0        0        0    13280 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/mapping_provider_interface.py
+-rw-r--r--   0        0        0     3262 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/merge_interface.py
+-rw-r--r--   0        0        0     3103 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/metadata_interface.py
+-rw-r--r--   0        0        0    17700 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/obograph_interface.py
+-rw-r--r--   0        0        0     1003 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/obolegacy_interface.py
+-rw-r--r--   0        0        0      784 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/ontology_interface.py
+-rw-r--r--   0        0        0    10988 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/owl_interface.py
+-rw-r--r--   0        0        0     8236 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/patcher_interface.py
+-rw-r--r--   0        0        0     1955 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/rdf_interface.py
+-rw-r--r--   0        0        0     2459 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/relation_graph_interface.py
+-rw-r--r--   0        0        0     1386 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/search_interface.py
+-rw-r--r--   0        0        0    12778 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/semsim_interface.py
+-rw-r--r--   0        0        0     1063 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/skos_interface.py
+-rw-r--r--   0        0        0     2112 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/subsetter_interface.py
+-rw-r--r--   0        0        0    10140 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/summary_statistics_interface.py
+-rw-r--r--   0        0        0    18296 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/taxon_constraint_interface.py
+-rw-r--r--   0        0        0     7511 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/text_annotator_interface.py
+-rw-r--r--   0        0        0     3033 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/validator_interface.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/__init__.py
+-rw-r--r--   0        0        0     1539 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/heatmap_writer.py
+-rw-r--r--   0        0        0     1698 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/html_writer.py
+-rw-r--r--   0        0        0     1379 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/obograph_writer.py
+-rw-r--r--   0        0        0     3444 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/rollup_report_writer.py
+-rw-r--r--   0        0        0      739 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_axiom_writer.py
+-rw-r--r--   0        0        0     7833 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_csv_writer.py
+-rw-r--r--   0        0        0     1284 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_fhir_writer.py
+-rw-r--r--   0        0        0     2524 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_info_writer.py
+-rw-r--r--   0        0        0     1231 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_json_lines_writer.py
+-rw-r--r--   0        0        0     1806 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_json_writer.py
+-rw-r--r--   0        0        0      741 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_kgcl_writer.py
+-rw-r--r--   0        0        0     2088 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_markdown_writer.py
+-rw-r--r--   0        0        0     1152 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_nl_writer.py
+-rw-r--r--   0        0        0     1117 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_obo_json_writer.py
+-rw-r--r--   0        0        0     3496 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_obo_writer.py
+-rw-r--r--   0        0        0     1270 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_owl_functional_writer.py
+-rw-r--r--   0        0        0     2244 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_rdf_writer.py
+-rw-r--r--   0        0        0     5129 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_writer.py
+-rw-r--r--   0        0        0     1301 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_yaml_writer.py
+-rw-r--r--   0        0        0      113 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/mappers/__init__.py
+-rw-r--r--   0        0        0     3717 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/mappers/base_mapper.py
+-rw-r--r--   0        0        0     1849 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/mappers/ontology_metadata_mapper.py
+-rw-r--r--   0        0        0     2179 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/__init__.py
+-rw-r--r--   0        0        0      650 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/association_parser.py
+-rw-r--r--   0        0        0      522 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/association_parser_factory.py
+-rw-r--r--   0        0        0     4731 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/boomer_parser.py
+-rw-r--r--   0        0        0     1178 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/gaf_association_parser.py
+-rw-r--r--   0        0        0     1090 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/gencc_association_parser.py
+-rw-r--r--   0        0        0      563 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/hpoa_association_parser.py
+-rw-r--r--   0        0        0      602 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/hpoa_g2p_association_parser.py
+-rw-r--r--   0        0        0      653 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/kgx_association_parser.py
+-rw-r--r--   0        0        0     1666 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/mim2gene_association_parser.py
+-rw-r--r--   0        0        0      525 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/pairwise_association_parser.py
+-rw-r--r--   0        0        0     1328 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/parser_base.py
+-rw-r--r--   0        0        0      707 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/phaf_association_parser.py
+-rw-r--r--   0        0        0     6282 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/xaf_association_parser.py
+-rw-r--r--   0        0        0     2210 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/resource.py
+-rw-r--r--   0        0        0    13501 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/selector.py
+-rw-r--r--   0        0        0      177 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/types.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/__init__.py
+-rw-r--r--   0        0        0     1613 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/apikey_manager.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/associations/__init__.py
+-rw-r--r--   0        0        0     2810 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/associations/association_differ.py
+-rw-r--r--   0        0        0     2865 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/associations/association_index.py
+-rw-r--r--   0        0        0     1182 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/basic_utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/graph/__init__.py
+-rw-r--r--   0        0        0     2490 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/graph/networkx_bridge.py
+-rw-r--r--   0        0        0     2918 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/graph/relationship_walker.py
+-rw-r--r--   0        0        0      993 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/identifier_utils.py
+-rw-r--r--   0        0        0      999 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/iterator_utils.py
+-rw-r--r--   0        0        0     3345 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/kgcl_utilities.py
+-rw-r--r--   0        0        0      850 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/label_utilities.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/lexical/__init__.py
+-rw-r--r--   0        0        0    19516 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/lexical/lexical_indexer.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/mapping/__init__.py
+-rw-r--r--   0        0        0    14443 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/mapping/boomer_utils.py
+-rw-r--r--   0        0        0    15328 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/mapping/cross_ontology_diffs.py
+-rw-r--r--   0        0        0      751 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/mapping/mapping_propagator.py
+-rw-r--r--   0        0        0     2270 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/mapping/mapping_validation.py
+-rw-r--r--   0        0        0     2694 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/mapping/sssom_utils.py
+-rw-r--r--   0        0        0      684 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/ner_utilities.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/nlp/__init__.py
+-rw-r--r--   0        0        0     3358 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/nlp/natual_language_generation.py
+-rw-r--r--   0        0        0      136 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/oboformat_utils.py
+-rw-r--r--   0        0        0    22266 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/obograph_utils.py
+-rw-r--r--   0        0        0     2275 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/ontology_builder.py
+-rw-r--r--   0        0        0      379 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/rate_limiter.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/reasoning/__init__.py
+-rw-r--r--   0        0        0      569 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/reasoning/relation_graph.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/semsim/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/semsim/similarity_utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/stats/__init__.py
+-rw-r--r--   0        0        0     1511 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/stats/hypergeometric.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/subsets/__init__.py
+-rw-r--r--   0        0        0     2676 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/subsets/slimmer_utils.py
+-rw-r--r--   0        0        0     4701 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/subsets/subset_analysis.py
+-rw-r--r--   0        0        0    11592 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/subsets/value_set_expander.py
+-rw-r--r--   0        0        0    13212 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/table_filler.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/taxon/__init__.py
+-rw-r--r--   0        0        0     1743 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/taxon/taxon_constraint_utils.py
+-rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/validation/__init__.py
+-rw-r--r--   0        0        0    10097 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/validation/definition_ontology_rule.py
+-rw-r--r--   0        0        0     7492 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/validation/disjointness_rule.py
+-rw-r--r--   0        0        0     1729 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/validation/lint_utils.py
+-rw-r--r--   0        0        0     1402 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/validation/ontology_rule.py
+-rw-r--r--   0        0        0     1313 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/validation/rule_runner.py
+-rw-r--r--   0        0        0     8957 1970-01-01 00:00:00.000000 oaklib-0.5.1/PKG-INFO
```

### Comparing `oaklib-0.5.0/LICENSE` & `oaklib-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/README.md` & `oaklib-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/pyproject.toml` & `oaklib-0.5.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oaklib"
-version = "v0.5.0"
+version = "v0.5.1"
 description = "Ontology Access Kit: Python library for common ontology operations over a variety of backends"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
@@ -22,36 +22,40 @@
 semsql = "^0.3.1"
 lark = "^1.1.2"
 kgcl-schema = "^0.3.5"
 funowl = "^0.1.12"
 gilda = {version = "^0.10.1", optional = true}
 kgcl-rdflib = "^0.3.0"
 pystow = "^0.5.0"
-class-resolver = "^0.3.10"
+class-resolver = ">=0.4.2"
 ontoportal-client = "0.0.3"
 bioregistry = "^0.6.35"
 prefixmaps = "^0.1.2"
 ols-client = "^0.1.1"
 pandas = "^1.5.1"
 linkml-renderer = "^0.1.2"
 airium = "^0.2.5"
 ndex2 = "^3.5.0"
+upsetplot = "^0.8.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 Sphinx = ">=6.1.3"
 jupyter = "^1.0.0"
 sphinx-rtd-theme = "^1.0.0"
 sphinx-click = "^3.1.0"
 myst-parser = ">=1.0.0"
 linkml = "^1.2.14"
 sphinxcontrib-mermaid = "^0.8.1"
 sphinx-copybutton = "0.5.1"
 coverage = "^6.3.2"
 
+[tool.poetry.group.dev.dependencies]
+seaborn = "^0.12.2"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 runoak = "oaklib.cli:main"
 vskit = "oaklib.utilities.subsets.value_set_expander:main"
```

### Comparing `oaklib-0.5.0/src/oaklib/cli.py` & `oaklib-0.5.1/src/oaklib/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -3600,15 +3600,15 @@
     writer.autolabel = autolabel
     if not isinstance(impl, MappingProviderInterface):
         raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
     if len(terms) == 0:
         raise ValueError("Must provide at least one term")
     curies = query_terms_iterator(terms, impl)
     logging.info(f"Normalizing: {curies}")
-    for mapping in impl.sssom_mappings(curies):
+    for mapping in impl.sssom_mappings(curies, source=maps_to_source):
         if not mapping.object_id.startswith(f"{maps_to_source}:"):
             continue
         writer.emit_curie(mapping.object_id, mapping.object_label)
     writer.finish()
 
 
 @main.command()
```

### Comparing `oaklib-0.5.0/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml` & `oaklib-0.5.1/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/conf/obograph-style.json` & `oaklib-0.5.1/src/oaklib/conf/obograph-style.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/converters/data_model_converter.py` & `oaklib-0.5.1/src/oaklib/converters/data_model_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/converters/logical_definition_flattener.py` & `oaklib-0.5.1/src/oaklib/converters/logical_definition_flattener.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/converters/obo_graph_to_cx_converter.py` & `oaklib-0.5.1/src/oaklib/converters/obo_graph_to_cx_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/converters/obo_graph_to_fhir_converter.py` & `oaklib-0.5.1/src/oaklib/converters/obo_graph_to_fhir_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/converters/obo_graph_to_obo_format_converter.py` & `oaklib-0.5.1/src/oaklib/converters/obo_graph_to_obo_format_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py` & `oaklib-0.5.1/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/association.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/association.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/association.py` & `oaklib-0.5.1/src/oaklib/datamodels/association.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from association.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-03-15T10:56:08
+# Generation date: 2023-04-11T11:50:59
 # Schema: association
 #
 # id: https://w3id.org/oak/association
 # description: A datamodel for representing generic associations. The core datamodel is broad, encompassing the W3
 #              Open Annotation data model as well as common ontology annotation data models using in the
 #              biosciences.
 # license: https://creativecommons.org/publicdomain/zero/1.0/
@@ -16,15 +16,15 @@
 
 from jsonasobj2 import JsonObj, as_dict
 from linkml_runtime.linkml_model.meta import (
     EnumDefinition,
     PermissibleValue,
     PvFormulaOptions,
 )
-from linkml_runtime.linkml_model.types import Boolean, Uriorcurie
+from linkml_runtime.linkml_model.types import Boolean, String, Uriorcurie
 from linkml_runtime.utils.curienamespace import CurieNamespace
 from linkml_runtime.utils.dataclass_extensions_376 import (
     dataclasses_init_fn_with_kwargs,
 )
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from linkml_runtime.utils.formatutils import camelcase, sfx, underscore
 from linkml_runtime.utils.metamodelcore import (
@@ -46,18 +46,20 @@
 metamodel_version = "1.7.0"
 version = None
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
+BIOLINK = CurieNamespace("biolink", "https://w3id.org/biolink/vocab/")
 LINKML = CurieNamespace("linkml", "https://w3id.org/linkml/")
 OA = CurieNamespace("oa", "http://www.w3.org/ns/oa#")
 ONTOASSOC = CurieNamespace("ontoassoc", "https://w3id.org/oak/association/")
 RDF = CurieNamespace("rdf", "http://example.org/UNKNOWN/rdf/")
+SSSOM = CurieNamespace("sssom", "https://w3id.org/sssom/")
 DEFAULT_ = ONTOASSOC
 
 
 # Types
 
 # Class references
 
@@ -77,14 +79,17 @@
 
     subject: Optional[Union[str, URIorCURIE]] = None
     predicate: Optional[Union[str, URIorCURIE]] = None
     object: Optional[Union[str, URIorCURIE]] = None
     property_values: Optional[
         Union[Union[dict, "PropertyValue"], List[Union[dict, "PropertyValue"]]]
     ] = empty_list()
+    subject_label: Optional[str] = None
+    predicate_label: Optional[str] = None
+    object_label: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.subject is not None and not isinstance(self.subject, URIorCURIE):
             self.subject = URIorCURIE(self.subject)
 
         if self.predicate is not None and not isinstance(self.predicate, URIorCURIE):
             self.predicate = URIorCURIE(self.predicate)
@@ -97,14 +102,23 @@
                 [self.property_values] if self.property_values is not None else []
             )
         self.property_values = [
             v if isinstance(v, PropertyValue) else PropertyValue(**as_dict(v))
             for v in self.property_values
         ]
 
+        if self.subject_label is not None and not isinstance(self.subject_label, str):
+            self.subject_label = str(self.subject_label)
+
+        if self.predicate_label is not None and not isinstance(self.predicate_label, str):
+            self.predicate_label = str(self.predicate_label)
+
+        if self.object_label is not None and not isinstance(self.object_label, str):
+            self.object_label = str(self.object_label)
+
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class NegatedAssociation(YAMLRoot):
     """
     A negated association between a thing (subject) and another thing (object).
@@ -119,14 +133,17 @@
 
     subject: Optional[Union[str, URIorCURIE]] = None
     predicate: Optional[Union[str, URIorCURIE]] = None
     object: Optional[Union[str, URIorCURIE]] = None
     property_values: Optional[
         Union[Union[dict, "PropertyValue"], List[Union[dict, "PropertyValue"]]]
     ] = empty_list()
+    subject_label: Optional[str] = None
+    predicate_label: Optional[str] = None
+    object_label: Optional[str] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.subject is not None and not isinstance(self.subject, URIorCURIE):
             self.subject = URIorCURIE(self.subject)
 
         if self.predicate is not None and not isinstance(self.predicate, URIorCURIE):
             self.predicate = URIorCURIE(self.predicate)
@@ -139,14 +156,23 @@
                 [self.property_values] if self.property_values is not None else []
             )
         self.property_values = [
             v if isinstance(v, PropertyValue) else PropertyValue(**as_dict(v))
             for v in self.property_values
         ]
 
+        if self.subject_label is not None and not isinstance(self.subject_label, str):
+            self.subject_label = str(self.subject_label)
+
+        if self.predicate_label is not None and not isinstance(self.predicate_label, str):
+            self.predicate_label = str(self.predicate_label)
+
+        if self.object_label is not None and not isinstance(self.object_label, str):
+            self.object_label = str(self.object_label)
+
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class PropertyValue(YAMLRoot):
     """
     A generic tag-value that can be associated with an association.
@@ -248,32 +274,59 @@
     name="subject",
     curie=RDF.curie("subject"),
     model_uri=ONTOASSOC.subject,
     domain=None,
     range=Optional[Union[str, URIorCURIE]],
 )
 
+slots.subject_label = Slot(
+    uri=SSSOM.subject_label,
+    name="subject_label",
+    curie=SSSOM.curie("subject_label"),
+    model_uri=ONTOASSOC.subject_label,
+    domain=None,
+    range=Optional[str],
+)
+
 slots.predicate = Slot(
     uri=RDF.predicate,
     name="predicate",
     curie=RDF.curie("predicate"),
     model_uri=ONTOASSOC.predicate,
     domain=None,
     range=Optional[Union[str, URIorCURIE]],
 )
 
+slots.predicate_label = Slot(
+    uri=SSSOM.predicate_label,
+    name="predicate_label",
+    curie=SSSOM.curie("predicate_label"),
+    model_uri=ONTOASSOC.predicate_label,
+    domain=None,
+    range=Optional[str],
+)
+
 slots.object = Slot(
     uri=RDF.object,
     name="object",
     curie=RDF.curie("object"),
     model_uri=ONTOASSOC.object,
     domain=None,
     range=Optional[Union[str, URIorCURIE]],
 )
 
+slots.object_label = Slot(
+    uri=SSSOM.object_label,
+    name="object_label",
+    curie=SSSOM.curie("object_label"),
+    model_uri=ONTOASSOC.object_label,
+    domain=None,
+    range=Optional[str],
+)
+
 slots.property_values = Slot(
     uri=ONTOASSOC.property_values,
     name="property_values",
     curie=ONTOASSOC.curie("property_values"),
     model_uri=ONTOASSOC.property_values,
     domain=None,
     range=Optional[Union[Union[dict, PropertyValue], List[Union[dict, PropertyValue]]]],
@@ -302,14 +355,50 @@
     name="associations",
     curie=ONTOASSOC.curie("associations"),
     model_uri=ONTOASSOC.associations,
     domain=None,
     range=Optional[Union[Union[dict, Association], List[Union[dict, Association]]]],
 )
 
+slots.original_subject = Slot(
+    uri=RDF.subject,
+    name="original_subject",
+    curie=RDF.curie("subject"),
+    model_uri=ONTOASSOC.original_subject,
+    domain=None,
+    range=Optional[Union[str, URIorCURIE]],
+)
+
+slots.original_predicate = Slot(
+    uri=RDF.predicate,
+    name="original_predicate",
+    curie=RDF.curie("predicate"),
+    model_uri=ONTOASSOC.original_predicate,
+    domain=None,
+    range=Optional[Union[str, URIorCURIE]],
+)
+
+slots.original_object = Slot(
+    uri=RDF.subject,
+    name="original_object",
+    curie=RDF.curie("subject"),
+    model_uri=ONTOASSOC.original_object,
+    domain=None,
+    range=Optional[Union[str, URIorCURIE]],
+)
+
+slots.denormalized_slot = Slot(
+    uri=ONTOASSOC.denormalized_slot,
+    name="denormalized_slot",
+    curie=ONTOASSOC.curie("denormalized_slot"),
+    model_uri=ONTOASSOC.denormalized_slot,
+    domain=None,
+    range=Optional[str],
+)
+
 slots.parserConfiguration__preserve_negated_associations = Slot(
     uri=ONTOASSOC.preserve_negated_associations,
     name="parserConfiguration__preserve_negated_associations",
     curie=ONTOASSOC.curie("preserve_negated_associations"),
     model_uri=ONTOASSOC.parserConfiguration__preserve_negated_associations,
     domain=None,
     range=Optional[Union[bool, Bool]],
```

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/association.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/input_specification.yaml`

 * *Files 27% similar despite different names*

```diff
@@ -1,101 +1,121 @@
-id: https://w3id.org/oak/association
-title: OAK Association Data Model
-name: association
-description: |-
-  A datamodel for representing generic associations.
-  
-  The core datamodel is broad, encompassing the W3 Open Annotation data model as well
-  as common ontology annotation data models using in the biosciences.
-
+id: https://w3id.org/oaklib/input-specification
+title: Input Specification Data Model
+name: inputspec
+description: >-
+  A data model for representing a set of inputs to OAK
 license: https://creativecommons.org/publicdomain/zero/1.0/
 
 prefixes:
+  itemList: https://w3id.org/linkml/item-list/
   linkml: https://w3id.org/linkml/
-  ontoassoc: https://w3id.org/oak/association/
-  oa: http://www.w3.org/ns/oa#
+  schema: http://schema.org/
+  dcterms: http://purl.org/dc/terms/
+  rdf: http://www.w3.org/1999/02/22-rdf-syntax-ns#
+  prov: http://www.w3.org/ns/prov#
+
+default_prefix: itemList
+default_range: string
+
 imports:
   - linkml:types
-default_prefix: ontoassoc
 
+#==================================
+# Classes                         #
+#==================================
 classes:
 
-  Association:
-    class_uri: oa:Annotation
-    description: A generic association between a thing (subject) and another thing (object).
-    slots:
-      - subject
-      - predicate
-      - object
-      - property_values
-
-  NegatedAssociation:
-    description: A negated association between a thing (subject) and another thing (object).
-    slots:
-      - subject
-      - predicate
-      - object
-      - property_values
-
-  PropertyValue:
-    description: A generic tag-value that can be associated with an association.
-    slots:
-      - predicate
-      - object
-
-  RollupGroup:
-    slots:
-      - group_object
-      - sub_groups
-      - associations
+  InputSpecification:
+    description: input spec
+    attributes:
+      ontology_resources:
+        range: OntologyResource
+        multivalued: true
+        inlined: true
+        description: >-
+          The ontologies used in the input specification
+      association_resources:
+        range: AssociationResource
+        multivalued: true
+        inlined: true
+        description: >-
+          The associations used in the input specification
 
-  ParserConfiguration:
+  Resource:
+    abstract: true
+    attributes:
+      id:
+        range: string
+        identifier: true
+        description: >-
+          The identifier of the ontology resource
+      path:
+        range: string
+        description: >-
+          The path of the resource. May be a URL or file path
+      format:
+        range: string
+      selector:
+        range: string
+        description: >-
+          The selector of the ontology resource
+
+  OntologyResource:
+    description: >-
+      A resource that points to an ontology
+    is_a: Resource
+
+  AssociationResource:
+    description: >-
+      A resource that points to a set of associations
+    is_a: Resource
+    attributes:
+      normalizers:
+        range: Normalizer
+        multivalued: true
+        inlined: true
+        description: >-
+          The subject normalizers used in the input specification
+
+  PrefixAlias:
+    description: >-
+      Maps a prefix from the canonical prefix to an alias used in a particular adapter
+    attributes:
+      prefix:
+        range: string
+        description: >-
+          The source prefix
+        key: true
+      alias:
+        range: string
+        description: >-
+          The target prefix
+
+  Normalizer:
+    description: >-
+      specification of how identifier fields in an association resource should be normalized
     attributes:
-      preserve_negated_associations:
-        range: boolean
-        description: |-
-          If true, then the parser will keep negated associations in the output.
-          If false, then the parser will remove negated associations from the output.
-      include_association_attributes:
-        range: boolean
-        description: |-
-          If true, then the parser will include non S/P/O properties as additional attributes.
-          This may result in slower parsing
-      
-
-slots:
-  subject:
-    description: The thing which the association is about.
-    slot_uri: rdf:subject
-    range: uriorcurie
-    exact_mappings:
-      - oa:hasBody
-  predicate:
-    description: The type of relationship between the subject and object.
-    slot_uri: rdf:predicate
-    range: uriorcurie
-  object:
-    description: An ontology entity that is associated with the subject.
-    slot_uri: rdf:object
-    range: uriorcurie
-    exact_mappings:
-      - oa:hasTarget
-  property_values:
-    multivalued: true
-    range: PropertyValue
-    inlined: true
-  group_object:
-    description: |-
-      An ontology entity that is the ancestor of the objects in the group's 
-      associations and sub-group associations.
-    slot_uri: rdf:object
-    range: uriorcurie
-  sub_groups:
-    description: Container for groups within a rollup group.
-    range: RollupGroup
-    multivalued: true
-    inlined_as_list: true
-  associations:
-    range: Association
-    multivalued: true
-    inlined_as_list: true
-  
+      selector:
+        range: string
+        description: >-
+          The selector of the normalizer
+      prefix_alias_map:
+        range: PrefixAlias
+        multivalued: true
+        inlined: true
+        description: >-
+          The prefix aliases used in the input specification
+      source_prefixes:
+        range: string
+        multivalued: true
+        description: >-
+          The prefixes to normalize to
+      target_prefixes:
+        range: string
+        multivalued: true
+        description: >-
+          The prefixes to normalize to
+      slots:
+        range: string
+        multivalued: true
+        description: >-
+          The slots to normalize
```

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/class_enrichment.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/class_enrichment.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/class_enrichment.py` & `oaklib-0.5.1/src/oaklib/datamodels/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/class_enrichment.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/cross_ontology_diff.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/cross_ontology_diff.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/cross_ontology_diff.py` & `oaklib-0.5.1/src/oaklib/datamodels/cross_ontology_diff.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/cross_ontology_diff.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/cross_ontology_diff.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/cx.py` & `oaklib-0.5.1/src/oaklib/datamodels/cx.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/cx.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/cx.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/fhir.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/fhir.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/fhir.py` & `oaklib-0.5.1/src/oaklib/datamodels/fhir.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/fhir.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/fhir.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/item_list.py` & `oaklib-0.5.1/src/oaklib/datamodels/item_list.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from item_list.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-04-10T09:39:02
+# Generation date: 2023-04-10T16:46:21
 # Schema: itemList
 #
 # id: https://w3id.org/oak/item-list
 # description: A data model for representing simple lists of entities such as genes. The data model is based on
 #              the schema.org ItemList class.
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
@@ -57,15 +57,18 @@
 RDFS = CurieNamespace("rdfs", "http://example.org/UNKNOWN/rdfs/")
 SCHEMA = CurieNamespace("schema", "http://schema.org/")
 DEFAULT_ = ITEMLIST
 
 
 # Types
 
+
 # Class references
+class ListItemId(extended_str):
+    pass
 
 
 @dataclass
 class ItemListCollection(YAMLRoot):
     """
     a set of item lists
     """
@@ -104,20 +107,20 @@
     class_name: ClassVar[str] = "ItemList"
     class_model_uri: ClassVar[URIRef] = ITEMLIST.ItemList
 
     id: Optional[Union[str, URIorCURIE]] = None
     name: Optional[str] = None
     description: Optional[str] = None
     itemListElements: Optional[
-        Union[Union[dict, "ListItem"], List[Union[dict, "ListItem"]]]
+        Union[Union[str, ListItemId], List[Union[str, ListItemId]]]
     ] = empty_list()
     numberOfItems: Optional[Union[str, "ItemListOrderType"]] = None
     itemMetadataMap: Optional[
-        Union[Union[dict, "ListItem"], List[Union[dict, "ListItem"]]]
-    ] = empty_list()
+        Union[Dict[Union[str, ListItemId], Union[dict, "ListItem"]], List[Union[dict, "ListItem"]]]
+    ] = empty_dict()
     categories: Optional[Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]] = empty_list()
     keywords: Optional[Union[str, List[str]]] = empty_list()
     additionalType: Optional[
         Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]
     ] = empty_list()
     wasGeneratedBy: Optional[
         Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]
@@ -134,27 +137,23 @@
             self.description = str(self.description)
 
         if not isinstance(self.itemListElements, list):
             self.itemListElements = (
                 [self.itemListElements] if self.itemListElements is not None else []
             )
         self.itemListElements = [
-            v if isinstance(v, ListItem) else ListItem(**as_dict(v)) for v in self.itemListElements
+            v if isinstance(v, ListItemId) else ListItemId(v) for v in self.itemListElements
         ]
 
         if self.numberOfItems is not None and not isinstance(self.numberOfItems, ItemListOrderType):
             self.numberOfItems = ItemListOrderType(self.numberOfItems)
 
-        if not isinstance(self.itemMetadataMap, list):
-            self.itemMetadataMap = (
-                [self.itemMetadataMap] if self.itemMetadataMap is not None else []
-            )
-        self.itemMetadataMap = [
-            v if isinstance(v, ListItem) else ListItem(**as_dict(v)) for v in self.itemMetadataMap
-        ]
+        self._normalize_inlined_as_dict(
+            slot_name="itemMetadataMap", slot_type=ListItem, key_name="id", keyed=True
+        )
 
         if not isinstance(self.categories, list):
             self.categories = [self.categories] if self.categories is not None else []
         self.categories = [
             v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.categories
         ]
 
@@ -186,35 +185,37 @@
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = SCHEMA.ListItem
     class_class_curie: ClassVar[str] = "schema:ListItem"
     class_name: ClassVar[str] = "ListItem"
     class_model_uri: ClassVar[URIRef] = ITEMLIST.ListItem
 
-    id: Optional[str] = None
+    id: Union[str, ListItemId] = None
     idType: Optional[Union[str, URIorCURIE]] = None
     item: Optional[Union[dict, "Thing"]] = None
     position: Optional[int] = None
-    previousItem: Optional[Union[dict, "ListItem"]] = None
+    previousItem: Optional[Union[str, ListItemId]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.id is not None and not isinstance(self.id, str):
-            self.id = str(self.id)
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, ListItemId):
+            self.id = ListItemId(self.id)
 
         if self.idType is not None and not isinstance(self.idType, URIorCURIE):
             self.idType = URIorCURIE(self.idType)
 
         if self.item is not None and not isinstance(self.item, Thing):
             self.item = Thing(**as_dict(self.item))
 
         if self.position is not None and not isinstance(self.position, int):
             self.position = int(self.position)
 
-        if self.previousItem is not None and not isinstance(self.previousItem, ListItem):
-            self.previousItem = ListItem(**as_dict(self.previousItem))
+        if self.previousItem is not None and not isinstance(self.previousItem, ListItemId):
+            self.previousItem = ListItemId(self.previousItem)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class Thing(YAMLRoot):
     _inherited_slots: ClassVar[List[str]] = []
@@ -327,15 +328,15 @@
 
 slots.itemList__itemListElements = Slot(
     uri=SCHEMA.itemListElement,
     name="itemList__itemListElements",
     curie=SCHEMA.curie("itemListElement"),
     model_uri=ITEMLIST.itemList__itemListElements,
     domain=None,
-    range=Optional[Union[Union[dict, ListItem], List[Union[dict, ListItem]]]],
+    range=Optional[Union[Union[str, ListItemId], List[Union[str, ListItemId]]]],
 )
 
 slots.itemList__numberOfItems = Slot(
     uri=SCHEMA.numberOfItems,
     name="itemList__numberOfItems",
     curie=SCHEMA.curie("numberOfItems"),
     model_uri=ITEMLIST.itemList__numberOfItems,
@@ -345,15 +346,17 @@
 
 slots.itemList__itemMetadataMap = Slot(
     uri=ITEMLIST.itemMetadataMap,
     name="itemList__itemMetadataMap",
     curie=ITEMLIST.curie("itemMetadataMap"),
     model_uri=ITEMLIST.itemList__itemMetadataMap,
     domain=None,
-    range=Optional[Union[Union[dict, ListItem], List[Union[dict, ListItem]]]],
+    range=Optional[
+        Union[Dict[Union[str, ListItemId], Union[dict, ListItem]], List[Union[dict, ListItem]]]
+    ],
 )
 
 slots.itemList__categories = Slot(
     uri=DCTERMS.subject,
     name="itemList__categories",
     curie=DCTERMS.curie("subject"),
     model_uri=ITEMLIST.itemList__categories,
@@ -390,15 +393,15 @@
 
 slots.listItem__id = Slot(
     uri=ITEMLIST.id,
     name="listItem__id",
     curie=ITEMLIST.curie("id"),
     model_uri=ITEMLIST.listItem__id,
     domain=None,
-    range=Optional[str],
+    range=URIRef,
 )
 
 slots.listItem__idType = Slot(
     uri=ITEMLIST.idType,
     name="listItem__idType",
     curie=ITEMLIST.curie("idType"),
     model_uri=ITEMLIST.listItem__idType,
@@ -426,15 +429,15 @@
 
 slots.listItem__previousItem = Slot(
     uri=SCHEMA.previousItem,
     name="listItem__previousItem",
     curie=SCHEMA.curie("previousItem"),
     model_uri=ITEMLIST.listItem__previousItem,
     domain=None,
-    range=Optional[Union[dict, ListItem]],
+    range=Optional[Union[str, ListItemId]],
 )
 
 slots.thing__identifier = Slot(
     uri=SCHEMA.identifier,
     name="thing__identifier",
     curie=SCHEMA.curie("identifier"),
     model_uri=ITEMLIST.thing__identifier,
```

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/item_list.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/item_list.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -102,14 +102,15 @@
     class_uri: schema:ListItem
     attributes:
       id:
         range: string
         description: >
           The identifier of the item. Note this can be a 'proper' CURIE ID or any other unique field,
           for example symbol
+        key: true
       idType:
         range: uriorcurie
         description: >-
           The type of the identifier. For example, if the id is a symbol, this would be 'symbol'
         examples:
           - value: biolink:symbol
           - value: skos:prefLabel
```

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/lexical_index.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/lexical_index.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/lexical_index.py` & `oaklib-0.5.1/src/oaklib/datamodels/lexical_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/lexical_index.schema.json` & `oaklib-0.5.1/src/oaklib/datamodels/lexical_index.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/lexical_index.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/lexical_index.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/mapping_cluster_datamodel.py` & `oaklib-0.5.1/src/oaklib/datamodels/mapping_cluster_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/mapping_cluster_datamodel.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/mapping_cluster_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.py` & `oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from mapping_rules_datamodel.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-04-09T14:06:46
+# Generation date: 2023-04-12T14:50:11
 # Schema: mapping-rules-datamodel
 #
 # id: https://w3id.org/oak/mapping-rules-datamodel
 # description: A datamodel for specifying lexical mapping rules.
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
@@ -263,14 +263,16 @@
     class_model_uri: ClassVar[URIRef] = MAPPINGRULES.Synonymizer
 
     the_rule: Optional[str] = None
     match: Optional[str] = None
     match_scope: Optional[str] = None
     replacement: Optional[str] = None
     qualifier: Optional[str] = None
+    prefix: Optional[str] = None
+    tests: Optional[Union[dict, "Test"]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self.the_rule is not None and not isinstance(self.the_rule, str):
             self.the_rule = str(self.the_rule)
 
         if self.match is not None and not isinstance(self.match, str):
             self.match = str(self.match)
@@ -280,14 +282,46 @@
 
         if self.replacement is not None and not isinstance(self.replacement, str):
             self.replacement = str(self.replacement)
 
         if self.qualifier is not None and not isinstance(self.qualifier, str):
             self.qualifier = str(self.qualifier)
 
+        if self.prefix is not None and not isinstance(self.prefix, str):
+            self.prefix = str(self.prefix)
+
+        if self.tests is not None and not isinstance(self.tests, Test):
+            self.tests = Test(**as_dict(self.tests))
+
+        super().__post_init__(**kwargs)
+
+
+@dataclass
+class Test(YAMLRoot):
+    _inherited_slots: ClassVar[List[str]] = []
+
+    class_class_uri: ClassVar[URIRef] = MAPPINGRULES.Test
+    class_class_curie: ClassVar[str] = "mappingrules:Test"
+    class_name: ClassVar[str] = "Test"
+    class_model_uri: ClassVar[URIRef] = MAPPINGRULES.Test
+
+    input: Optional[str] = None
+    output: Optional[str] = None
+    prefix: Optional[str] = None
+
+    def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
+        if self.input is not None and not isinstance(self.input, str):
+            self.input = str(self.input)
+
+        if self.output is not None and not isinstance(self.output, str):
+            self.output = str(self.output)
+
+        if self.prefix is not None and not isinstance(self.prefix, str):
+            self.prefix = str(self.prefix)
+
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class LexicalIndex(YAMLRoot):
     """
     An index over an ontology keyed by lexical unit
@@ -726,14 +760,59 @@
     name="synonymizer__qualifier",
     curie=MAPPINGRULES.curie("qualifier"),
     model_uri=MAPPINGRULES.synonymizer__qualifier,
     domain=None,
     range=Optional[str],
 )
 
+slots.synonymizer__prefix = Slot(
+    uri=MAPPINGRULES.prefix,
+    name="synonymizer__prefix",
+    curie=MAPPINGRULES.curie("prefix"),
+    model_uri=MAPPINGRULES.synonymizer__prefix,
+    domain=None,
+    range=Optional[str],
+)
+
+slots.synonymizer__tests = Slot(
+    uri=MAPPINGRULES.tests,
+    name="synonymizer__tests",
+    curie=MAPPINGRULES.curie("tests"),
+    model_uri=MAPPINGRULES.synonymizer__tests,
+    domain=None,
+    range=Optional[Union[dict, Test]],
+)
+
+slots.test__input = Slot(
+    uri=MAPPINGRULES.input,
+    name="test__input",
+    curie=MAPPINGRULES.curie("input"),
+    model_uri=MAPPINGRULES.test__input,
+    domain=None,
+    range=Optional[str],
+)
+
+slots.test__output = Slot(
+    uri=MAPPINGRULES.output,
+    name="test__output",
+    curie=MAPPINGRULES.curie("output"),
+    model_uri=MAPPINGRULES.test__output,
+    domain=None,
+    range=Optional[str],
+)
+
+slots.test__prefix = Slot(
+    uri=MAPPINGRULES.prefix,
+    name="test__prefix",
+    curie=MAPPINGRULES.curie("prefix"),
+    model_uri=MAPPINGRULES.test__prefix,
+    domain=None,
+    range=Optional[str],
+)
+
 slots.lexicalIndex__groupings = Slot(
     uri=ONTOLEXINDEX.groupings,
     name="lexicalIndex__groupings",
     curie=ONTOLEXINDEX.curie("groupings"),
     model_uri=MAPPINGRULES.lexicalIndex__groupings,
     domain=None,
     range=Optional[
```

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.schema.json` & `oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.schema.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9924900793650794%*

 * *Differences: {"'$defs'": "{'LexicalTransformation': {'properties': {'params': {'type': 'array', 'items': "*

 * *            "OrderedDict([('$ref', '#/$defs/Any')])}}}, 'Precondition': {'properties': "*

 * *            "{'predicate_id_one_of': OrderedDict([('items', OrderedDict([('type', 'string')])), "*

 * *            "('type', 'array')])}}, 'Synonymizer': {'properties': {'prefix': "*

 * *            "OrderedDict([('description', 'The rule applies to nodes of a specific prefix.'), "*

 * *            "('type', 'string')]), 'tests': OrderedDict( […]*

```diff
@@ -1,9 +1,15 @@
 {
     "$defs": {
+        "Any": {
+            "additionalProperties": true,
+            "description": "",
+            "title": "Any",
+            "type": "object"
+        },
         "LexicalGrouping": {
             "additionalProperties": false,
             "description": "A grouping of ontology elements by a shared lexical term",
             "properties": {
                 "relationships": {
                     "description": "All ontology elements grouped and their relationship to the normalized term",
                     "items": {
@@ -66,15 +72,18 @@
         },
         "LexicalTransformation": {
             "additionalProperties": false,
             "description": "An atomic lexical transformation applied on a term (string) yielding a transformed string",
             "properties": {
                 "params": {
                     "description": "Any parameters to be applied to the transformation algorithm",
-                    "type": "string"
+                    "items": {
+                        "$ref": "#/$defs/Any"
+                    },
+                    "type": "array"
                 },
                 "type": {
                     "$ref": "#/$defs/TransformationType",
                     "description": "The type of transformation"
                 }
             },
             "title": "LexicalTransformation",
@@ -196,14 +205,20 @@
                 },
                 "object_source_one_of": {
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
+                "predicate_id_one_of": {
+                    "items": {
+                        "type": "string"
+                    },
+                    "type": "array"
+                },
                 "subject_match_field_one_of": {
                     "items": {
                         "type": "string"
                     },
                     "type": "array"
                 },
                 "subject_source_one_of": {
@@ -260,30 +275,58 @@
                     "description": "Reg-ex rule to match substrings in labels.",
                     "type": "string"
                 },
                 "match_scope": {
                     "description": "Scope of the reg-ex rule",
                     "type": "string"
                 },
+                "prefix": {
+                    "description": "The rule applies to nodes of a specific prefix.",
+                    "type": "string"
+                },
                 "qualifier": {
                     "description": "Type of match for the new synonym generated.",
                     "type": "string"
                 },
                 "replacement": {
                     "description": "Reg-ex rule to replace substrings in labels",
                     "type": "string"
                 },
+                "tests": {
+                    "$ref": "#/$defs/Test",
+                    "description": "Unit tests for each rules."
+                },
                 "the_rule": {
                     "description": "Description of the rule.",
                     "type": "string"
                 }
             },
             "title": "Synonymizer",
             "type": "object"
         },
+        "Test": {
+            "additionalProperties": false,
+            "description": "",
+            "properties": {
+                "input": {
+                    "description": "Input string for the rule.",
+                    "type": "string"
+                },
+                "output": {
+                    "description": "Output based on the rule.",
+                    "type": "string"
+                },
+                "prefix": {
+                    "description": "The prefix that qualifies for the rule.",
+                    "type": "string"
+                }
+            },
+            "title": "Test",
+            "type": "object"
+        },
         "TransformationType": {
             "description": "A controlled datamodels of the types of transformation that can be applied to",
             "enum": [
                 "Stemming",
                 "Lemmatization",
                 "WordOrderNormalization",
                 "Depluralization",
```

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/mapping_rules_datamodel.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -110,9 +110,25 @@
     match_scope:
       description: Scope of the reg-ex rule
       range: string
     replacement:
       description: Reg-ex rule to replace substrings in labels
       range: string
     qualifier:
-       description: Type of match for the new synonym generated.
-       range: string
+      description: Type of match for the new synonym generated.
+      range: string
+    prefix:
+      description: The rule applies to nodes of a specific prefix.
+      range: string
+    tests:
+      description: Unit tests for each rules.
+      range: Test
+  
+  Test:
+   attributes:
+    input:
+     description: Input string for the rule.
+    output:
+     description: Output based on the rule.
+    prefix:
+      description: The prefix that qualifies for the rule.
+
```

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/obograph.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/obograph.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/obograph.py` & `oaklib-0.5.1/src/oaklib/datamodels/obograph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/obograph.schema.json` & `oaklib-0.5.1/src/oaklib/datamodels/obograph.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/obograph.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/obograph.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.py` & `oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.schema.json` & `oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/ontology_metadata.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/oxo.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/oxo.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/oxo.py` & `oaklib-0.5.1/src/oaklib/datamodels/oxo.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/oxo.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/oxo.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/search.py` & `oaklib-0.5.1/src/oaklib/datamodels/search.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/search_datamodel.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/search_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/search_datamodel.py` & `oaklib-0.5.1/src/oaklib/datamodels/search_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/search_datamodel.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/search_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/similarity.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/similarity.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/similarity.py` & `oaklib-0.5.1/src/oaklib/datamodels/similarity.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/similarity.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/similarity.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.py` & `oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.schema.json` & `oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/summary_statistics_datamodel.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/taxon_constraints.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/taxon_constraints.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/taxon_constraints.py` & `oaklib-0.5.1/src/oaklib/datamodels/taxon_constraints.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/taxon_constraints.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/taxon_constraints.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/text_annotator.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/text_annotator.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/text_annotator.py` & `oaklib-0.5.1/src/oaklib/datamodels/text_annotator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/text_annotator.schema.json` & `oaklib-0.5.1/src/oaklib/datamodels/text_annotator.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/text_annotator.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/text_annotator.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.py` & `oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.schema.json` & `oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/validation_datamodel.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/value_set_configuration.owl.ttl` & `oaklib-0.5.1/src/oaklib/datamodels/value_set_configuration.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/value_set_configuration.py` & `oaklib-0.5.1/src/oaklib/datamodels/value_set_configuration.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/value_set_configuration.yaml` & `oaklib-0.5.1/src/oaklib/datamodels/value_set_configuration.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/datamodels/vocabulary.py` & `oaklib-0.5.1/src/oaklib/datamodels/vocabulary.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/__init__.py` & `oaklib-0.5.1/src/oaklib/implementations/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/aggregator/aggregator_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/aggregator/aggregator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/cx/cx_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/cx/cx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/funowl/funowl_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/funowl/funowl_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/gilda.py` & `oaklib-0.5.1/src/oaklib/implementations/gilda.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/kgx/kgx_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/kgx/kgx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/obograph/obograph_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/obograph/obograph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/ols/ols_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/ols/ols_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/ols/oxo_utils.py` & `oaklib-0.5.1/src/oaklib/implementations/ols/oxo_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/ontobee/ontobee_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/ontobee/ontobee_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/ontoportal/bioportal_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/ontoportal/bioportal_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py` & `oaklib-0.5.1/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/pronto/pronto_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/pronto/pronto_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 from oaklib.interfaces.semsim_interface import SemanticSimilarityInterface
 from oaklib.interfaces.summary_statistics_interface import SummaryStatisticsInterface
 from oaklib.interfaces.taxon_constraint_interface import TaxonConstraintInterface
 from oaklib.interfaces.validator_interface import ValidatorInterface
 from oaklib.resource import OntologyResource
 from oaklib.types import CURIE, SUBSET_CURIE
 from oaklib.utilities.kgcl_utilities import tidy_change_object
+from oaklib.utilities.mapping.sssom_utils import inject_mapping_sources
 
 warnings.filterwarnings("ignore", category=pronto.warnings.SyntaxWarning, module="pronto")
 
 
 def _synonym_scope_pred(s: pronto.Synonym) -> str:
     scope = s.scope.upper()
     if scope in SCOPE_TO_SYNONYM_PRED_MAP:
@@ -602,44 +603,54 @@
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
     def sssom_mappings(
         self, curies: Optional[Union[CURIE, Iterable[CURIE]]] = None, source: Optional[str] = None
     ) -> Iterable[sssom.Mapping]:
         if isinstance(curies, CURIE):
             curies = [curies]
+        elif curies is None:
+            curies = list(self.entities())
         else:
             curies = list(curies)
         # mappings where curie is the subject:
         for curie in curies:
             t = self._entity(curie)
             if t:
                 for x in t.xrefs:
-                    yield sssom.Mapping(
+                    m = sssom.Mapping(
                         subject_id=t.id,
                         predicate_id=SKOS_CLOSE_MATCH,
                         object_id=x.id,
                         mapping_justification=sssom.EntityReference(
                             SEMAPV.UnspecifiedMatching.value
                         ),
                     )
+                    inject_mapping_sources(m)
+                    if source and m.object_source != source and m.subject_source != source:
+                        continue
+                    yield m
         # mappings where curie is the object:
         # TODO: use a cache to avoid re-calculating
         for e in self.entities():
             t = self._entity(e)
             if t:
                 for x in t.xrefs:
                     if x.id in curies:
-                        yield sssom.Mapping(
+                        m = sssom.Mapping(
                             subject_id=e,
                             predicate_id=SKOS_CLOSE_MATCH,
                             object_id=x.id,
                             mapping_justification=sssom.EntityReference(
                                 SEMAPV.UnspecifiedMatching.value
                             ),
                         )
+                        inject_mapping_sources(m)
+                        if source and m.object_source != source and m.subject_source != source:
+                            continue
+                        yield m
 
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     # Implements: OboGraphInterface
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
     def node(self, curie: CURIE, strict=False, include_metadata=False) -> obograph.Node:
         t = self._entity(curie)
@@ -833,14 +844,18 @@
             else:
                 self.create_entity(patch.node_id, patch.name)
         elif isinstance(patch, kgcl.SynonymReplacement):
             t = self._entity(patch.about_node, strict=True)
             for syn in t.synonyms:
                 if syn.description == patch.old_value:
                     syn.description = patch.new_value
+        elif isinstance(patch, kgcl.NewTextDefinition):
+            t = self._entity(patch.about_node, strict=True)
+            xrefs = t.definition.xrefs if t.definition else []
+            t.definition = pronto.Definition(patch.new_value, xrefs=xrefs)
         elif isinstance(patch, kgcl.NodeTextDefinitionChange):
             t = self._entity(patch.about_node, strict=True)
             xrefs = t.definition.xrefs if t.definition else []
             t.definition = pronto.Definition(patch.new_value, xrefs=xrefs)
         elif isinstance(patch, kgcl.NewSynonym):
             t = self._entity(patch.about_node, strict=True)
             # Get scope from patch.qualifier
```

### Comparing `oaklib-0.5.0/src/oaklib/implementations/simpleobo/simple_obo_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/simpleobo/simple_obo_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,14 +106,15 @@
 from oaklib.interfaces.search_interface import SearchInterface
 from oaklib.interfaces.summary_statistics_interface import SummaryStatisticsInterface
 from oaklib.interfaces.taxon_constraint_interface import TaxonConstraintInterface
 from oaklib.interfaces.validator_interface import ValidatorInterface
 from oaklib.resource import OntologyResource
 from oaklib.types import CURIE, PRED_CURIE, SUBSET_CURIE
 from oaklib.utilities.kgcl_utilities import tidy_change_object
+from oaklib.utilities.mapping.sssom_utils import inject_mapping_sources
 
 
 def _is_isa(x: str):
     return x == IS_A or x.lower() == "is_a" or x.lower() == "isa"
 
 
 @dataclass
@@ -623,31 +624,35 @@
     # Implements: MappingsInterface
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
     def get_sssom_mappings_by_curie(self, curie: Union[str, CURIE]) -> Iterator[sssom.Mapping]:
         s = self._stanza(curie, strict=False)
         if s:
             for x in s.simple_values(TAG_XREF):
-                yield sssom.Mapping(
+                m = sssom.Mapping(
                     subject_id=curie,
                     predicate_id=SKOS_CLOSE_MATCH,
                     object_id=x,
                     mapping_justification=sssom.EntityReference(SEMAPV.UnspecifiedMatching.value),
                 )
+                inject_mapping_sources(m)
+                yield m
         # TODO: use a cache to avoid re-calculating
         for _, stanza in self.obo_document.stanzas.items():
             if len(stanza.simple_values(TAG_XREF)) > 0:
                 for x in stanza.simple_values(TAG_XREF):
                     if x == curie:
-                        yield sssom.Mapping(
+                        m = sssom.Mapping(
                             subject_id=stanza.id,
                             predicate_id=SKOS_CLOSE_MATCH,
                             object_id=curie,
                             mapping_justification=SEMAPV.UnspecifiedMatching.value,
                         )
+                        inject_mapping_sources(m)
+                        yield m
 
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     # Implements: OboGraphInterface
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
     def node(self, curie: CURIE, strict=False, include_metadata=False) -> obograph.Node:
         t = self._stanza(curie, strict=False)
@@ -798,20 +803,21 @@
                         tv.replace_quoted_part(patch.new_value)
                         n += 1
             if not n:
                 raise ValueError(f"Failed to find synonym {patch.old_value} for {t.id}")
             modified_entities.append(patch.about_node)
         elif isinstance(patch, kgcl.NewTextDefinition):
             t = self._stanza(patch.about_node, strict=True)
-            t.add_tag_value(TAG_DEFINITION, patch.new_value)
+            t.add_quoted_tag_value(TAG_DEFINITION, patch.new_value.strip("'"), xrefs=[])
             modified_entities.append(patch.about_node)
         elif isinstance(patch, kgcl.NodeTextDefinitionChange):
             t = self._stanza(patch.about_node, strict=True)
             for tv in t.tag_values:
                 if tv.tag == TAG_DEFINITION:
+                    # The strip() portion is to handle a KGCL bug
                     tv.replace_quoted_part(patch.new_value.strip("'"))
         elif isinstance(patch, kgcl.NewSynonym):
             t = self._stanza(patch.about_node, strict=True)
             # Get scope from patch.qualifier
             # rather than forcing all synonyms to be related.
             if type(patch.qualifier) == str:
                 scope = patch.qualifier.upper()
```

### Comparing `oaklib-0.5.0/src/oaklib/implementations/simpleobo/simple_obo_parser.py` & `oaklib-0.5.1/src/oaklib/implementations/simpleobo/simple_obo_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -516,14 +516,24 @@
 
         :param tag:
         :param val:
         :return:
         """
         self.tag_values.append(TagValue(tag, val))
 
+    def add_quoted_tag_value(self, tag: TAG, val: str, xrefs: List[str]) -> None:
+        """
+        Adds a tag-value pair
+
+        :param tag:
+        :param val:
+        :return:
+        """
+        self.tag_values.append(TagValue(tag, f"\"{val}\" [{','.join(xrefs)}]"))
+
     def add_tag_value_pair(self, tag: TAG, val1: str, val2: str) -> None:
         """
         Adds a tag-value pair where the value is a pair
 
         :param tag:
         :param val1:
         :param val2:
```

### Comparing `oaklib-0.5.0/src/oaklib/implementations/sparql/abstract_sparql_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/sparql/abstract_sparql_implementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -45,15 +45,18 @@
     RELATIONSHIP_MAP,
 )
 from oaklib.interfaces.dumper_interface import DumperInterface
 from oaklib.interfaces.rdf_interface import RDF_TRIPLE, TRIPLE, RdfInterface
 from oaklib.resource import OntologyResource
 from oaklib.types import CURIE, URI
 from oaklib.utilities.basic_utils import pairs_as_dict
-from oaklib.utilities.mapping.sssom_utils import create_sssom_mapping
+from oaklib.utilities.mapping.sssom_utils import (
+    create_sssom_mapping,
+    inject_mapping_sources,
+)
 from oaklib.utilities.rate_limiter import check_limit
 
 VAL_VAR = "v"
 
 
 def _sparql_values(var_name: str, vals: List[str]):
     if vals is None:
@@ -794,14 +797,15 @@
             m = create_sssom_mapping(
                 subject_id=curie,
                 predicate_id=self.uri_to_curie(row["p"]["value"]),
                 object_id=self.uri_to_curie(row["o"]["value"]),
                 mapping_justification=SEMAPV.UnspecifiedMatching.value,
             )
             if m is not None:
+                inject_mapping_sources(m)
                 yield m
         # input curie is object
         query = SparqlQuery(
             select=["?s", "?p"],
             where=[
                 "?s ?p ?o",
                 _sparql_values(
@@ -820,14 +824,15 @@
             m = create_sssom_mapping(
                 subject_id=self.uri_to_curie(row["s"]["value"]),
                 predicate_id=self.uri_to_curie(row["p"]["value"]),
                 object_id=curie,
                 mapping_justification=SEMAPV.UnspecifiedMatching.value,
             )
             if m is not None:
+                inject_mapping_sources(m)
                 yield m
 
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     # Implements: RdfInterface
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
     def extract_triples(
```

### Comparing `oaklib-0.5.0/src/oaklib/implementations/sparql/lov_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/sparql/lov_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/sparql/oak_metamodel_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/sparql/oak_metamodel_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/sparql/sparql_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/sparql/sparql_implementation.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,28 +4,32 @@
 import rdflib
 
 from oaklib import BasicOntologyInterface
 from oaklib.implementations.sparql.abstract_sparql_implementation import (
     AbstractSparqlImplementation,
 )
 from oaklib.interfaces import TextAnnotatorInterface
+from oaklib.interfaces.association_provider_interface import (
+    AssociationProviderInterface,
+)
 from oaklib.interfaces.differ_interface import DifferInterface
 from oaklib.interfaces.mapping_provider_interface import MappingProviderInterface
 from oaklib.interfaces.merge_interface import MergeConfiguration, MergeInterface
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.interfaces.patcher_interface import PatcherInterface
 from oaklib.interfaces.rdf_interface import RdfInterface
 from oaklib.interfaces.search_interface import SearchInterface
 from oaklib.interfaces.semsim_interface import SemanticSimilarityInterface
 from oaklib.interfaces.taxon_constraint_interface import TaxonConstraintInterface
 
 
 @dataclass
 class SparqlImplementation(
     AbstractSparqlImplementation,
+    AssociationProviderInterface,
     RdfInterface,
     DifferInterface,
     SearchInterface,
     MappingProviderInterface,
     OboGraphInterface,
     PatcherInterface,
     SemanticSimilarityInterface,
```

### Comparing `oaklib-0.5.0/src/oaklib/implementations/sparql/sparql_query.py` & `oaklib-0.5.1/src/oaklib/implementations/sparql/sparql_query.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/sqldb/sql_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/sqldb/sql_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,15 @@
     SYNONYM_PREDICATES,
     TERM_REPLACED_BY,
     TERMS_MERGED,
     omd_slots,
 )
 from oaklib.implementations.sqldb import SEARCH_CONFIG
 from oaklib.interfaces import SubsetterInterface, TextAnnotatorInterface
+from oaklib.interfaces.association_provider_interface import EntityNormalizer
 from oaklib.interfaces.basic_ontology_interface import (
     ALIAS_MAP,
     DEFINITION,
     LANGUAGE_TAG,
     METADATA_MAP,
     PRED_CURIE,
     PREFIX_MAP,
@@ -1183,18 +1184,22 @@
                 logging.info(f"Object subquery: {q} // {object_closure_predicates}")
                 q = q.filter(TermAssociation.object.in_(subquery))
             else:
                 q = q.filter(TermAssociation.object.in_(tuple(objects)))
         logging.info(f"Association query: {q}")
         return q
 
-    def add_associations(self, associations: Iterable[Association]) -> bool:
+    def add_associations(
+        self, associations: Iterable[Association], normalizers: List[EntityNormalizer] = None
+    ) -> bool:
         if not self.can_store_associations:
-            return super().add_associations(associations)
+            return super().add_associations(associations, normalizers=normalizers)
         for a in associations:
+            if normalizers:
+                a = a.normalize(normalizers)
             if a.property_values:
                 raise NotImplementedError
             stmt = insert(TermAssociation).values(
                 subject=a.subject, predicate=a.predicate, object=a.object
             )
             self._execute(stmt)
         self.session.flush()
@@ -1551,45 +1556,61 @@
                     raise ValueError(f"not a CURIE: {v}")
 
     def sssom_mappings(
         self, curies: Optional[Union[CURIE, Iterable[CURIE]]] = None, source: Optional[str] = None
     ) -> Iterator[Mapping]:
         if isinstance(curies, CURIE):
             curies = [curies]
-        else:
+        elif curies is not None:
             curies = list(curies)
         justification = str(SEMAPV.UnspecifiedMatching.value)
         predicates = tuple(ALL_MATCH_PREDICATES)
         base_query = self.session.query(Statements).filter(Statements.predicate.in_(predicates))
-        for row in base_query.filter(Statements.subject.in_(curies)):
+        if curies is None:
+            by_subject_query = base_query
+        else:
+            by_subject_query = base_query.filter(Statements.subject.in_(curies))
+        for row in by_subject_query:
             mpg = Mapping(
                 subject_id=row.subject,
                 object_id=row.value if row.value is not None else row.object,
                 predicate_id=row.predicate,
                 mapping_justification=justification,
             )
-            yield inject_mapping_sources(mpg)
+            inject_mapping_sources(mpg)
+            if source and mpg.subject_source != source and mpg.object_source != source:
+                continue
+            yield mpg
+        if curies is None:
+            # all mappings have been returned
+            return
         # xrefs are stored as literals
         for row in base_query.filter(Statements.value.in_(curies)):
             mpg = Mapping(
                 subject_id=row.subject,
                 object_id=row.value,
                 predicate_id=row.predicate,
                 mapping_justification=justification,
             )
-            yield inject_mapping_sources(mpg)
+            inject_mapping_sources(mpg)
+            if source and mpg.subject_source != source and mpg.object_source != source:
+                continue
+            yield mpg
         # skos mappings are stored as objects
         for row in base_query.filter(Statements.object.in_(curies)):
             mpg = Mapping(
                 subject_id=row.subject,
                 object_id=row.object,
                 predicate_id=row.predicate,
                 mapping_justification=justification,
             )
-            yield inject_mapping_sources(mpg)
+            inject_mapping_sources(mpg)
+            if source and mpg.subject_source != source and mpg.object_source != source:
+                continue
+            yield mpg
 
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     # Implements: ValidatorInterface
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
     def validate(
         self, configuration: vdm.ValidationConfiguration = None
```

### Comparing `oaklib-0.5.0/src/oaklib/implementations/sqldb/sqlite_utils.py` & `oaklib-0.5.1/src/oaklib/implementations/sqldb/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/translator/translator_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/translator/translator_implementation.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         else:
             curies = list(curies)
         r = requests.get(NODE_NORMALIZER_ENDPOINT, params={"curie": curies, "conflate": "false"})
         non_conflated_results = r.json()
         r = requests.get(NODE_NORMALIZER_ENDPOINT, params={"curie": curies, "conflate": "true"})
         results = r.json()
         objects = set()
+        subjects = set()
         if "detail" in results:
             if results["detail"] == "Not found.":
                 return
         for curie, data in results.items():
             if not data:
                 logging.info(f"No results for {curie} in {curies}")
                 continue
@@ -77,15 +78,19 @@
                     subject_label=label,
                     predicate_id=pred,
                     object_id=object_id,
                     object_label=x.get("label", None),
                     mapping_justification=str(SEMAPV.ManualMappingCuration.value),
                 )
                 inject_mapping_sources(m)
+                if source:
+                    if m.object_source != source:
+                        continue
                 yield m
                 objects.add(object_id)
+                subjects.add(curie)
         for curie in curies:
-            if curie not in objects:
+            if curie not in subjects:
                 logging.warning(f"Could not find any mappings for {curie}")
 
     def inject_mapping_labels(self, mappings: Iterable[Mapping]) -> None:
         return
```

### Comparing `oaklib-0.5.0/src/oaklib/implementations/ubergraph/ubergraph_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/ubergraph/ubergraph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/uniprot/uniprot_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/uniprot/uniprot_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/implementations/wikidata/wikidata_implementation.py` & `oaklib-0.5.1/src/oaklib/implementations/wikidata/wikidata_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/__init__.py` & `oaklib-0.5.1/src/oaklib/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/basic_ontology_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/basic_ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/class_enrichment_calculation_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/class_enrichment_calculation_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from abc import ABC
 from dataclasses import dataclass
 from typing import Iterable, Iterator, List, Optional
 
 from oaklib.datamodels.association import Association
 from oaklib.datamodels.class_enrichment import ClassEnrichmentResult
+from oaklib.datamodels.item_list import ItemList
 from oaklib.datamodels.vocabulary import EQUIVALENT_CLASS
 from oaklib.interfaces.association_provider_interface import (
     AssociationProviderInterface,
 )
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.types import CURIE, PRED_CURIE
 from oaklib.utilities.stats.hypergeometric import hypergeometric_p_value
@@ -23,15 +24,16 @@
 
     for example: to
     test for over representation of a disease in a set of genes.
     """
 
     def enriched_classes(
         self,
-        subjects: Iterable[CURIE],
+        subjects: Optional[Iterable[CURIE]] = None,
+        item_list: Optional[ItemList] = None,
         predicates: Iterable[CURIE] = None,
         object_closure_predicates: Optional[List[PRED_CURIE]] = None,
         background: Iterable[CURIE] = None,
         hypotheses: Iterable[CURIE] = None,
         cutoff=0.05,
         autolabel=False,
         filter_redundant=False,
@@ -48,24 +50,33 @@
         ...    assert result.p_value < 0.05
         ...    print(f"{result.class_id} {result.class_label}")
         <BLANKLINE>
         GO:0006620 post-translational protein targeting to endoplasmic reticulum membrane
         ...
 
         :param subjects: The set of entities to test for over-representation of classes
+        :param item_list: An item list objects as an alternate way to specify subjects
         :param background: The set of entities to use as a background for the test (recommended)
         :param hypotheses: The set of classes to test for over-representation (default is all)
         :param cutoff: The threshold to use for p-value
         :param labels: Whether to include labels (names) for the classes
         :param direction: The direction of the test. One of 'greater', 'less', 'two-sided'
         :param filter_redundant: Whether to filter out redundant hypotheses
         :param sort_by: The field to sort by. One of 'p_value', 'sample_count', 'background_count', 'odds_ratio'
         :param direction: The direction of the test. One of 'greater', 'less', 'two-sided'
         :return: An iterator over ClassEnrichmentResult objects
         """
+        if subjects and item_list:
+            raise ValueError("Only one of subjects or item_list may be provided")
+        if subjects is None:
+            if not item_list:
+                raise ValueError("Either subjects or item_list must be provided")
+            if not item_list.itemListElements:
+                raise ValueError("item_list must not be empty")
+            subjects = item_list.itemListElements
         subjects = list(subjects)
         sample_size = len(subjects)
         logging.info(f"Calculating sample_counts for {sample_size} subjects")
         if not sample_size:
             raise ValueError("No subjects provided")
         sample_count = {
             k: v
```

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/differ_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/differ_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/dumper_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/dumper_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/merge_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/merge_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/metadata_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/metadata_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/obograph_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/obograph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/obolegacy_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/obolegacy_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/ontology_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/owl_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/owl_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/patcher_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/patcher_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/rdf_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/rdf_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/relation_graph_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/relation_graph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/search_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/semsim_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/semsim_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/skos_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/skos_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/subsetter_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/subsetter_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/summary_statistics_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/summary_statistics_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/taxon_constraint_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/taxon_constraint_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/text_annotator_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/text_annotator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/interfaces/validator_interface.py` & `oaklib-0.5.1/src/oaklib/interfaces/validator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/heatmap_writer.py` & `oaklib-0.5.1/src/oaklib/io/heatmap_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/html_writer.py` & `oaklib-0.5.1/src/oaklib/io/html_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/obograph_writer.py` & `oaklib-0.5.1/src/oaklib/io/obograph_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/rollup_report_writer.py` & `oaklib-0.5.1/src/oaklib/io/rollup_report_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_axiom_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_axiom_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_csv_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_csv_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_fhir_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_fhir_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_info_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_info_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_json_lines_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_json_lines_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_json_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_kgcl_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_kgcl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_markdown_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_markdown_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_nl_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_nl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_obo_json_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_obo_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_obo_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_obo_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_owl_functional_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_owl_functional_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_rdf_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/io/streaming_yaml_writer.py` & `oaklib-0.5.1/src/oaklib/io/streaming_yaml_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/mappers/base_mapper.py` & `oaklib-0.5.1/src/oaklib/mappers/base_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/mappers/ontology_metadata_mapper.py` & `oaklib-0.5.1/src/oaklib/mappers/ontology_metadata_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/parsers/__init__.py` & `oaklib-0.5.1/src/oaklib/parsers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,52 @@
 from functools import cache
 
 from class_resolver import ClassResolver
 
 from oaklib.parsers.association_parser import AssociationParser
 from oaklib.parsers.gaf_association_parser import GafAssociationParser
+from oaklib.parsers.gencc_association_parser import GenCCAssociationParser
 from oaklib.parsers.hpoa_association_parser import HpoaAssociationParser
+from oaklib.parsers.hpoa_g2p_association_parser import HpoaG2PAssociationParser
+from oaklib.parsers.mim2gene_association_parser import MedgenMimG2DAssociationParser
+from oaklib.parsers.pairwise_association_parser import PairwiseAssociationParser
 from oaklib.parsers.phaf_association_parser import PhafAssociationParser
 
 __all__ = [
     "get_association_parser_resolver",
     # Concrete classes
     "AssociationParser",
     "PairwiseAssociationParser",
     "GafAssociationParser",
+    "GenCCAssociationParser",
     "HpoaAssociationParser",
     "HpoaG2PAssociationParser",
     "PhafAssociationParser",
+    "MedgenMimG2DAssociationParser",
 ]
 
-from oaklib.parsers.hpoa_g2p_association_parser import HpoaG2PAssociationParser
-from oaklib.parsers.pairwise_association_parser import PairwiseAssociationParser
 
 GAF = "gaf"
 """Gene Ontology GAF syntax"""
 
 G2T = "g2t"
 """Simple pairwise gene to term 2 column syntax"""
 
 HPOA = "hpoa"
 """HPO Annotation syntax"""
 
 HPOA_G2P = "hpoa_g2p"
 """HPO Gene-to-Phenotype syntax"""
 
+GENCC = "gencc"
+"""GenCC CSV format"""
+
+MEDGEN_MIM_G2D = "medgen_mim_g2d"
+"""Medgen/NCBI MIM G2D format"""
+
 KGX = "kgx"
 """KGX TSV syntax"""
 
 PHAF = "phaf"
 """PomBase Phenotype Association Format"""
 
 
@@ -54,11 +64,13 @@
     association_parser_resolver.synonyms.update(
         {
             GAF: GafAssociationParser,
             HPOA: HpoaAssociationParser,
             G2T: PairwiseAssociationParser,
             HPOA_G2P: HpoaG2PAssociationParser,
             PHAF: PhafAssociationParser,
+            GENCC: GenCCAssociationParser,
+            MEDGEN_MIM_G2D: MedgenMimG2DAssociationParser,
         }
     )
 
     return association_parser_resolver
```

### Comparing `oaklib-0.5.0/src/oaklib/parsers/association_parser.py` & `oaklib-0.5.1/src/oaklib/parsers/association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/parsers/association_parser_factory.py` & `oaklib-0.5.1/src/oaklib/parsers/association_parser_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/parsers/boomer_parser.py` & `oaklib-0.5.1/src/oaklib/parsers/boomer_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/parsers/gaf_association_parser.py` & `oaklib-0.5.1/src/oaklib/parsers/gaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/parsers/hpoa_association_parser.py` & `oaklib-0.5.1/src/oaklib/parsers/hpoa_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/parsers/hpoa_g2p_association_parser.py` & `oaklib-0.5.1/src/oaklib/parsers/hpoa_g2p_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/parsers/kgx_association_parser.py` & `oaklib-0.5.1/src/oaklib/parsers/kgx_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/parsers/pairwise_association_parser.py` & `oaklib-0.5.1/src/oaklib/parsers/pairwise_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/parsers/parser_base.py` & `oaklib-0.5.1/src/oaklib/parsers/parser_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/parsers/phaf_association_parser.py` & `oaklib-0.5.1/src/oaklib/parsers/phaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/parsers/xaf_association_parser.py` & `oaklib-0.5.1/src/oaklib/parsers/xaf_association_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 
     comment_character: str = field(default_factory=lambda: "!")
     """
     Character that indicates a comment line.
     Comment lines should be at the beginning of the file. They may include metadata that can be parsed
     """
 
+    delimiter: str = field(default_factory=lambda: "\t")
+    """
+    Delimiter
+    """
+
     subject_prefix = None
     """
     Prefix to use for subjects that do not have a prefix. This is prepended onto the subject_prefix_column
     If not specified, then EITHER subject_prefix_column MUST be specified, OR subject_column MUST be a CURIE
     """
 
     subject_prefix_column: Optional[ColumnReference] = None
```

### Comparing `oaklib-0.5.0/src/oaklib/resource.py` & `oaklib-0.5.1/src/oaklib/resource.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/selector.py` & `oaklib-0.5.1/src/oaklib/selector.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 import gzip
 import io
 import logging
 import os
 from pathlib import Path
-from typing import Optional, Type, Union
+from typing import List, Optional, Type, Union
 
 import requests
 from deprecation import deprecated
 from linkml_runtime.loaders import yaml_loader
 
 from oaklib import BasicOntologyInterface
 from oaklib import datamodels as datamodels_package
-from oaklib.datamodels.input_specification import InputSpecification
+from oaklib.datamodels.input_specification import InputSpecification, Normalizer
 from oaklib.implementations.funowl.funowl_implementation import FunOwlImplementation
 from oaklib.interfaces import OntologyInterface
 from oaklib.interfaces.association_provider_interface import (
     AssociationProviderInterface,
+    EntityNormalizer,
 )
 from oaklib.parsers.association_parser_factory import get_association_parser
 from oaklib.resource import OntologyResource
 
 RDF_SUFFIX_TO_FORMAT = {
     "ttl": "turtle",
     "nt": "ntriples",
@@ -36,14 +37,26 @@
     "hpoa_g2p": (
         [],
         "hpoa_g2p",
         "http://purl.obolibrary.org/obo/hp/hpoa/genes_to_phenotype.txt",
         False,
     ),
     "gaf": (["group"], "gaf", "http://current.geneontology.org/annotations/{group}.gaf.gz", True),
+    "gencc": (
+        [],
+        "gencc",
+        "https://search.thegencc.org/download/action/submissions-export-csv",
+        False,
+    ),
+    "medgen_mim_g2d": (
+        [],
+        "medgen_mim_g2d",
+        "http://ftp.ncbi.nih.gov/gene/DATA/mim2gene_medgen",
+        False,
+    ),
 }
 
 
 def get_adapter(
     descriptor: Union[str, Path, InputSpecification], format: str = None
 ) -> BasicOntologyInterface:
     """
@@ -116,40 +129,55 @@
     :param input_specification:
     :return:
     """
     if not input_specification.ontology_resources:
         raise ValueError("No ontology resources specified")
     if len(input_specification.ontology_resources) == 1:
         r = list(input_specification.ontology_resources.values())[0]
-        adapter = get_adapter(r.selector)
+        adapter = get_adapter(str(r.selector))
     else:
         from oaklib.implementations import AggregatorImplementation
 
         adapter = AggregatorImplementation(
             implementations=[
                 get_adapter(r.selector) for r in input_specification.ontology_resources.values()
             ]
         )
     if input_specification.association_resources:
         if not isinstance(adapter, AssociationProviderInterface):
             raise ValueError(f"Adapter {adapter} does not support associations")
         for r in input_specification.association_resources.values():
-            add_associations(adapter, r.selector, r.format)
+            normalizers = [
+                EntityNormalizer(
+                    adapter=get_adapter(n.selector),
+                    source_prefixes=n.source_prefixes,
+                    target_prefixes=n.target_prefixes,
+                    slots=n.slots,
+                    prefix_alias_map={str(k): str(v.alias) for k, v in n.prefix_alias_map.items()},
+                )
+                for n in r.normalizers
+            ]
+            logging.info(f"Normalizers: {normalizers}")
+            add_associations(adapter, r.selector, r.format, normalizers)
     return adapter
 
 
 def add_associations(
-    adapter: AssociationProviderInterface, descriptor: str, format: str = None
+    adapter: AssociationProviderInterface,
+    descriptor: str,
+    format: str = None,
+    normalizers: List[Normalizer] = None,
 ) -> None:
     """
     Adds associations to an adapter.
 
     :param adapter:
     :param descriptor:
     :param format:
+    :param normalizers:
     :return:
     """
     # TODO: do more robust windows check
     if ":" in descriptor and not descriptor.startswith("file:") and not descriptor[1] == ":":
         scheme, path = descriptor.split(":", 1)
         if scheme not in ASSOCIATION_REGISTRY:
             raise ValueError(f"Unknown association scheme: {scheme}")
@@ -164,24 +192,31 @@
         if compressed:
             file = file_from_gzip_url(url)
         else:
             file = file_from_url(url)
         association_parser = get_association_parser(format)
         logging.info(f"Adding associations from {path}")
         assocs = association_parser.parse(file)
-        adapter.add_associations(assocs)
+        adapter.add_associations(assocs, normalizers=normalizers)
         return
     if not format:
-        format = descriptor.split(".")[-1]
+        toks = descriptor.split(".")
+        while toks:
+            format = toks[-1]
+            if format not in ("csv", "tsv", "txt"):
+                break
+            toks = toks[:-1]
+    if not format:
+        raise ValueError(f"Could not determine format from descriptor {descriptor}")
     association_parser = get_association_parser(format)
     path = descriptor
     with open(path) as file:
         logging.info(f"Adding associations from {path}")
         assocs = association_parser.parse(file)
-        adapter.add_associations(assocs)
+        adapter.add_associations(assocs, normalizers=normalizers)
 
 
 def file_from_gzip_url(url, is_compressed=False):
     with requests.get(url, stream=True) as response:
         response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
         # Wrap the response's raw stream in a binary file-like object
         binary_file_like_object = io.BytesIO(response.raw.read())
```

### Comparing `oaklib-0.5.0/src/oaklib/utilities/apikey_manager.py` & `oaklib-0.5.1/src/oaklib/utilities/apikey_manager.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/associations/association_differ.py` & `oaklib-0.5.1/src/oaklib/utilities/associations/association_differ.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/associations/association_index.py` & `oaklib-0.5.1/src/oaklib/utilities/associations/association_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/basic_utils.py` & `oaklib-0.5.1/src/oaklib/utilities/basic_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/graph/networkx_bridge.py` & `oaklib-0.5.1/src/oaklib/utilities/graph/networkx_bridge.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/graph/relationship_walker.py` & `oaklib-0.5.1/src/oaklib/utilities/graph/relationship_walker.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/identifier_utils.py` & `oaklib-0.5.1/src/oaklib/utilities/identifier_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/iterator_utils.py` & `oaklib-0.5.1/src/oaklib/utilities/iterator_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/kgcl_utilities.py` & `oaklib-0.5.1/src/oaklib/utilities/kgcl_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/label_utilities.py` & `oaklib-0.5.1/src/oaklib/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/lexical/lexical_indexer.py` & `oaklib-0.5.1/src/oaklib/utilities/lexical/lexical_indexer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/mapping/boomer_utils.py` & `oaklib-0.5.1/src/oaklib/utilities/mapping/boomer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/mapping/cross_ontology_diffs.py` & `oaklib-0.5.1/src/oaklib/utilities/mapping/cross_ontology_diffs.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/mapping/mapping_propagator.py` & `oaklib-0.5.1/src/oaklib/utilities/mapping/mapping_propagator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/mapping/mapping_validation.py` & `oaklib-0.5.1/src/oaklib/utilities/mapping/mapping_validation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/mapping/sssom_utils.py` & `oaklib-0.5.1/src/oaklib/utilities/mapping/sssom_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/ner_utilities.py` & `oaklib-0.5.1/src/oaklib/utilities/ner_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/nlp/natual_language_generation.py` & `oaklib-0.5.1/src/oaklib/utilities/nlp/natual_language_generation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/obograph_utils.py` & `oaklib-0.5.1/src/oaklib/utilities/obograph_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/ontology_builder.py` & `oaklib-0.5.1/src/oaklib/utilities/ontology_builder.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/reasoning/relation_graph.py` & `oaklib-0.5.1/src/oaklib/utilities/reasoning/relation_graph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/semsim/similarity_utils.py` & `oaklib-0.5.1/src/oaklib/utilities/semsim/similarity_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/stats/hypergeometric.py` & `oaklib-0.5.1/src/oaklib/utilities/stats/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/subsets/slimmer_utils.py` & `oaklib-0.5.1/src/oaklib/utilities/subsets/slimmer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/subsets/subset_analysis.py` & `oaklib-0.5.1/src/oaklib/utilities/subsets/subset_analysis.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/subsets/value_set_expander.py` & `oaklib-0.5.1/src/oaklib/utilities/subsets/value_set_expander.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/table_filler.py` & `oaklib-0.5.1/src/oaklib/utilities/table_filler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/taxon/taxon_constraint_utils.py` & `oaklib-0.5.1/src/oaklib/utilities/taxon/taxon_constraint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/validation/definition_ontology_rule.py` & `oaklib-0.5.1/src/oaklib/utilities/validation/definition_ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/validation/disjointness_rule.py` & `oaklib-0.5.1/src/oaklib/utilities/validation/disjointness_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/validation/lint_utils.py` & `oaklib-0.5.1/src/oaklib/utilities/validation/lint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/validation/ontology_rule.py` & `oaklib-0.5.1/src/oaklib/utilities/validation/ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/src/oaklib/utilities/validation/rule_runner.py` & `oaklib-0.5.1/src/oaklib/utilities/validation/rule_runner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.0/PKG-INFO` & `oaklib-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oaklib
-Version: 0.5.0
+Version: 0.5.1
 Summary: Ontology Access Kit: Python library for common ontology operations over a variety of backends
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,15 +13,15 @@
 Provides-Extra: gilda
 Provides-Extra: seaborn
 Requires-Dist: SPARQLWrapper
 Requires-Dist: SQLAlchemy (>=1.4.32,<2.0.0)
 Requires-Dist: airium (>=0.2.5,<0.3.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: bioregistry (>=0.6.35,<0.7.0)
-Requires-Dist: class-resolver (>=0.3.10,<0.4.0)
+Requires-Dist: class-resolver (>=0.4.2)
 Requires-Dist: curies (>=0.4.0,<0.5.0)
 Requires-Dist: funowl (>=0.1.12,<0.2.0)
 Requires-Dist: gilda (>=0.10.1,<0.11.0) ; extra == "gilda"
 Requires-Dist: kgcl-rdflib (>=0.3.0,<0.4.0)
 Requires-Dist: kgcl-schema (>=0.3.5,<0.4.0)
 Requires-Dist: lark (>=1.1.2,<2.0.0)
 Requires-Dist: linkml-renderer (>=0.1.2,<0.2.0)
@@ -35,14 +35,15 @@
 Requires-Dist: prefixmaps (>=0.1.2,<0.2.0)
 Requires-Dist: pronto (>=2.5.0,<3.0.0)
 Requires-Dist: pystow (>=0.5.0,<0.6.0)
 Requires-Dist: ratelimit (>=2.2.1,<3.0.0)
 Requires-Dist: semsql (>=0.3.1,<0.4.0)
 Requires-Dist: sssom (>=0.3.26,<0.4.0)
 Requires-Dist: sssom-schema (>=0.11.0,<0.12.0)
+Requires-Dist: upsetplot (>=0.8.0,<0.9.0)
 Description-Content-Type: text/markdown
 
 # Ontology Access Kit (OAK)
 
 Python lib for common ontology operations over a variety of backends.
 
 <img src="docs/logos/oak-logo_black-icon.png" width="20%">
```

