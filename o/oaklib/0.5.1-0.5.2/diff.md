# Comparing `tmp/oaklib-0.5.1.tar.gz` & `tmp/oaklib-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oaklib-0.5.1.tar", max compression
+gzip compressed data, was "oaklib-0.5.2.tar", max compression
```

## Comparing `oaklib-0.5.1.tar` & `oaklib-0.5.2.tar`

### file list

```diff
@@ -1,262 +1,269 @@
--rw-r--r--   0        0        0    11357 2023-04-13 14:49:46.691053 oaklib-0.5.1/LICENSE
--rw-r--r--   0        0        0     7241 2023-04-13 14:49:46.691053 oaklib-0.5.1/README.md
--rw-r--r--   0        0        0     1807 2023-04-13 14:50:39.991624 oaklib-0.5.1/pyproject.toml
--rw-r--r--   0        0        0      271 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/__init__.py
--rw-r--r--   0        0        0   188779 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/cli.py
--rw-r--r--   0        0        0       64 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/__init__.py
--rw-r--r--   0        0        0      117 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/go-human-input-spec.yaml
--rw-r--r--   0        0        0      115 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/go-pombase-input-spec.yaml
--rw-r--r--   0        0        0      109 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/hpoa-g2p-input-spec.yaml
--rw-r--r--   0        0        0      106 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/hpoa-input-spec.yaml
--rw-r--r--   0        0        0     1903 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
--rw-r--r--   0        0        0      562 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/mondo-g2d-input-spec.yaml
--rw-r--r--   0        0        0      109 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/mondo-gencc-input-spec.yaml
--rw-r--r--   0        0        0      118 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
--rw-r--r--   0        0        0     4537 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/obograph-style.json
--rw-r--r--   0        0        0      256 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/omo-to-skos.sssom.tsv
--rw-r--r--   0        0        0      131 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/conf/value-set-expander.conf.yaml
--rw-r--r--   0        0        0      128 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/constants.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/converters/__init__.py
--rw-r--r--   0        0        0     1456 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/converters/data_model_converter.py
--rw-r--r--   0        0        0     2561 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/converters/logical_definition_flattener.py
--rw-r--r--   0        0        0     2371 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/converters/obo_graph_to_cx_converter.py
--rw-r--r--   0        0        0    12163 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/converters/obo_graph_to_fhir_converter.py
--rw-r--r--   0        0        0     5713 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/converters/obo_graph_to_obo_format_converter.py
--rw-r--r--   0        0        0     5155 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
--rw-r--r--   0        0        0       60 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/__init__.py
--rw-r--r--   0        0        0     4034 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/association.owl.ttl
--rw-r--r--   0        0        0    13782 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/association.py
--rw-r--r--   0        0        0     4506 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/association.yaml
--rw-r--r--   0        0        0     6165 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/class_enrichment.owl.ttl
--rw-r--r--   0        0        0    10853 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/class_enrichment.py
--rw-r--r--   0        0        0     2648 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/class_enrichment.yaml
--rw-r--r--   0        0        0    19083 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
--rw-r--r--   0        0        0    24246 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/cross_ontology_diff.py
--rw-r--r--   0        0        0    10687 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/cross_ontology_diff.yaml
--rw-r--r--   0        0        0    29418 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/cx.py
--rw-r--r--   0        0        0     6314 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/cx.yaml
--rw-r--r--   0        0        0    15826 2023-04-13 14:49:46.815054 oaklib-0.5.1/src/oaklib/datamodels/fhir.owl.ttl
--rw-r--r--   0        0        0    35744 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/fhir.py
--rw-r--r--   0        0        0     5064 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/fhir.yaml
--rw-r--r--   0        0        0    13217 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/input_specification.py
--rw-r--r--   0        0        0     3134 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/input_specification.yaml
--rw-r--r--   0        0        0    15518 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/item_list.py
--rw-r--r--   0        0        0     5765 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/item_list.yaml
--rw-r--r--   0        0        0     8984 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/lexical_index.owl.ttl
--rw-r--r--   0        0        0    17256 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/lexical_index.py
--rw-r--r--   0        0        0     6429 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/lexical_index.schema.json
--rw-r--r--   0        0        0     4016 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/lexical_index.yaml
--rw-r--r--   0        0        0    26434 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/mapping_cluster_datamodel.py
--rw-r--r--   0        0        0     7317 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
--rw-r--r--   0        0        0   226115 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
--rw-r--r--   0        0        0    32727 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.py
--rw-r--r--   0        0        0    12889 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
--rw-r--r--   0        0        0     3607 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.yaml
--rw-r--r--   0        0        0    25354 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/obograph.owl.ttl
--rw-r--r--   0        0        0    45533 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/obograph.py
--rw-r--r--   0        0        0    22375 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/obograph.schema.json
--rw-r--r--   0        0        0    17625 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/obograph.yaml
--rw-r--r--   0        0        0    59793 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.owl.ttl
--rw-r--r--   0        0        0   117175 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.py
--rw-r--r--   0        0        0    95288 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.schema.json
--rw-r--r--   0        0        0    30433 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.yaml
--rw-r--r--   0        0        0    14759 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/oxo.owl.ttl
--rw-r--r--   0        0        0    21914 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/oxo.py
--rw-r--r--   0        0        0     4392 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/oxo.yaml
--rw-r--r--   0        0        0     3240 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/search.py
--rw-r--r--   0        0        0    16948 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/search_datamodel.owl.ttl
--rw-r--r--   0        0        0    25145 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/search_datamodel.py
--rw-r--r--   0        0        0     6683 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/search_datamodel.yaml
--rw-r--r--   0        0        0      287 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/settings.py
--rw-r--r--   0        0        0    12767 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/similarity.owl.ttl
--rw-r--r--   0        0        0    22226 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/similarity.py
--rw-r--r--   0        0        0     5511 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/similarity.yaml
--rw-r--r--   0        0        0    31217 2023-04-13 14:49:46.819054 oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
--rw-r--r--   0        0        0    50743 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.py
--rw-r--r--   0        0        0    21176 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
--rw-r--r--   0        0        0    16246 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.yaml
--rw-r--r--   0        0        0     9909 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/taxon_constraints.owl.ttl
--rw-r--r--   0        0        0    18430 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/taxon_constraints.py
--rw-r--r--   0        0        0     5879 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/taxon_constraints.yaml
--rw-r--r--   0        0        0    11599 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/text_annotator.owl.ttl
--rw-r--r--   0        0        0    20418 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/text_annotator.py
--rw-r--r--   0        0        0     2464 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/text_annotator.schema.json
--rw-r--r--   0        0        0     4219 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/text_annotator.yaml
--rw-r--r--   0        0        0    13670 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.owl.ttl
--rw-r--r--   0        0        0    25351 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.py
--rw-r--r--   0        0        0    10783 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.schema.json
--rw-r--r--   0        0        0     7510 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.yaml
--rw-r--r--   0        0        0     6640 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/value_set_configuration.owl.ttl
--rw-r--r--   0        0        0     8458 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/value_set_configuration.py
--rw-r--r--   0        0        0     2276 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/value_set_configuration.yaml
--rw-r--r--   0        0        0     5588 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/datamodels/vocabulary.py
--rw-r--r--   0        0        0     5217 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/aggregator/__init__.py
--rw-r--r--   0        0        0     5454 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/aggregator/aggregator_implementation.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/amigo/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/cx/__init__.py
--rw-r--r--   0        0        0     1985 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/cx/cx_implementation.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/fhir/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/funowl/__init__.py
--rw-r--r--   0        0        0     8473 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/funowl/funowl_implementation.py
--rw-r--r--   0        0        0     2313 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/gilda.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/kgx/__init__.py
--rw-r--r--   0        0        0    30631 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/kgx/kgx_implementation.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/neo4j/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/obograph/__init__.py
--rw-r--r--   0        0        0    16141 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/obograph/obograph_implementation.py
--rw-r--r--   0        0        0      267 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ols/__init__.py
--rw-r--r--   0        0        0      132 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ols/constants.py
--rw-r--r--   0        0        0     7942 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ols/ols_implementation.py
--rw-r--r--   0        0        0      686 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ols/oxo_utils.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontobee/__init__.py
--rw-r--r--   0        0        0     1391 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontobee/ontobee_implementation.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontoportal/__init__.py
--rw-r--r--   0        0        0      382 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontoportal/agroportal_implementation.py
--rw-r--r--   0        0        0      821 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontoportal/bioportal_implementation.py
--rw-r--r--   0        0        0      378 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
--rw-r--r--   0        0        0      378 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontoportal/matportal_implementation.py
--rw-r--r--   0        0        0    12106 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/owlery/__init__.py
--rw-r--r--   0        0        0      427 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/owlery/owlery_implementation.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/pronto/__init__.py
--rw-r--r--   0        0        0    35361 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/pronto/pronto_implementation.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/robot/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/scigraph/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/simpleobo/__init__.py
--rw-r--r--   0        0        0    34101 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
--rw-r--r--   0        0        0    21451 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/simpleobo/simple_obo_parser.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/skos/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/solor/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/solr/__init__.py
--rw-r--r--   0        0        0       96 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/sparql/__init__.py
--rw-r--r--   0        0        0    36699 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
--rw-r--r--   0        0        0      885 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/sparql/lov_implementation.py
--rw-r--r--   0        0        0     1721 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
--rw-r--r--   0        0        0     2658 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/sparql/sparql_implementation.py
--rw-r--r--   0        0        0     2326 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/sparql/sparql_query.py
--rw-r--r--   0        0        0       96 2023-04-13 14:49:46.823054 oaklib-0.5.1/src/oaklib/implementations/sqldb/__init__.py
--rw-r--r--   0        0        0   105245 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/sqldb/sql_implementation.py
--rw-r--r--   0        0        0     1903 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/sqldb/sqlite_utils.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/tccm/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/translator/__init__.py
--rw-r--r--   0        0        0     3283 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/translator/translator_implementation.py
--rw-r--r--   0        0        0      108 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/ubergraph/__init__.py
--rw-r--r--   0        0        0    19393 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/umls/__init__.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/uniprot/__init__.py
--rw-r--r--   0        0        0     9603 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/uniprot/uniprot_implementation.py
--rw-r--r--   0        0        0       96 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/wikidata/__init__.py
--rw-r--r--   0        0        0    17121 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/implementations/wikidata/wikidata_implementation.py
--rw-r--r--   0        0        0      913 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/__init__.py
--rw-r--r--   0        0        0    13371 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/association_provider_interface.py
--rw-r--r--   0        0        0    50981 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/basic_ontology_interface.py
--rw-r--r--   0        0        0     8640 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/class_enrichment_calculation_interface.py
--rw-r--r--   0        0        0    11720 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/differ_interface.py
--rw-r--r--   0        0        0     2649 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/dumper_interface.py
--rw-r--r--   0        0        0    13280 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/mapping_provider_interface.py
--rw-r--r--   0        0        0     3262 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/merge_interface.py
--rw-r--r--   0        0        0     3103 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/metadata_interface.py
--rw-r--r--   0        0        0    17700 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/obograph_interface.py
--rw-r--r--   0        0        0     1003 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/obolegacy_interface.py
--rw-r--r--   0        0        0      784 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/ontology_interface.py
--rw-r--r--   0        0        0    10988 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/owl_interface.py
--rw-r--r--   0        0        0     8236 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/patcher_interface.py
--rw-r--r--   0        0        0     1955 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/rdf_interface.py
--rw-r--r--   0        0        0     2459 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/relation_graph_interface.py
--rw-r--r--   0        0        0     1386 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/search_interface.py
--rw-r--r--   0        0        0    12778 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/semsim_interface.py
--rw-r--r--   0        0        0     1063 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/skos_interface.py
--rw-r--r--   0        0        0     2112 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/subsetter_interface.py
--rw-r--r--   0        0        0    10140 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/summary_statistics_interface.py
--rw-r--r--   0        0        0    18296 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/taxon_constraint_interface.py
--rw-r--r--   0        0        0     7511 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/text_annotator_interface.py
--rw-r--r--   0        0        0     3033 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/interfaces/validator_interface.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/__init__.py
--rw-r--r--   0        0        0     1539 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/heatmap_writer.py
--rw-r--r--   0        0        0     1698 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/html_writer.py
--rw-r--r--   0        0        0     1379 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/obograph_writer.py
--rw-r--r--   0        0        0     3444 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/rollup_report_writer.py
--rw-r--r--   0        0        0      739 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_axiom_writer.py
--rw-r--r--   0        0        0     7833 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_csv_writer.py
--rw-r--r--   0        0        0     1284 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_fhir_writer.py
--rw-r--r--   0        0        0     2524 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_info_writer.py
--rw-r--r--   0        0        0     1231 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_json_lines_writer.py
--rw-r--r--   0        0        0     1806 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_json_writer.py
--rw-r--r--   0        0        0      741 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_kgcl_writer.py
--rw-r--r--   0        0        0     2088 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_markdown_writer.py
--rw-r--r--   0        0        0     1152 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_nl_writer.py
--rw-r--r--   0        0        0     1117 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_obo_json_writer.py
--rw-r--r--   0        0        0     3496 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_obo_writer.py
--rw-r--r--   0        0        0     1270 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_owl_functional_writer.py
--rw-r--r--   0        0        0     2244 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_rdf_writer.py
--rw-r--r--   0        0        0     5129 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_writer.py
--rw-r--r--   0        0        0     1301 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/io/streaming_yaml_writer.py
--rw-r--r--   0        0        0      113 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/mappers/__init__.py
--rw-r--r--   0        0        0     3717 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/mappers/base_mapper.py
--rw-r--r--   0        0        0     1849 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/mappers/ontology_metadata_mapper.py
--rw-r--r--   0        0        0     2179 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/__init__.py
--rw-r--r--   0        0        0      650 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/association_parser.py
--rw-r--r--   0        0        0      522 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/association_parser_factory.py
--rw-r--r--   0        0        0     4731 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/boomer_parser.py
--rw-r--r--   0        0        0     1178 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/gaf_association_parser.py
--rw-r--r--   0        0        0     1090 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/gencc_association_parser.py
--rw-r--r--   0        0        0      563 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/hpoa_association_parser.py
--rw-r--r--   0        0        0      602 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/hpoa_g2p_association_parser.py
--rw-r--r--   0        0        0      653 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/kgx_association_parser.py
--rw-r--r--   0        0        0     1666 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/mim2gene_association_parser.py
--rw-r--r--   0        0        0      525 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/pairwise_association_parser.py
--rw-r--r--   0        0        0     1328 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/parser_base.py
--rw-r--r--   0        0        0      707 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/phaf_association_parser.py
--rw-r--r--   0        0        0     6282 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/parsers/xaf_association_parser.py
--rw-r--r--   0        0        0     2210 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/resource.py
--rw-r--r--   0        0        0    13501 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/selector.py
--rw-r--r--   0        0        0      177 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/types.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/__init__.py
--rw-r--r--   0        0        0     1613 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/apikey_manager.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/associations/__init__.py
--rw-r--r--   0        0        0     2810 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/associations/association_differ.py
--rw-r--r--   0        0        0     2865 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/associations/association_index.py
--rw-r--r--   0        0        0     1182 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/basic_utils.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/graph/__init__.py
--rw-r--r--   0        0        0     2490 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/graph/networkx_bridge.py
--rw-r--r--   0        0        0     2918 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/graph/relationship_walker.py
--rw-r--r--   0        0        0      993 2023-04-13 14:49:46.827054 oaklib-0.5.1/src/oaklib/utilities/identifier_utils.py
--rw-r--r--   0        0        0      999 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/iterator_utils.py
--rw-r--r--   0        0        0     3345 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/kgcl_utilities.py
--rw-r--r--   0        0        0      850 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/label_utilities.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/lexical/__init__.py
--rw-r--r--   0        0        0    19516 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/lexical/lexical_indexer.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/mapping/__init__.py
--rw-r--r--   0        0        0    14443 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/mapping/boomer_utils.py
--rw-r--r--   0        0        0    15328 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/mapping/cross_ontology_diffs.py
--rw-r--r--   0        0        0      751 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/mapping/mapping_propagator.py
--rw-r--r--   0        0        0     2270 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/mapping/mapping_validation.py
--rw-r--r--   0        0        0     2694 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/mapping/sssom_utils.py
--rw-r--r--   0        0        0      684 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/ner_utilities.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/nlp/__init__.py
--rw-r--r--   0        0        0     3358 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/nlp/natual_language_generation.py
--rw-r--r--   0        0        0      136 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/oboformat_utils.py
--rw-r--r--   0        0        0    22266 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/obograph_utils.py
--rw-r--r--   0        0        0     2275 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/ontology_builder.py
--rw-r--r--   0        0        0      379 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/rate_limiter.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/reasoning/__init__.py
--rw-r--r--   0        0        0      569 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/reasoning/relation_graph.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/semsim/__init__.py
--rw-r--r--   0        0        0     1739 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/semsim/similarity_utils.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/stats/__init__.py
--rw-r--r--   0        0        0     1511 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/stats/hypergeometric.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/subsets/__init__.py
--rw-r--r--   0        0        0     2676 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/subsets/slimmer_utils.py
--rw-r--r--   0        0        0     4701 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/subsets/subset_analysis.py
--rw-r--r--   0        0        0    11592 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/subsets/value_set_expander.py
--rw-r--r--   0        0        0    13212 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/table_filler.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/taxon/__init__.py
--rw-r--r--   0        0        0     1743 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/taxon/taxon_constraint_utils.py
--rw-r--r--   0        0        0        0 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/validation/__init__.py
--rw-r--r--   0        0        0    10097 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/validation/definition_ontology_rule.py
--rw-r--r--   0        0        0     7492 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/validation/disjointness_rule.py
--rw-r--r--   0        0        0     1729 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/validation/lint_utils.py
--rw-r--r--   0        0        0     1402 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/validation/ontology_rule.py
--rw-r--r--   0        0        0     1313 2023-04-13 14:49:46.831055 oaklib-0.5.1/src/oaklib/utilities/validation/rule_runner.py
--rw-r--r--   0        0        0     8957 1970-01-01 00:00:00.000000 oaklib-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-04-21 22:04:18.977975 oaklib-0.5.2/LICENSE
+-rw-r--r--   0        0        0     7241 2023-04-21 22:04:18.977975 oaklib-0.5.2/README.md
+-rw-r--r--   0        0        0     1915 2023-04-21 22:05:13.409768 oaklib-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0      271 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/__init__.py
+-rw-r--r--   0        0        0   190704 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/cli.py
+-rw-r--r--   0        0        0       64 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/conf/__init__.py
+-rw-r--r--   0        0        0      372 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/conf/go-human-input-spec.yaml
+-rw-r--r--   0        0        0      115 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/conf/go-pombase-input-spec.yaml
+-rw-r--r--   0        0        0      109 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/conf/hpoa-g2p-input-spec.yaml
+-rw-r--r--   0        0        0      106 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/conf/hpoa-input-spec.yaml
+-rw-r--r--   0        0        0     1903 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml
+-rw-r--r--   0        0        0      562 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/conf/mondo-g2d-input-spec.yaml
+-rw-r--r--   0        0        0      109 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/conf/mondo-gencc-input-spec.yaml
+-rw-r--r--   0        0        0      118 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/conf/mondo-medgen-g2d-input-spec.yaml
+-rw-r--r--   0        0        0     4537 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/conf/obograph-style.json
+-rw-r--r--   0        0        0      256 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/conf/omo-to-skos.sssom.tsv
+-rw-r--r--   0        0        0      131 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/conf/value-set-expander.conf.yaml
+-rw-r--r--   0        0        0      128 2023-04-21 22:04:19.109974 oaklib-0.5.2/src/oaklib/constants.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/converters/__init__.py
+-rw-r--r--   0        0        0     1456 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/converters/data_model_converter.py
+-rw-r--r--   0        0        0     2561 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/converters/logical_definition_flattener.py
+-rw-r--r--   0        0        0     2371 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/converters/obo_graph_to_cx_converter.py
+-rw-r--r--   0        0        0    12159 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/converters/obo_graph_to_fhir_converter.py
+-rw-r--r--   0        0        0     5713 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/converters/obo_graph_to_obo_format_converter.py
+-rw-r--r--   0        0        0     5155 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py
+-rw-r--r--   0        0        0       60 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/__init__.py
+-rw-r--r--   0        0        0     4034 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/association.owl.ttl
+-rw-r--r--   0        0        0    25704 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/association.py
+-rw-r--r--   0        0        0     6615 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/association.yaml
+-rw-r--r--   0        0        0     6165 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/class_enrichment.owl.ttl
+-rw-r--r--   0        0        0    13328 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/class_enrichment.py
+-rw-r--r--   0        0        0     3192 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/class_enrichment.yaml
+-rw-r--r--   0        0        0    19083 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/cross_ontology_diff.owl.ttl
+-rw-r--r--   0        0        0    24246 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/cross_ontology_diff.py
+-rw-r--r--   0        0        0    10687 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/cross_ontology_diff.yaml
+-rw-r--r--   0        0        0    29418 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/cx.py
+-rw-r--r--   0        0        0     6314 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/cx.yaml
+-rw-r--r--   0        0        0    15826 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/fhir.owl.ttl
+-rw-r--r--   0        0        0    35744 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/fhir.py
+-rw-r--r--   0        0        0     5064 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/fhir.yaml
+-rw-r--r--   0        0        0    14564 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/input_specification.py
+-rw-r--r--   0        0        0     3560 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/input_specification.yaml
+-rw-r--r--   0        0        0    15768 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/item_list.py
+-rw-r--r--   0        0        0     6339 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/item_list.yaml
+-rw-r--r--   0        0        0     8984 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/lexical_index.owl.ttl
+-rw-r--r--   0        0        0    17256 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/lexical_index.py
+-rw-r--r--   0        0        0     6429 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/lexical_index.schema.json
+-rw-r--r--   0        0        0     4016 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/lexical_index.yaml
+-rw-r--r--   0        0        0    26434 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/mapping_cluster_datamodel.py
+-rw-r--r--   0        0        0     7317 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/mapping_cluster_datamodel.yaml
+-rw-r--r--   0        0        0   226115 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl
+-rw-r--r--   0        0        0    32727 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/mapping_rules_datamodel.py
+-rw-r--r--   0        0        0    12889 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/mapping_rules_datamodel.schema.json
+-rw-r--r--   0        0        0     3607 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/mapping_rules_datamodel.yaml
+-rw-r--r--   0        0        0    25354 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/obograph.owl.ttl
+-rw-r--r--   0        0        0    45533 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/obograph.py
+-rw-r--r--   0        0        0    22375 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/obograph.schema.json
+-rw-r--r--   0        0        0    17625 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/obograph.yaml
+-rw-r--r--   0        0        0    59793 2023-04-21 22:04:19.113974 oaklib-0.5.2/src/oaklib/datamodels/ontology_metadata.owl.ttl
+-rw-r--r--   0        0        0   117175 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/ontology_metadata.py
+-rw-r--r--   0        0        0    95288 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/ontology_metadata.schema.json
+-rw-r--r--   0        0        0    30433 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/ontology_metadata.yaml
+-rw-r--r--   0        0        0    14759 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/oxo.owl.ttl
+-rw-r--r--   0        0        0    21914 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/oxo.py
+-rw-r--r--   0        0        0     4392 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/oxo.yaml
+-rw-r--r--   0        0        0     3240 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/search.py
+-rw-r--r--   0        0        0    16948 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/search_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25145 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/search_datamodel.py
+-rw-r--r--   0        0        0     6683 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/search_datamodel.yaml
+-rw-r--r--   0        0        0      287 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/settings.py
+-rw-r--r--   0        0        0    12767 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/similarity.owl.ttl
+-rw-r--r--   0        0        0    22226 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/similarity.py
+-rw-r--r--   0        0        0     5511 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/similarity.yaml
+-rw-r--r--   0        0        0    31217 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl
+-rw-r--r--   0        0        0    50743 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/summary_statistics_datamodel.py
+-rw-r--r--   0        0        0    21176 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/summary_statistics_datamodel.schema.json
+-rw-r--r--   0        0        0    16246 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/summary_statistics_datamodel.yaml
+-rw-r--r--   0        0        0     9909 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/taxon_constraints.owl.ttl
+-rw-r--r--   0        0        0    18430 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/taxon_constraints.py
+-rw-r--r--   0        0        0     5879 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/taxon_constraints.yaml
+-rw-r--r--   0        0        0    11599 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/text_annotator.owl.ttl
+-rw-r--r--   0        0        0    20418 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/text_annotator.py
+-rw-r--r--   0        0        0     2464 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/text_annotator.schema.json
+-rw-r--r--   0        0        0     4219 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/text_annotator.yaml
+-rw-r--r--   0        0        0    13670 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/validation_datamodel.owl.ttl
+-rw-r--r--   0        0        0    25351 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/validation_datamodel.py
+-rw-r--r--   0        0        0    10783 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/validation_datamodel.schema.json
+-rw-r--r--   0        0        0     7510 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/validation_datamodel.yaml
+-rw-r--r--   0        0        0     6640 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/value_set_configuration.owl.ttl
+-rw-r--r--   0        0        0     8458 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/value_set_configuration.py
+-rw-r--r--   0        0        0     2276 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/value_set_configuration.yaml
+-rw-r--r--   0        0        0     5588 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/datamodels/vocabulary.py
+-rw-r--r--   0        0        0     5602 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/aggregator/__init__.py
+-rw-r--r--   0        0        0     5996 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/aggregator/aggregator_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/amigo/__init__.py
+-rw-r--r--   0        0        0     3332 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/amigo/amigo_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/cx/__init__.py
+-rw-r--r--   0        0        0     1985 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/cx/cx_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/eutils/__init__.py
+-rw-r--r--   0        0        0     2179 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/eutils/eutils_implementation.py
+-rw-r--r--   0        0        0     1053 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/eutils/pubmed_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/fhir/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/funowl/__init__.py
+-rw-r--r--   0        0        0     8473 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/funowl/funowl_implementation.py
+-rw-r--r--   0        0        0     2313 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/gilda.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/kgx/__init__.py
+-rw-r--r--   0        0        0    30434 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/kgx/kgx_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/neo4j/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/obograph/__init__.py
+-rw-r--r--   0        0        0    16240 2023-04-21 22:04:19.117974 oaklib-0.5.2/src/oaklib/implementations/obograph/obograph_implementation.py
+-rw-r--r--   0        0        0      267 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/ols/__init__.py
+-rw-r--r--   0        0        0      132 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/ols/constants.py
+-rw-r--r--   0        0        0     7942 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/ols/ols_implementation.py
+-rw-r--r--   0        0        0      686 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/ols/oxo_utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/ontobee/__init__.py
+-rw-r--r--   0        0        0     2532 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/ontobee/ontobee_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/ontoportal/__init__.py
+-rw-r--r--   0        0        0      382 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/ontoportal/agroportal_implementation.py
+-rw-r--r--   0        0        0     1238 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/ontoportal/bioportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/ontoportal/ecoportal_implementation.py
+-rw-r--r--   0        0        0      378 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/ontoportal/matportal_implementation.py
+-rw-r--r--   0        0        0    12106 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/owlery/__init__.py
+-rw-r--r--   0        0        0      427 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/owlery/owlery_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/pronto/__init__.py
+-rw-r--r--   0        0        0    35620 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/pronto/pronto_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/robot/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/rustsim/__init__.py
+-rw-r--r--   0        0        0    14065 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/rustsim/rustsim_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/scigraph/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/simpleobo/__init__.py
+-rw-r--r--   0        0        0    34101 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/simpleobo/simple_obo_implementation.py
+-rw-r--r--   0        0        0    21451 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/simpleobo/simple_obo_parser.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/skos/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/solor/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/solr/__init__.py
+-rw-r--r--   0        0        0       96 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/sparql/__init__.py
+-rw-r--r--   0        0        0    36699 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/sparql/abstract_sparql_implementation.py
+-rw-r--r--   0        0        0      885 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/sparql/lov_implementation.py
+-rw-r--r--   0        0        0     1721 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/sparql/oak_metamodel_implementation.py
+-rw-r--r--   0        0        0     2658 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/sparql/sparql_implementation.py
+-rw-r--r--   0        0        0     2326 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/sparql/sparql_query.py
+-rw-r--r--   0        0        0       96 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/sqldb/__init__.py
+-rw-r--r--   0        0        0   105396 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/sqldb/sql_implementation.py
+-rw-r--r--   0        0        0     1903 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/sqldb/sqlite_utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/tccm/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/translator/__init__.py
+-rw-r--r--   0        0        0     3283 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/translator/translator_implementation.py
+-rw-r--r--   0        0        0      108 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/ubergraph/__init__.py
+-rw-r--r--   0        0        0    19393 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/ubergraph/ubergraph_implementation.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/umls/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/uniprot/__init__.py
+-rw-r--r--   0        0        0     9603 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/uniprot/uniprot_implementation.py
+-rw-r--r--   0        0        0       96 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/wikidata/__init__.py
+-rw-r--r--   0        0        0    17121 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/implementations/wikidata/wikidata_implementation.py
+-rw-r--r--   0        0        0      913 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/__init__.py
+-rw-r--r--   0        0        0    13406 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/association_provider_interface.py
+-rw-r--r--   0        0        0    50981 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/basic_ontology_interface.py
+-rw-r--r--   0        0        0     8817 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/class_enrichment_calculation_interface.py
+-rw-r--r--   0        0        0    11720 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/differ_interface.py
+-rw-r--r--   0        0        0     2649 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/dumper_interface.py
+-rw-r--r--   0        0        0      977 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/embedding_provider_interface.py
+-rw-r--r--   0        0        0    13280 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/mapping_provider_interface.py
+-rw-r--r--   0        0        0     3262 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/merge_interface.py
+-rw-r--r--   0        0        0     3103 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/metadata_interface.py
+-rw-r--r--   0        0        0    18964 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/obograph_interface.py
+-rw-r--r--   0        0        0     1003 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/obolegacy_interface.py
+-rw-r--r--   0        0        0      784 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/ontology_interface.py
+-rw-r--r--   0        0        0    10988 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/owl_interface.py
+-rw-r--r--   0        0        0     8236 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/patcher_interface.py
+-rw-r--r--   0        0        0     1955 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/rdf_interface.py
+-rw-r--r--   0        0        0     2459 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/relation_graph_interface.py
+-rw-r--r--   0        0        0     1386 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/search_interface.py
+-rw-r--r--   0        0        0    12778 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/semsim_interface.py
+-rw-r--r--   0        0        0     1063 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/skos_interface.py
+-rw-r--r--   0        0        0     2112 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/subsetter_interface.py
+-rw-r--r--   0        0        0    10140 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/summary_statistics_interface.py
+-rw-r--r--   0        0        0    18296 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/taxon_constraint_interface.py
+-rw-r--r--   0        0        0     7511 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/text_annotator_interface.py
+-rw-r--r--   0        0        0     3033 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/interfaces/validator_interface.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/io/__init__.py
+-rw-r--r--   0        0        0     1539 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/io/heatmap_writer.py
+-rw-r--r--   0        0        0     1698 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/io/html_writer.py
+-rw-r--r--   0        0        0     1379 2023-04-21 22:04:19.121974 oaklib-0.5.2/src/oaklib/io/obograph_writer.py
+-rw-r--r--   0        0        0     3444 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/rollup_report_writer.py
+-rw-r--r--   0        0        0      739 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_axiom_writer.py
+-rw-r--r--   0        0        0     7833 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_csv_writer.py
+-rw-r--r--   0        0        0     1284 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_fhir_writer.py
+-rw-r--r--   0        0        0     2524 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_info_writer.py
+-rw-r--r--   0        0        0     1231 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_json_lines_writer.py
+-rw-r--r--   0        0        0     1806 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_json_writer.py
+-rw-r--r--   0        0        0      741 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_kgcl_writer.py
+-rw-r--r--   0        0        0     2088 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_markdown_writer.py
+-rw-r--r--   0        0        0     1152 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_nl_writer.py
+-rw-r--r--   0        0        0     1117 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_obo_json_writer.py
+-rw-r--r--   0        0        0     3496 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_obo_writer.py
+-rw-r--r--   0        0        0     1270 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_owl_functional_writer.py
+-rw-r--r--   0        0        0     2244 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_rdf_writer.py
+-rw-r--r--   0        0        0     5129 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_writer.py
+-rw-r--r--   0        0        0     1301 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/io/streaming_yaml_writer.py
+-rw-r--r--   0        0        0      113 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/mappers/__init__.py
+-rw-r--r--   0        0        0     3717 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/mappers/base_mapper.py
+-rw-r--r--   0        0        0     1849 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/mappers/ontology_metadata_mapper.py
+-rw-r--r--   0        0        0     2179 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/parsers/__init__.py
+-rw-r--r--   0        0        0     1154 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/parsers/association_parser.py
+-rw-r--r--   0        0        0      522 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/parsers/association_parser_factory.py
+-rw-r--r--   0        0        0     4731 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/parsers/boomer_parser.py
+-rw-r--r--   0        0        0     1391 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/parsers/gaf_association_parser.py
+-rw-r--r--   0        0        0     1090 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/parsers/gencc_association_parser.py
+-rw-r--r--   0        0        0      563 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/parsers/hpoa_association_parser.py
+-rw-r--r--   0        0        0      602 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/parsers/hpoa_g2p_association_parser.py
+-rw-r--r--   0        0        0      653 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/parsers/kgx_association_parser.py
+-rw-r--r--   0        0        0     1666 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/parsers/mim2gene_association_parser.py
+-rw-r--r--   0        0        0      525 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/parsers/pairwise_association_parser.py
+-rw-r--r--   0        0        0     1408 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/parsers/parser_base.py
+-rw-r--r--   0        0        0      707 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/parsers/phaf_association_parser.py
+-rw-r--r--   0        0        0     7511 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/parsers/xaf_association_parser.py
+-rw-r--r--   0        0        0     2210 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/resource.py
+-rw-r--r--   0        0        0    14395 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/selector.py
+-rw-r--r--   0        0        0      177 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/types.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/__init__.py
+-rw-r--r--   0        0        0     1613 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/apikey_manager.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/associations/__init__.py
+-rw-r--r--   0        0        0    11026 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/associations/association_differ.py
+-rw-r--r--   0        0        0     3054 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/associations/association_index.py
+-rw-r--r--   0        0        0     1540 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/basic_utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/graph/__init__.py
+-rw-r--r--   0        0        0     2490 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/graph/networkx_bridge.py
+-rw-r--r--   0        0        0     2918 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/graph/relationship_walker.py
+-rw-r--r--   0        0        0      993 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/identifier_utils.py
+-rw-r--r--   0        0        0      999 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/iterator_utils.py
+-rw-r--r--   0        0        0     3345 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/kgcl_utilities.py
+-rw-r--r--   0        0        0      850 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/label_utilities.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/lexical/__init__.py
+-rw-r--r--   0        0        0    19516 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/lexical/lexical_indexer.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/mapping/__init__.py
+-rw-r--r--   0        0        0    14443 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/mapping/boomer_utils.py
+-rw-r--r--   0        0        0    15328 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/mapping/cross_ontology_diffs.py
+-rw-r--r--   0        0        0      751 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/mapping/mapping_propagator.py
+-rw-r--r--   0        0        0     2270 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/mapping/mapping_validation.py
+-rw-r--r--   0        0        0     2694 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/mapping/sssom_utils.py
+-rw-r--r--   0        0        0      684 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/ner_utilities.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/nlp/__init__.py
+-rw-r--r--   0        0        0     3358 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/nlp/natual_language_generation.py
+-rw-r--r--   0        0        0      136 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/oboformat_utils.py
+-rw-r--r--   0        0        0    22274 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/obograph_utils.py
+-rw-r--r--   0        0        0     2275 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/ontology_builder.py
+-rw-r--r--   0        0        0      379 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/rate_limiter.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/reasoning/__init__.py
+-rw-r--r--   0        0        0      569 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/reasoning/relation_graph.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/semsim/__init__.py
+-rw-r--r--   0        0        0     1739 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/semsim/similarity_utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/stats/__init__.py
+-rw-r--r--   0        0        0     1511 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/stats/hypergeometric.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/subsets/__init__.py
+-rw-r--r--   0        0        0     2676 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/subsets/slimmer_utils.py
+-rw-r--r--   0        0        0     4701 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/subsets/subset_analysis.py
+-rw-r--r--   0        0        0    11592 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/subsets/value_set_expander.py
+-rw-r--r--   0        0        0    13212 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/table_filler.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/taxon/__init__.py
+-rw-r--r--   0        0        0     1743 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/taxon/taxon_constraint_utils.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/validation/__init__.py
+-rw-r--r--   0        0        0    10097 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/validation/definition_ontology_rule.py
+-rw-r--r--   0        0        0     7492 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/validation/disjointness_rule.py
+-rw-r--r--   0        0        0     1729 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/validation/lint_utils.py
+-rw-r--r--   0        0        0     1402 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/validation/ontology_rule.py
+-rw-r--r--   0        0        0     1313 2023-04-21 22:04:19.125974 oaklib-0.5.2/src/oaklib/utilities/validation/rule_runner.py
+-rw-r--r--   0        0        0     9120 1970-01-01 00:00:00.000000 oaklib-0.5.2/PKG-INFO
```

### Comparing `oaklib-0.5.1/LICENSE` & `oaklib-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/README.md` & `oaklib-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/pyproject.toml` & `oaklib-0.5.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oaklib"
-version = "v0.5.1"
+version = "v0.5.2"
 description = "Ontology Access Kit: Python library for common ontology operations over a variety of backends"
 authors = ["cmungall <cjm@berkeleybop.org>"]
 
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0.0"
@@ -31,22 +31,26 @@
 bioregistry = "^0.6.35"
 prefixmaps = "^0.1.2"
 ols-client = "^0.1.1"
 pandas = "^1.5.1"
 linkml-renderer = "^0.1.2"
 airium = "^0.2.5"
 ndex2 = "^3.5.0"
+rustsim = {version = "^0.1.6", optional = true}
 upsetplot = "^0.8.0"
+pysolr = "^3.9.0"
+eutils = "^0.6.0"
+
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 Sphinx = ">=6.1.3"
 jupyter = "^1.0.0"
 sphinx-rtd-theme = "^1.0.0"
-sphinx-click = "^3.1.0"
+sphinx-click = ">=4.4.0"
 myst-parser = ">=1.0.0"
 linkml = "^1.2.14"
 sphinxcontrib-mermaid = "^0.8.1"
 sphinx-copybutton = "0.5.1"
 coverage = "^6.3.2"
 
 [tool.poetry.group.dev.dependencies]
@@ -61,14 +65,15 @@
 vskit = "oaklib.utilities.subsets.value_set_expander:main"
 boomerang = "oaklib.utilities.mapping.boomer_utils:main"
 
 [tool.poetry.extras]
 docs = ["Sphinx", "sphinx-rtd-theme", "sphinxcontrib-mermaid", "sphinx-copybutton"]
 gilda = ["scipy", "gilda"]
 seaborn = ["seaborn"]
+rustsim = ["rustsim"]
 
 [tool.black]
 line-length = 100
 target-version = ["py39", "py310"]
 
 [tool.isort]
 profile = "black"
```

### Comparing `oaklib-0.5.1/src/oaklib/cli.py` & `oaklib-0.5.2/src/oaklib/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -368,15 +368,22 @@
 )
 ontological_output_type_option = click.option(
     "-O",
     "--output-type",
     type=click.Choice(ONT_FORMATS),
     help="Desired output type",
 )
-predicates_option = click.option("-p", "--predicates", help="A comma-separated list of predicates")
+predicates_option = click.option(
+    "-p",
+    "--predicates",
+    help="A comma-separated list of predicates. This may be a shorthand (i, p) or CURIE",
+)
+exclude_predicates_option = click.option(
+    "--exclude-predicates", help="A comma-separated list of predicates to exclude"
+)
 graph_traversal_method_option = click.option(
     "-M",
     "--graph-traversal-method",
     type=click.Choice([v.value for v in GraphTraversalMethod]),
     help="Desired output type",
 )
 display_option = click.option(
@@ -424,25 +431,42 @@
     default=False,
     show_default=True,
     help="shortcut for --group-by-property sh:prefix. Groups by the prefix of the CURIE",
 )
 
 
 def _process_predicates_arg(
-    preds_str: str, expected_number: Optional[int] = None
+    predicates_str: str,
+    expected_number: Optional[int] = None,
+    exclude_predicates_str: Optional[str] = None,
+    impl: Optional[OntologyInterface] = None,
 ) -> Optional[List[PRED_CURIE]]:
-    if preds_str is None:
+    if predicates_str is None and exclude_predicates_str is None:
         return None
-    if "," in preds_str:
-        inputs = preds_str.split(",")
+    if predicates_str is None:
+        inputs = []
+    elif "," in predicates_str:
+        inputs = predicates_str.split(",")
     else:
-        inputs = preds_str.split("+")
+        inputs = predicates_str.split("+")
     preds = [_shorthand_to_pred_curie(p) for p in inputs]
+    if exclude_predicates_str:
+        if "," in exclude_predicates_str:
+            exclude_inputs = exclude_predicates_str.split(",")
+        else:
+            exclude_inputs = exclude_predicates_str.split("+")
+        exclude_preds = [_shorthand_to_pred_curie(p) for p in exclude_inputs]
+        if not preds:
+            if not impl or not isinstance(impl, BasicOntologyInterface):
+                raise ValueError("Must provide an BasicOntologyInterface to exclude predicates")
+            preds = list(impl.entities(owl_type=OWL_OBJECT_PROPERTY))
+        preds = [p for p in preds if p not in exclude_preds]
+        logging.info(f"Excluding predicates: {exclude_preds} yields: {preds}")
     if expected_number and len(preds) != expected_number:
-        raise ValueError(f"Expected {expected_number} parses of {preds_str}, got: {preds}")
+        raise ValueError(f"Expected {expected_number} parses of {predicates_str}, got: {preds}")
     return preds
 
 
 # TODO: move to vocab
 def _shorthand_to_pred_curie(shorthand: str) -> PRED_CURIE:
     if shorthand == "i":
         return IS_A
@@ -2012,14 +2036,15 @@
     "--viz/--no-viz",
     default=False,
     show_default=True,
     help="If true then generate a path graph from output",
 )
 @autolabel_option
 @predicates_option
+@exclude_predicates_option
 @output_type_option
 @click.option(
     "--directed/--no-directed", default=False, show_default=True, help="only show directed paths"
 )
 @click.option(
     "--include-predicates/--no-include-predicates",
     default=False,
@@ -2038,14 +2063,15 @@
     predicates,
     predicate_weights,
     autolabel: bool,
     narrow: bool,
     viz: bool,
     directed: bool,
     include_predicates: bool,
+    exclude_predicates: str,
     target,
     stylemap,
     configure,
     output_type: str,
     output: str,
 ):
     """
@@ -2101,15 +2127,18 @@
     writer.autolabel = autolabel
     if output:
         writer.file = output
     else:
         writer.file = sys.stdout
     if not isinstance(impl, OboGraphInterface):
         raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
-    actual_predicates = _process_predicates_arg(predicates)
+    actual_predicates = _process_predicates_arg(
+        predicates, exclude_predicates_str=exclude_predicates, impl=impl
+    )
+    logging.info(f"Using predicates {actual_predicates}")
     if predicate_weights:
         pw = {}
         for k, v in yaml.safe_load(predicate_weights).items():
             [p] = _process_predicates_arg(k, expected_number=1)
             pw[k] = v
     else:
         pw = None
@@ -2194,14 +2223,16 @@
                 )
         elif not viz:
             writer.emit(
                 dict(subject=s, object=o, path=path),
                 label_fields=["subject", "object", "path"],
             )
         writer.finish()
+    if not node_ids:
+        logging.warning("No paths found")
     if viz:
         for node_id in node_ids:
             [n] = [n for n in graph.nodes if n.id == node_id]
             path_graph.nodes.append(n)
         # TODO: abstract this out
         if output_type:
             write_graph(path_graph, format=output_type, output=output)
@@ -4321,19 +4352,24 @@
 @output_option
 @predicates_option
 @autolabel_option
 @output_type_option
 @output_option
 @click.option("-g", "--associations", help="associations")
 @click.option("-X", "--other-associations", help="other associations")
+@click.option(
+    "--group-by",
+    help="One of: publications; primary_knowledge_source",
+)
 def diff_associations(
     predicates: str,
     autolabel: bool,
     output_type: str,
     output: str,
+    group_by: str,
     associations: str,
     other_associations: str,
 ):
     """
     Diffs two association sources. EXPERIMENTAL.
 
     This functionality may move out of core
@@ -4341,34 +4377,43 @@
     impl = settings.impl
     writer = _get_writer(output_type, impl, StreamingCsvWriter)
     writer.autolabel = autolabel
     writer.output = output
     actual_predicates = _process_predicates_arg(predicates)
     logging.info(f"Fetching parser for {settings.associations_type}")
     association_parser = get_association_parser(settings.associations_type)
-    if isinstance(impl, AssociationProviderInterface):
-        if associations:
-            logging.info(f"Loading main associations from {associations}")
-            with open(associations) as file:
-                assocs1 = list(association_parser.parse(file))
-        else:
-            assocs1 = list(impl.associations(predicates=actual_predicates))
-        if len(assocs1) == 0:
-            raise ValueError("No associations to compare")
-        logging.info(f"Loading other associations from {other_associations}")
-        with open(other_associations) as file:
-            assocs2 = list(association_parser.parse(file))
-            if isinstance(impl, OboGraphInterface):
-                differ = AssociationDiffer(impl)
-                impl.enable_transitive_query_cache()
-                for change in differ.changes(assocs1, assocs2, actual_predicates):
-                    writer.emit(
-                        {"entity": change[0], "set": change[1], "term": change[2]},
-                        label_fields=["term"],
-                    )
+    if not isinstance(impl, AssociationProviderInterface):
+        raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
+    if associations:
+        logging.info(f"Loading main associations from {associations}")
+        with open(associations) as file:
+            assocs1 = list(association_parser.parse(file))
+    else:
+        assocs1 = list(impl.associations(predicates=actual_predicates))
+    if len(assocs1) == 0:
+        raise ValueError("No associations to compare")
+    logging.info(f"Loading other associations from {other_associations}")
+    with open(other_associations) as file:
+        assocs2 = list(association_parser.parse(file))
+        if not isinstance(impl, OboGraphInterface):
+            raise NotImplementedError(f"Cannot execute this using {impl} of type {type(impl)}")
+        differ = AssociationDiffer(impl)
+        impl.enable_transitive_query_cache()
+        if group_by == "publications":
+            changes = differ.changes_by_publication(assocs1, assocs2, actual_predicates)
+        elif group_by == "primary_knowledge_source":
+            changes = differ.changes_by_primary_knowledge_source(
+                assocs1, assocs2, actual_predicates
+            )
+        elif group_by:
+            raise ValueError(f"Unknown group-by: {group_by}")
+        else:
+            changes = differ.calculate_change_objects(assocs1, assocs2, actual_predicates)
+        for change in changes:
+            writer.emit(change, label_fields=["old_object", "new_object"])
     writer.finish()
 
 
 @main.command()
 @click.option(
     "--cutoff",
     default=50,
```

### Comparing `oaklib-0.5.1/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml` & `oaklib-0.5.2/src/oaklib/conf/lexmatch-rules-oboinowl-default.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/conf/mondo-g2d-input-spec.yaml` & `oaklib-0.5.2/src/oaklib/conf/mondo-g2d-input-spec.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/conf/obograph-style.json` & `oaklib-0.5.2/src/oaklib/conf/obograph-style.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/converters/data_model_converter.py` & `oaklib-0.5.2/src/oaklib/converters/data_model_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/converters/logical_definition_flattener.py` & `oaklib-0.5.2/src/oaklib/converters/logical_definition_flattener.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/converters/obo_graph_to_cx_converter.py` & `oaklib-0.5.2/src/oaklib/converters/obo_graph_to_cx_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/converters/obo_graph_to_fhir_converter.py` & `oaklib-0.5.2/src/oaklib/converters/obo_graph_to_fhir_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,15 @@
         >>> graph = json_loader.load("tests/input/hp_test.json", target_class=GraphDocument)
         >>> code_system = converter.convert(graph)
         >>> print(json_dumper.dumps(code_system))
         <BLANKLINE>
         ...
          "concept": [
             {
-            "packages": "HP:0012639",
+            "code": "HP:0012639",
             "display": "Abnormal nervous system morphology",
             "definition": "A structural anomaly of the nervous system.",
             "designation": [
          ...
 
         :param code_system_id: The packages system ID to use for identification on the server uploaded to.
                                See: https://hl7.org/fhir/resource-definitions.html#Resource.id
```

### Comparing `oaklib-0.5.1/src/oaklib/converters/obo_graph_to_obo_format_converter.py` & `oaklib-0.5.2/src/oaklib/converters/obo_graph_to_obo_format_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py` & `oaklib-0.5.2/src/oaklib/converters/obo_graph_to_rdf_owl_converter.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/association.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/association.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/association.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/association.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -28,25 +28,31 @@
       - subject
       - predicate
       - object
       - property_values
       - subject_label
       - predicate_label
       - object_label
+      - publications
+      - primary_knowledge_source
+      - aggregator_knowledge_source
 
   NegatedAssociation:
     description: A negated association between a thing (subject) and another thing (object).
     slots:
       - subject
       - predicate
       - object
       - property_values
       - subject_label
       - predicate_label
       - object_label
+      - publications
+      - primary_knowledge_source
+      - aggregator_knowledge_source
 
   PropertyValue:
     description: A generic tag-value that can be associated with an association.
     slots:
       - predicate
       - object
 
@@ -64,14 +70,43 @@
           If true, then the parser will keep negated associations in the output.
           If false, then the parser will remove negated associations from the output.
       include_association_attributes:
         range: boolean
         description: |-
           If true, then the parser will include non S/P/O properties as additional attributes.
           This may result in slower parsing
+      primary_knowledge_source:
+        range: uriorcurie
+        slot_uri: biolink:primary_knowledge_source
+        description: |-
+          The default primary knowledge source for all associations in this resource.
+      aggregator_knowledge_source:
+        range: uriorcurie
+        slot_uri: biolink:aggregator_knowledge_source
+        description: |-
+          The default aggregator knowledge source for all associations in this resource.
+
+  AssociationChange:
+    slots:
+      - summary_group
+      - publications
+      - publication_is_added
+      - publication_is_deleted
+      - subject
+      - old_predicate
+      - new_predicate
+      - old_object
+      - new_object
+      - old_object_obsolete
+      - is_migration
+      - is_generalization
+      - is_specialization
+      - is_creation
+      - is_deletion
+      - closure_predicates
       
 
 slots:
   subject:
     description: The thing which the association is about.
     comments:
       - it is conventional for the subject to be the "entity" and the object to be the ontological descriptor
@@ -126,28 +161,69 @@
     inlined_as_list: true
   associations:
     range: Association
     multivalued: true
     inlined_as_list: true
   original_subject:
     description: The original subject of the association prior to normalization
-    slot_uri: rdf:subject
+    slot_uri: biolink:original_subject
     range: uriorcurie
     exact_mappings:
       - biolink:original_subject
   original_predicate:
     description: The original subject of the association prior to normalization
-    slot_uri: rdf:predicate
+    slot_uri: biolink:original_predicate
     range: uriorcurie
     exact_mappings:
       - biolink:original_predicate
   original_object:
     description: The original object of the association prior to normalization
-    slot_uri: rdf:subject
+    slot_uri: biolink:original_object
     range: uriorcurie
     exact_mappings:
       - biolink:original_object
+  publications:
+    description: The publications that support the association
+    slot_uri: biolink:publications
+    range: uriorcurie
+    multivalued: true
+  primary_knowledge_source:
+    description: The primary knowledge source for the association
+    slot_uri: biolink:primary_knowledge_source
+    range: uriorcurie
+  aggregator_knowledge_source:
+    description: The knowledge source that aggregated the association
+    slot_uri: biolink:aggregator_knowledge_source
+    range: uriorcurie
   denormalized_slot:
     mixin: true
     description: |-
       denormalized slots are for models that follow a denormalized data model
-  
+  summary_group:
+    range: string
+  publication_is_added:
+    range: boolean
+  publication_is_deleted:
+    range: boolean
+  old_predicate:
+    is_a: predicate
+  new_predicate:
+    is_a: predicate
+  old_object:
+    is_a: object
+  new_object:
+    is_a: object
+  old_object_obsolete:
+    range: boolean
+  is_migration:
+    range: boolean
+  is_generalization:
+    range: boolean
+  is_specialization:
+    range: boolean
+  is_creation:
+    range: boolean
+  is_deletion:
+    range: boolean
+  closure_predicates:
+    range: uriorcurie
+    multivalued: true
```

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/class_enrichment.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/class_enrichment.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/class_enrichment.py` & `oaklib-0.5.2/src/oaklib/datamodels/class_enrichment.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from class_enrichment.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-02-27T09:56:45
+# Generation date: 2023-04-21T10:35:22
 # Schema: class-enrichment
 #
 # id: https://w3id.org/oak/class-enrichment
 # description: A datamodel for representing the results of class enrichment on gene sets
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
@@ -14,22 +14,34 @@
 
 from jsonasobj2 import JsonObj, as_dict
 from linkml_runtime.linkml_model.meta import (
     EnumDefinition,
     PermissibleValue,
     PvFormulaOptions,
 )
-from linkml_runtime.linkml_model.types import Float, Integer, String, Uriorcurie
+from linkml_runtime.linkml_model.types import (
+    Boolean,
+    Float,
+    Integer,
+    String,
+    Uriorcurie,
+)
 from linkml_runtime.utils.curienamespace import CurieNamespace
 from linkml_runtime.utils.dataclass_extensions_376 import (
     dataclasses_init_fn_with_kwargs,
 )
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from linkml_runtime.utils.formatutils import camelcase, sfx, underscore
-from linkml_runtime.utils.metamodelcore import URIorCURIE, bnode, empty_dict, empty_list
+from linkml_runtime.utils.metamodelcore import (
+    Bool,
+    URIorCURIE,
+    bnode,
+    empty_dict,
+    empty_list,
+)
 from linkml_runtime.utils.slot import Slot
 from linkml_runtime.utils.yamlutils import (
     YAMLRoot,
     extended_float,
     extended_int,
     extended_str,
 )
@@ -133,21 +145,25 @@
     class_class_curie: ClassVar[str] = "ontoenrich:ClassEnrichmentResult"
     class_name: ClassVar[str] = "ClassEnrichmentResult"
     class_model_uri: ClassVar[URIRef] = ONTOENRICH.ClassEnrichmentResult
 
     class_id: Union[str, URIorCURIE] = None
     p_value: float = None
     class_label: Optional[str] = None
+    rank: Optional[int] = None
     p_value_adjusted: Optional[float] = None
     false_discovery_rate: Optional[float] = None
     fold_enrichment: Optional[float] = None
+    probability: Optional[float] = None
     sample_count: Optional[int] = None
     sample_total: Optional[int] = None
     background_count: Optional[int] = None
     background_total: Optional[int] = None
+    ancestor_of_more_informative_result: Optional[Union[bool, Bool]] = None
+    descendant_of_more_informative_result: Optional[Union[bool, Bool]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.class_id):
             self.MissingRequiredField("class_id")
         if not isinstance(self.class_id, URIorCURIE):
             self.class_id = URIorCURIE(self.class_id)
 
@@ -155,37 +171,57 @@
             self.MissingRequiredField("p_value")
         if not isinstance(self.p_value, float):
             self.p_value = float(self.p_value)
 
         if self.class_label is not None and not isinstance(self.class_label, str):
             self.class_label = str(self.class_label)
 
+        if self.rank is not None and not isinstance(self.rank, int):
+            self.rank = int(self.rank)
+
         if self.p_value_adjusted is not None and not isinstance(self.p_value_adjusted, float):
             self.p_value_adjusted = float(self.p_value_adjusted)
 
         if self.false_discovery_rate is not None and not isinstance(
             self.false_discovery_rate, float
         ):
             self.false_discovery_rate = float(self.false_discovery_rate)
 
         if self.fold_enrichment is not None and not isinstance(self.fold_enrichment, float):
             self.fold_enrichment = float(self.fold_enrichment)
 
+        if self.probability is not None and not isinstance(self.probability, float):
+            self.probability = float(self.probability)
+
         if self.sample_count is not None and not isinstance(self.sample_count, int):
             self.sample_count = int(self.sample_count)
 
         if self.sample_total is not None and not isinstance(self.sample_total, int):
             self.sample_total = int(self.sample_total)
 
         if self.background_count is not None and not isinstance(self.background_count, int):
             self.background_count = int(self.background_count)
 
         if self.background_total is not None and not isinstance(self.background_total, int):
             self.background_total = int(self.background_total)
 
+        if self.ancestor_of_more_informative_result is not None and not isinstance(
+            self.ancestor_of_more_informative_result, Bool
+        ):
+            self.ancestor_of_more_informative_result = Bool(
+                self.ancestor_of_more_informative_result
+            )
+
+        if self.descendant_of_more_informative_result is not None and not isinstance(
+            self.descendant_of_more_informative_result, Bool
+        ):
+            self.descendant_of_more_informative_result = Bool(
+                self.descendant_of_more_informative_result
+            )
+
         super().__post_init__(**kwargs)
 
 
 # Enumerations
 class SortFieldEnum(EnumDefinitionImpl):
     """
     The field to sort by
@@ -239,14 +275,23 @@
     name="classEnrichmentResult__class_label",
     curie=ONTOENRICH.curie("class_label"),
     model_uri=ONTOENRICH.classEnrichmentResult__class_label,
     domain=None,
     range=Optional[str],
 )
 
+slots.classEnrichmentResult__rank = Slot(
+    uri=ONTOENRICH.rank,
+    name="classEnrichmentResult__rank",
+    curie=ONTOENRICH.curie("rank"),
+    model_uri=ONTOENRICH.classEnrichmentResult__rank,
+    domain=None,
+    range=Optional[int],
+)
+
 slots.classEnrichmentResult__p_value = Slot(
     uri=OBI["0000175"],
     name="classEnrichmentResult__p_value",
     curie=OBI.curie("0000175"),
     model_uri=ONTOENRICH.classEnrichmentResult__p_value,
     domain=None,
     range=float,
@@ -275,14 +320,23 @@
     name="classEnrichmentResult__fold_enrichment",
     curie=ONTOENRICH.curie("fold_enrichment"),
     model_uri=ONTOENRICH.classEnrichmentResult__fold_enrichment,
     domain=None,
     range=Optional[float],
 )
 
+slots.classEnrichmentResult__probability = Slot(
+    uri=ONTOENRICH.probability,
+    name="classEnrichmentResult__probability",
+    curie=ONTOENRICH.curie("probability"),
+    model_uri=ONTOENRICH.classEnrichmentResult__probability,
+    domain=None,
+    range=Optional[float],
+)
+
 slots.classEnrichmentResult__sample_count = Slot(
     uri=ONTOENRICH.sample_count,
     name="classEnrichmentResult__sample_count",
     curie=ONTOENRICH.curie("sample_count"),
     model_uri=ONTOENRICH.classEnrichmentResult__sample_count,
     domain=None,
     range=Optional[int],
@@ -310,7 +364,25 @@
     uri=ONTOENRICH.background_total,
     name="classEnrichmentResult__background_total",
     curie=ONTOENRICH.curie("background_total"),
     model_uri=ONTOENRICH.classEnrichmentResult__background_total,
     domain=None,
     range=Optional[int],
 )
+
+slots.classEnrichmentResult__ancestor_of_more_informative_result = Slot(
+    uri=ONTOENRICH.ancestor_of_more_informative_result,
+    name="classEnrichmentResult__ancestor_of_more_informative_result",
+    curie=ONTOENRICH.curie("ancestor_of_more_informative_result"),
+    model_uri=ONTOENRICH.classEnrichmentResult__ancestor_of_more_informative_result,
+    domain=None,
+    range=Optional[Union[bool, Bool]],
+)
+
+slots.classEnrichmentResult__descendant_of_more_informative_result = Slot(
+    uri=ONTOENRICH.descendant_of_more_informative_result,
+    name="classEnrichmentResult__descendant_of_more_informative_result",
+    curie=ONTOENRICH.curie("descendant_of_more_informative_result"),
+    model_uri=ONTOENRICH.classEnrichmentResult__descendant_of_more_informative_result,
+    domain=None,
+    range=Optional[Union[bool, Bool]],
+)
```

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/class_enrichment.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/class_enrichment.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -65,40 +65,54 @@
       class_id:
         description: The class id
         range: uriorcurie
         required: true
       class_label:
         description: The class label
         range: string
+      rank:
+        description: The rank of this result
+        range: integer
       p_value:
         slot_uri: OBI:0000175
         description: The p-value
         range: float
         required: true
       p_value_adjusted:
         description: The adjusted p-value
         range: float
       false_discovery_rate:
         description: The false discovery rate
         range: float
       fold_enrichment:
         description: The fold enrichment
         range: float
+      probability:
+        description: The probability, as estimated by model-based approaches
+        range: float
+        minimum_value: 0
+        maximum_value: 1
       sample_count:
         description: The number of entities in the sample with this class
         range: integer
       sample_total:
         description: The total number of entities in the sample
         range: integer
       background_count:
         description: The background count
         range: integer
       background_total:
         description: The background total
         range: integer
+      ancestor_of_more_informative_result:
+        description: This term is more general than a previously reported result
+        range: boolean
+      descendant_of_more_informative_result:
+        description: This term is more specific than a previously reported result
+        range: boolean
 
 enums:
   SortFieldEnum:
     description: The field to sort by
     permissible_values:
       ANY:
       P_VALUE:
```

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/cross_ontology_diff.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/cross_ontology_diff.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/cross_ontology_diff.py` & `oaklib-0.5.2/src/oaklib/datamodels/cross_ontology_diff.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/cross_ontology_diff.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/cross_ontology_diff.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/cx.py` & `oaklib-0.5.2/src/oaklib/datamodels/cx.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/cx.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/cx.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/fhir.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/fhir.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/fhir.py` & `oaklib-0.5.2/src/oaklib/datamodels/fhir.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/fhir.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/fhir.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/input_specification.py` & `oaklib-0.5.2/src/oaklib/datamodels/input_specification.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from input_specification.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-04-12T10:17:53
+# Generation date: 2023-04-13T08:19:53
 # Schema: inputspec
 #
 # id: https://w3id.org/oaklib/input-specification
 # description: A data model for representing a set of inputs to OAK
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
 import dataclasses
@@ -14,22 +14,22 @@
 
 from jsonasobj2 import JsonObj, as_dict
 from linkml_runtime.linkml_model.meta import (
     EnumDefinition,
     PermissibleValue,
     PvFormulaOptions,
 )
-from linkml_runtime.linkml_model.types import String
+from linkml_runtime.linkml_model.types import String, Uriorcurie
 from linkml_runtime.utils.curienamespace import CurieNamespace
 from linkml_runtime.utils.dataclass_extensions_376 import (
     dataclasses_init_fn_with_kwargs,
 )
 from linkml_runtime.utils.enumerations import EnumDefinitionImpl
 from linkml_runtime.utils.formatutils import camelcase, sfx, underscore
-from linkml_runtime.utils.metamodelcore import bnode, empty_dict, empty_list
+from linkml_runtime.utils.metamodelcore import URIorCURIE, bnode, empty_dict, empty_list
 from linkml_runtime.utils.slot import Slot
 from linkml_runtime.utils.yamlutils import (
     YAMLRoot,
     extended_float,
     extended_int,
     extended_str,
 )
@@ -38,14 +38,15 @@
 metamodel_version = "1.7.0"
 version = None
 
 # Overwrite dataclasses _init_fn to add **kwargs in __init__
 dataclasses._init_fn = dataclasses_init_fn_with_kwargs
 
 # Namespaces
+BIOLINK = CurieNamespace("biolink", "http://example.org/UNKNOWN/biolink/")
 DCTERMS = CurieNamespace("dcterms", "http://purl.org/dc/terms/")
 ITEMLIST = CurieNamespace("itemList", "https://w3id.org/linkml/item-list/")
 LINKML = CurieNamespace("linkml", "https://w3id.org/linkml/")
 PROV = CurieNamespace("prov", "http://www.w3.org/ns/prov#")
 RDF = CurieNamespace("rdf", "http://www.w3.org/1999/02/22-rdf-syntax-ns#")
 SCHEMA = CurieNamespace("schema", "http://schema.org/")
 DEFAULT_ = ITEMLIST
@@ -121,14 +122,16 @@
     class_name: ClassVar[str] = "Resource"
     class_model_uri: ClassVar[URIRef] = ITEMLIST.Resource
 
     id: Union[str, ResourceId] = None
     path: Optional[str] = None
     format: Optional[str] = None
     selector: Optional[str] = None
+    aggregator_knowledge_source: Optional[Union[str, URIorCURIE]] = None
+    primary_knowledge_source: Optional[Union[str, URIorCURIE]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
         if self._is_empty(self.id):
             self.MissingRequiredField("id")
         if not isinstance(self.id, ResourceId):
             self.id = ResourceId(self.id)
 
@@ -137,14 +140,24 @@
 
         if self.format is not None and not isinstance(self.format, str):
             self.format = str(self.format)
 
         if self.selector is not None and not isinstance(self.selector, str):
             self.selector = str(self.selector)
 
+        if self.aggregator_knowledge_source is not None and not isinstance(
+            self.aggregator_knowledge_source, URIorCURIE
+        ):
+            self.aggregator_knowledge_source = URIorCURIE(self.aggregator_knowledge_source)
+
+        if self.primary_knowledge_source is not None and not isinstance(
+            self.primary_knowledge_source, URIorCURIE
+        ):
+            self.primary_knowledge_source = URIorCURIE(self.primary_knowledge_source)
+
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class OntologyResource(Resource):
     """
     A resource that points to an ontology
@@ -348,14 +361,32 @@
     name="resource__selector",
     curie=ITEMLIST.curie("selector"),
     model_uri=ITEMLIST.resource__selector,
     domain=None,
     range=Optional[str],
 )
 
+slots.resource__aggregator_knowledge_source = Slot(
+    uri=BIOLINK.aggregator_knowledge_source,
+    name="resource__aggregator_knowledge_source",
+    curie=BIOLINK.curie("aggregator_knowledge_source"),
+    model_uri=ITEMLIST.resource__aggregator_knowledge_source,
+    domain=None,
+    range=Optional[Union[str, URIorCURIE]],
+)
+
+slots.resource__primary_knowledge_source = Slot(
+    uri=BIOLINK.primary_knowledge_source,
+    name="resource__primary_knowledge_source",
+    curie=BIOLINK.curie("primary_knowledge_source"),
+    model_uri=ITEMLIST.resource__primary_knowledge_source,
+    domain=None,
+    range=Optional[Union[str, URIorCURIE]],
+)
+
 slots.associationResource__normalizers = Slot(
     uri=ITEMLIST.normalizers,
     name="associationResource__normalizers",
     curie=ITEMLIST.curie("normalizers"),
     model_uri=ITEMLIST.associationResource__normalizers,
     domain=None,
     range=Optional[Union[Union[dict, Normalizer], List[Union[dict, Normalizer]]]],
```

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/input_specification.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/input_specification.yaml`

 * *Files 22% similar despite different names*

```diff
@@ -54,14 +54,25 @@
           The path of the resource. May be a URL or file path
       format:
         range: string
       selector:
         range: string
         description: >-
           The selector of the ontology resource
+      aggregator_knowledge_source:
+        range: uriorcurie
+        slot_uri: biolink:aggregator_knowledge_source
+        description: >-
+          The knowledge source that is the aggregator of the resource
+      primary_knowledge_source:
+        range: uriorcurie
+        slot_uri: biolink:primary_knowledge_source
+        description: >-
+          The knowledge source that is the primary source of the resource
+         
 
   OntologyResource:
     description: >-
       A resource that points to an ontology
     is_a: Resource
 
   AssociationResource:
```

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/item_list.py` & `oaklib-0.5.2/src/oaklib/datamodels/item_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Auto generated from item_list.yaml by pythongen.py version: 0.9.0
-# Generation date: 2023-04-10T16:46:21
+# Generation date: 2023-04-13T19:34:47
 # Schema: itemList
 #
 # id: https://w3id.org/oak/item-list
 # description: A data model for representing simple lists of entities such as genes. The data model is based on
 #              the schema.org ItemList class.
 # license: https://creativecommons.org/publicdomain/zero/1.0/
 
@@ -59,15 +59,19 @@
 DEFAULT_ = ITEMLIST
 
 
 # Types
 
 
 # Class references
-class ListItemId(extended_str):
+class ListItemElementId(extended_str):
+    pass
+
+
+class ThingId(URIorCURIE):
     pass
 
 
 @dataclass
 class ItemListCollection(YAMLRoot):
     """
     a set of item lists
@@ -107,19 +111,22 @@
     class_name: ClassVar[str] = "ItemList"
     class_model_uri: ClassVar[URIRef] = ITEMLIST.ItemList
 
     id: Optional[Union[str, URIorCURIE]] = None
     name: Optional[str] = None
     description: Optional[str] = None
     itemListElements: Optional[
-        Union[Union[str, ListItemId], List[Union[str, ListItemId]]]
+        Union[Union[str, ListItemElementId], List[Union[str, ListItemElementId]]]
     ] = empty_list()
     numberOfItems: Optional[Union[str, "ItemListOrderType"]] = None
     itemMetadataMap: Optional[
-        Union[Dict[Union[str, ListItemId], Union[dict, "ListItem"]], List[Union[dict, "ListItem"]]]
+        Union[
+            Dict[Union[str, ListItemElementId], Union[dict, "ListItem"]],
+            List[Union[dict, "ListItem"]],
+        ]
     ] = empty_dict()
     categories: Optional[Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]] = empty_list()
     keywords: Optional[Union[str, List[str]]] = empty_list()
     additionalType: Optional[
         Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]
     ] = empty_list()
     wasGeneratedBy: Optional[
@@ -137,22 +144,23 @@
             self.description = str(self.description)
 
         if not isinstance(self.itemListElements, list):
             self.itemListElements = (
                 [self.itemListElements] if self.itemListElements is not None else []
             )
         self.itemListElements = [
-            v if isinstance(v, ListItemId) else ListItemId(v) for v in self.itemListElements
+            v if isinstance(v, ListItemElementId) else ListItemElementId(v)
+            for v in self.itemListElements
         ]
 
         if self.numberOfItems is not None and not isinstance(self.numberOfItems, ItemListOrderType):
             self.numberOfItems = ItemListOrderType(self.numberOfItems)
 
         self._normalize_inlined_as_dict(
-            slot_name="itemMetadataMap", slot_type=ListItem, key_name="id", keyed=True
+            slot_name="itemMetadataMap", slot_type=ListItem, key_name="elementId", keyed=True
         )
 
         if not isinstance(self.categories, list):
             self.categories = [self.categories] if self.categories is not None else []
         self.categories = [
             v if isinstance(v, URIorCURIE) else URIorCURIE(v) for v in self.categories
         ]
@@ -185,62 +193,64 @@
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = SCHEMA.ListItem
     class_class_curie: ClassVar[str] = "schema:ListItem"
     class_name: ClassVar[str] = "ListItem"
     class_model_uri: ClassVar[URIRef] = ITEMLIST.ListItem
 
-    id: Union[str, ListItemId] = None
+    elementId: Union[str, ListItemElementId] = None
     idType: Optional[Union[str, URIorCURIE]] = None
     item: Optional[Union[dict, "Thing"]] = None
     position: Optional[int] = None
-    previousItem: Optional[Union[str, ListItemId]] = None
+    previousItem: Optional[Union[str, ListItemElementId]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self._is_empty(self.id):
-            self.MissingRequiredField("id")
-        if not isinstance(self.id, ListItemId):
-            self.id = ListItemId(self.id)
+        if self._is_empty(self.elementId):
+            self.MissingRequiredField("elementId")
+        if not isinstance(self.elementId, ListItemElementId):
+            self.elementId = ListItemElementId(self.elementId)
 
         if self.idType is not None and not isinstance(self.idType, URIorCURIE):
             self.idType = URIorCURIE(self.idType)
 
         if self.item is not None and not isinstance(self.item, Thing):
             self.item = Thing(**as_dict(self.item))
 
         if self.position is not None and not isinstance(self.position, int):
             self.position = int(self.position)
 
-        if self.previousItem is not None and not isinstance(self.previousItem, ListItemId):
-            self.previousItem = ListItemId(self.previousItem)
+        if self.previousItem is not None and not isinstance(self.previousItem, ListItemElementId):
+            self.previousItem = ListItemElementId(self.previousItem)
 
         super().__post_init__(**kwargs)
 
 
 @dataclass
 class Thing(YAMLRoot):
     _inherited_slots: ClassVar[List[str]] = []
 
     class_class_uri: ClassVar[URIRef] = SCHEMA.Thing
     class_class_curie: ClassVar[str] = "schema:Thing"
     class_name: ClassVar[str] = "Thing"
     class_model_uri: ClassVar[URIRef] = ITEMLIST.Thing
 
-    identifier: Optional[Union[str, URIorCURIE]] = None
+    id: Union[str, ThingId] = None
     name: Optional[str] = None
     url: Optional[Union[str, URI]] = None
     identifiers: Optional[
         Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]
     ] = empty_list()
     description: Optional[str] = None
     type: Optional[Union[str, URIorCURIE]] = None
 
     def __post_init__(self, *_: List[str], **kwargs: Dict[str, Any]):
-        if self.identifier is not None and not isinstance(self.identifier, URIorCURIE):
-            self.identifier = URIorCURIE(self.identifier)
+        if self._is_empty(self.id):
+            self.MissingRequiredField("id")
+        if not isinstance(self.id, ThingId):
+            self.id = ThingId(self.id)
 
         if self.name is not None and not isinstance(self.name, str):
             self.name = str(self.name)
 
         if self.url is not None and not isinstance(self.url, URI):
             self.url = URI(self.url)
 
@@ -328,15 +338,15 @@
 
 slots.itemList__itemListElements = Slot(
     uri=SCHEMA.itemListElement,
     name="itemList__itemListElements",
     curie=SCHEMA.curie("itemListElement"),
     model_uri=ITEMLIST.itemList__itemListElements,
     domain=None,
-    range=Optional[Union[Union[str, ListItemId], List[Union[str, ListItemId]]]],
+    range=Optional[Union[Union[str, ListItemElementId], List[Union[str, ListItemElementId]]]],
 )
 
 slots.itemList__numberOfItems = Slot(
     uri=SCHEMA.numberOfItems,
     name="itemList__numberOfItems",
     curie=SCHEMA.curie("numberOfItems"),
     model_uri=ITEMLIST.itemList__numberOfItems,
@@ -347,15 +357,17 @@
 slots.itemList__itemMetadataMap = Slot(
     uri=ITEMLIST.itemMetadataMap,
     name="itemList__itemMetadataMap",
     curie=ITEMLIST.curie("itemMetadataMap"),
     model_uri=ITEMLIST.itemList__itemMetadataMap,
     domain=None,
     range=Optional[
-        Union[Dict[Union[str, ListItemId], Union[dict, ListItem]], List[Union[dict, ListItem]]]
+        Union[
+            Dict[Union[str, ListItemElementId], Union[dict, ListItem]], List[Union[dict, ListItem]]
+        ]
     ],
 )
 
 slots.itemList__categories = Slot(
     uri=DCTERMS.subject,
     name="itemList__categories",
     curie=DCTERMS.curie("subject"),
@@ -387,19 +399,19 @@
     name="itemList__wasGeneratedBy",
     curie=PROV.curie("wasGeneratedBy"),
     model_uri=ITEMLIST.itemList__wasGeneratedBy,
     domain=None,
     range=Optional[Union[Union[str, URIorCURIE], List[Union[str, URIorCURIE]]]],
 )
 
-slots.listItem__id = Slot(
-    uri=ITEMLIST.id,
-    name="listItem__id",
-    curie=ITEMLIST.curie("id"),
-    model_uri=ITEMLIST.listItem__id,
+slots.listItem__elementId = Slot(
+    uri=ITEMLIST.elementId,
+    name="listItem__elementId",
+    curie=ITEMLIST.curie("elementId"),
+    model_uri=ITEMLIST.listItem__elementId,
     domain=None,
     range=URIRef,
 )
 
 slots.listItem__idType = Slot(
     uri=ITEMLIST.idType,
     name="listItem__idType",
@@ -429,24 +441,24 @@
 
 slots.listItem__previousItem = Slot(
     uri=SCHEMA.previousItem,
     name="listItem__previousItem",
     curie=SCHEMA.curie("previousItem"),
     model_uri=ITEMLIST.listItem__previousItem,
     domain=None,
-    range=Optional[Union[str, ListItemId]],
+    range=Optional[Union[str, ListItemElementId]],
 )
 
-slots.thing__identifier = Slot(
+slots.thing__id = Slot(
     uri=SCHEMA.identifier,
-    name="thing__identifier",
+    name="thing__id",
     curie=SCHEMA.curie("identifier"),
-    model_uri=ITEMLIST.thing__identifier,
+    model_uri=ITEMLIST.thing__id,
     domain=None,
-    range=Optional[Union[str, URIorCURIE]],
+    range=URIRef,
 )
 
 slots.thing__name = Slot(
     uri=RDFS.label,
     name="thing__name",
     curie=RDFS.curie("label"),
     model_uri=ITEMLIST.thing__name,
```

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/item_list.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/item_list.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -22,36 +22,52 @@
 
 #==================================
 # Classes                         #
 #==================================
 classes:
 
   ItemListCollection:
+    aliases:
+      - item list catalog
     description: a set of item lists
+    comments:
+      - this is used for when you wish to pass around multiple lists.
     attributes:
       itemLists:
         range: ItemList
         multivalued: true
         inlined: true
 
   ItemList:
+    aliases:
+      - list
     description: a list of entities plus metadata
     class_uri: schema:ItemList
     close_mappings:
       - rdf:List
     attributes:
       id:
         range: uriorcurie
         description: The identifier of the list
+        comments:
+          - this is optional and hence declared as an identifier
       name:
         range: string
         description: The name of the list
+        examples:
+          - description: mTOR-pathway
+          - description: my-shopping-list
+        recommended: true
       description:
         range: string
         description: A description of the list
+        examples:
+          - description: A list of genes in the mTOR pathway
+          - description: A list of items to buy at the supermarket
+        recommended: true
       itemListElements:
         singular_name: itemListElement
         slot_uri: schema:itemListElement
         range: ListItem
         multivalued: true
         inlined: false
         description: The entities in the list, represented as a simple list
@@ -97,15 +113,15 @@
         slot_uri: prov:wasGeneratedBy
         multivalued: true
 
   ListItem:
     description: an item in an item list
     class_uri: schema:ListItem
     attributes:
-      id:
+      elementId:
         range: string
         description: >
           The identifier of the item. Note this can be a 'proper' CURIE ID or any other unique field,
           for example symbol
         key: true
       idType:
         range: uriorcurie
@@ -115,32 +131,34 @@
           - value: biolink:symbol
           - value: skos:prefLabel
           - value: schema:identifier
       item:
         range: Thing
         description: The item represented by the list item
         slot_uri: schema:item
+        inlined: true
       position:
         range: integer
         description: The position of the item in the list
         slot_uri: schema:position
       previousItem:
         range: ListItem
         description: The previous item in the list
         slot_uri: schema:previousItem
 
   Thing:
     class_uri: schema:Thing
     attributes:
-      identifier:
+      id:
         range: uriorcurie
         description: >-
           The identifier of the item. Note this can be a 'proper' CURIE ID or any other unique field,
           for example symbol
         slot_uri: schema:identifier
+        identifier: true
       name:
         range: string
         description: The name of the item
         slot_uri: rdfs:label
       url:
         range: uri
         description: A URL for the item
```

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/lexical_index.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/lexical_index.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/lexical_index.py` & `oaklib-0.5.2/src/oaklib/datamodels/lexical_index.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/lexical_index.schema.json` & `oaklib-0.5.2/src/oaklib/datamodels/lexical_index.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/lexical_index.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/lexical_index.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/mapping_cluster_datamodel.py` & `oaklib-0.5.2/src/oaklib/datamodels/mapping_cluster_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/mapping_cluster_datamodel.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/mapping_cluster_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/mapping_rules_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.py` & `oaklib-0.5.2/src/oaklib/datamodels/mapping_rules_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.schema.json` & `oaklib-0.5.2/src/oaklib/datamodels/mapping_rules_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/mapping_rules_datamodel.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/mapping_rules_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/obograph.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/obograph.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/obograph.py` & `oaklib-0.5.2/src/oaklib/datamodels/obograph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/obograph.schema.json` & `oaklib-0.5.2/src/oaklib/datamodels/obograph.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/obograph.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/obograph.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/ontology_metadata.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.py` & `oaklib-0.5.2/src/oaklib/datamodels/ontology_metadata.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.schema.json` & `oaklib-0.5.2/src/oaklib/datamodels/ontology_metadata.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/ontology_metadata.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/ontology_metadata.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/oxo.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/oxo.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/oxo.py` & `oaklib-0.5.2/src/oaklib/datamodels/oxo.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/oxo.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/oxo.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/search.py` & `oaklib-0.5.2/src/oaklib/datamodels/search.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/search_datamodel.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/search_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/search_datamodel.py` & `oaklib-0.5.2/src/oaklib/datamodels/search_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/search_datamodel.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/search_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/similarity.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/similarity.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/similarity.py` & `oaklib-0.5.2/src/oaklib/datamodels/similarity.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/similarity.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/similarity.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/summary_statistics_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.py` & `oaklib-0.5.2/src/oaklib/datamodels/summary_statistics_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.schema.json` & `oaklib-0.5.2/src/oaklib/datamodels/summary_statistics_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/summary_statistics_datamodel.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/summary_statistics_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/taxon_constraints.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/taxon_constraints.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/taxon_constraints.py` & `oaklib-0.5.2/src/oaklib/datamodels/taxon_constraints.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/taxon_constraints.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/taxon_constraints.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/text_annotator.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/text_annotator.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/text_annotator.py` & `oaklib-0.5.2/src/oaklib/datamodels/text_annotator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/text_annotator.schema.json` & `oaklib-0.5.2/src/oaklib/datamodels/text_annotator.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/text_annotator.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/text_annotator.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/validation_datamodel.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.py` & `oaklib-0.5.2/src/oaklib/datamodels/validation_datamodel.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.schema.json` & `oaklib-0.5.2/src/oaklib/datamodels/validation_datamodel.schema.json`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/validation_datamodel.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/validation_datamodel.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/value_set_configuration.owl.ttl` & `oaklib-0.5.2/src/oaklib/datamodels/value_set_configuration.owl.ttl`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/value_set_configuration.py` & `oaklib-0.5.2/src/oaklib/datamodels/value_set_configuration.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/value_set_configuration.yaml` & `oaklib-0.5.2/src/oaklib/datamodels/value_set_configuration.yaml`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/datamodels/vocabulary.py` & `oaklib-0.5.2/src/oaklib/datamodels/vocabulary.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/__init__.py` & `oaklib-0.5.2/src/oaklib/implementations/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 from functools import cache
 
 from class_resolver import ClassResolver
 
 from oaklib.implementations.aggregator.aggregator_implementation import (
     AggregatorImplementation,
 )
+from oaklib.implementations.amigo.amigo_implementation import AmiGOImplementation
 from oaklib.implementations.cx.cx_implementation import CXImplementation
+from oaklib.implementations.eutils.pubmed_implementation import PubMedImplementation
 from oaklib.implementations.funowl.funowl_implementation import FunOwlImplementation
 from oaklib.implementations.gilda import GildaImplementation
 from oaklib.implementations.kgx.kgx_implementation import KGXImplementation
 from oaklib.implementations.ols import (
     BaseOlsImplementation,
     OlsImplementation,
     TIBOlsImplementation,
@@ -30,14 +32,15 @@
 from oaklib.implementations.ontoportal.matportal_implementation import (
     MatPortalImplementation,
 )
 from oaklib.implementations.ontoportal.ontoportal_implementation_base import (
     OntoPortalImplementationBase,
 )
 from oaklib.implementations.pronto.pronto_implementation import ProntoImplementation
+from oaklib.implementations.rustsim.rustsim_implementation import RustSimImplementation
 from oaklib.implementations.simpleobo.simple_obo_implementation import (
     SimpleOboImplementation,
 )
 from oaklib.implementations.sparql.lov_implementation import LovImplementation
 from oaklib.implementations.sparql.oak_metamodel_implementation import (
     OakMetaModelImplementation,
 )
@@ -55,33 +58,36 @@
 from oaklib.interfaces import OntologyInterface
 
 __all__ = [
     "get_implementation_resolver",
     # Concrete classes
     "AggregatorImplementation",
     "AgroPortalImplementation",
+    "AmiGOImplementation",
     "BioPortalImplementation",
     "CXImplementation",
     "EcoPortalImplementation",
     "MatPortalImplementation",
     "OlsImplementation",
     "TIBOlsImplementation",
     "OntobeeImplementation",
     "ProntoImplementation",
     "SimpleOboImplementation",
     "SqlImplementation",
     "UbergraphImplementation",
     "LovImplementation",
     "SparqlImplementation",
     "WikidataImplementation",
+    "PubMedImplementation",
     "FunOwlImplementation",
     "GildaImplementation",
     "KGXImplementation",
     "TranslatorImplementation",
     "OakMetaModelImplementation",
+    "RustSimImplementation",
 ]
 
 
 @cache
 def get_implementation_resolver() -> ClassResolver[OntologyInterface]:
     """
     Get a class resolver for all implementations (adapters).
@@ -120,14 +126,15 @@
             "prontolib": ProntoImplementation,
             "simpleobo": SimpleOboImplementation,
             "sqlite": SqlImplementation,
             "rdflib": SparqlImplementation,
             "oak": OakMetaModelImplementation,
             "cx": CXImplementation,
             "ndexbio": CXImplementation,
+            "rustsim": RustSimImplementation,
         }
     )
 
     # Plugins which want to register an implementation should use
     # the entrypoint group "oaklib.plugins". The name of the entry
     # point will be used as a possible match against the input scheme
     # prefix. The value of the entry point should be an implementation
```

### Comparing `oaklib-0.5.1/src/oaklib/implementations/aggregator/aggregator_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/aggregator/aggregator_implementation.py`

 * *Files 9% similar despite different names*

```diff
@@ -36,23 +36,46 @@
     RelationGraphInterface,
     OboGraphInterface,
     SearchInterface,
     MappingProviderInterface,
     TextAnnotatorInterface,
 ):
     """
-    Wraps multiple implementations and integrates results together.
+    An OAK adapter that wraps multiple implementations and integrates results together.
 
     This allows for multiple implementations to be wrapped, with calls to
     the aggregator farming out queries to multiple implementations, and weaving
     the results together.
 
-    Documentation:
+    >>> from oaklib import get_adapter
+    >>> from oaklib.implementations import AggregatorImplementation
+    >>> hp = get_adapter("sqlite:obo:hp")
+    >>> mp = get_adapter("sqlite:obo:mp")
+    >>> agg = AggregatorImplementation(implementations=[hp, mp])
+    >>> for entity in sorted(agg.basic_search("morphology")):
+    ...     print(entity)
+    <BLANKLINE>
+    ...
+    HP:3000036
+    ...
+    MP:0031139
+    ...
+
+    Command Line Usage
+    ------------------
+
+    Use the :code:`--add` (:code:`-a`) option before the main command to add additional implementations.
+
+    E.g
+
+    .. code::
+
+        runoak -i db/mp.db -a db/hp.db COMMAND [COMMAND OPTIONS]
+
 
-    - `Aggregator Implementation <https://incatools.github.io/ontology-access-kit/implementations/aggregator.html>`_
     """
 
     implementations: List[BasicOntologyInterface] = None
 
     def _delegate_iterator(self, func: Callable) -> Iterable:
         for i in self.implementations:
             for v in func(i):
```

### Comparing `oaklib-0.5.1/src/oaklib/implementations/cx/cx_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/cx/cx_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/funowl/funowl_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/funowl/funowl_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/gilda.py` & `oaklib-0.5.2/src/oaklib/implementations/gilda.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/kgx/kgx_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/kgx/kgx_implementation.py`

 * *Files 1% similar despite different names*

```diff
@@ -204,25 +204,16 @@
     DumperInterface,
 ):
     """
     A :class:`OntologyInterface` implementation that wraps a KGX Relational Database.
 
     This could be a local file (accessed via SQL Lite) or a local/remote server (e.g PostgreSQL).
 
-    To connect, either use KGXImplementation directly:
-
-    .. packages:: python
-
-        >>> oi = KGXImplementation(OntologyResource(slug=f"sqlite:///{path}"))
-
-    Or use a selector:
-
-    .. packages:: python
-
-        >>> oi = get_implementation_from_shorthand('obojson:path/to/my/ontology.db')
+    >>> from oaklib import get_adapter
+    >>> oi = get_adapter('../semantic-sql/db/monarch-kg.db')
 
     The schema is assumed to follow the `semantic-sql <https://github.com/incatools/semantic-sql>`_ schema.
 
     This uses SQLAlchemy ORM Models:
 
     - :class:`NodeProperty`
     - :class:`Edge`
```

### Comparing `oaklib-0.5.1/src/oaklib/implementations/obograph/obograph_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/obograph/obograph_implementation.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,17 +74,22 @@
 
     This implementation works off of an in-memory GraphDocument object.
 
     To use:
 
     .. packages :: python
 
-        >>> oi = get_implementation_from_shorthand('obojson:path/to/my/ontology.json')
-        >>> for term in oi.entities():
-        >>>     ...
+    >>> from oaklib import get_adapter
+    >>> oi = get_adapter('obograph:tests/input/go-nucleus.json')
+    >>> for node_id in oi.entities():
+    ...     print(node_id, oi.label(node_id))
+    <BLANKLINE>
+    ...
+    GO:0043226 organelle
+    ...
     """
 
     obograph_document: GraphDocument = None
     _relationship_index_cache: Dict[CURIE, List[RELATIONSHIP]] = None
 
     def __post_init__(self):
         if self.obograph_document is None:
```

### Comparing `oaklib-0.5.1/src/oaklib/implementations/ols/ols_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/ols/ols_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/ols/oxo_utils.py` & `oaklib-0.5.2/src/oaklib/implementations/ols/oxo_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/ontobee/ontobee_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/sparql/oak_metamodel_implementation.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,49 +1,53 @@
 from dataclasses import dataclass
-from typing import Optional
 
+import rdflib
+
+import oaklib.datamodels as dm
 from oaklib.implementations.sparql.abstract_sparql_implementation import (
     AbstractSparqlImplementation,
 )
+from oaklib.interfaces.differ_interface import DifferInterface
 from oaklib.interfaces.mapping_provider_interface import MappingProviderInterface
 from oaklib.interfaces.obograph_interface import OboGraphInterface
+from oaklib.interfaces.patcher_interface import PatcherInterface
 from oaklib.interfaces.search_interface import SearchInterface
+from oaklib.interfaces.semsim_interface import SemanticSimilarityInterface
+
+__all__ = [
+    "OakMetaModelImplementation",
+]
 
-ONTOBEE_MERGED_GRAPH_PREFIX = "http://purl.obolibrary.org/obo/merged/"
+from oaklib.mappers.ontology_metadata_mapper import load_default_sssom
 
 
 @dataclass
-class OntobeeImplementation(
-    AbstractSparqlImplementation, SearchInterface, MappingProviderInterface, OboGraphInterface
+class OakMetaModelImplementation(
+    AbstractSparqlImplementation,
+    DifferInterface,
+    SearchInterface,
+    MappingProviderInterface,
+    OboGraphInterface,
+    PatcherInterface,
+    SemanticSimilarityInterface,
 ):
     """
-    Wraps the Ontobee sparql endpoint
-
-    An OntobeeImplementation can be initialed by:
-
-        .. packages:: python
+    Wraps the internal OAK data models.
 
-           >>>  oi = OntobeeImplementation()
+    OAK uses a number of different data models, see:
 
-    The default ontobee endpoint will be assumed
+    `<https://incatools.github.io/ontology-access-kit/datamodels>`_
 
-    Alternatively, use a selector:
-
-    .. packages :: python
-
-        >>> oi = get_implementation_from_shorthand("ontobee:")
-        >>> for a in oi.ancestors("UBERON:0002398", predicates=[IS_A]):
-        >>>     ...
-
-
-    See: `<https://www.ontobee.org/>`_
+    Each of these datamodels is also stored as RDF/OWL, which allows
+    for introspection as ontologies.
     """
 
-    def _default_url(self) -> str:
-        return "http://sparql.hegroup.org/sparql"
-
-    @property
-    def named_graph(self) -> Optional[str]:
-        if self.resource.slug is None:
-            return None
-        else:
-            return f"{ONTOBEE_MERGED_GRAPH_PREFIX}{self.resource.slug.upper()}"
+    def __post_init__(self):
+        if self.resource is None:
+            raise ValueError("resource must be set")
+        graph = rdflib.Graph()
+        graph.parse(str(dm.this_path / f"{self.resource.slug}.owl.ttl"), format="turtle")
+        self.graph = graph
+        mappings = load_default_sssom("omo-to-skos")
+        self.set_metamodel_mappings(mappings)
+        # TODO: register this with w3id.org
+        self.prefix_map()["oaklib"] = "https://w3id.org/oaklib/"
```

### Comparing `oaklib-0.5.1/src/oaklib/implementations/ontoportal/bioportal_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/ontoportal/bioportal_implementation.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,17 +12,25 @@
     """
     A :ref:`OntoPortal` implementation that connects to a bioportal endpoint.
 
     Example:
 
     .. packages :: python
 
+        >>> from oaklib.implementations.ontoportal.bioportal_implementation import BioPortalImplementation
+        >>> from oaklib.implementations.ontoportal.ontoportal_implementation_base import get_apikey_value
         >>> api_key = get_apikey_value(BioPortalImplementation.ontoportal_client_class.name)
         >>> oi = BioPortalImplementation(api_key=api_key)
         >>> text = "increased expression of Shh in interneuron populations in the forebrain"
-        >>> for ann in oi.annotate_text(text)
-        >>>     ...
+        >>> for ann in oi.annotate_text(text):
+        ...     print(ann.subject_start, ann.subject_end, ann.object_id, ann.object_label)
+        <BLANKLINE>
+        ...
+        1 9 PATO:0000470 increased amount
+        ...
+        63 71 FMA:61992 Forebrain
+        ...
 
     See `<https://data.bioontology.org/documentation>`_
     """
 
     ontoportal_client_class = BioPortalClient
```

### Comparing `oaklib-0.5.1/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py` & `oaklib-0.5.2/src/oaklib/implementations/ontoportal/ontoportal_implementation_base.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/pronto/pronto_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/pronto/pronto_implementation.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,43 +101,47 @@
     TextAnnotatorInterface,
     SummaryStatisticsInterface,
     TaxonConstraintInterface,
     DumperInterface,
     MergeInterface,
 ):
     """
-    Pronto wraps local-file based ontologies in the following formats:
+    An adapter that standardizes access to OBO Format files by wrapping the Pronto library.
 
-    - obo
-    - obojson
-    - owl rdf/xml
+    `Pronto <https://github.com/althonos/pronto/>`_ is a high-performance parsing library
+    for parsing obo format 1.4 and other formats.
 
-    To load a local file:
+    Input Selector
+    --------------
 
-    .. packages:: python
+    This adapter uses the ``pronto:`` :term:`Input Selector`; e.g.
 
-        >>> resource = OntologyResource(slug='go.obo', directory='input', local=True)
-        >>> oi = ProntoImplementation(resource)
+    - ``pronto:path/to/my/file``
+    - ``pronto:https://example.com/my/file``
+    - ``prontolib:go`
 
-    To load from the OBO library:
+    Examples
+    --------
 
-    .. packages:: python
+    >>> from oaklib.implementations import ProntoImplementation
+    >>> resource = OntologyResource(slug='go-nucleus.obo', directory='test/inputinput', local=True)
+    >>> oi = ProntoImplementation(resource)
 
-        >>> resource = OntologyResource(local=False, slug='go.obo'))
-        >>> oi = ProntoImplementation(resource)
+    Or use a selector:
 
-    Currently this implementation implements most of the BaseOntologyInterface
+    >>> from oaklib import get_adapter
+    >>> oi = get_adapter("pronto:tests/input/go-nucleus.obo")
 
-    .. packages:: python
+    Then you can use any of the methods implemented by pronto
 
-        >>> rels = oi.outgoing_relationships('GO:0005773')
-        >>> for rel, parents in rels.items():
-        >>>    print(f'  {rel} ! {oi.label(rel)}')
-        >>>        for parent in parents:
-        >>>            print(f'    {parent} ! {oi.label(parent)}')
+    >>> rels = oi.outgoing_relationships('GO:0005773')
+    >>> for rel, parents in rels.items():
+    >>>    print(f'  {rel} ! {oi.label(rel)}')
+    >>>        for parent in parents:
+    >>>            print(f'    {parent} ! {oi.label(parent)}')
 
     .. warning::
 
        pronto uses the fastobo library for loading ontologies. This follows a strict
        interpretation of obo format, and some ontologies may fail to load.
        In these cases, consider an alternative implementation
```

### Comparing `oaklib-0.5.1/src/oaklib/implementations/simpleobo/simple_obo_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/simpleobo/simple_obo_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/simpleobo/simple_obo_parser.py` & `oaklib-0.5.2/src/oaklib/implementations/simpleobo/simple_obo_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/sparql/abstract_sparql_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/sparql/abstract_sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/sparql/lov_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/sparql/lov_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/sparql/sparql_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/sparql/sparql_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/sparql/sparql_query.py` & `oaklib-0.5.2/src/oaklib/implementations/sparql/sparql_query.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/sqldb/sql_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/sqldb/sql_implementation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1136,15 +1136,17 @@
 
     def associations(self, *args, **kwargs) -> Iterator[Association]:
         if not self.can_store_associations:
             yield from super().associations(*args, **kwargs)
             return
         q = self._associations_query(*args, **kwargs)
         for row in q:
-            yield Association(row.subject, row.predicate, row.object)
+            yield Association(
+                row.subject, row.predicate, row.object, primary_knowledge_source=row.source
+            )
 
     def _associations_query(
         self,
         subjects: Iterable[CURIE] = None,
         predicates: Iterable[PRED_CURIE] = None,
         objects: Iterable[CURIE] = None,
         property_filter: Dict[PRED_CURIE, Any] = None,
@@ -1195,15 +1197,18 @@
             return super().add_associations(associations, normalizers=normalizers)
         for a in associations:
             if normalizers:
                 a = a.normalize(normalizers)
             if a.property_values:
                 raise NotImplementedError
             stmt = insert(TermAssociation).values(
-                subject=a.subject, predicate=a.predicate, object=a.object
+                subject=a.subject,
+                predicate=a.predicate,
+                object=a.object,
+                source=a.primary_knowledge_source,
             )
             self._execute(stmt)
         self.session.flush()
         return True
 
     # ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
     # Implements: OboGraphInterface
```

### Comparing `oaklib-0.5.1/src/oaklib/implementations/sqldb/sqlite_utils.py` & `oaklib-0.5.2/src/oaklib/implementations/sqldb/sqlite_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/translator/translator_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/translator/translator_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/ubergraph/ubergraph_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/ubergraph/ubergraph_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/uniprot/uniprot_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/uniprot/uniprot_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/implementations/wikidata/wikidata_implementation.py` & `oaklib-0.5.2/src/oaklib/implementations/wikidata/wikidata_implementation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/__init__.py` & `oaklib-0.5.2/src/oaklib/interfaces/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/association_provider_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/association_provider_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,15 +119,18 @@
         if ix is None:
             logging.warning("No association index")
             return
         for a in ix.lookup(subjects, predicates, objects):
             yield a
 
     def add_associations(
-        self, associations: Iterable[Association], normalizers: List[EntityNormalizer] = None
+        self,
+        associations: Iterable[Association],
+        normalizers: List[EntityNormalizer] = None,
+        **kwargs,
     ) -> bool:
         """
         Store a collection of associations for later retrievals.
 
         :param associations:
         :param normalizers:
         :return:
```

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/basic_ontology_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/basic_ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/class_enrichment_calculation_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/class_enrichment_calculation_interface.py`

 * *Files 3% similar despite different names*

```diff
@@ -154,27 +154,30 @@
             }
         else:
             anc_counts = {}
         results.sort(key=lambda x: (x.p_value, -anc_counts.get(x.class_id, 0)))
         yielded = set()
         yielded_ancs = set()
         for r in results:
-            if filter_redundant:
-                if yielded.intersection(
-                    set(self.ancestors(r.class_id, predicates=object_closure_predicates))
-                ):
-                    continue
-                if r.class_id in yielded_ancs:
-                    continue
+            if yielded.intersection(
+                set(self.ancestors(r.class_id, predicates=object_closure_predicates))
+            ):
+                r.descendant_of_more_informative_result = True
+            if r.class_id in yielded_ancs:
+                r.ancestor_of_more_informative_result = True
+            yielded.add(r.class_id)
+            yielded_ancs.update(
+                list(self.ancestors(r.class_id, predicates=object_closure_predicates))
+            )
+            if filter_redundant and (
+                r.ancestor_of_more_informative_result or r.descendant_of_more_informative_result
+            ):
+                continue
+            r.rank = len(yielded)
             yield r
-            if filter_redundant:
-                yielded.add(r.class_id)
-                yielded_ancs.update(
-                    list(self.ancestors(r.class_id, predicates=object_closure_predicates))
-                )
 
     def create_self_associations(self):
         """
         Create self associations for all terms in the ontology.
 
         >>> from oaklib import get_adapter
         >>> adapter = get_adapter("tests/input/go-nucleus.obo")
```

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/differ_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/differ_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/dumper_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/dumper_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/mapping_provider_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/mapping_provider_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/merge_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/merge_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/metadata_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/metadata_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/obograph_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/obograph_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -306,30 +306,53 @@
     def subgraph_from_traversal(
         self,
         start_curies: Union[CURIE, List[CURIE]],
         predicates: List[PRED_CURIE] = None,
         traversal: TraversalConfiguration = None,
     ) -> Graph:
         """
-        Combines ancestors and descendants according to a traversal configuration
+        Combines ancestors and descendants according to a traversal configuration.
+
+        >>> from oaklib import get_adapter
+        >>> from oaklib.interfaces.obograph_interface import TraversalConfiguration, Distance
+        >>> from oaklib.datamodels.vocabulary import IS_A, PART_OF
+        >>> # use an adapter to talk to an endpoint (here, sqlite)
+        >>> adapter = get_adapter("tests/input/go-nucleus.db")
+        >>> # get a subgraph centered around these nodes
+        >>> seeds = ["GO:0005634", "GO:0005773"] # nucleus, vacuole
+        >>> # walk up the graph to get ancestors, and also get direct children
+        >>> traversal = TraversalConfiguration(up_distance=Distance.TRANSITIVE, down_distance=Distance.DIRECT)
+        >>> graph = adapter.subgraph_from_traversal(seeds, predicates=[IS_A, PART_OF], traversal=traversal)
+        >>> len(graph.nodes)
+        22
+        >>> len(graph.edges)
+        27
 
         :param start_curies:
         :param predicates:
         :param traversal:
         :return:
         """
+        if not isinstance(start_curies, list):
+            start_curies = [start_curies]
         if traversal is None:
             traversal = TraversalConfiguration()
         if traversal.up_distance == Distance.TRANSITIVE:
             logging.info(f"Getting ancestor graph from {type(self)}, start={start_curies}")
             up_graph = self.ancestor_graph(start_curies, predicates=predicates)
+        elif traversal.up_distance == Distance.DIRECT:
+            up_graph = self._graph(self.relationships(start_curies, predicates=predicates))
         else:
             up_graph = None
         if traversal.down_distance == Distance.TRANSITIVE:
             down_graph = self.descendant_graph(start_curies, predicates=predicates)
+        elif traversal.down_distance == Distance.DIRECT:
+            down_graph = self._graph(
+                self.relationships(objects=start_curies, predicates=predicates)
+            )
         else:
             down_graph = None
         g = self._merge_graphs([up_graph, down_graph])
         return g
 
     def extract_graph(
         self,
```

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/obolegacy_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/obolegacy_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/ontology_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/ontology_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/owl_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/owl_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/patcher_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/patcher_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/rdf_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/rdf_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/relation_graph_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/relation_graph_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/search_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/search_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/semsim_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/semsim_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/skos_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/skos_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/subsetter_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/subsetter_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/summary_statistics_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/summary_statistics_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/taxon_constraint_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/taxon_constraint_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/text_annotator_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/text_annotator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/interfaces/validator_interface.py` & `oaklib-0.5.2/src/oaklib/interfaces/validator_interface.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/heatmap_writer.py` & `oaklib-0.5.2/src/oaklib/io/heatmap_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/html_writer.py` & `oaklib-0.5.2/src/oaklib/io/html_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/obograph_writer.py` & `oaklib-0.5.2/src/oaklib/io/obograph_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/rollup_report_writer.py` & `oaklib-0.5.2/src/oaklib/io/rollup_report_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_axiom_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_axiom_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_csv_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_csv_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_fhir_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_fhir_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_info_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_info_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_json_lines_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_json_lines_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_json_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_kgcl_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_kgcl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_markdown_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_markdown_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_nl_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_nl_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_obo_json_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_obo_json_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_obo_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_obo_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_owl_functional_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_owl_functional_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_rdf_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_rdf_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/io/streaming_yaml_writer.py` & `oaklib-0.5.2/src/oaklib/io/streaming_yaml_writer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/mappers/base_mapper.py` & `oaklib-0.5.2/src/oaklib/mappers/base_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/mappers/ontology_metadata_mapper.py` & `oaklib-0.5.2/src/oaklib/mappers/ontology_metadata_mapper.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/parsers/__init__.py` & `oaklib-0.5.2/src/oaklib/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/parsers/association_parser_factory.py` & `oaklib-0.5.2/src/oaklib/parsers/association_parser_factory.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/parsers/boomer_parser.py` & `oaklib-0.5.2/src/oaklib/parsers/boomer_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/parsers/gaf_association_parser.py` & `oaklib-0.5.2/src/oaklib/parsers/gaf_association_parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,14 +11,18 @@
 class GafAssociationParser(XafAssociationParser):
     """Parsers for GAF format."""
 
     subject_prefix_column: ColumnReference = field(default_factory=lambda: ColumnReference(0))
     subject_column: ColumnReference = field(default_factory=lambda: ColumnReference(1))
     predicate_column: ColumnReference = field(default_factory=lambda: ColumnReference(3))
     object_column: ColumnReference = field(default_factory=lambda: ColumnReference(4))
+    publications_column: ColumnReference = field(default_factory=lambda: ColumnReference(5))
+    primary_knowledge_source_column: ColumnReference = field(
+        default_factory=lambda: ColumnReference(14)
+    )
     expected_object_prefixes = ["GO"]
 
     def post_process(
         self, association: Association
     ) -> List[Union[Association, NegatedAssociation]]:
         if association.predicate and "not" in association.predicate.lower():
             # in future this may return a NegatedAssociation
```

### Comparing `oaklib-0.5.1/src/oaklib/parsers/gencc_association_parser.py` & `oaklib-0.5.2/src/oaklib/parsers/gencc_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/parsers/hpoa_association_parser.py` & `oaklib-0.5.2/src/oaklib/parsers/hpoa_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/parsers/hpoa_g2p_association_parser.py` & `oaklib-0.5.2/src/oaklib/parsers/hpoa_g2p_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/parsers/kgx_association_parser.py` & `oaklib-0.5.2/src/oaklib/parsers/kgx_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/parsers/mim2gene_association_parser.py` & `oaklib-0.5.2/src/oaklib/parsers/mim2gene_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/parsers/pairwise_association_parser.py` & `oaklib-0.5.2/src/oaklib/parsers/pairwise_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/parsers/parser_base.py` & `oaklib-0.5.2/src/oaklib/parsers/parser_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -19,19 +19,20 @@
 
 
 @dataclass
 class Parser(ABC):
     """Base class for all parsers."""
 
     @abstractmethod
-    def parse(self, file: TextIO) -> Iterator:
+    def parse(self, file: TextIO, **kwargs) -> Iterator:
         """
         Abstract method for all parsers.
 
-        :param file:
+        :param file: file-like object to parse
+        :param kwargs: additional arguments
         :return:
         """
         raise NotImplementedError
 
     def index_lookup_function(self, column_reference: Optional[ColumnReference]) -> Callable:
         """
         Returns a function that can be used to lookup a row by reference.
```

### Comparing `oaklib-0.5.1/src/oaklib/parsers/phaf_association_parser.py` & `oaklib-0.5.2/src/oaklib/parsers/phaf_association_parser.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/parsers/xaf_association_parser.py` & `oaklib-0.5.2/src/oaklib/parsers/xaf_association_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -100,37 +100,62 @@
     """
 
     default_predicate_value: Optional[str] = None
     """
     If specified, then this value is used as the predicate if the predicate_column is not specified
     """
 
+    publications_column: Optional[ColumnReference] = None
+    """
+    Column that contains the publications (e.g. PMID, DOI).
+    """
+
+    primary_knowledge_source_column: Optional[ColumnReference] = None
+    """
+    Column that contains the primary association provider
+    """
+
     other_column_mappings: Optional[Dict[int, str]] = None
     """
     Mapping of column indices to attribute names.
     """
 
     def post_process(
         self, association: Association
     ) -> List[Union[Association, NegatedAssociation]]:
         return [association]
 
     def parse(
-        self, file: TextIO, configuration: Optional[ParserConfiguration] = None
+        self,
+        file: TextIO,
+        configuration: Optional[ParserConfiguration] = None,
+        **kwargs,
     ) -> Iterator[Union[NegatedAssociation, Association]]:
         """
         Yields annotations from a GAF or GAF-like file
 
-        :param file:
+        :param file: File to parse
+        :param configuration: Configuration for the parser
+        :param kwargs: Additional arguments
         :return:
         """
         lookup_subject_prefix = self.index_lookup_function(self.subject_prefix_column)
         lookup_subject = self.index_lookup_function(self.subject_column)
         lookup_predicate = self.index_lookup_function(self.predicate_column)
         lookup_object = self.index_lookup_function(self.object_column)
+        if self.publications_column:
+            lookup_publications = self.index_lookup_function(self.publications_column)
+        else:
+            lookup_publications = None
+        if self.primary_knowledge_source_column:
+            lookup_primary_knowledge_source = self.index_lookup_function(
+                self.primary_knowledge_source_column
+            )
+        else:
+            lookup_primary_knowledge_source = None
         if (
             self.subject_prefix_column
             and self.expected_subject_prefixes
             and self.subject_prefix not in self.expected_subject_prefixes
         ):
             raise ValueError(f"Unexpected subject prefix {self.subject_prefix} in file")
         if (
@@ -157,14 +182,22 @@
                 s = f"{self.subject_prefix}:{s}"
             else:
                 _check_identifier(s, self.expected_subject_prefixes, self.subject_must_be_curie)
             _check_identifier(o, self.expected_object_prefixes, self.object_must_be_curie)
             if self.expected_predicates and p not in self.expected_predicates:
                 raise ValueError(f"Unexpected predicate {p} in line: {line}")
             association = Association(s, p, o)
+            if lookup_publications:
+                pub = lookup_publications(vals)
+                if pub:
+                    association.publications = pub.split("|")
+            if lookup_primary_knowledge_source:
+                src = lookup_primary_knowledge_source(vals)
+                if src:
+                    association.primary_knowledge_source = src
             if self.other_column_mappings:
                 for i, attr in self.other_column_mappings.items():
                     setattr(association, attr, vals[i])
             for processed_association in self.post_process(association):
                 if isinstance(processed_association, NegatedAssociation):
                     if configuration and configuration.preserve_negated_associations:
                         yield processed_association
```

### Comparing `oaklib-0.5.1/src/oaklib/resource.py` & `oaklib-0.5.2/src/oaklib/resource.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/selector.py` & `oaklib-0.5.2/src/oaklib/selector.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,20 @@
     "hpoa_g2p": (
         [],
         "hpoa_g2p",
         "http://purl.obolibrary.org/obo/hp/hpoa/genes_to_phenotype.txt",
         False,
     ),
     "gaf": (["group"], "gaf", "http://current.geneontology.org/annotations/{group}.gaf.gz", True),
+    "gaf_archive": (
+        ["date", "group"],
+        "gaf",
+        "http://release.geneontology.org/{date}/annotations/{group}.gaf.gz",
+        True,
+    ),
     "gencc": (
         [],
         "gencc",
         "https://search.thegencc.org/download/action/submissions-export-csv",
         False,
     ),
     "medgen_mim_g2d": (
@@ -153,33 +159,43 @@
                     target_prefixes=n.target_prefixes,
                     slots=n.slots,
                     prefix_alias_map={str(k): str(v.alias) for k, v in n.prefix_alias_map.items()},
                 )
                 for n in r.normalizers
             ]
             logging.info(f"Normalizers: {normalizers}")
-            add_associations(adapter, r.selector, r.format, normalizers)
+            add_associations(
+                adapter,
+                r.selector,
+                r.format,
+                normalizers,
+                primary_knowledge_source=r.primary_knowledge_source,
+            )
     return adapter
 
 
 def add_associations(
     adapter: AssociationProviderInterface,
     descriptor: str,
     format: str = None,
-    normalizers: List[Normalizer] = None,
+    normalizers: Optional[List[Normalizer]] = None,
+    primary_knowledge_source: Optional[str] = None,
 ) -> None:
     """
     Adds associations to an adapter.
 
     :param adapter:
     :param descriptor:
     :param format:
     :param normalizers:
     :return:
     """
+    logging.info(
+        f"Adding associations from {descriptor} ({primary_knowledge_source}) using {format} format"
+    )
     # TODO: do more robust windows check
     if ":" in descriptor and not descriptor.startswith("file:") and not descriptor[1] == ":":
         scheme, path = descriptor.split(":", 1)
         if scheme not in ASSOCIATION_REGISTRY:
             raise ValueError(f"Unknown association scheme: {scheme}")
         entry = ASSOCIATION_REGISTRY[scheme]
         params, format, url_template, compressed = entry
@@ -190,32 +206,37 @@
         url = url_template.format(**param_vals)
         # TODO: add option to cache using pystow
         if compressed:
             file = file_from_gzip_url(url)
         else:
             file = file_from_url(url)
         association_parser = get_association_parser(format)
-        logging.info(f"Adding associations from {path}")
-        assocs = association_parser.parse(file)
+        logging.info(f"Adding associations from {url}")
+        if primary_knowledge_source is None:
+            primary_knowledge_source = f"infores:{scheme}"
+        assocs = list(association_parser.parse(file))
+        association_parser.add_metadata(assocs, primary_knowledge_source=primary_knowledge_source)
         adapter.add_associations(assocs, normalizers=normalizers)
         return
     if not format:
         toks = descriptor.split(".")
         while toks:
             format = toks[-1]
             if format not in ("csv", "tsv", "txt"):
                 break
             toks = toks[:-1]
     if not format:
         raise ValueError(f"Could not determine format from descriptor {descriptor}")
     association_parser = get_association_parser(format)
     path = descriptor
     with open(path) as file:
-        logging.info(f"Adding associations from {path}")
-        assocs = association_parser.parse(file)
+        logging.info(f"Adding associations from {path} ({descriptor})")
+        assocs = list(association_parser.parse(file))
+        logging.info(f"Read {len(assocs)} associations from {path}")
+        association_parser.add_metadata(assocs, primary_knowledge_source=primary_knowledge_source)
         adapter.add_associations(assocs, normalizers=normalizers)
 
 
 def file_from_gzip_url(url, is_compressed=False):
     with requests.get(url, stream=True) as response:
         response.raise_for_status()  # Raise an exception if the response contains an HTTP error status code
         # Wrap the response's raw stream in a binary file-like object
@@ -317,14 +338,15 @@
         SparqlImplementation,
     )
 
     resource = OntologyResource(format=format)
     resource.import_depth = import_depth
     resource.slug = descriptor
     impl_class: Optional[Type[OntologyInterface]] = None
+
     if not descriptor:
         raise ValueError("No descriptor provided")
     # Pre-processing
     if descriptor.startswith("datamodel:"):
         # introspect the internal OAK datamodel.
         # the oak data models are intended for programmatic use, but the documentation
         # is also exposed as a pseudo-ontology by default.
@@ -358,14 +380,15 @@
         elif impl_class == ProntoImplementation:
             if resource.slug and resource.slug.endswith(".obo"):
                 resource.format = "obo"
             if scheme == "prontolib":
                 resource.local = False
             else:
                 resource.local = True
+
             resource.slug = rest
         elif not impl_class:
             raise ValueError(f"Scheme {scheme} not known")
     else:
         logging.info(f"No schema: assuming file path {descriptor}")
         suffix = descriptor.split(".")[-1]
         impl_class, resource = get_resource_imp_class_from_suffix_descriptor(
```

### Comparing `oaklib-0.5.1/src/oaklib/utilities/apikey_manager.py` & `oaklib-0.5.2/src/oaklib/utilities/apikey_manager.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/associations/association_index.py` & `oaklib-0.5.2/src/oaklib/utilities/associations/association_index.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,18 +46,21 @@
         con.execute(f"create table term_association({','.join(COLS)})")
         self._connection = con
         session_cls = sessionmaker(engine)
         self._session = session_cls()
         self._engine = engine
 
     def populate(self, associations: Iterable[Association]):
-        tups = [(a.subject, a.predicate, a.object) for a in associations]
+        tups = [
+            (a.subject, a.predicate, a.object, a.primary_knowledge_source) for a in associations
+        ]
         logging.info(f"Bulk loading {len(tups)} associations")
         self._connection.executemany(
-            "insert into term_association(subject, predicate, object) values (?,?,?)", tups
+            "insert into term_association(subject, predicate, object, source) values (?,?,?,?)",
+            tups,
         )
 
     def lookup(
         self,
         subjects: Iterable[CURIE] = None,
         predicates: Iterable[PRED_CURIE] = None,
         objects: Iterable[CURIE] = None,
@@ -71,8 +74,13 @@
             q = q.filter(TermAssociation.subject.in_(tuple(subjects)))
         if predicates:
             q = q.filter(TermAssociation.predicate.in_(tuple(predicates)))
         if objects:
             q = q.filter(TermAssociation.object.in_(tuple(objects)))
         logging.info(f"Association query: {q}")
         for row in q:
-            yield Association(subject=row.subject, predicate=row.predicate, object=row.object)
+            yield Association(
+                subject=row.subject,
+                predicate=row.predicate,
+                object=row.object,
+                primary_knowledge_source=row.source,
+            )
```

### Comparing `oaklib-0.5.1/src/oaklib/utilities/basic_utils.py` & `oaklib-0.5.2/src/oaklib/utilities/basic_utils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 from collections import defaultdict
+from itertools import chain, combinations
 from typing import Any, Dict, Iterable, List, Optional, Tuple
 
 from oaklib.types import CURIE
 
 
+def powerset(iterable):
+    """
+    Calculate the powerset of an iterable.
+
+    >>> list(powerset([1,2,3]))
+    [(), (1,), (2,), (3,), (1, 2), (1, 3), (2, 3), (1, 2, 3)]
+
+    :param iterable:
+    :return:
+    """
+    s = list(iterable)
+    return chain.from_iterable(combinations(s, r) for r in range(len(s) + 1))
+
+
 def pairs_as_dict(pairs: Iterable[Tuple[Any, Any]]) -> Dict[Any, List[Any]]:
     """
     Translates a collection of key-value pairs into a key-values dictionary
 
     :param pairs:
     :return:
     """
```

### Comparing `oaklib-0.5.1/src/oaklib/utilities/graph/networkx_bridge.py` & `oaklib-0.5.2/src/oaklib/utilities/graph/networkx_bridge.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/graph/relationship_walker.py` & `oaklib-0.5.2/src/oaklib/utilities/graph/relationship_walker.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/identifier_utils.py` & `oaklib-0.5.2/src/oaklib/utilities/identifier_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/iterator_utils.py` & `oaklib-0.5.2/src/oaklib/utilities/iterator_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/kgcl_utilities.py` & `oaklib-0.5.2/src/oaklib/utilities/kgcl_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/label_utilities.py` & `oaklib-0.5.2/src/oaklib/utilities/label_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/lexical/lexical_indexer.py` & `oaklib-0.5.2/src/oaklib/utilities/lexical/lexical_indexer.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/mapping/boomer_utils.py` & `oaklib-0.5.2/src/oaklib/utilities/mapping/boomer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/mapping/cross_ontology_diffs.py` & `oaklib-0.5.2/src/oaklib/utilities/mapping/cross_ontology_diffs.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/mapping/mapping_propagator.py` & `oaklib-0.5.2/src/oaklib/utilities/mapping/mapping_propagator.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/mapping/mapping_validation.py` & `oaklib-0.5.2/src/oaklib/utilities/mapping/mapping_validation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/mapping/sssom_utils.py` & `oaklib-0.5.2/src/oaklib/utilities/mapping/sssom_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/ner_utilities.py` & `oaklib-0.5.2/src/oaklib/utilities/ner_utilities.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/nlp/natual_language_generation.py` & `oaklib-0.5.2/src/oaklib/utilities/nlp/natual_language_generation.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/obograph_utils.py` & `oaklib-0.5.2/src/oaklib/utilities/obograph_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 def graph_as_dict(graph: Graph) -> Dict[str, Any]:
     """
     Serialize a graph to a dict.
 
     :param graph:
     """
     obj = json_dumper.to_dict(graph)
-    for n in obj["nodes"]:
+    for n in obj.get("nodes", []):
         # normalization: no longer needed?
         if "label" in n:
             # annoying mutation: the json format uses 'lbl' not label
             n["lbl"] = n["label"]
             del n["label"]
     return obj
```

### Comparing `oaklib-0.5.1/src/oaklib/utilities/ontology_builder.py` & `oaklib-0.5.2/src/oaklib/utilities/ontology_builder.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/reasoning/relation_graph.py` & `oaklib-0.5.2/src/oaklib/utilities/reasoning/relation_graph.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/semsim/similarity_utils.py` & `oaklib-0.5.2/src/oaklib/utilities/semsim/similarity_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/stats/hypergeometric.py` & `oaklib-0.5.2/src/oaklib/utilities/stats/hypergeometric.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/subsets/slimmer_utils.py` & `oaklib-0.5.2/src/oaklib/utilities/subsets/slimmer_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/subsets/subset_analysis.py` & `oaklib-0.5.2/src/oaklib/utilities/subsets/subset_analysis.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/subsets/value_set_expander.py` & `oaklib-0.5.2/src/oaklib/utilities/subsets/value_set_expander.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/table_filler.py` & `oaklib-0.5.2/src/oaklib/utilities/table_filler.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/taxon/taxon_constraint_utils.py` & `oaklib-0.5.2/src/oaklib/utilities/taxon/taxon_constraint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/validation/definition_ontology_rule.py` & `oaklib-0.5.2/src/oaklib/utilities/validation/definition_ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/validation/disjointness_rule.py` & `oaklib-0.5.2/src/oaklib/utilities/validation/disjointness_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/validation/lint_utils.py` & `oaklib-0.5.2/src/oaklib/utilities/validation/lint_utils.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/validation/ontology_rule.py` & `oaklib-0.5.2/src/oaklib/utilities/validation/ontology_rule.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/src/oaklib/utilities/validation/rule_runner.py` & `oaklib-0.5.2/src/oaklib/utilities/validation/rule_runner.py`

 * *Files identical despite different names*

### Comparing `oaklib-0.5.1/PKG-INFO` & `oaklib-0.5.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: oaklib
-Version: 0.5.1
+Version: 0.5.2
 Summary: Ontology Access Kit: Python library for common ontology operations over a variety of backends
 Author: cmungall
 Author-email: cjm@berkeleybop.org
 Requires-Python: >=3.9,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Provides-Extra: gilda
+Provides-Extra: rustsim
 Provides-Extra: seaborn
 Requires-Dist: SPARQLWrapper
 Requires-Dist: SQLAlchemy (>=1.4.32,<2.0.0)
 Requires-Dist: airium (>=0.2.5,<0.3.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: bioregistry (>=0.6.35,<0.7.0)
 Requires-Dist: class-resolver (>=0.4.2)
 Requires-Dist: curies (>=0.4.0,<0.5.0)
+Requires-Dist: eutils (>=0.6.0,<0.7.0)
 Requires-Dist: funowl (>=0.1.12,<0.2.0)
 Requires-Dist: gilda (>=0.10.1,<0.11.0) ; extra == "gilda"
 Requires-Dist: kgcl-rdflib (>=0.3.0,<0.4.0)
 Requires-Dist: kgcl-schema (>=0.3.5,<0.4.0)
 Requires-Dist: lark (>=1.1.2,<2.0.0)
 Requires-Dist: linkml-renderer (>=0.1.2,<0.2.0)
 Requires-Dist: linkml-runtime (>=1.2.15,<2.0.0)
@@ -30,16 +32,18 @@
 Requires-Dist: networkx (>=2.7.1,<3.0.0)
 Requires-Dist: nxontology (>=0.4.0,<0.5.0)
 Requires-Dist: ols-client (>=0.1.1,<0.2.0)
 Requires-Dist: ontoportal-client (==0.0.3)
 Requires-Dist: pandas (>=1.5.1,<2.0.0)
 Requires-Dist: prefixmaps (>=0.1.2,<0.2.0)
 Requires-Dist: pronto (>=2.5.0,<3.0.0)
+Requires-Dist: pysolr (>=3.9.0,<4.0.0)
 Requires-Dist: pystow (>=0.5.0,<0.6.0)
 Requires-Dist: ratelimit (>=2.2.1,<3.0.0)
+Requires-Dist: rustsim (>=0.1.6,<0.2.0) ; extra == "rustsim"
 Requires-Dist: semsql (>=0.3.1,<0.4.0)
 Requires-Dist: sssom (>=0.3.26,<0.4.0)
 Requires-Dist: sssom-schema (>=0.11.0,<0.12.0)
 Requires-Dist: upsetplot (>=0.8.0,<0.9.0)
 Description-Content-Type: text/markdown
 
 # Ontology Access Kit (OAK)
```

