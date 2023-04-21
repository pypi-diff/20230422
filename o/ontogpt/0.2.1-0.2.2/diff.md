# Comparing `tmp/ontogpt-0.2.1.tar.gz` & `tmp/ontogpt-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontogpt-0.2.1.tar", max compression
+gzip compressed data, was "ontogpt-0.2.2.tar", max compression
```

## Comparing `ontogpt-0.2.1.tar` & `ontogpt-0.2.2.tar`

### file list

```diff
@@ -1,75 +1,92 @@
--rw-r--r--   0        0        0     1485 2023-04-06 15:21:19.285790 ontogpt-0.2.1/LICENSE
--rw-r--r--   0        0        0     9428 2023-04-06 15:21:19.285790 ontogpt-0.2.1/README.md
--rw-r--r--   0        0        0     2174 2023-04-06 15:22:18.729142 ontogpt-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      219 2023-04-06 15:21:19.313792 ontogpt-0.2.1/src/ontogpt/__init__.py
--rw-r--r--   0        0        0    16152 2023-04-06 15:21:19.313792 ontogpt-0.2.1/src/ontogpt/cli.py
--rw-r--r--   0        0        0      244 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/clients/__init__.py
--rw-r--r--   0        0        0     3192 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/clients/openai_client.py
--rw-r--r--   0        0        0     2900 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/clients/pubmed_client.py
--rw-r--r--   0        0        0      598 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/clients/soup_client.py
--rw-r--r--   0        0        0       81 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/converters/__init__.py
--rw-r--r--   0        0        0     5280 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/converters/ontology_converter.py
--rw-r--r--   0        0        0       51 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/engines/__init__.py
--rw-r--r--   0        0        0    19204 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/engines/halo_engine.py
--rw-r--r--   0        0        0    22101 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/engines/knowledge_engine.py
--rw-r--r--   0        0        0      648 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/engines/resolver.py
--rw-r--r--   0        0        0    17711 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/engines/spires_engine.py
--rw-r--r--   0        0        0      697 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/engines/synonym_engine.py
--rw-r--r--   0        0        0       70 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/evaluation/ctd/__init__.py
--rw-r--r--   0        0        0   425228 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
--rw-r--r--   0        0        0   409439 2023-04-06 15:21:19.317792 ontogpt-0.2.1/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
--rw-r--r--   0        0        0   413985 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/evaluation/ctd/database/synonyms.yaml
--rw-r--r--   0        0        0    10351 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/evaluation/ctd/eval_ctd.py
--rw-r--r--   0        0        0        0 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/evaluation/drugmechdb/__init__.py
--rw-r--r--   0        0        0     2200 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
--rw-r--r--   0        0        0     2027 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
--rw-r--r--   0        0        0    10682 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
--rw-r--r--   0        0        0     2851 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/evaluation/evaluation_engine.py
--rw-r--r--   0        0        0     6159 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/evaluation/go/eval_go.py
--rw-r--r--   0        0        0        0 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/evaluation/hpoa/__init__.py
--rw-r--r--   0        0        0     8972 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/evaluation/hpoa/eval_hpoa.py
--rw-r--r--   0        0        0      541 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/evaluation/resolver.py
--rw-r--r--   0        0        0        0 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/io/__init__.py
--rw-r--r--   0        0        0      370 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/io/exporter.py
--rw-r--r--   0        0        0     4308 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/io/html_exporter.py
--rw-r--r--   0        0        0     3232 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/io/markdown_exporter.py
--rw-r--r--   0        0        0     2351 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/io/owl_exporter.py
--rw-r--r--   0        0        0      741 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/io/yaml_wrapper.py
--rw-r--r--   0        0        0       68 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/__init__.py
--rw-r--r--   0        0        0      401 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/all.yaml
--rw-r--r--   0        0        0     5918 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/biological_process.py
--rw-r--r--   0        0        0     2027 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/biological_process.yaml
--rw-r--r--   0        0        0     3634 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/core.py
--rw-r--r--   0        0        0     3098 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/core.yaml
--rw-r--r--   0        0        0     6200 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/ctd.py
--rw-r--r--   0        0        0     6683 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/ctd.yaml
--rw-r--r--   0        0        0     5500 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/drug.py
--rw-r--r--   0        0        0     1856 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/drug.yaml
--rw-r--r--   0        0        0     6125 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/environmental_sample.py
--rw-r--r--   0        0        0     2880 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/environmental_sample.yaml
--rw-r--r--   0        0        0     8171 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/gocam.py
--rw-r--r--   0        0        0     4871 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/gocam.yaml
--rw-r--r--   0        0        0     6857 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/halo.py
--rw-r--r--   0        0        0     2367 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/halo.yaml
--rw-r--r--   0        0        0     6131 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/mendelian_disease.py
--rw-r--r--   0        0        0     3130 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/mendelian_disease.yaml
--rw-r--r--   0        0        0     5389 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/metabolic_process.py
--rw-r--r--   0        0        0     1633 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/metabolic_process.yaml
--rw-r--r--   0        0        0     7149 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/metagenome_study.py
--rw-r--r--   0        0        0     3910 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/metagenome_study.yaml
--rw-r--r--   0        0        0     5029 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/ontology_class.py
--rw-r--r--   0        0        0     2686 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/ontology_class.yaml
--rw-r--r--   0        0        0     5004 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/phenotype.py
--rw-r--r--   0        0        0     1532 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/phenotype.yaml
--rw-r--r--   0        0        0     7491 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/reaction.py
--rw-r--r--   0        0        0     3187 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/reaction.yaml
--rw-r--r--   0        0        0     7286 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/recipe.py
--rw-r--r--   0        0        0     5792 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/recipe.yaml
--rw-r--r--   0        0        0     7864 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/treatment.py
--rw-r--r--   0        0        0     4485 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/templates/treatment.yaml
--rw-r--r--   0        0        0        0 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/webapp/__init__.py
--rw-r--r--   0        0        0      861 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/webapp/html/form.html
--rw-r--r--   0        0        0      201 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/webapp/html/results.html
--rw-r--r--   0        0        0     1769 2023-04-06 15:21:19.321792 ontogpt-0.2.1/src/ontogpt/webapp/main.py
--rw-r--r--   0        0        0    11570 1970-01-01 00:00:00.000000 ontogpt-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1485 2023-04-21 22:19:33.094970 ontogpt-0.2.2/LICENSE
+-rw-r--r--   0        0        0    11152 2023-04-21 22:19:33.094970 ontogpt-0.2.2/README.md
+-rw-r--r--   0        0        0     2290 2023-04-21 22:20:30.911600 ontogpt-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/__init__.py
+-rw-r--r--   0        0        0    30092 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/cli.py
+-rw-r--r--   0        0        0      244 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/clients/__init__.py
+-rw-r--r--   0        0        0     6962 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/clients/openai_client.py
+-rw-r--r--   0        0        0     2921 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/clients/pubmed_client.py
+-rw-r--r--   0        0        0      617 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/clients/soup_client.py
+-rw-r--r--   0        0        0     1122 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/clients/wikipedia_client.py
+-rw-r--r--   0        0        0       81 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/converters/__init__.py
+-rw-r--r--   0        0        0     5289 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/converters/ontology_converter.py
+-rw-r--r--   0        0        0       59 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/__init__.py
+-rw-r--r--   0        0        0    15446 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/enrichment.py
+-rw-r--r--   0        0        0    19185 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/halo_engine.py
+-rw-r--r--   0        0        0    23173 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/knowledge_engine.py
+-rw-r--r--   0        0        0      752 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/resolver.py
+-rw-r--r--   0        0        0     3748 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/similarity_engine.py
+-rw-r--r--   0        0        0    17537 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/spires_engine.py
+-rw-r--r--   0        0        0      719 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/engines/synonym_engine.py
+-rw-r--r--   0        0        0       70 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/evaluation/ctd/__init__.py
+-rw-r--r--   0        0        0   425228 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
+-rw-r--r--   0        0        0   409439 2023-04-21 22:19:33.126970 ontogpt-0.2.2/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
+-rw-r--r--   0        0        0   413985 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/ctd/database/synonyms.yaml
+-rw-r--r--   0        0        0    10390 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/ctd/eval_ctd.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/drugmechdb/__init__.py
+-rw-r--r--   0        0        0     2145 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
+-rw-r--r--   0        0        0     2027 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
+-rw-r--r--   0        0        0    10670 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/enrichment/__init__.py
+-rw-r--r--   0        0        0    12248 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/enrichment/eval_enrichment.py
+-rw-r--r--   0        0        0     2950 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/evaluation_engine.py
+-rw-r--r--   0        0        0     6164 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/go/eval_go.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/hpoa/__init__.py
+-rw-r--r--   0        0        0     8973 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/hpoa/eval_hpoa.py
+-rw-r--r--   0        0        0     1191 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt
+-rw-r--r--   0        0        0        0 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
+-rw-r--r--   0        0        0     4791 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml
+-rwxr-xr-x   0        0        0       95 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/ibd/run.sh
+-rwxr-xr-x   0        0        0       99 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/ibd/run.sh~
+-rw-r--r--   0        0        0      586 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/evaluation/resolver.py
+-rw-r--r--   0        0        0        0 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/io/__init__.py
+-rw-r--r--   0        0        0      386 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/io/exporter.py
+-rw-r--r--   0        0        0     4329 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/io/html_exporter.py
+-rw-r--r--   0        0        0     3255 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/io/markdown_exporter.py
+-rw-r--r--   0        0        0     2350 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/io/owl_exporter.py
+-rw-r--r--   0        0        0     1440 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/io/rdf_exporter.py
+-rw-r--r--   0        0        0      899 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/io/yaml_wrapper.py
+-rw-r--r--   0        0        0       68 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/__init__.py
+-rw-r--r--   0        0        0      401 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/all.yaml
+-rw-r--r--   0        0        0     5942 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/biological_process.py
+-rw-r--r--   0        0        0     2027 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/biological_process.yaml
+-rw-r--r--   0        0        0     3593 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/core.py
+-rw-r--r--   0        0        0     3098 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/core.yaml
+-rw-r--r--   0        0        0     6210 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/ctd.py
+-rw-r--r--   0        0        0     6683 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/ctd.yaml
+-rw-r--r--   0        0        0     5466 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/drug.py
+-rw-r--r--   0        0        0     1856 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/drug.yaml
+-rw-r--r--   0        0        0     6092 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/environmental_sample.py
+-rw-r--r--   0        0        0     2880 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/environmental_sample.yaml
+-rw-r--r--   0        0        0     4709 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/gene_description_term.py
+-rw-r--r--   0        0        0     1613 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/gene_description_term.yaml
+-rw-r--r--   0        0        0     8172 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/gocam.py
+-rw-r--r--   0        0        0     4871 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/gocam.yaml
+-rw-r--r--   0        0        0     6813 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/halo.py
+-rw-r--r--   0        0        0     2367 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/halo.yaml
+-rw-r--r--   0        0        0     8165 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/ibd.py
+-rw-r--r--   0        0        0     4869 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/ibd.yaml
+-rw-r--r--   0        0        0     6097 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/mendelian_disease.py
+-rw-r--r--   0        0        0     3130 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/mendelian_disease.yaml
+-rw-r--r--   0        0        0     5384 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/metabolic_process.py
+-rw-r--r--   0        0        0     1633 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/metabolic_process.yaml
+-rw-r--r--   0        0        0     7156 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/metagenome_study.py
+-rw-r--r--   0        0        0     3910 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/metagenome_study.yaml
+-rw-r--r--   0        0        0     5072 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/ontology_class.py
+-rw-r--r--   0        0        0     2686 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/ontology_class.yaml
+-rw-r--r--   0        0        0     4887 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/phenotype.py
+-rw-r--r--   0        0        0     1532 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/phenotype.yaml
+-rw-r--r--   0        0        0     7501 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/reaction.py
+-rw-r--r--   0        0        0     3187 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/reaction.yaml
+-rw-r--r--   0        0        0     7222 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/recipe.py
+-rw-r--r--   0        0        0     5792 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/recipe.yaml
+-rw-r--r--   0        0        0     7847 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/treatment.py
+-rw-r--r--   0        0        0     4485 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/templates/treatment.yaml
+-rw-r--r--   0        0        0        0 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/webapp/__init__.py
+-rw-r--r--   0        0        0      861 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/webapp/html/form.html
+-rw-r--r--   0        0        0      201 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/webapp/html/results.html
+-rw-r--r--   0        0        0      819 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/webapp/html/spindoctor/form.html
+-rw-r--r--   0        0        0      205 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/webapp/html/spindoctor/results.html
+-rw-r--r--   0        0        0     2682 2023-04-21 22:19:33.130970 ontogpt-0.2.2/src/ontogpt/webapp/main.py
+-rw-r--r--   0        0        0    13362 1970-01-01 00:00:00.000000 ontogpt-0.2.2/PKG-INFO
```

### Comparing `ontogpt-0.2.1/LICENSE` & `ontogpt-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/README.md` & `ontogpt-0.2.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,21 +6,27 @@
 
 This makes use of so-called *instruction prompts* in Large Language Models (LLMs) such as GPT-4.
 
 Currently there are two different pipelines implemented:
 
 - SPIRES: Structured Prompt Interrogation and Recursive Extraction of Semantics
     - Zero-shot learning approach to extracting nested semantic structures from text
-    - Inputs: LinkML schema + text
+    - Inputs: [LinkML](https://linkml.io/) schema + text
     - Outputs: JSON, YAML, or RDF or OWL that conforms to the schema
     - Uses text-davinci-003
 - HALO: HAllucinating Latent Ontologies 
     - Few-shot learning approach to generating/hallucinating a domain ontology given a few examples
     - Uses code-davinci-002
 
+SPIRES is described futher in: Caufield JH, Hegde H, Emonet V, Harris NL, Joachimiak MP, Matentzoglu N, et al. Structured prompt interrogation and recursive extraction of semantics (SPIRES): A method for populating knowledge bases using zero-shot learning. arXiv [cs.AI]. 2023. http://arxiv.org/abs/2304.02711
+
+## Citation
+
+ - https://arxiv.org/abs/2304.02711
+
 ## SPIRES: Usage
 
 Given a short text `abstract.txt` with content such as:
 
    > The cGAS/STING-mediated DNA-sensing signaling pathway is crucial
    for interferon (IFN) production and host antiviral
    responses
@@ -36,15 +42,15 @@
    > ...
 
 (see [full input](tests/input/cases/gocam-betacat.txt))
 
 We can extract this into the [GO pathway datamodel](src/ontogpt/templates/gocam.yaml):
 
 ```bash
-ontogpt extract -t gocam.GoCamAnnotations abstract.txt
+ontogpt extract -t gocam.GoCamAnnotations -i abstract.txt
 ```
 
 Giving schema-compliant yaml such as:
 
 ```yaml
 genes:
 - HGNC:2514
@@ -71,28 +77,28 @@
 
 Note in the above the grounding is very preliminary and can be improved. Ungrounded NamedEntities appear as text.
 
 ## How it works
 
 1. You provide an arbitrary data model, describing the structure you want to extract text into
     - this can be nested (but see limitations below)
-2. provide your preferred annotations for grounding NamedEntity fields
-3. ontogpt will:
+2. Provide your preferred annotations for grounding NamedEntity fields
+3. OntoGPT will:
     - generate a prompt
-    - feed the prompt to a language model (currently OpenAI)
+    - feed the prompt to a language model (currently OpenAI GPT models)
     - parse the results into a dictionary structure
     - ground the results using a preferred annotator
 
 ## Pre-requisites
 
-- python 3.9+
-- an OpenAI account
-- a BioPortal account (optional, for grounding)
+- Python 3.9+
+- An OpenAI account
+- A [BioPortal](https://bioportal.bioontology.org/) account (optional, for grounding)
 
-You will need to set both API keys using OAK (which is a dependency of this project)
+You will need to set both API keys using the [Ontology Access Kit](https://github.com/INCATools/ontology-access-kit) (OAK, a dependency of this project)
 
 ```
 poetry run runoak set-apikey -e openai <your openai api key>
 poetry run runoak set-apikey -e bioportal <your bioportal api key>
 ```
 
 ## How to define your own extraction data model
@@ -169,59 +175,61 @@
 - the schema is defined in LinkML
 - prompt hints can be specified using the `prompt` annotation (otherwise description is used)
 - multivalued fields are supported
 - the default range is string - these are not grounded. E.g. disease name, synonyms
 - define a class for each NamedEntity
 - for any NamedEntity, you can specify a preferred annotator using the `annotators` annotation
 
-We recommend following an established schema like Biolink, but you can define your own.
+We recommend following an established schema like [BioLink Model](https://github.com/biolink/biolink-model), but you can define your own.
 
 ### Step 2: Compile the schema
 
-Run the `make` command at the top level. This will compile the schema to pedantic
+Place the schema YAML in the directory `src/ontogpt/templates/`.
+
+Run the `make` command at the top level. This will compile the schema to Python (Pydantic classes).
 
 ### Step 3: Run the command line
 
 e.g.
 
 ```
-ontogpt extract -t mendelian_disease.MendelianDisease marfan-wikipedia.txt
+ontogpt extract -t mendelian_disease.MendelianDisease -i marfan-wikipedia.txt
 ```
 
 ## Web Application
 
 There is a bare bones web application
 
 ```
 poetry run web-ontogpt
 ```
 
 Note that the agent running uvicorn must have the API key set, so for obvious reasons
-don't host this publicly without authentication, unless you want your credits drained. 
+don't host this publicly without authentication, unless you want your credits drained.
 
 ## Features
 
 ### Multiple levels of nesting
 
 Currently no more than two levels of nesting are recommended.
 
-If a field has a range which is itself a class and not a primitive, it will attempt to nest
+If a field has a range which is itself a class and not a primitive, it will attempt to nest.
 
 E.g. the gocam schema has an attribute:
 
 ```yaml
   attributes:
       ...
       gene_functions:
         description: semicolon-separated list of gene to molecular activity relationships
         multivalued: true
         range: GeneMolecularActivityRelationship
 ```
 
-Because GeneMolecularActivityRelationship is *inlined* it will nest
+Because `GeneMolecularActivityRelationship` is *inlined* it will nest
 
 The generated prompt is:
 
 `gene_functions : <semicolon-separated list of gene to molecular activities relationships>`
 
 The output of this is then passed through further SPIRES iterations.
 
@@ -290,42 +298,67 @@
       source_nodes:
         - CL:0000000 ## cell
         
 ```
 
 ## OWL Exports
 
-The `extract` command will let you export the results as OWL axioms, utilizing linkml-owl mappings in the schema.
+The `extract` command will let you export the results as OWL axioms, utilizing [linkml-owl](https://linkml.io/linkml-owl) mappings in the schema.
 
 For example:
 
 ```bash
-ontogpt extract -t recipe recipe-spaghetti.txt -o recipe-spaghetti.owl -O owl
+ontogpt extract -t recipe -i recipe-spaghetti.txt -o recipe-spaghetti.owl -O owl
 ```
 
 See [src/ontogpt/templates/recipe.yaml](src/ontogpt/templates/recipe.yaml) 
 for an example of a schema that uses linkml-owl mappings.
 
 See the Makefile for a full pipeline that involves using robot to extract a subset of FOODON
-and merge in the extracted results.
+and merge in the extracted results. This uses [recipe-scrapers](https://github.com/hhursev/recipe-scrapers)
+
+Example output OWL here:
+
+- [recipe-all-merged.owl](https://github.com/monarch-initiative/ontogpt/blob/main/tests/output/owl/merged/recipe-all-merged.owl)
+
+Example classification:
+
+<img width="1329" alt="image" src="https://user-images.githubusercontent.com/50745/230427663-20d845e9-f1d5-490e-b1ad-cdccdd0dca70.png">
+
+
+Contributions on recipes to test welcome from anyone! Just make a PR [here](https://github.com/monarch-initiative/ontogpt/blob/main/tests/input/recipe-urls.csv). See [this list](https://github.com/hhursev/recipe-scrapers) for accepted URLs
+
 
 ## HALO: Usage
 
 TODO
 
 
 
+## Gene Enrichment
+
+Given a set of genes, OntoGPT can find similarities among them.
+
+Example:
+```
+ontogpt enrichment HGNC:8858 HGNC:8859 HGNC:9719
+```
+
+Results:
+
+```
+Commonality: Protein targeting to the Peroxisome. All the genes are involved in targeting proteins to the peroxisome membrane, matrix or both, and they are all located in cytoplasm; peroxisome; and/or endoplasmic reticulum. Additionally, they all enable different types of binding activity and/or hydrolysing activity which likely contribute to their roles in protein import
+```
+
 ## OntoGPT Limitations
 
 ### Non-deterministic
 
 This relies on an existing LLM, and LLMs can be fickle in their responses.
 
 ### Coupled to OpenAI
 
-You will need an openai account. In theory any LLM can be used but in practice the parser is tuned for OpenAI
-
-
+You will need an OpenAI account to use their API. In theory any LLM can be used but in practice the parser is tuned for OpenAI's models.
 
-# Acknowledgements
+## Acknowledgements
 
-This [cookiecutter](https://cookiecutter.readthedocs.io/en/stable/README.html) project was developed from the [sphintoxetry-cookiecutter](https://github.com/hrshdhgd/sphintoxetry-cookiecutter) template and will be kept up-to-date using [cruft](https://cruft.github.io/cruft/).
+We gratefully acknowledge [Bosch Research](https://www.bosch.com/research) for their support of this research project.
```

### Comparing `ontogpt-0.2.1/pyproject.toml` & `ontogpt-0.2.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 [tool.poetry]
 name = "ontogpt"
-version = "0.2.1"
+version = "0.2.2"
 description = "OntoGPT"
 authors = ["Chris Mungall <cjmungall@lbl.gov>"]
 license = "BSD-3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 click = "^8.1.3"
 importlib = "^1.0.4"
-openai = "^0.27.2"
-oaklib = "^0.3.1"
+openai = "^0.27.4"
+oaklib = "^0.5.1"
 gilda = "^0.10.3"
 jsonlines = "^3.1.0"
 python-multipart = "^0.0.5"
 linkml-owl = "^0.2.7"
 beautifulsoup4 = "^4.11.1"
 eutils = "^0.6.0"
-class-resolver = "^0.3.10"
+class-resolver = "*"
 inflect = "^6.0.2"
 bioc = "^2.0.post5"
 linkml = "^1.4.10"
 wikipedia = "^1.4.0"
-tiktoken = "^0.1.1"
+tiktoken = "^0.3.3"
 airium = "^0.2.5"
 SQLAlchemy = "^1.4.32, !=1.4.46"
 greenlet = "!=2.0.2"
 httpx = "^0.23.3"
 aiohttp = "^3.8.4"
 inflection = "^0.5.1"
 linkml-runtime = "^1.4.9"
@@ -37,18 +37,20 @@
 Jinja2 = {version = "^3.1.2", optional = true}
 sphinx = {version = "^5.3.0", extras = ["docs"], optional = true}
 sphinx-rtd-theme = {version = "^1.0.0", extras = ["docs"], optional = true}
 sphinx-autodoc-typehints = {version = "^1.19.4", extras = ["docs"], optional = true}
 sphinx-click = {version = "^4.3.0", extras = ["docs"], optional = true}
 myst-parser = {version = "^0.18.1", extras = ["docs"], optional = true}
 recipe-scrapers = {version = "^14.35.0", extras = ["recipes"], optional = true}
+cachier = "^2.1.0"
+wikipedia-api = "^0.5.8"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
-setuptools = "^65.5.0"
+setuptools = ">=65.5.0"
 tox = "^3.25.1"
 mkdocs-mermaid2-plugin = "^0.6.0"
 
 [tool.poetry.scripts]
 ontogpt = "ontogpt.cli:main"
 web-ontogpt = "ontogpt.webapp.main:start"
 
@@ -65,14 +67,18 @@
     "uvicorn",
     "Jinja2"
 ]
 recipes = [
     "recipe-scrapers"
 ]
 
+[tool.poetry.group.dev.dependencies]
+jupyter = "^1.0.0"
+seaborn = "^0.12.2"
+
 [tool.poetry-dynamic-versioning]
 enable = false
 vcs = "git"
 style = "pep440"
 
 [tool.black]
 line-length = 100
```

### Comparing `ontogpt-0.2.1/src/ontogpt/clients/pubmed_client.py` & `ontogpt-0.2.2/src/ontogpt/clients/pubmed_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Pubmed Client."""
 import logging
 from dataclasses import dataclass, field
 from typing import Iterator, List
 
 import inflection
 from eutils import Client
 from eutils._internal.xmlfacades.pubmedarticle import PubmedArticle
```

### Comparing `ontogpt-0.2.1/src/ontogpt/clients/soup_client.py` & `ontogpt-0.2.2/src/ontogpt/clients/soup_client.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Soup client."""
 from dataclasses import dataclass
 
 import requests
 from bs4 import BeautifulSoup
 
 PMID = str
```

### Comparing `ontogpt-0.2.1/src/ontogpt/converters/ontology_converter.py` & `ontogpt-0.2.2/src/ontogpt/converters/ontology_converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import importlib
+"""Ontology converter."""
 import logging
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Dict, List, Optional
 
 from linkml_runtime import SchemaView
 from linkml_runtime.utils.formatutils import camelcase
```

### Comparing `ontogpt-0.2.1/src/ontogpt/engines/halo_engine.py` & `ontogpt-0.2.2/src/ontogpt/engines/halo_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 from ontogpt.templates.halo import Ontology, OntologyElement
 
 this_path = Path(__file__).parent
 logger = logging.getLogger(__name__)
 
 
 ELEMENT_NAME = str
-FIELD = str
 
 INSTRUCTIONS = """
 ## Instructions:
 ## Add an additional element to the YAML below, which is for elements
 ## in an industrial ontology. Complete as far as possible the following
 ## fields:
 """
@@ -69,15 +68,15 @@
     element_scores: Dict[ELEMENT_NAME, float] = field(default_factory=lambda: {})
     """Ranks each element by estimated informativeness for training."""
 
     tokenizer_encoding: Encoding = field(default_factory=lambda: tiktoken.get_encoding("gpt2"))
 
     def __post_init__(self):
         self.template_class = self._get_template_class("halo.OntologyElement")
-        self.client = OpenAIClient(engine=self.engine)
+        self.client = OpenAIClient(model=self.engine)
         self.api_key = self._get_openai_api_key()
         openai.api_key = self.api_key
 
     def seed(self, seed_ontology: Ontology):
         """Seed the engine with an initial ontology.
 
         :param seed_ontology:
@@ -204,16 +203,15 @@
                         candidate_elements.add(ref)
                         visited.add(ref)
             if all_slots_have_refs and not self.always_extend:
                 visited.add(element.name)
         return list(candidate_elements)
 
     def hallucinate_element(self, element: ELEMENT_NAME) -> OntologyElement:
-        """
-        Generate an ontology element based on its name
+        """Generate an ontology element based on its name.
 
         :param element: example: LeftDigit1OfHand
         :return:
         """
         logger.info(f"Hallucinating element {element}")
         example_elements = self.get_example_elements(element)
         example_element_names = [x.name for x in example_elements]
@@ -225,41 +223,40 @@
         objs = self.integrate_payload(prompt, payload)
         logger.info(f"Integrated {len(objs)} objects")
         obj = objs[0]
         self.extend_candidates([obj.name])
         return obj
 
     def get_example_elements(self, element: ELEMENT_NAME) -> List[OntologyElement]:
-        """
-        Get example elements for HALO
+        """Get example elements for HALO.
+
         :param element:
         :return:
         """
         name = uncamel(element)
         toks = set(self.tokenizer_encoding.encode(name))
         score_element_pairs = [(self.get_element_score(e, toks), e) for e in self.ontology.elements]
         score_element_pairs.sort(key=lambda x: x[0], reverse=True)
         logger.info(f"Scores[{element}: {[x for x, _ in score_element_pairs]}")
         logger.info(f"Sorted elements: {score_element_pairs}")
         return [x for _, x in score_element_pairs]
 
     def get_element_score(self, element: OntologyElement, tokens: Set[int]) -> float:
-        """
-        Calculate a score for an element based on how informative it is for few-shot learning
+        """Calculate a score for an element based on how informative it is for few-shot learning.
 
         :param element:
         :param tokens: tokenized form of the element name
         :return:
         """
         element_name = element.name
         if element_name in self.element_scores:
             score = self.element_scores[element_name]
         else:
             score = 0
-            for k, v in element.dict().items():
+            for _, v in element.dict().items():
                 if v:
                     score += 1
             self.element_scores[element_name] = score
         element_tokens = set(self.tokenizer_encoding.encode(element_name))
         jaccard = len(tokens.intersection(element_tokens)) / len(tokens.union(element_tokens))
         return score / 100 + jaccard
 
@@ -286,15 +283,16 @@
         stub_object = {
             "name": seed_element,
         }
         for k, v in self.fixed_slot_values.items():
             stub_object[k] = v
         prompt.main_prompt = yaml.dump([stub_object])
         logger.info(
-            f"Generated prompt: {len(prompt.text)} = {len(prompt.header)} + {len(prompt.body)} + {len(prompt.main_prompt)}"
+            f"Generated prompt: {len(prompt.text)} = {len(prompt.header)} +\
+                {len(prompt.body)} + {len(prompt.main_prompt)}"
         )
         return prompt
 
     def integrate_payload(
         self, prompt: StructuredPrompt, payload: Dict[str, Any]
     ) -> List[OntologyElement]:
         """Integrate the payload from HALO into the ontology.
```

### Comparing `ontogpt-0.2.1/src/ontogpt/engines/knowledge_engine.py` & `ontogpt-0.2.2/src/ontogpt/engines/knowledge_engine.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,27 +1,26 @@
-"""
-Main Knowledge Extractor class.
-"""
+"""Main Knowledge Extractor class."""
 import importlib
 import logging
 import re
 from abc import ABC
 from dataclasses import dataclass, field
 from pathlib import Path
 from types import ModuleType
-from typing import Any, Dict, Iterator, List, Optional, TextIO, Tuple, Union
+from typing import Dict, Iterator, List, Optional, TextIO, Union
 from urllib.parse import quote
 
 import inflection
 import openai
 import pydantic
+import tiktoken
 import yaml
 from linkml_runtime import SchemaView
 from linkml_runtime.linkml_model import ClassDefinition, ElementName, SlotDefinition
-from oaklib import BasicOntologyInterface, get_implementation_from_shorthand, get_adapter
+from oaklib import BasicOntologyInterface, get_adapter
 from oaklib.datamodels.text_annotator import TextAnnotationConfiguration
 from oaklib.implementations import OntoPortalImplementationBase
 from oaklib.interfaces import MappingProviderInterface, TextAnnotatorInterface
 from oaklib.utilities.apikey_manager import get_apikey_value
 from oaklib.utilities.subsets.value_set_expander import ValueSetExpander
 
 from ontogpt.clients import OpenAIClient
@@ -31,38 +30,43 @@
 logger = logging.getLogger(__name__)
 
 
 OBJECT = Union[str, pydantic.BaseModel, dict]
 EXAMPLE = OBJECT
 FIELD = str
 TEMPLATE_NAME = str
+MODEL_NAME = str
 
 # annotation metamodel
 ANNOTATION_KEY_PROMPT = "prompt"
 ANNOTATION_KEY_PROMPT_SKIP = "prompt.skip"
 ANNOTATION_KEY_ANNOTATORS = "annotators"
 ANNOTATION_KEY_RECURSE = "ner.recurse"
 ANNOTATION_KEY_EXAMPLES = "prompt.examples"
 
+MODEL_GPT_3_5_TURBO = "gpt-3.5-turbo"
+MODEL_TEXT_DAVINCI_003 = "text-davinci-003"
+MODELS = [MODEL_GPT_3_5_TURBO, MODEL_TEXT_DAVINCI_003]
+
+DEFAULT_MODEL = MODEL_GPT_3_5_TURBO
+
 # TODO: introspect
 DATAMODELS = [
     "treatment.DiseaseTreatmentSummary",
     "gocam.GoCamAnnotations",
     "bioloigical_process.BiologicalProcess",
     "environmental_sample.Study",
     "mendelian_disease.MendelianDisease",
     "reaction.Reaction",
     "recipe.Recipe",
 ]
 
 
 def chunk_text(text: str, window_size=3) -> Iterator[str]:
-    """
-    Chunk text into windows of sentences.
-    """
+    """Chunk text into windows of sentences."""
     sentences = re.split(r"[.?!]\s+", text)
     for right_index in range(1, len(sentences)):
         left_index = max(0, right_index - window_size)
         yield ". ".join(sentences[left_index:right_index])
 
 
 @dataclass
@@ -93,16 +97,16 @@
     schemaview: SchemaView = None
     """LinkML SchemaView over the template.
     This is derived from the template and does not need to be set manually."""
 
     api_key: str = None
     """OpenAI API key."""
 
-    engine: str = None
-    """OpenAI Engine. This should be overridden in subclasses"""
+    model: MODEL_NAME = None
+    """OpenAI Model. This should be overridden in subclasses"""
 
     # annotator: TextAnnotatorInterface = None
     # """Default annotator. TODO: deprecate?"""
 
     annotators: Dict[str, List[TextAnnotatorInterface]] = None
     """Annotators for each class.
     An annotator will ground/map labels to CURIEs.
@@ -138,25 +142,31 @@
 
     last_text: str = None
     """Cache of last text."""
 
     last_prompt: str = None
     """Cache of last prompt used."""
 
+    encoding = None
+
     def __post_init__(self):
         if self.template:
             self.template_class = self._get_template_class(self.template)
-        logging.info(f"Using template {self.template_class.name}")
-        self.client = OpenAIClient()
+        if self.template_class:
+            logging.info(f"Using template {self.template_class.name}")
+        if not self.model:
+            self.model = DEFAULT_MODEL
+        self.client = OpenAIClient(model=self.model)
         logging.info("Setting up OpenAI client API Key")
         self.api_key = self._get_openai_api_key()
         openai.api_key = self.api_key
         if self.mappers is None:
             logging.info("Using mappers (currently hardcoded)")
-            self.mappers = [get_implementation_from_shorthand("translator:")]
+            self.mappers = [get_adapter("translator:")]
+        self.encoding = tiktoken.encoding_for_model(self.client.model)
 
     def extract_from_text(
         self, text: str, cls: ClassDefinition = None, object: OBJECT = None
     ) -> ExtractionResult:
         raise NotImplementedError
 
     def extract_from_file(self, file: Union[str, Path, TextIO]) -> pydantic.BaseModel:
@@ -189,16 +199,17 @@
         entries = sorted(entries, key=lambda x: len(x[0]), reverse=True)
         for syn, id in entries:
             if syn in self.dictionary and self.dictionary[syn] != id:
                 logger.warning(f"Duplicate synonym: {syn} => {id}, {self.dictionary[syn]}")
             self.dictionary[syn] = id
         logger.info(f"Loaded {len(self.dictionary)}")
 
+    # @abstractmethod
     def synthesize(self, cls: ClassDefinition = None, object: OBJECT = None) -> ExtractionResult:
-        pass
+        raise NotImplementedError
 
     def generalize(
         self, object: Union[pydantic.BaseModel, dict], examples: List[EXAMPLE]
     ) -> ExtractionResult:
         raise NotImplementedError
 
     def map_terms(self, terms: List[str], ontology: str) -> Dict[str, List[str]]:
@@ -263,27 +274,29 @@
             annotators = self.annotators[cls.name]
         else:
             if ANNOTATION_KEY_ANNOTATORS not in cls.annotations:
                 logger.error(f"No annotators for {cls.name}")
                 return []
             annotators = cls.annotations[ANNOTATION_KEY_ANNOTATORS].value.split(", ")
         logger.info(f" Annotators: {annotators} [will skip: {self.skip_annotators}]")
-        objs = []
+        annotators = []
         for annotator in annotators:
             if isinstance(annotator, str):
                 logger.info(f"Loading annotator {annotator}")
                 if self.skip_annotators and annotator in self.skip_annotators:
                     logger.info(f"Skipping annotator {annotator}")
                     continue
-                objs.append(get_implementation_from_shorthand(annotator))
+                if annotator not in self.annotators:
+                    self.annotators[annotator] = get_adapter(annotator)
+                annotators.append(self.annotators[annotator])
             elif isinstance(annotator, BasicOntologyInterface):
-                objs.append(annotator)
+                annotators.append(annotator)
             else:
                 raise ValueError(f"Unknown annotator type {annotator}")
-        return objs
+        return annotators
 
     def promptable_slots(self, cls: Optional[ClassDefinition] = None) -> List[SlotDefinition]:
         """
         List of all slots that are not skipped for purposes of prompting.
 
         Examples of slots that are skipped are:
 
@@ -442,14 +455,20 @@
         - annotators are yielded next, in order in which they are specified in the schema
 
         :param text: text to ground, e.g. gene symbol
         :param cls: schema class the ground object should instantiate
         :return:
         """
         logger.info(f"GROUNDING {text} using {cls.name}")
+        id_matches = re.match(r"^(\S+):(\d+)$", text)
+        if id_matches:
+            obj_prefix = id_matches.group(1)
+            matching_prefixes = [x for x in cls.id_prefixes if x.upper() == obj_prefix.upper()]
+            if matching_prefixes:
+                yield matching_prefixes[0] + ":" + id_matches.group(2)
         text_lower = text.lower()
         text_singularized = inflection.singularize(text_lower)
         if text_singularized != text_lower:
             logger.info(f"Singularized {text} to {text_singularized}")
             yield from self.groundings(text_singularized, cls)
         parenthetical_components = re.findall(r"\[(.*?)\]", text_lower)
         if not parenthetical_components:
@@ -484,16 +503,20 @@
         # prioritize whole matches by running these first
         for matches_whole_text in [True, False]:
             config = TextAnnotationConfiguration(matches_whole_text=matches_whole_text)
             for annotator in annotators:
                 if isinstance(annotator, str):
                     if self.skip_annotators and annotator in self.skip_annotators:
                         continue
-                    logger.info(f"Loading annotator {annotator}")
-                    annotator = get_adapter(annotator)
+                    if self.annotators is None:
+                        self.annotators = {}
+                    if annotator not in self.annotators:
+                        logger.info(f"Loading annotator {annotator}")
+                        self.annotators[annotator] = get_adapter(annotator)
+                    annotator = self.annotators[annotator]
                 if not matches_whole_text and not isinstance(
                     annotator, OntoPortalImplementationBase
                 ):
                     # TODO: allow more fine-grained control
                     logger.info(
                         f"Skipping {type(annotator)} as it does not support partial matches"
                     )
@@ -508,15 +531,15 @@
     # def ground_text_to_id(self, text: str, cls: ClassDefinition = None) -> str:
     #    raise NotImplementedError
 
     def merge_resultsets(
         self, resultset: List[ExtractionResult], unique_fields: List[str] = None
     ) -> ExtractionResult:
         """
-        Merges all resultsets into a single resultset.
+        Merge all resultsets into a single resultset.
 
         Note the first element of the list is mutated.
 
         :param resultset:
         :return:
         """
         result = resultset[0].extracted_object
```

### Comparing `ontogpt-0.2.1/src/ontogpt/engines/resolver.py` & `ontogpt-0.2.2/src/ontogpt/engines/resolver.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
+"""Resolver engine."""
 from typing import Optional, Type, Union
 
 from class_resolver import ClassResolver
 
+from ontogpt.engines.enrichment import EnrichmentEngine
 from ontogpt.engines.halo_engine import HALOEngine
 from ontogpt.engines.knowledge_engine import KnowledgeEngine
 from ontogpt.engines.spires_engine import SPIRESEngine
 
-resolver = ClassResolver([SPIRESEngine, HALOEngine], base=KnowledgeEngine)
+resolver = ClassResolver([SPIRESEngine, HALOEngine, EnrichmentEngine], base=KnowledgeEngine)
 
 
 def create_engine(
-    template: str, model: Optional[Union[str, Type]] = None, **kwargs
+    template: str, engine: Optional[Union[str, Type]] = None, **kwargs
 ) -> KnowledgeEngine:
     """Create a knowledge engine."""
-    if model is None:
-        model = SPIRESEngine
-    if isinstance(model, str):
-        model = resolver.get_class(model)(**kwargs)
-    return model(template, **kwargs)
+    if engine is None:
+        engine = SPIRESEngine
+    if isinstance(engine, str):
+        engine = resolver.get_class(engine)(**kwargs)
+    return engine(template, **kwargs)
```

### Comparing `ontogpt-0.2.1/src/ontogpt/engines/spires_engine.py` & `ontogpt-0.2.2/src/ontogpt/engines/spires_engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,25 @@
 import logging
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 
 import pydantic
 from linkml_runtime.linkml_model import ClassDefinition, SlotDefinition
-from oaklib import get_implementation_from_shorthand
-from oaklib.datamodels.text_annotator import TextAnnotation, TextAnnotationConfiguration
 
 from ontogpt.engines.knowledge_engine import (
-    ANNOTATION_KEY_ANNOTATORS,
     ANNOTATION_KEY_PROMPT,
     ANNOTATION_KEY_PROMPT_SKIP,
     EXAMPLE,
     FIELD,
     OBJECT,
     KnowledgeEngine,
     chunk_text,
 )
-from ontogpt.templates.core import ExtractionResult, NamedEntity
+from ontogpt.templates.core import ExtractionResult
 
 this_path = Path(__file__).parent
 
 
 RESPONSE_ATOM = Union[str, "ResponseAtom"]
 RESPONSE_DICT = Dict[FIELD, Union[RESPONSE_ATOM, List[RESPONSE_ATOM]]]
 
@@ -160,15 +157,16 @@
             },
         }
         ontology = ontology.lower()
         if ontology in examples:
             example = examples[ontology]
         else:
             example = examples["uberon"]
-        prompt = "Normalize the following semicolon separated list of terms to the {ontology.upper()} ontology\n\n"
+        prompt = "Normalize the following semicolon separated\
+            list of terms to the {ontology.upper()} ontology\n\n"
         prompt += "For example:\n\n"
         for k, v in example.items():
             prompt += f"{k}: {v}\n"
         prompt += "===\n\nTerms:"
         prompt += "; ".join(terms)
         prompt += "===\n\n"
         payload = self.client.complete(prompt)
@@ -289,15 +287,15 @@
                     prompt += f"{k}: {self._serialize_value(v, slot)}\n"
         return prompt
 
     def _parse_response_to_dict(
         self, results: str, cls: ClassDefinition = None
     ) -> Optional[RESPONSE_DICT]:
         """
-        Parses the pseudo-YAML response from OpenAI into a dictionary object.
+        Parse the pseudo-YAML response from OpenAI into a dictionary object.
 
         E.g.
 
             foo: a; b; c
 
         becomes
```

### Comparing `ontogpt-0.2.1/src/ontogpt/engines/synonym_engine.py` & `ontogpt-0.2.2/src/ontogpt/engines/synonym_engine.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Synonym engine."""
 from dataclasses import dataclass
 from typing import List
 
 from ontogpt.engines.knowledge_engine import KnowledgeEngine
 
 
 @dataclass
```

### Comparing `ontogpt-0.2.1/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz` & `ontogpt-0.2.2/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz` & `ontogpt-0.2.2/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/evaluation/ctd/database/synonyms.yaml` & `ontogpt-0.2.2/src/ontogpt/evaluation/ctd/database/synonyms.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/evaluation/ctd/eval_ctd.py` & `ontogpt-0.2.2/src/ontogpt/evaluation/ctd/eval_ctd.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,18 @@
 E.g. scopolamine induces drug overdose
 
 Biocreativ results here:
 
 https://biocreative.bioinformatics.udel.edu/media/store/files/2015/BC5CDR_overview.final.pdf
 
 A total of 18 teams successfully submitted CID results in 46 runs. As
-shown in Table 3 (only the best run of each team is included), the Fscore ranges from 32.01% to 57.03% (team 288) with an average of
-43.37%. All teams outperformed the baseline results by the simple abstract-level co-occurrence method (16.43% in precision, 76.45% in recall and 27.05% in F-score).
+shown in Table 3 (only the best run of each team is included),
+the Fscore ranges from 32.01% to 57.03% (team 288) with an average of
+43.37%. All teams outperformed the baseline results by the simple abstract-level
+co-occurrence method (16.43% in precision, 76.45% in recall and 27.05% in F-score).
 
 """
 import gzip
 import logging
 from collections import defaultdict
 from dataclasses import dataclass
 from pathlib import Path
@@ -25,15 +27,15 @@
 import yaml
 from bioc import biocxml
 from oaklib import BasicOntologyInterface, get_implementation_from_shorthand
 from pydantic import BaseModel
 
 from ontogpt.engines.knowledge_engine import chunk_text
 from ontogpt.engines.spires_engine import SPIRESEngine
-from ontogpt.evaluation.evaluation_engine import EvaluationEngine, SimilarityScore
+from ontogpt.evaluation.evaluation_engine import SimilarityScore, SPIRESEvaluationEngine
 from ontogpt.templates.core import Publication, Triple
 from ontogpt.templates.ctd import (
     ChemicalToDiseaseDocument,
     ChemicalToDiseaseRelationship,
     TextWithTriples,
 )
 
@@ -103,29 +105,27 @@
         self.false_negatives = list(test_pairs.difference(pred_pairs))
         self.num_false_negatives = len(self.false_negatives)
         self.num_false_positives = len(self.false_positives)
         self.num_true_positives = len(self.true_positives)
 
 
 class EvaluationObjectSetRE(BaseModel):
-    """
-    A result of predicting relationextractions
-    """
+    """A result of predicting relationextractions."""
 
     precision: float = None
     recall: float = None
     f1: float = None
 
     training: List[TextWithTriples] = None
     predictions: List[PredictionRE] = None
     test: List[TextWithTriples] = None
 
 
 @dataclass
-class EvalCTD(EvaluationEngine):
+class EvalCTD(SPIRESEvaluationEngine):
     # ontology: OboGraphInterface = None
     subject_prefix = "MESH"
     object_prefix = "MESH"
 
     def __post_init__(self):
         self.extractor = SPIRESEngine("ctd.ChemicalToDiseaseDocument")
         # synonyms are derived entirely from training set
@@ -169,17 +169,15 @@
         for doc in docs[0:num]:
             text = doc.text
             prompt = ke.get_completion_prompt(None, text)
             completion = ke.serialize_object(m)
             yield dict(prompt=prompt, completion=completion)
 
     def eval(self) -> EvaluationObjectSetRE:
-        """
-        Evaluates the ability to extract relations
-        """
+        """Evaluate the ability to extract relations."""
         labeler = get_implementation_from_shorthand("sqlite:obo:mesh")
         num_test = self.num_tests
         ke = self.extractor
         docs = list(self.load_test_cases())
         shuffle(docs)
         eos = EvaluationObjectSetRE(
             test=docs[:num_test],
@@ -193,28 +191,31 @@
             logger.info(doc)
             text = f"Title: {doc.publication.title} Abstract: {doc.publication.abstract}"
             predicted_obj = None
             named_entities = []
             for chunked_text in chunk_text(text):
                 extraction = ke.extract_from_text(chunked_text)
                 logger.info(
-                    f"{len(extraction.extracted_object.triples)} triples from window: {chunked_text}"
+                    f"{len(extraction.extracted_object.triples)}\
+                        triples from window: {chunked_text}"
                 )
                 if not predicted_obj:
                     predicted_obj = extraction.extracted_object
                 else:
                     predicted_obj.triples.extend(extraction.extracted_object.triples)
                     logger.info(f"{len(predicted_obj.triples)} total triples, after concatenation")
                     logger.debug(f"concatenated triples: {predicted_obj.triples}")
                 named_entities.extend(extraction.named_entities)
 
             # title_extraction = ke.extract_from_text(doc.publication.title)
-            # logger.info(f"{len(title_extraction.extracted_object.triples)} triples from: Title {doc.publication.title}")
+            # logger.info(f"{len(title_extraction.extracted_object.triples)}\
+            # triples from: Title {doc.publication.title}")
             # abstract_extraction = ke.extract_from_text(doc.publication.abstract)
-            # logger.info(f"{len(abstract_extraction.extracted_object.triples)} triples from: Abstract {doc.publication.abstract}")
+            # logger.info(f"{len(abstract_extraction.extracted_object.triples)}\
+            # triples from: Abstract {doc.publication.abstract}")
             # ke.merge_resultsets([results, results2])
             # predicted_obj = title_extraction.extracted_object
             # predicted_obj.triples.extend(abstract_extraction.extracted_object.triples)
             # logger.info(f"{len(predicted_obj.triples)} total triples, after concatenation")
             # logger.debug(f"concatenated triples: {predicted_obj.triples}")
 
             def included(t: ChemicalToDiseaseRelationship):
@@ -229,15 +230,15 @@
 
             predicted_obj.triples = [t for t in predicted_obj.triples if included(t)]
             logger.info(
                 f"{len(predicted_obj.triples)} filtered triples (CID only, between MESH only)"
             )
             pred = PredictionRE(predicted_object=predicted_obj, test_object=doc)
             pred.named_entities = named_entities
-            logger.info(f"PRED")
+            logger.info("PRED")
             logger.info(yaml.dump(pred.dict()))
             logger.info("Calc scores")
             pred.calculate_scores(labelers=[labeler])
             logger.info(yaml.dump(pred.dict()))
             eos.predictions.append(pred)
         self.calc_stats(eos)
         return eos
```

### Comparing `ontogpt-0.2.1/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py` & `ontogpt-0.2.2/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+"""DrugMechDB."""
 from __future__ import annotations
 
-from datetime import date, datetime
-from enum import Enum
-from typing import Any, Dict, List, Optional
+from typing import List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
 metamodel_version = "None"
 version = "None"
 
@@ -23,48 +22,44 @@
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
 class Mechanism(ConfiguredBaseModel):
-
     directed: Optional[bool] = Field(None)
     multigraph: Optional[bool] = Field(None)
     reference: Optional[List[str]] = Field(default_factory=list)
     references: Optional[str] = Field(None)
     comment: Optional[str] = Field(None)
     comments: Optional[str] = Field(None)
     commments: Optional[str] = Field(None)
     graph: Optional[Graph] = Field(None)
     links: Optional[List[Link]] = Field(default_factory=list)
     nodes: Optional[List[Node]] = Field(default_factory=list)
 
 
 class Graph(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None)
     disease: Optional[str] = Field(None)
     disease_mesh: Optional[str] = Field(None)
     drug: Optional[str] = Field(None)
     drug_mesh: Optional[str] = Field(None)
     drugbank: Optional[str] = Field(None)
     alt_ids: Optional[str] = Field(None)
 
 
 class Link(ConfiguredBaseModel):
-
     key: Optional[str] = Field(None)
     source: Optional[str] = Field(None)
     target: Optional[str] = Field(None)
     reference: Optional[str] = Field(None)
 
 
 class Node(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None)
     label: Optional[str] = Field(None)
     name: Optional[str] = Field(None)
     all_id: Optional[str] = Field(None)
     alt_ids: Optional[List[str]] = Field(default_factory=list)
     alt_names: Optional[List[str]] = Field(default_factory=list)
     alt_name: Optional[str] = Field(None)
```

### Comparing `ontogpt-0.2.1/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml` & `ontogpt-0.2.2/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py` & `ontogpt-0.2.2/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import yaml
 from oaklib import get_implementation_from_shorthand
 from pydantic import BaseModel
 
 import ontogpt.evaluation.drugmechdb.datamodel.drugmechdb as source_datamodel
 import ontogpt.templates.drug as target_datamodel
 from ontogpt.engines.spires_engine import SPIRESEngine
-from ontogpt.evaluation.evaluation_engine import EvaluationEngine, SimilarityScore
+from ontogpt.evaluation.evaluation_engine import SimilarityScore, SPIRESEvaluationEngine
 
 THIS_DIR = Path(__file__).parent
 DATABASE_DIR = Path(__file__).parent / "database"
 MOA_TEXTS = DATABASE_DIR / "drugbank-to-mechanism-text.tsv"
 TEST_CASES_DIR = THIS_DIR / "test_cases"
 EXEMPLARS_DIR = THIS_DIR / "exemplars"
 EXEMPLAR_CASES = EXEMPLARS_DIR / "drugmechdb-exemplars.yaml"
@@ -77,40 +77,38 @@
         self.scores["similarity"] = SimilarityScore.from_set(
             all_objects(self.test_object),
             all_objects(self.predicted_object),
         )
 
 
 class EvaluationObjectSetDrugMechDB(BaseModel):
-    """
-    A result of predicting paths
-    """
+    """A result of predicting paths."""
 
     test: List[target_datamodel.DrugMechanism] = None
     training: List[target_datamodel.DrugMechanism] = None
     predictions: List[PredictionDrugMechDB] = None
 
 
 @dataclass
-class EvalDrugMechDB(EvaluationEngine):
+class EvalDrugMechDB(SPIRESEvaluationEngine):
     # ontology: OboGraphInterface = None
     data: List[target_datamodel.DrugMechanism] = None
     _drug_to_mechanism_text: Dict[str, str] = None
     default_labelers = [
         "sqlite:obo:mesh",
         "sqlite:obo:drugbank",
         "sqlite:obo:go",
         "sqlite:obo:uberon",
         "sqlite:obo:pr",
     ]
 
     def __post_init__(self):
         self.extractor = SPIRESEngine("drug.DrugMechanism")
         self.extractor.labelers = [
-            get_implementation_from_shorthand(l) for l in self.default_labelers
+            get_implementation_from_shorthand(lab) for lab in self.default_labelers
         ]
 
     @property
     def drug_to_mechanism_text(self) -> Dict[str, str]:
         """Mapping between drugbank id and MOA text from drugbank record.
 
         :return:
@@ -210,17 +208,15 @@
             }
             text = self.drug_to_mechanism_text[m.drug]
             prompt = ke.get_completion_prompt(None, text, object=stub)
             completion = ke.serialize_object(m)
             yield dict(prompt=prompt, completion=completion)
 
     def eval(self) -> EvaluationObjectSetDrugMechDB:
-        """
-        Evaluates the ability to extract a path from MOA text
-        """
+        """Evaluate the ability to extract a path from MOA text."""
         num_test = self.num_tests
         ke = self.extractor
         mechanisms = self.load_target_database()
 
         def is_candidate(m: target_datamodel.DrugMechanism):
             if m.drug not in self.drug_to_mechanism_text:
                 return False
@@ -257,15 +253,15 @@
             print(yaml.dump(pred.dict()))
             pred.calculate_scores()
             print(yaml.dump(pred.dict()))
             eos.predictions.append(pred)
         return eos
 
     def eval_path_prediction(self) -> EvaluationObjectSetDrugMechDB:
-        """Evaluates the ability to predict a path purely from background knowledge in the LLM.
+        """Evaluate the ability to predict a path purely from background knowledge in the LLM.
 
         :return:
         """
         ke = self.extractor
         eos = self.create_test_and_training(num_test=self.num_tests, num_training=self.num_training)
         eos.predictions = []
         print(yaml.dump(eos.dict()))
```

### Comparing `ontogpt-0.2.1/src/ontogpt/evaluation/evaluation_engine.py` & `ontogpt-0.2.2/src/ontogpt/evaluation/evaluation_engine.py`

 * *Files 9% similar despite different names*

```diff
@@ -61,24 +61,31 @@
             false_negatives=list(test_set - prediction_set),
             common=list(test_set & prediction_set),
         )
 
 
 @dataclass
 class EvaluationEngine:
-    """Base class for all evaluation engines
+    pass
+
+
+@dataclass
+class SPIRESEvaluationEngine(EvaluationEngine):
+    """Base class for all evaluation engines in SPIRES.
 
     TODO: currently there is a lot of repetition between the different evaluation engines.
     This should be refactored so we have common base classes for different tasks
 
     - NamedEntity Recognition
     - Simple Relation Extraction, i.e. pairs of subject-object (e.g CTD task)
     - Triple Extraction, i.e. triples of subject-predicate-object
-    - Complex Relation Extraction, i.e. triples of subject-predicate-object with additional information, e.g. qualifiers
-    - Structured Knowledge Extraction, i.e. arbitrary nested objects including both literals and edges
+    - Complex Relation Extraction, i.e. triples of subject-predicate-object with\
+        additional information, e.g. qualifiers
+    - Structured Knowledge Extraction, i.e. arbitrary nested objects including\
+        both literals and edges
     """
 
     extractor: SPIRESEngine = None
     """Knowledge extractor to use"""
 
     num_tests: int = 10
     """Number of test cases to use for evaluation"""
```

### Comparing `ontogpt-0.2.1/src/ontogpt/evaluation/go/eval_go.py` & `ontogpt-0.2.2/src/ontogpt/evaluation/go/eval_go.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
+"""Evaluate GO."""
 from dataclasses import dataclass
 from pathlib import Path
 from random import shuffle
 from typing import Dict, List
 
 import yaml
 from oaklib import get_implementation_from_shorthand
 from oaklib.datamodels.obograph import LogicalDefinitionAxiom
 from oaklib.datamodels.vocabulary import IS_A
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from pydantic import BaseModel
 
 from ontogpt.engines.spires_engine import SPIRESEngine
-from ontogpt.evaluation.evaluation_engine import EvaluationEngine, SimilarityScore
+from ontogpt.evaluation.evaluation_engine import SimilarityScore, SPIRESEvaluationEngine
 from ontogpt.templates.metabolic_process import MetabolicProcess
 
 TEST_CASES_DIR = Path(__file__).parent / "test_cases"
 
 METABOLIC_PROCESS = "GO:0008152"
 BIOSYNTHESIS = "GO:0009058"
 HAS_PRIMARY_OUTPUT = "RO:0004008"
@@ -37,41 +38,37 @@
             self.scores[k] = SimilarityScore.from_set(
                 getattr(self.test_object, k, "").split(),
                 getattr(self.predicted_object, k, "").split(),
             )
 
 
 class EvaluationObjectSetGO(BaseModel):
-    """
-    A result of extracting knowledge on text
-    """
+    """A result of extracting knowledge on text."""
 
     test: List[MetabolicProcess] = None
     training: List[MetabolicProcess] = None
     predictions: List[PredictionGO] = None
 
 
 @dataclass
-class EvalGO(EvaluationEngine):
+class EvalGO(SPIRESEvaluationEngine):
     ontology: OboGraphInterface = None
     genus: str = BIOSYNTHESIS
     differentia_relation: str = HAS_PRIMARY_OUTPUT
 
     def __post_init__(self):
         ontology = get_implementation_from_shorthand("sqlite:obo:go")
         if not isinstance(ontology, OboGraphInterface):
             raise TypeError
         self.ontology = ontology
         self.extractor = SPIRESEngine("metabolic_process.MetabolicProcess")
         self.extractor.labelers = [ontology]
 
     def make_term_from_ldef(self, ldef: LogicalDefinitionAxiom) -> MetabolicProcess:
-        """
-        Make a term from a logical definition
-        """
+        """Make a term from a logical definition."""
         ontology = self.ontology
         term = ldef.definedClassId
         parents = [rel[2] for rel in ontology.relationships([term], [IS_A])]
         mp = MetabolicProcess(
             id=term,
             label=ontology.label(term),
             description=ontology.definition(term),
@@ -85,17 +82,15 @@
         return mp
 
     def valid_test_ids(self) -> List[str]:
         with open(TEST_CASES_DIR / "go-ids-2022.txt") as f:
             return [x.strip() for x in f.readlines()]
 
     def ldef_matches(self, ldef: LogicalDefinitionAxiom) -> bool:
-        """
-        Check if a logical definition matches the genus and differentia
-        """
+        """Check if a logical definition matches the genus and differentia."""
         if self.genus not in ldef.genusIds:
             return False
         if len(ldef.restrictions) != 1:
             return False
         if self.differentia_relation != ldef.restrictions[0].propertyId:
             return False
         return True
@@ -107,15 +102,16 @@
         Create a test and training set of GO terms.
 
         This takes around 1m to run.
         """
         ontology = self.ontology
         entities = set(ontology.descendants([self.genus], [IS_A]))
         print(
-            f"Found {len(entities)} entities that are descendants of genus {self.genus}; {list(entities)[0:5]}"
+            f"Found {len(entities)} entities that are descendants of\
+                genus {self.genus}; {list(entities)[0:5]}"
         )
         assert "GO:0140872" in entities
         all_test_ids = set(self.valid_test_ids())
         assert "GO:0140872" in all_test_ids
         print(f"Found {len(all_test_ids)} test id candidates; {list(entities)[0:5]}")
         candidate_test_ids = entities.intersection(all_test_ids)
         print(f"Found {len(candidate_test_ids)} candidate test ids")
```

### Comparing `ontogpt-0.2.1/src/ontogpt/evaluation/hpoa/eval_hpoa.py` & `ontogpt-0.2.2/src/ontogpt/evaluation/hpoa/eval_hpoa.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
-"""
-HPOA evaluation.
-"""
+"""HPOA evaluation."""
 import csv
 import logging
 from collections import defaultdict
 from dataclasses import dataclass
 from pathlib import Path
 from random import shuffle
 from typing import Dict, Iterable, Iterator, List, Tuple
@@ -13,15 +11,15 @@
 from oaklib.datamodels.search import SearchConfiguration
 from oaklib.datamodels.search_datamodel import SearchProperty
 from oaklib.interfaces import SearchInterface
 from pydantic import BaseModel
 
 from ontogpt.clients.pubmed_client import PubmedClient
 from ontogpt.engines.spires_engine import SPIRESEngine
-from ontogpt.evaluation.evaluation_engine import EvaluationEngine, SimilarityScore
+from ontogpt.evaluation.evaluation_engine import SimilarityScore, SPIRESEvaluationEngine
 from ontogpt.templates.mendelian_disease import MendelianDisease
 
 THIS_DIR = Path(__file__).parent
 DATABASE_DIR = Path(__file__).parent / "database"
 TEST_CASES_DIR = THIS_DIR / "test_cases"
 EXEMPLARS_DIR = THIS_DIR / "exemplars"
 EXEMPLAR_CASES = EXEMPLARS_DIR / "drugmechdb-exemplars.yaml"
@@ -50,32 +48,30 @@
                 self.scores[k] = SimilarityScore.from_set(
                     getattr(self.test_object, k, "").split(),
                     getattr(self.predicted_object, k, "").split(),
                 )
 
 
 class EvaluationObjectSetHPOA(BaseModel):
-    """
-    A result of predicting paths
-    """
+    """A result of predicting paths."""
 
     test: List[MendelianDisease] = None
     training: List[MendelianDisease] = None
     predictions: List = None
 
 
 class HPOAnnotation(BaseModel):
     subject: DISEASE_ID = None
     term: TERM = None
     aspect: ASPECT = None
     publication: PUBLICATION = None
 
 
 @dataclass
-class EvalHPOA(EvaluationEngine):
+class EvalHPOA(SPIRESEvaluationEngine):
     mondo: BasicOntologyInterface = None
 
     def __post_init__(self):
         self.extractor = SPIRESEngine("mendelian_disease.MendelianDisease")
         self.mondo = get_implementation_from_shorthand("sqlite:obo:mondo")
 
     def load_test_cases(self) -> List[MendelianDisease]:
```

### Comparing `ontogpt-0.2.1/src/ontogpt/evaluation/resolver.py` & `ontogpt-0.2.2/src/ontogpt/evaluation/resolver.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+"""Evaluation Resolver."""
 from typing import Optional, Type, Union
 
 from class_resolver import ClassResolver
 
 from ontogpt.evaluation.ctd.eval_ctd import EvalCTD
-from ontogpt.evaluation.evaluation_engine import EvaluationEngine
+from ontogpt.evaluation.evaluation_engine import SPIRESEvaluationEngine
 
-resolver = ClassResolver([EvalCTD], base=EvaluationEngine)
+resolver = ClassResolver([EvalCTD], base=SPIRESEvaluationEngine)
 
 
-def create_evaluator(name: Optional[Union[str, Type]] = None, **kwargs) -> EvaluationEngine:
+def create_evaluator(name: Optional[Union[str, Type]] = None, **kwargs) -> SPIRESEvaluationEngine:
     """Create a knowledge engine."""
     if name is None:
         name = EvalCTD
     if isinstance(name, str):
         return resolver.lookup(name)(**kwargs)
     return name(**kwargs)
```

### Comparing `ontogpt-0.2.1/src/ontogpt/io/html_exporter.py` & `ontogpt-0.2.2/src/ontogpt/io/html_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""HTML Exporter."""
 import html
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, TextIO, Union
 
 import pydantic
 import yaml
```

### Comparing `ontogpt-0.2.1/src/ontogpt/io/markdown_exporter.py` & `ontogpt-0.2.2/src/ontogpt/io/markdown_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Markdown exporter."""
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TextIO, Union
 
 import pydantic
 import yaml
 
@@ -13,18 +14,18 @@
 class MarkdownExporter(Exporter):
     def export(self, extraction_output: ExtractionResult, output: Union[str, Path, TextIO]):
         if isinstance(output, Path):
             output = str(output)
         if isinstance(output, str):
             output = open(str(output), "w", encoding="utf-8")
         output.write(f"# {extraction_output.input_id}\n\n")
-        output.write(f"## Input\n\n")
+        output.write("## Input\n\n")
         for block in extraction_output.input_text.split("\n"):
             output.write(f"_{block.replace('_', '')}_\n\n")
-        output.write(f"## Results\n\n")
+        output.write("## Results\n\n")
         obj = extraction_output.extracted_object
         self.export_object(obj, extraction_output, output, -1)
         output.write("\n\nYAML:\n\n")
         self.details(yaml.dump(extraction_output.dict()), output, code="yaml")
         output.write("\n\nPrompt:\n\n")
         self.details(extraction_output.prompt, output)
         output.write("\n\nCompletion:\n\n")
```

### Comparing `ontogpt-0.2.1/src/ontogpt/io/owl_exporter.py` & `ontogpt-0.2.2/src/ontogpt/io/owl_exporter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
+"""OWL convertor."""
 from dataclasses import dataclass
 from pathlib import Path
 from typing import TextIO, Union
 
 import pydantic
-import yaml
 from linkml.generators.pythongen import PythonGenerator
 from linkml_owl.dumpers.owl_dumper import OWLDumper
 from linkml_runtime import SchemaView
 
-from ontogpt.io.exporter import Exporter, is_curie
+from ontogpt.io.exporter import Exporter
 from ontogpt.templates.core import ExtractionResult
 
 
 @dataclass
 class OWLExporter(Exporter):
     def export(
         self,
```

### Comparing `ontogpt-0.2.1/src/ontogpt/io/yaml_wrapper.py` & `ontogpt-0.2.2/src/ontogpt/io/yaml_wrapper.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,26 @@
+"""YAML Wrapper."""
 from typing import Any
 
 import pydantic
 import yaml
 
 
 def eliminate_empty(obj: Any, preserve=False) -> Any:
     """Eliminate empty lists and dicts from an object."""
     if isinstance(obj, list):
         return [eliminate_empty(x, preserve) for x in obj if x or preserve]
     elif isinstance(obj, dict):
         return {k: eliminate_empty(v, preserve) for k, v in obj.items() if v or preserve}
     elif isinstance(obj, pydantic.BaseModel):
         return eliminate_empty(obj.dict(), preserve)
+    elif isinstance(obj, tuple):
+        return [eliminate_empty(x, preserve) for x in obj]
+    elif isinstance(obj, str):
+        return str(obj)
     else:
         return obj
 
 
 def dump_minimal_yaml(obj: Any, minimize=True) -> str:
-    """
-    Dump a YAML string, but eliminating Nones and empty lists and dicts
-    """
+    """Dump a YAML string, but eliminating Nones and empty lists and dicts."""
     return yaml.dump(eliminate_empty(obj, not minimize), sort_keys=False)
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/biological_process.py` & `ontogpt-0.2.2/src/ontogpt/templates/biological_process.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Biological process template."""
 from __future__ import annotations
 
 from typing import Any, List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
@@ -21,15 +22,14 @@
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
 class GeneMolecularActivityRelationship(ConfiguredBaseModel):
-
     gene: Optional[str] = Field(None)
     molecular_activity: Optional[str] = Field(None)
 
 
 class ExtractionResult(ConfiguredBaseModel):
     """A result of extracting knowledge on text."""
 
@@ -43,21 +43,19 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class BiologicalProcess(NamedEntity):
-
     label: Optional[str] = Field(None, description="""the name of the biological process""")
     description: Optional[str] = Field(
         None, description="""a textual description of the biological process"""
     )
     synonyms: Optional[List[str]] = Field(
         default_factory=list, description="""alternative names of the biological process"""
     )
@@ -78,34 +76,30 @@
         default_factory=list,
         description="""semicolon-separated list of gene to molecular activity relationships""",
     )
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
 
 
 class Gene(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class MolecularActivity(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class ChemicalEntity(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
-
-    None
+    pass
 
 
 class Triple(CompoundExpression):
     """Abstract parent for Relation Extraction tasks."""
 
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
@@ -122,36 +116,32 @@
         None,
         description="""An optional qualifier or modifier for the object of the statement,\
             e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/biological_process.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/biological_process.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/core.py` & `ontogpt-0.2.2/src/ontogpt/templates/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+"""Core template."""
 from __future__ import annotations
 
-from datetime import date, datetime
-from enum import Enum
-from typing import Any, Dict, List, Optional
+from typing import Any, List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
 metamodel_version = "None"
 version = "None"
 
@@ -23,17 +22,15 @@
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
 class ExtractionResult(ConfiguredBaseModel):
-    """
-    A result of extracting knowledge on text
-    """
+    """A result of extracting knowledge on text."""
 
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(
@@ -41,68 +38,62 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
-
-    None
+    pass
 
 
 class Triple(CompoundExpression):
-    """
-    Abstract parent for Relation Extraction tasks
-    """
+    """Abstract parent for Relation Extraction tasks."""
 
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(
         None, description="""A qualifier for the statements, e.g. \"NOT\" for negation"""
     )
     subject_qualifier: Optional[str] = Field(
         None,
-        description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""",
+        description="""An optional qualifier or modifier for the subject of the\
+            statement, e.g. \"high dose\" or \"intravenously administered\"""",
     )
     object_qualifier: Optional[str] = Field(
         None,
-        description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""",
+        description="""An optional qualifier or modifier for the object of\
+            the statement, e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/core.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/core.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/ctd.py` & `ontogpt-0.2.2/src/ontogpt/templates/ctd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""CTD template."""
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
@@ -22,20 +23,18 @@
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
 class MeshChemicalIdentifier(str, Enum):
-
     dummy = "dummy"
 
 
 class MeshDiseaseIdentifier(str, Enum):
-
     dummy = "dummy"
 
 
 class ExtractionResult(ConfiguredBaseModel):
     """A result of extracting knowledge on text."""
 
     input_id: Optional[str] = Field(None)
@@ -48,34 +47,30 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Disease(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Chemical(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
-
-    None
+    pass
 
 
 class Triple(CompoundExpression):
     """Abstract parent for Relation Extraction tasks."""
 
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
@@ -123,50 +118,46 @@
         None,
         description="""An optional qualifier or modifier for the disease,\
             e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class ChemicalToDiseaseDocument(TextWithTriples):
     """A document that contains chemical to disease relations."""
 
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[ChemicalToDiseaseRelationship]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class ChemicalToDiseasePredicate(RelationshipType):
     """A predicate for chemical to disease relationships."""
 
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/ctd.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/ctd.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/drug.py` & `ontogpt-0.2.2/src/ontogpt/templates/environmental_sample.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+"""Environmental sample template."""
 from __future__ import annotations
 
-from datetime import date, datetime
-from enum import Enum
-from typing import Any, Dict, List, Optional
+from typing import Any, List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
 metamodel_version = "None"
 version = "None"
 
@@ -22,32 +21,29 @@
     underscore_attrs_are_private=True,
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
-class DrugMechanism(ConfiguredBaseModel):
-
-    disease: Optional[str] = Field(None, description="""the name of the disease that is treated""")
-    drug: Optional[str] = Field(
-        None, description="""the name of the drug that treats the disease"""
-    )
-    mechanism_links: Optional[List[MechanismLink]] = Field(
-        default_factory=list,
-        description="""semicolon-separated list of links, where each link is a triple connecting two entities via a relationship type""",
-    )
-    references: Optional[List[str]] = Field(default_factory=list)
-    source_text: Optional[str] = Field(None)
+class Study(ConfiguredBaseModel):
+    location: Optional[List[str]] = Field(
+        default_factory=list, description="""the sites at which the study was conducted"""
+    )
+    environmental_material: Optional[List[str]] = Field(
+        default_factory=list, description="""the environmental material that was sampled"""
+    )
+    environments: Optional[List[str]] = Field(default_factory=list)
+    causal_relationships: Optional[List[CausalRelationship]] = Field(default_factory=list)
+    variables: Optional[List[str]] = Field(default_factory=list)
+    measurements: Optional[List[Measurement]] = Field(default_factory=list)
 
 
 class ExtractionResult(ConfiguredBaseModel):
-    """
-    A result of extracting knowledge on text
-    """
+    """A result of extracting knowledge on text."""
 
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(
@@ -55,113 +51,115 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
-class MechanismElement(NamedEntity):
-
+class Location(NamedEntity):
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
-class Disease(NamedEntity):
-
+class EnvironmentalMaterial(NamedEntity):
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
-class Drug(NamedEntity):
-
+class Environment(NamedEntity):
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
-class Predicate(NamedEntity):
+class Variable(NamedEntity):
+    id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
+    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
+
 
+class Unit(NamedEntity):
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
+    pass
 
-    None
 
+class Measurement(CompoundExpression):
+    value: Optional[str] = Field(None, description="""the value of the measurement""")
+    unit: Optional[str] = Field(None, description="""the unit of the measurement""")
 
-class MechanismLink(CompoundExpression):
 
-    subject: Optional[str] = Field(None)
-    predicate: Optional[str] = Field(None)
-    object: Optional[str] = Field(None)
+class CausalRelationship(CompoundExpression):
+    cause: Optional[str] = Field(
+        None, description="""the variable that is the cause of the effect"""
+    )
+    effect: Optional[str] = Field(None, description="""the things that is affected""")
 
 
 class Triple(CompoundExpression):
-    """
-    Abstract parent for Relation Extraction tasks
-    """
+    """Abstract parent for Relation Extraction tasks."""
 
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(
         None, description="""A qualifier for the statements, e.g. \"NOT\" for negation"""
     )
     subject_qualifier: Optional[str] = Field(
         None,
-        description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""",
+        description="""An optional qualifier or modifier for the subject of\
+            the statement, e.g. \"high dose\" or \"intravenously administered\"""",
     )
     object_qualifier: Optional[str] = Field(
         None,
-        description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""",
+        description="""An optional qualifier or modifier for the object of\
+            the statement, e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
-DrugMechanism.update_forward_refs()
+Study.update_forward_refs()
 ExtractionResult.update_forward_refs()
 NamedEntity.update_forward_refs()
-MechanismElement.update_forward_refs()
-Disease.update_forward_refs()
-Drug.update_forward_refs()
-Predicate.update_forward_refs()
+Location.update_forward_refs()
+EnvironmentalMaterial.update_forward_refs()
+Environment.update_forward_refs()
+Variable.update_forward_refs()
+Unit.update_forward_refs()
 CompoundExpression.update_forward_refs()
-MechanismLink.update_forward_refs()
+Measurement.update_forward_refs()
+CausalRelationship.update_forward_refs()
 Triple.update_forward_refs()
 TextWithTriples.update_forward_refs()
 RelationshipType.update_forward_refs()
 Publication.update_forward_refs()
 AnnotatorResult.update_forward_refs()
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/drug.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/drug.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/environmental_sample.py` & `ontogpt-0.2.2/src/ontogpt/templates/metabolic_process.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+"""Metabolic process template."""
 from __future__ import annotations
 
-from datetime import date, datetime
-from enum import Enum
-from typing import Any, Dict, List, Optional
+from typing import Any, List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
 metamodel_version = "None"
 version = "None"
 
@@ -22,32 +21,16 @@
     underscore_attrs_are_private=True,
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
-class Study(ConfiguredBaseModel):
-
-    location: Optional[List[str]] = Field(
-        default_factory=list, description="""the sites at which the study was conducted"""
-    )
-    environmental_material: Optional[List[str]] = Field(
-        default_factory=list, description="""the environmental material that was sampled"""
-    )
-    environments: Optional[List[str]] = Field(default_factory=list)
-    causal_relationships: Optional[List[CausalRelationship]] = Field(default_factory=list)
-    variables: Optional[List[str]] = Field(default_factory=list)
-    measurements: Optional[List[Measurement]] = Field(default_factory=list)
-
-
 class ExtractionResult(ConfiguredBaseModel):
-    """
-    A result of extracting knowledge on text
-    """
+    """A result of extracting knowledge on text."""
 
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(
@@ -55,128 +38,110 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
-class Location(NamedEntity):
-
-    id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
-    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
-
-
-class EnvironmentalMaterial(NamedEntity):
-
-    id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
-    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
-
-
-class Environment(NamedEntity):
-
+class MetabolicProcess(NamedEntity):
+    label: Optional[str] = Field(None, description="""the name of the metabolic process""")
+    description: Optional[str] = Field(
+        None, description="""a textual description of the metabolic process"""
+    )
+    synonyms: Optional[List[str]] = Field(
+        default_factory=list, description="""alternative names of the metabolic process"""
+    )
+    subclass_of: Optional[List[str]] = Field(
+        default_factory=list,
+        description="""a semicolon separated list of broader metabolic\
+            processes which this is a subclass of""",
+    )
+    category: Optional[str] = Field(
+        None,
+        description="""the category of metabolic process, e.g metabolic process,\
+            catabolic process, biosynthetic process, small molecule sensor activity""",
+    )
+    inputs: Optional[List[str]] = Field(
+        default_factory=list, description="""the inputs of the metabolic process"""
+    )
+    outputs: Optional[List[str]] = Field(
+        default_factory=list, description="""the outputs of the metabolic process"""
+    )
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
-    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
-
 
-class Variable(NamedEntity):
 
+class MetabolicProcessCategory(NamedEntity):
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
-class Unit(NamedEntity):
-
+class ChemicalEntity(NamedEntity):
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
-
-    None
-
-
-class Measurement(CompoundExpression):
-
-    value: Optional[str] = Field(None, description="""the value of the measurement""")
-    unit: Optional[str] = Field(None, description="""the unit of the measurement""")
-
-
-class CausalRelationship(CompoundExpression):
-
-    cause: Optional[str] = Field(
-        None, description="""the variable that is the cause of the effect"""
-    )
-    effect: Optional[str] = Field(None, description="""the things that is affected""")
+    pass
 
 
 class Triple(CompoundExpression):
-    """
-    Abstract parent for Relation Extraction tasks
-    """
+    """Abstract parent for Relation Extraction tasks."""
 
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(
         None, description="""A qualifier for the statements, e.g. \"NOT\" for negation"""
     )
     subject_qualifier: Optional[str] = Field(
         None,
-        description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""",
+        description="""An optional qualifier or modifier for the subject of the\
+            statement, e.g. \"high dose\" or \"intravenously administered\"""",
     )
     object_qualifier: Optional[str] = Field(
         None,
-        description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""",
+        description="""An optional qualifier or modifier for the object of the\
+            statement, e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
-Study.update_forward_refs()
 ExtractionResult.update_forward_refs()
 NamedEntity.update_forward_refs()
-Location.update_forward_refs()
-EnvironmentalMaterial.update_forward_refs()
-Environment.update_forward_refs()
-Variable.update_forward_refs()
-Unit.update_forward_refs()
+MetabolicProcess.update_forward_refs()
+MetabolicProcessCategory.update_forward_refs()
+ChemicalEntity.update_forward_refs()
 CompoundExpression.update_forward_refs()
-Measurement.update_forward_refs()
-CausalRelationship.update_forward_refs()
 Triple.update_forward_refs()
 TextWithTriples.update_forward_refs()
 RelationshipType.update_forward_refs()
 Publication.update_forward_refs()
 AnnotatorResult.update_forward_refs()
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/environmental_sample.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/environmental_sample.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/gocam.py` & `ontogpt-0.2.2/src/ontogpt/templates/gocam.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""GO-CAM template."""
 from __future__ import annotations
 
 from enum import Enum
 from typing import Any, List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
@@ -22,30 +23,26 @@
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
 class GeneLocationEnum(str, Enum):
-
     dummy = "dummy"
 
 
 class GOCellComponentType(str, Enum):
-
     dummy = "dummy"
 
 
 class CellType(str, Enum):
-
     dummy = "dummy"
 
 
 class GoCamAnnotations(ConfiguredBaseModel):
-
     genes: Optional[List[str]] = Field(
         default_factory=list, description="""semicolon-separated list of genes"""
     )
     organisms: Optional[List[str]] = Field(
         default_factory=list, description="""semicolon-separated list of organism taxons"""
     )
     gene_organisms: Optional[List[GeneOrganismRelationship]] = Field(default_factory=list)
@@ -86,93 +83,79 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Gene(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Pathway(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CellularProcess(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class MolecularActivity(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class GeneLocation(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Organism(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Molecule(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
-
     pass
 
 
 class GeneOrganismRelationship(CompoundExpression):
-
     gene: Optional[str] = Field(None)
     organism: Optional[str] = Field(None)
 
 
 class GeneMolecularActivityRelationship(CompoundExpression):
-
     gene: Optional[str] = Field(None)
     molecular_activity: Optional[str] = Field(None)
 
 
 class GeneMolecularActivityRelationship2(CompoundExpression):
-
     gene: Optional[str] = Field(None)
     molecular_activity: Optional[str] = Field(None)
     target: Optional[str] = Field(None)
 
 
 class GeneSubcellularLocalizationRelationship(CompoundExpression):
-
     gene: Optional[str] = Field(None)
     location: Optional[str] = Field(None)
 
 
 class GeneGeneInteraction(CompoundExpression):
-
     gene1: Optional[str] = Field(None)
     gene2: Optional[str] = Field(None)
 
 
 class Triple(CompoundExpression):
     """Abstract parent for Relation Extraction tasks."""
 
@@ -191,36 +174,32 @@
         None,
         description="""An optional qualifier or modifier for the object of the statement,\
             e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/gocam.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/gocam.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/halo.py` & `ontogpt-0.2.2/src/ontogpt/templates/halo.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+"""HALO template."""
 from __future__ import annotations
 
-from datetime import date, datetime
-from enum import Enum
-from typing import Any, Dict, List, Optional
+from typing import Any, List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
 metamodel_version = "None"
 version = "None"
 
@@ -23,20 +22,18 @@
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
 class Ontology(ConfiguredBaseModel):
-
     elements: Optional[List[OntologyElement]] = Field(default_factory=list)
 
 
 class OntologyElement(ConfiguredBaseModel):
-
     name: Optional[str] = Field(None, description="""the name of the entity""")
     context: Optional[str] = Field(
         None, description="""the ontology to which this belongs (single-valued)"""
     )
     description: Optional[str] = Field(
         None, description="""a textual description of the entity (single-valued)"""
     )
@@ -58,20 +55,20 @@
     )
     parts: Optional[List[str]] = Field(
         default_factory=list,
         description="""a list of names of things this element has as parts (components)""",
     )
     equivalent_to: Optional[str] = Field(
         None,
-        description="""an OWL class expression with the necessary and sufficient conditions for this entity to be an instance of this class""",
+        description="""an OWL class expression with the necessary and\
+            sufficient conditions for this entity to be an instance of this class""",
     )
 
 
 class Category(OntologyElement):
-
     name: Optional[str] = Field(None, description="""the name of the entity""")
     context: Optional[str] = Field(
         None, description="""the ontology to which this belongs (single-valued)"""
     )
     description: Optional[str] = Field(
         None, description="""a textual description of the entity (single-valued)"""
     )
@@ -93,22 +90,21 @@
     )
     parts: Optional[List[str]] = Field(
         default_factory=list,
         description="""a list of names of things this element has as parts (components)""",
     )
     equivalent_to: Optional[str] = Field(
         None,
-        description="""an OWL class expression with the necessary and sufficient conditions for this entity to be an instance of this class""",
+        description="""an OWL class expression with the necessary and\
+            sufficient conditions for this entity to be an instance of this class""",
     )
 
 
 class ExtractionResult(ConfiguredBaseModel):
-    """
-    A result of extracting knowledge on text
-    """
+    """A result of extracting knowledge on text."""
 
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(
@@ -116,28 +112,24 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
-
-    None
+    pass
 
 
 class Triple(CompoundExpression):
-    """
-    Abstract parent for Relation Extraction tasks
-    """
+    """Abstract parent for Relation Extraction tasks."""
 
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(
         None, description="""A qualifier for the statements, e.g. \"NOT\" for negation"""
     )
@@ -150,36 +142,32 @@
         None,
         description="""An optional qualifier or modifier for the object of the statement,\
             e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/halo.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/halo.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/mendelian_disease.py` & `ontogpt-0.2.2/src/ontogpt/templates/drug.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+"""Drug template."""
 from __future__ import annotations
 
-from datetime import date, datetime
-from enum import Enum
-from typing import Any, Dict, List, Optional
+from typing import Any, List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
 metamodel_version = "None"
 version = "None"
 
@@ -22,18 +21,30 @@
     underscore_attrs_are_private=True,
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
+class DrugMechanism(ConfiguredBaseModel):
+    disease: Optional[str] = Field(None, description="""the name of the disease that is treated""")
+    drug: Optional[str] = Field(
+        None, description="""the name of the drug that treats the disease"""
+    )
+    mechanism_links: Optional[List[MechanismLink]] = Field(
+        default_factory=list,
+        description="""semicolon-separated list of links, where each link is a triple\
+            connecting two entities via a relationship type""",
+    )
+    references: Optional[List[str]] = Field(default_factory=list)
+    source_text: Optional[str] = Field(None)
+
+
 class ExtractionResult(ConfiguredBaseModel):
-    """
-    A result of extracting knowledge on text
-    """
+    """A result of extracting knowledge on text."""
 
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(
@@ -41,134 +52,102 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
-    id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
-    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
-
-
-class MendelianDisease(NamedEntity):
-
-    name: Optional[str] = Field(None, description="""the name of the disease""")
-    description: Optional[str] = Field(None, description="""a description of the disease""")
-    synonyms: Optional[List[str]] = Field(default_factory=list)
-    subclass_of: Optional[List[str]] = Field(default_factory=list)
-    symptoms: Optional[List[str]] = Field(default_factory=list)
-    inheritance: Optional[str] = Field(None)
-    genes: Optional[List[str]] = Field(default_factory=list)
-    disease_onsets: Optional[List[str]] = Field(default_factory=list)
-    publications: Optional[List[Publication]] = Field(default_factory=list)
-    id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
-    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
-
-
-class DiseaseCategory(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
-class Gene(NamedEntity):
-
+class MechanismElement(NamedEntity):
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
-class Symptom(NamedEntity):
-
-    characteristic: Optional[str] = Field(None)
-    affects: Optional[str] = Field(None)
-    severity: Optional[str] = Field(None)
-    onset_of_symptom: Optional[str] = Field(None)
+class Disease(NamedEntity):
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
-class Onset(NamedEntity):
-
-    years_old: Optional[str] = Field(None)
-    decades: Optional[List[str]] = Field(default_factory=list)
-    juvenile_or_adult: Optional[str] = Field(None)
+class Drug(NamedEntity):
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
-class Inheritance(NamedEntity):
-
+class Predicate(NamedEntity):
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
+    pass
+
 
-    None
+class MechanismLink(CompoundExpression):
+    subject: Optional[str] = Field(None)
+    predicate: Optional[str] = Field(None)
+    object: Optional[str] = Field(None)
 
 
 class Triple(CompoundExpression):
-    """
-    Abstract parent for Relation Extraction tasks
-    """
+    """Abstract parent for Relation Extraction tasks."""
 
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(
         None, description="""A qualifier for the statements, e.g. \"NOT\" for negation"""
     )
     subject_qualifier: Optional[str] = Field(
         None,
-        description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""",
+        description="""An optional qualifier or modifier for the subject of the statement,\
+            e.g. \"high dose\" or \"intravenously administered\"""",
     )
     object_qualifier: Optional[str] = Field(
         None,
-        description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""",
+        description="""An optional qualifier or modifier for the object of the statement,\
+            e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
+DrugMechanism.update_forward_refs()
 ExtractionResult.update_forward_refs()
 NamedEntity.update_forward_refs()
-MendelianDisease.update_forward_refs()
-DiseaseCategory.update_forward_refs()
-Gene.update_forward_refs()
-Symptom.update_forward_refs()
-Onset.update_forward_refs()
-Inheritance.update_forward_refs()
+MechanismElement.update_forward_refs()
+Disease.update_forward_refs()
+Drug.update_forward_refs()
+Predicate.update_forward_refs()
 CompoundExpression.update_forward_refs()
+MechanismLink.update_forward_refs()
 Triple.update_forward_refs()
 TextWithTriples.update_forward_refs()
 RelationshipType.update_forward_refs()
 Publication.update_forward_refs()
 AnnotatorResult.update_forward_refs()
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/mendelian_disease.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/mendelian_disease.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/metabolic_process.py` & `ontogpt-0.2.2/src/ontogpt/templates/gene_description_term.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 from datetime import date, datetime
 from enum import Enum
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Literal, Optional, Union
 
+from linkml_runtime.linkml_model import Decimal
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
 metamodel_version = "None"
 version = "None"
 
 
@@ -22,14 +23,29 @@
     underscore_attrs_are_private=True,
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
+class GeneDescription(ConfiguredBaseModel):
+    """
+    A summarization of an individual gene
+    """
+
+    about: Optional[str] = Field(None)
+    narrative_summary: Optional[str] = Field(
+        None, description="""A free text summary describing the function of the gene"""
+    )
+    terms: Optional[List[str]] = Field(
+        default_factory=list,
+        description="""A semicolon separated list of controlled terms that describe the function of the gene""",
+    )
+
+
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
 
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
@@ -41,59 +57,29 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
-class MetabolicProcess(NamedEntity):
-
-    label: Optional[str] = Field(None, description="""the name of the metabolic process""")
-    description: Optional[str] = Field(
-        None, description="""a textual description of the metabolic process"""
-    )
-    synonyms: Optional[List[str]] = Field(
-        default_factory=list, description="""alternative names of the metabolic process"""
-    )
-    subclass_of: Optional[List[str]] = Field(
-        default_factory=list,
-        description="""a semicolon separated list of broader metabolic processes which this is a subclass of""",
-    )
-    category: Optional[str] = Field(
-        None,
-        description="""the category of metabolic process, e.g metabolic process, catabolic process, biosynthetic process, small molecule sensor activity""",
-    )
-    inputs: Optional[List[str]] = Field(
-        default_factory=list, description="""the inputs of the metabolic process"""
-    )
-    outputs: Optional[List[str]] = Field(
-        default_factory=list, description="""the outputs of the metabolic process"""
-    )
-    id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
-
-
-class MetabolicProcessCategory(NamedEntity):
-
+class Gene(NamedEntity):
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
-class ChemicalEntity(NamedEntity):
-
+class GeneDescriptionTerm(NamedEntity):
+    label: Optional[str] = Field(None, description="""the name of the GO term""")
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
-    label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
-
     None
 
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
@@ -111,47 +97,43 @@
     object_qualifier: Optional[str] = Field(
         None,
         description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
+GeneDescription.update_forward_refs()
 ExtractionResult.update_forward_refs()
 NamedEntity.update_forward_refs()
-MetabolicProcess.update_forward_refs()
-MetabolicProcessCategory.update_forward_refs()
-ChemicalEntity.update_forward_refs()
+Gene.update_forward_refs()
+GeneDescriptionTerm.update_forward_refs()
 CompoundExpression.update_forward_refs()
 Triple.update_forward_refs()
 TextWithTriples.update_forward_refs()
 RelationshipType.update_forward_refs()
 Publication.update_forward_refs()
 AnnotatorResult.update_forward_refs()
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/metabolic_process.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/metabolic_process.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/metagenome_study.py` & `ontogpt-0.2.2/src/ontogpt/templates/metagenome_study.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Metagenome study template."""
 from __future__ import annotations
 
 from typing import Any, List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
@@ -21,15 +22,14 @@
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
 class Study(ConfiguredBaseModel):
-
     environments: Optional[List[str]] = Field(default_factory=list)
     causal_relationships: Optional[List[CausalRelationship]] = Field(default_factory=list)
     variables: Optional[List[str]] = Field(default_factory=list)
     treatments: Optional[List[str]] = Field(default_factory=list)
     measurements: Optional[List[Measurement]] = Field(default_factory=list)
     location: Optional[List[str]] = Field(
         default_factory=list, description="""the sites at which the study was conducted"""
@@ -41,17 +41,15 @@
     organisms: Optional[List[str]] = Field(
         default_factory=list,
         description="""semicolon-separated list of all studied organism taxons""",
     )
 
 
 class ExtractionResult(ConfiguredBaseModel):
-    """
-    A result of extracting knowledge on text
-    """
+    """A result of extracting knowledge on text."""
 
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(
@@ -59,80 +57,68 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Location(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class EnvironmentalMaterial(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Environment(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Variable(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Unit(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class SequencingTechnology(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Treatment(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Organism(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
-
-    None
+    pass
 
 
 class Measurement(CompoundExpression):
-
     value: Optional[str] = Field(None, description="""the value of the measurement""")
     unit: Optional[str] = Field(None, description="""the unit of the measurement""")
 
 
 class CausalRelationship(CompoundExpression):
-
     cause: Optional[str] = Field(
         None, description="""the variable that is the cause of the effect"""
     )
     effect: Optional[str] = Field(None, description="""the things that is affected""")
 
 
 class Triple(CompoundExpression):
@@ -153,36 +139,32 @@
         None,
         description="""An optional qualifier or modifier for the object of the statement,\
             e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/metagenome_study.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/metagenome_study.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/ontology_class.py` & `ontogpt-0.2.2/src/ontogpt/templates/ontology_class.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Ontology Class template."""
 from __future__ import annotations
 
 from typing import Any, List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
@@ -21,24 +22,21 @@
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
 class LogicalDefinition(ConfiguredBaseModel):
-
     genus: Optional[List[str]] = Field(default_factory=list)
     differentiating_characteristic_relationship: Optional[str] = Field(None)
     differentiating_characteristic_parents: Optional[List[str]] = Field(default_factory=list)
 
 
 class ExtractionResult(ConfiguredBaseModel):
-    """
-    A result of extracting knowledge on text
-    """
+    """A result of extracting knowledge on text."""
 
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(
@@ -46,92 +44,85 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class OntologyClass(NamedEntity):
-
     label: Optional[str] = Field(None, description="""the name of the entity""")
     description: Optional[str] = Field(None, description="""a textual description of the entity""")
     synonyms: Optional[List[str]] = Field(
         default_factory=list, description="""alternative names of the entity"""
     )
     categories: Optional[List[str]] = Field(
         default_factory=list, description="""the categories to which this entity belongs"""
     )
     subclass_of: Optional[List[str]] = Field(default_factory=list)
     logical_definition: Optional[LogicalDefinition] = Field(
         None,
-        description="""the necessary and sufficient conditions for this entity to be an instance of this class""",
+        description="""the necessary and sufficient conditions for this\
+            entity to be an instance of this class""",
     )
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
 
 
 class Relation(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
-
-    None
+    pass
 
 
 class Triple(CompoundExpression):
-    """
-    Abstract parent for Relation Extraction tasks
-    """
+    """Abstract parent for Relation Extraction tasks."""
 
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(
         None, description="""A qualifier for the statements, e.g. \"NOT\" for negation"""
     )
     subject_qualifier: Optional[str] = Field(
         None,
-        description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""",
+        description="""An optional qualifier or modifier for the subject\
+            of the statement, e.g. \"high dose\" or \"intravenously administered\"""",
     )
     object_qualifier: Optional[str] = Field(
         None,
-        description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""",
+        description="""An optional qualifier or modifier for the\
+            object of the statement, e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/ontology_class.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/ontology_class.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/phenotype.py` & `ontogpt-0.2.2/src/ontogpt/templates/phenotype.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,12 @@
+"""Phenotype template."""
 from __future__ import annotations
 
-from datetime import date, datetime
-from enum import Enum
-from typing import Any, Dict, List, Literal, Optional, Union
+from typing import Any, List, Optional
 
-from linkml_runtime.linkml_model import Decimal
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
 metamodel_version = "None"
 version = "None"
 
 
@@ -24,31 +22,29 @@
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
 class Trait(ConfiguredBaseModel):
-
     quality: Optional[str] = Field(
         None, description="""the phenotypic quality exibited by the phenotype"""
     )
     anatomical_entity: Optional[str] = Field(
         None, description="""the name of the disease that is treated."""
     )
     chemical_entity: Optional[str] = Field(
         None,
-        description="""semicolon-separated list of treatment to adverse effect associations, e.g. Imatinib*nausea""",
+        description="""semicolon-separated list of treatment\
+            to adverse effect associations, e.g. Imatinib*nausea""",
     )
 
 
 class ExtractionResult(ConfiguredBaseModel):
-    """
-    A result of extracting knowledge on text
-    """
+    """A result of extracting knowledge on text."""
 
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(
@@ -56,46 +52,39 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Quality(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class ChemicalEntity(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class AnatomicalEntity(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
-
-    None
+    pass
 
 
 class Triple(CompoundExpression):
-    """
-    Abstract parent for Relation Extraction tasks
-    """
+    """Abstract parent for Relation Extraction tasks."""
 
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(
         None, description="""A qualifier for the statements, e.g. \"NOT\" for negation"""
     )
@@ -108,36 +97,32 @@
         None,
         description="""An optional qualifier or modifier for the object of the statement,\
             e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/phenotype.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/phenotype.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/reaction.py` & `ontogpt-0.2.2/src/ontogpt/templates/reaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+"""Reaction template."""
 from __future__ import annotations
 
 from typing import Any, Dict, List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
@@ -21,28 +22,26 @@
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
 class GeneToReaction(ConfiguredBaseModel):
-
     gene: Optional[str] = Field(
         None, description="""name of the gene that catalyzes the reaction"""
     )
     reactions: Optional[Dict[str, Reaction]] = Field(
         default_factory=dict,
         description="""semicolon separated list of reaction equations\
             (e.g. A+B = C+D) catalyzed by the gene""",
     )
     organism: Optional[str] = Field(None)
 
 
 class ReactionDocument(ConfiguredBaseModel):
-
     genes: Optional[List[str]] = Field(
         default_factory=list,
         description="""semicolon separated list of genes that catalyzes the mentioned reactions""",
     )
     reactions: Optional[Dict[str, Reaction]] = Field(
         default_factory=dict,
         description="""semicolon separated list of reaction equations\
@@ -71,21 +70,19 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Reaction(NamedEntity):
-
     label: Optional[str] = Field(None, description="""the name of the reaction""")
     description: Optional[str] = Field(
         None, description="""a textual description of the reaction"""
     )
     synonyms: Optional[List[str]] = Field(
         default_factory=list, description="""alternative names of the reaction"""
     )
@@ -100,50 +97,43 @@
         default_factory=list,
         description="""semicolon separated list of chemical entities on the right side""",
     )
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
 
 
 class ReactionGrouping(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class ChemicalEntity(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Evidence(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Gene(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Organism(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
-
-    None
+    pass
 
 
 class GeneReactionPairing(CompoundExpression):
-
     gene: Optional[str] = Field(
         None, description="""name of the gene that catalyzes the reaction"""
     )
     reaction: Optional[str] = Field(
         None,
         description="""equation describing the reaction (e.g. A+B = C+D) catalyzed by the gene""",
     )
@@ -167,36 +157,32 @@
         None,
         description="""An optional qualifier or modifier for the object of the statement,\
             e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/reaction.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/reaction.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/recipe.py` & `ontogpt-0.2.2/src/ontogpt/templates/recipe.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,11 @@
+"""Recipe template."""
 from __future__ import annotations
 
-from datetime import date, datetime
-from enum import Enum
-from typing import Any, Dict, List, Optional
+from typing import Any, List, Optional
 
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
 metamodel_version = "None"
 version = "None"
 
@@ -23,38 +22,37 @@
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
 class Recipe(ConfiguredBaseModel):
-
     url: Optional[str] = Field(None)
     label: Optional[str] = Field(None, description="""the name of the recipe""")
     description: Optional[str] = Field(
         None, description="""a brief textual description of the recipe"""
     )
     categories: Optional[List[str]] = Field(
         default_factory=list,
-        description="""a semicolon separated list of the categories to which this recipe belongs""",  # noqa
+        description="""a semicolon separated list of the categories to which this recipe belongs""",
     )
     ingredients: Optional[List[Ingredient]] = Field(
         default_factory=list,
-        description="""a semicolon separated list of the ingredients plus quantities of the recipe""",  # noqa
+        description="""a semicolon separated list of the\
+            ingredients plus quantities of the recipe""",
     )
     steps: Optional[List[Step]] = Field(
         default_factory=list,
-        description="""a semicolon separated list of the individual steps involved in this recipe""",  # noqa
+        description="""a semicolon separated list of the\
+            individual steps involved in this recipe""",
     )
 
 
 class ExtractionResult(ConfiguredBaseModel):
-    """
-    A result of extracting knowledge on text
-    """
+    """A result of extracting knowledge on text."""
 
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(
@@ -62,72 +60,62 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class FoodType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class RecipeCategory(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Action(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class UtensilType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Unit(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
-
-    None
+    pass
 
 
 class Ingredient(CompoundExpression):
-
     food_item: Optional[FoodItem] = Field(None, description="""the food item""")
     amount: Optional[Quantity] = Field(
         None, description="""the quantity of the ingredient, e.g. 2 lbs"""
     )
 
 
 class Quantity(CompoundExpression):
-
     value: Optional[str] = Field(None, description="""the value of the quantity""")
     unit: Optional[str] = Field(
         None, description="""the unit of the quantity, e.g. grams, cups, etc."""
     )
 
 
 class Step(CompoundExpression):
-
     action: Optional[str] = Field(
         None, description="""the action taken in this step (e.g. mix, add)"""
     )
     inputs: Optional[List[FoodItem]] = Field(
         default_factory=list,
         description="""a semicolon separated list of the inputs of this step""",
     )
@@ -138,15 +126,14 @@
     utensils: Optional[List[str]] = Field(
         default_factory=list,
         description="""the kitchen utensil used in this step (e.g. pan, bowl)""",
     )
 
 
 class FoodItem(CompoundExpression):
-
     food: Optional[str] = Field(None, description="""the food item""")
     state: Optional[str] = Field(
         None, description="""the state of the food item (e.g. chopped, diced)"""
     )
 
 
 class Triple(CompoundExpression):
@@ -156,47 +143,43 @@
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(
         None, description="""A qualifier for the statements, e.g. \"NOT\" for negation"""
     )
     subject_qualifier: Optional[str] = Field(
         None,
-        description="""An optional qualifier or modifier for the subject of the statement,\
-            e.g. \"high dose\" or \"intravenously administered\"""",
+        description="""An optional qualifier or modifier for the subject of the\
+            statement, e.g. \"high dose\" or \"intravenously administered\"""",
     )
     object_qualifier: Optional[str] = Field(
         None,
-        description="""An optional qualifier or modifier for the object of the statement,\
-            e.g. \"severe\" or \"with additional complications\"""",
+        description="""An optional qualifier or modifier for the object of\
+            the statement, e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/recipe.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/recipe.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/treatment.py` & `ontogpt-0.2.2/src/ontogpt/templates/treatment.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
+"""Treatment template."""
 from __future__ import annotations
 
-from datetime import date, datetime
 from enum import Enum
-from typing import Any, Dict, List, Literal, Optional, Union
+from typing import Any, List, Optional
 
-from linkml_runtime.linkml_model import Decimal
 from pydantic import BaseModel as BaseModel
 from pydantic import Field
 
 metamodel_version = "None"
 version = "None"
 
 
@@ -24,76 +23,73 @@
     extra="forbid",
     arbitrary_types_allowed=True,
 ):
     pass
 
 
 class NCITDrugType(str, Enum):
-
     dummy = "dummy"
 
 
 class NCITTreatmentType(str, Enum):
-
     dummy = "dummy"
 
 
 class NCITTActivityType(str, Enum):
-
     dummy = "dummy"
 
 
 class MAXOActionType(str, Enum):
-
     dummy = "dummy"
 
 
 class MESHTherapeuticType(str, Enum):
-
     dummy = "dummy"
 
 
 class CHEBIDrugType(str, Enum):
-
     dummy = "dummy"
 
 
 class DiseaseTreatmentSummary(ConfiguredBaseModel):
-
     disease: Optional[str] = Field(None, description="""the name of the disease that is treated""")
     drugs: Optional[List[str]] = Field(
         default_factory=list,
         description="""semicolon-separated list of named small molecule drugs""",
     )
     treatments: Optional[List[str]] = Field(
         default_factory=list,
-        description="""semicolon-separated list of therapies and treatments are indicated for treating the disease.""",
+        description="""semicolon-separated list of therapies and treatments are\
+            indicated for treating the disease.""",
     )
     contraindications: Optional[List[str]] = Field(
         default_factory=list,
-        description="""semicolon-separated list of therapies and treatments that are contra-indicated for the disease, and should not be used, due to risk of adverse effects.""",
+        description="""semicolon-separated list of therapies and treatments that are\
+            contra-indicated for the disease, and should not be used,\
+            due to risk of adverse effects.""",
     )
     treatment_mechanisms: Optional[List[TreatmentMechanism]] = Field(
         default_factory=list,
-        description="""semicolon-separated list of treatment to asterisk-separated mechanism associations""",
+        description="""semicolon-separated list of treatment to asterisk-separated\
+            mechanism associations""",
     )
     treatment_efficacies: Optional[List[TreatmentEfficacy]] = Field(
         default_factory=list,
-        description="""semicolon-separated list of treatment to efficacy associations, e.g. Imatinib*effective""",
+        description="""semicolon-separated list of treatment to efficacy associations,\
+            e.g. Imatinib*effective""",
     )
     treatment_adverse_effects: Optional[List[TreatmentAdverseEffect]] = Field(
         default_factory=list,
-        description="""semicolon-separated list of treatment to adverse effect associations, e.g. Imatinib*nausea""",
+        description="""semicolon-separated list of treatment to adverse effect associations,\
+            e.g. Imatinib*nausea""",
     )
 
 
 class ExtractionResult(ConfiguredBaseModel):
-    """
-    A result of extracting knowledge on text
-    """
+    """A result of extracting knowledge on text."""
 
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
     extracted_object: Optional[Any] = Field(
@@ -101,128 +97,112 @@
     )
     named_entities: Optional[List[Any]] = Field(
         default_factory=list, description="""Named entities extracted from the text"""
     )
 
 
 class NamedEntity(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Gene(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Symptom(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Disease(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class AdverseEffect(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Treatment(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Mechanism(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Drug(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class CompoundExpression(ConfiguredBaseModel):
-
-    None
+    pass
 
 
 class TreatmentMechanism(CompoundExpression):
-
     treatment: Optional[str] = Field(None)
     mechanism: Optional[str] = Field(None)
 
 
 class TreatmentAdverseEffect(CompoundExpression):
-
     treatment: Optional[str] = Field(None)
     adverse_effects: Optional[List[str]] = Field(default_factory=list)
 
 
 class TreatmentEfficacy(CompoundExpression):
-
     treatment: Optional[str] = Field(None)
     efficacy: Optional[str] = Field(None)
 
 
 class Triple(CompoundExpression):
-    """
-    Abstract parent for Relation Extraction tasks
-    """
+    """Abstract parent for Relation Extraction tasks."""
 
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
     qualifier: Optional[str] = Field(
         None, description="""A qualifier for the statements, e.g. \"NOT\" for negation"""
     )
     subject_qualifier: Optional[str] = Field(
         None,
-        description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""",
+        description="""An optional qualifier or modifier for the subject of the statement,\
+            e.g. \"high dose\" or \"intravenously administered\"""",
     )
     object_qualifier: Optional[str] = Field(
         None,
-        description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""",
+        description="""An optional qualifier or modifier for the object of the statement,\
+            e.g. \"severe\" or \"with additional complications\"""",
     )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
 
 
 class RelationshipType(NamedEntity):
-
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
 
 
 class Publication(ConfiguredBaseModel):
-
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
```

### Comparing `ontogpt-0.2.1/src/ontogpt/templates/treatment.yaml` & `ontogpt-0.2.2/src/ontogpt/templates/treatment.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/webapp/html/form.html` & `ontogpt-0.2.2/src/ontogpt/webapp/html/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.1/src/ontogpt/webapp/main.py` & `ontogpt-0.2.2/src/ontogpt/webapp/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,20 @@
+"""Webapp main function."""
 from io import StringIO
 from pathlib import Path
 from typing import Dict
 
 import uvicorn
 from fastapi import FastAPI, Form, Request
 from pydantic import BaseModel
 from starlette.staticfiles import StaticFiles
 from starlette.templating import Jinja2Templates
 
-from ontogpt.engines.knowledge_engine import DATAMODELS
+from ontogpt.engines.enrichment import EnrichmentEngine, GeneSet
+from ontogpt.engines.knowledge_engine import DATAMODELS, MODELS
 from ontogpt.engines.spires_engine import SPIRESEngine
 from ontogpt.io.html_exporter import HTMLExporter
 
 this_path = Path(__file__).parent
 static_dir = this_path / "static"
 html_dir = this_path / "html"
 
@@ -54,10 +56,33 @@
     output = StringIO()
     html_exporter.export(ann, output)
     return templates.TemplateResponse(
         "results.html", context={"request": request, "inner_html": output.getvalue()}
     )
 
 
+@app.get("/spindoctor")
+def sd_read_root(request: Request):
+    return templates.TemplateResponse(
+        "spindoctor/form.html", context={"request": request, "models": MODELS}
+    )
+
+
+@app.post("/spindoctor")
+def sd_form_post(request: Request, model: str = Form(...), text: str = Form(...)):
+    print(f"Received request with model {model}")
+    print(f"Received request with text {text}")
+    symbols = [s.strip() for s in text.split("\n")]
+    engine = EnrichmentEngine(model=model)
+    gene_set = GeneSet(name="TEMP", gene_symbols=symbols)
+    ann = engine.summarize(gene_set)
+    print(f"Got {ann}")
+    output = StringIO()
+    html_exporter.export(ann, output)
+    return templates.TemplateResponse(
+        "spindoctor/results.html", context={"request": request, "inner_html": output.getvalue()}
+    )
+
+
 def start():
-    """Launched with `poetry run start` at root level."""
-    uvicorn.run("ontogpt.webapp.main:app", host="0.0.0.0", port=8000, reload=True)
+    """Launch with `poetry run start` at root level."""
+    uvicorn.run("ontogpt.webapp.main:app", host="127.0.0.1", port=8000, reload=True)
```

### Comparing `ontogpt-0.2.1/PKG-INFO` & `ontogpt-0.2.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ontogpt
-Version: 0.2.1
+Version: 0.2.2
 Summary: OntoGPT
 License: BSD-3
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,16 @@
 Provides-Extra: web
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0) ; extra == "web"
 Requires-Dist: SQLAlchemy (>=1.4.32,<2.0.0,!=1.4.46)
 Requires-Dist: aiohttp (>=3.8.4,<4.0.0)
 Requires-Dist: airium (>=0.2.5,<0.3.0)
 Requires-Dist: beautifulsoup4 (>=4.11.1,<5.0.0)
 Requires-Dist: bioc (>=2.0.post5,<3.0)
-Requires-Dist: class-resolver (>=0.3.10,<0.4.0)
+Requires-Dist: cachier (>=2.1.0,<3.0.0)
+Requires-Dist: class-resolver
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: eutils (>=0.6.0,<0.7.0)
 Requires-Dist: fastapi (>=0.88.0,<0.89.0) ; extra == "web"
 Requires-Dist: gilda (>=0.10.3,<0.11.0)
 Requires-Dist: greenlet (!=2.0.2)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: importlib (>=1.0.4,<2.0.0)
@@ -32,46 +33,53 @@
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: linkml (>=1.4.10,<2.0.0)
 Requires-Dist: linkml-owl (>=0.2.7,<0.3.0)
 Requires-Dist: linkml-runtime (>=1.4.9,<2.0.0)
 Requires-Dist: myst-parser[docs] (>=0.18.1,<0.19.0) ; extra == "docs"
 Requires-Dist: nlpcloud (>=1.0.39,<2.0.0)
-Requires-Dist: oaklib (>=0.3.1,<0.4.0)
-Requires-Dist: openai (>=0.27.2,<0.28.0)
+Requires-Dist: oaklib (>=0.5.1,<0.6.0)
+Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: recipe-scrapers[recipes] (>=14.35.0,<15.0.0) ; extra == "recipes"
 Requires-Dist: sphinx-autodoc-typehints[docs] (>=1.19.4,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinx-click[docs] (>=4.3.0,<5.0.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme[docs] (>=1.0.0,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinx[docs] (>=5.3.0,<6.0.0) ; extra == "docs"
-Requires-Dist: tiktoken (>=0.1.1,<0.2.0)
+Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0) ; extra == "web"
 Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
+Requires-Dist: wikipedia-api (>=0.5.8,<0.6.0)
 Description-Content-Type: text/markdown
 
 # OntoGPT
 
 Generation of Ontologies and Knowledge Bases using GPT
 
 A knowledge extraction tool that uses a large language model to extract semantic information from text.
 
 This makes use of so-called *instruction prompts* in Large Language Models (LLMs) such as GPT-4.
 
 Currently there are two different pipelines implemented:
 
 - SPIRES: Structured Prompt Interrogation and Recursive Extraction of Semantics
     - Zero-shot learning approach to extracting nested semantic structures from text
-    - Inputs: LinkML schema + text
+    - Inputs: [LinkML](https://linkml.io/) schema + text
     - Outputs: JSON, YAML, or RDF or OWL that conforms to the schema
     - Uses text-davinci-003
 - HALO: HAllucinating Latent Ontologies 
     - Few-shot learning approach to generating/hallucinating a domain ontology given a few examples
     - Uses code-davinci-002
 
+SPIRES is described futher in: Caufield JH, Hegde H, Emonet V, Harris NL, Joachimiak MP, Matentzoglu N, et al. Structured prompt interrogation and recursive extraction of semantics (SPIRES): A method for populating knowledge bases using zero-shot learning. arXiv [cs.AI]. 2023. http://arxiv.org/abs/2304.02711
+
+## Citation
+
+ - https://arxiv.org/abs/2304.02711
+
 ## SPIRES: Usage
 
 Given a short text `abstract.txt` with content such as:
 
    > The cGAS/STING-mediated DNA-sensing signaling pathway is crucial
    for interferon (IFN) production and host antiviral
    responses
@@ -87,15 +95,15 @@
    > ...
 
 (see [full input](tests/input/cases/gocam-betacat.txt))
 
 We can extract this into the [GO pathway datamodel](src/ontogpt/templates/gocam.yaml):
 
 ```bash
-ontogpt extract -t gocam.GoCamAnnotations abstract.txt
+ontogpt extract -t gocam.GoCamAnnotations -i abstract.txt
 ```
 
 Giving schema-compliant yaml such as:
 
 ```yaml
 genes:
 - HGNC:2514
@@ -122,28 +130,28 @@
 
 Note in the above the grounding is very preliminary and can be improved. Ungrounded NamedEntities appear as text.
 
 ## How it works
 
 1. You provide an arbitrary data model, describing the structure you want to extract text into
     - this can be nested (but see limitations below)
-2. provide your preferred annotations for grounding NamedEntity fields
-3. ontogpt will:
+2. Provide your preferred annotations for grounding NamedEntity fields
+3. OntoGPT will:
     - generate a prompt
-    - feed the prompt to a language model (currently OpenAI)
+    - feed the prompt to a language model (currently OpenAI GPT models)
     - parse the results into a dictionary structure
     - ground the results using a preferred annotator
 
 ## Pre-requisites
 
-- python 3.9+
-- an OpenAI account
-- a BioPortal account (optional, for grounding)
+- Python 3.9+
+- An OpenAI account
+- A [BioPortal](https://bioportal.bioontology.org/) account (optional, for grounding)
 
-You will need to set both API keys using OAK (which is a dependency of this project)
+You will need to set both API keys using the [Ontology Access Kit](https://github.com/INCATools/ontology-access-kit) (OAK, a dependency of this project)
 
 ```
 poetry run runoak set-apikey -e openai <your openai api key>
 poetry run runoak set-apikey -e bioportal <your bioportal api key>
 ```
 
 ## How to define your own extraction data model
@@ -220,59 +228,61 @@
 - the schema is defined in LinkML
 - prompt hints can be specified using the `prompt` annotation (otherwise description is used)
 - multivalued fields are supported
 - the default range is string - these are not grounded. E.g. disease name, synonyms
 - define a class for each NamedEntity
 - for any NamedEntity, you can specify a preferred annotator using the `annotators` annotation
 
-We recommend following an established schema like Biolink, but you can define your own.
+We recommend following an established schema like [BioLink Model](https://github.com/biolink/biolink-model), but you can define your own.
 
 ### Step 2: Compile the schema
 
-Run the `make` command at the top level. This will compile the schema to pedantic
+Place the schema YAML in the directory `src/ontogpt/templates/`.
+
+Run the `make` command at the top level. This will compile the schema to Python (Pydantic classes).
 
 ### Step 3: Run the command line
 
 e.g.
 
 ```
-ontogpt extract -t mendelian_disease.MendelianDisease marfan-wikipedia.txt
+ontogpt extract -t mendelian_disease.MendelianDisease -i marfan-wikipedia.txt
 ```
 
 ## Web Application
 
 There is a bare bones web application
 
 ```
 poetry run web-ontogpt
 ```
 
 Note that the agent running uvicorn must have the API key set, so for obvious reasons
-don't host this publicly without authentication, unless you want your credits drained. 
+don't host this publicly without authentication, unless you want your credits drained.
 
 ## Features
 
 ### Multiple levels of nesting
 
 Currently no more than two levels of nesting are recommended.
 
-If a field has a range which is itself a class and not a primitive, it will attempt to nest
+If a field has a range which is itself a class and not a primitive, it will attempt to nest.
 
 E.g. the gocam schema has an attribute:
 
 ```yaml
   attributes:
       ...
       gene_functions:
         description: semicolon-separated list of gene to molecular activity relationships
         multivalued: true
         range: GeneMolecularActivityRelationship
 ```
 
-Because GeneMolecularActivityRelationship is *inlined* it will nest
+Because `GeneMolecularActivityRelationship` is *inlined* it will nest
 
 The generated prompt is:
 
 `gene_functions : <semicolon-separated list of gene to molecular activities relationships>`
 
 The output of this is then passed through further SPIRES iterations.
 
@@ -341,43 +351,68 @@
       source_nodes:
         - CL:0000000 ## cell
         
 ```
 
 ## OWL Exports
 
-The `extract` command will let you export the results as OWL axioms, utilizing linkml-owl mappings in the schema.
+The `extract` command will let you export the results as OWL axioms, utilizing [linkml-owl](https://linkml.io/linkml-owl) mappings in the schema.
 
 For example:
 
 ```bash
-ontogpt extract -t recipe recipe-spaghetti.txt -o recipe-spaghetti.owl -O owl
+ontogpt extract -t recipe -i recipe-spaghetti.txt -o recipe-spaghetti.owl -O owl
 ```
 
 See [src/ontogpt/templates/recipe.yaml](src/ontogpt/templates/recipe.yaml) 
 for an example of a schema that uses linkml-owl mappings.
 
 See the Makefile for a full pipeline that involves using robot to extract a subset of FOODON
-and merge in the extracted results.
+and merge in the extracted results. This uses [recipe-scrapers](https://github.com/hhursev/recipe-scrapers)
+
+Example output OWL here:
+
+- [recipe-all-merged.owl](https://github.com/monarch-initiative/ontogpt/blob/main/tests/output/owl/merged/recipe-all-merged.owl)
+
+Example classification:
+
+<img width="1329" alt="image" src="https://user-images.githubusercontent.com/50745/230427663-20d845e9-f1d5-490e-b1ad-cdccdd0dca70.png">
+
+
+Contributions on recipes to test welcome from anyone! Just make a PR [here](https://github.com/monarch-initiative/ontogpt/blob/main/tests/input/recipe-urls.csv). See [this list](https://github.com/hhursev/recipe-scrapers) for accepted URLs
+
 
 ## HALO: Usage
 
 TODO
 
 
 
+## Gene Enrichment
+
+Given a set of genes, OntoGPT can find similarities among them.
+
+Example:
+```
+ontogpt enrichment HGNC:8858 HGNC:8859 HGNC:9719
+```
+
+Results:
+
+```
+Commonality: Protein targeting to the Peroxisome. All the genes are involved in targeting proteins to the peroxisome membrane, matrix or both, and they are all located in cytoplasm; peroxisome; and/or endoplasmic reticulum. Additionally, they all enable different types of binding activity and/or hydrolysing activity which likely contribute to their roles in protein import
+```
+
 ## OntoGPT Limitations
 
 ### Non-deterministic
 
 This relies on an existing LLM, and LLMs can be fickle in their responses.
 
 ### Coupled to OpenAI
 
-You will need an openai account. In theory any LLM can be used but in practice the parser is tuned for OpenAI
-
-
+You will need an OpenAI account to use their API. In theory any LLM can be used but in practice the parser is tuned for OpenAI's models.
 
-# Acknowledgements
+## Acknowledgements
 
-This [cookiecutter](https://cookiecutter.readthedocs.io/en/stable/README.html) project was developed from the [sphintoxetry-cookiecutter](https://github.com/hrshdhgd/sphintoxetry-cookiecutter) template and will be kept up-to-date using [cruft](https://cruft.github.io/cruft/).
+We gratefully acknowledge [Bosch Research](https://www.bosch.com/research) for their support of this research project.
```

