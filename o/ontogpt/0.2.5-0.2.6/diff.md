# Comparing `tmp/ontogpt-0.2.5.tar.gz` & `tmp/ontogpt-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ontogpt-0.2.5.tar", max compression
+gzip compressed data, was "ontogpt-0.2.6.tar", max compression
```

## Comparing `ontogpt-0.2.5.tar` & `ontogpt-0.2.6.tar`

### file list

```diff
@@ -1,110 +1,110 @@
--rw-r--r--   0        0        0     1485 2023-05-12 21:38:29.111857 ontogpt-0.2.5/LICENSE
--rw-r--r--   0        0        0    11651 2023-05-12 21:38:29.111857 ontogpt-0.2.5/README.md
--rw-r--r--   0        0        0     2356 2023-05-12 21:39:44.607110 ontogpt-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      219 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/__init__.py
--rw-r--r--   0        0        0    32676 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/cli.py
--rw-r--r--   0        0        0      244 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/clients/__init__.py
--rw-r--r--   0        0        0     6962 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/clients/openai_client.py
--rw-r--r--   0        0        0     2921 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/clients/pubmed_client.py
--rw-r--r--   0        0        0      617 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/clients/soup_client.py
--rw-r--r--   0        0        0     1122 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/clients/wikipedia_client.py
--rw-r--r--   0        0        0      684 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/conf/synonymizer-conf.yaml
--rw-r--r--   0        0        0       81 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/converters/__init__.py
--rw-r--r--   0        0        0     5289 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/converters/ontology_converter.py
--rw-r--r--   0        0        0       59 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/__init__.py
--rw-r--r--   0        0        0     3748 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/embedding_similarity_engine.py
--rw-r--r--   0        0        0    12456 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/enrichment.py
--rw-r--r--   0        0        0    19185 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/halo_engine.py
--rw-r--r--   0        0        0    24102 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/knowledge_engine.py
--rw-r--r--   0        0        0      752 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/resolver.py
--rw-r--r--   0        0        0    18520 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/spires_engine.py
--rw-r--r--   0        0        0      719 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/engines/synonym_engine.py
--rw-r--r--   0        0        0       70 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/evaluation/__init__.py
--rw-r--r--   0        0        0        0 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/evaluation/ctd/__init__.py
--rw-r--r--   0        0        0   425228 2023-05-12 21:38:29.159860 ontogpt-0.2.5/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
--rw-r--r--   0        0        0   409439 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
--rw-r--r--   0        0        0   413985 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ctd/database/synonyms.yaml
--rw-r--r--   0        0        0    10390 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ctd/eval_ctd.py
--rw-r--r--   0        0        0        0 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/drugmechdb/__init__.py
--rw-r--r--   0        0        0     2145 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
--rw-r--r--   0        0        0     2027 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
--rw-r--r--   0        0        0    10670 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
--rw-r--r--   0        0        0        0 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/enrichment/__init__.py
--rw-r--r--   0        0        0    13705 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/enrichment/eval_enrichment.py
--rw-r--r--   0        0        0     2950 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/evaluation_engine.py
--rw-r--r--   0        0        0     6164 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/go/eval_go.py
--rw-r--r--   0        0        0        0 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/hpoa/__init__.py
--rw-r--r--   0        0        0     8973 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/hpoa/eval_hpoa.py
--rw-r--r--   0        0        0     1191 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt
--rw-r--r--   0        0        0        0 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
--rw-r--r--   0        0        0     4791 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml
--rwxr-xr-x   0        0        0       95 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ibd/run.sh
--rwxr-xr-x   0        0        0       99 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/ibd/run.sh~
--rw-r--r--   0        0        0      586 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/evaluation/resolver.py
--rw-r--r--   0        0        0        0 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/io/__init__.py
--rw-r--r--   0        0        0      386 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/io/exporter.py
--rw-r--r--   0        0        0     4329 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/io/html_exporter.py
--rw-r--r--   0        0        0     3255 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/io/markdown_exporter.py
--rw-r--r--   0        0        0     2350 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/io/owl_exporter.py
--rw-r--r--   0        0        0     1440 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/io/rdf_exporter.py
--rw-r--r--   0        0        0      899 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/io/yaml_wrapper.py
--rw-r--r--   0        0        0        0 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/__init__.py
--rw-r--r--   0        0        0      159 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/enrichment/__init__.py
--rw-r--r--   0        0        0     1257 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2
--rw-r--r--   0        0        0     1016 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2
--rw-r--r--   0        0        0      993 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2
--rw-r--r--   0        0        0      994 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2
--rw-r--r--   0        0        0      995 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2
--rw-r--r--   0        0        0      560 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/prompts/similarity/connections.jinja2
--rw-r--r--   0        0        0       68 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/templates/__init__.py
--rw-r--r--   0        0        0      401 2023-05-12 21:38:29.163860 ontogpt-0.2.5/src/ontogpt/templates/all.yaml
--rw-r--r--   0        0        0     5942 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/biological_process.py
--rw-r--r--   0        0        0     2027 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/biological_process.yaml
--rw-r--r--   0        0        0     2938 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/class_enrichment.py
--rw-r--r--   0        0        0     3192 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/class_enrichment.yaml
--rw-r--r--   0        0        0     4519 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/composite_disease.yaml
--rw-r--r--   0        0        0     3593 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/core.py
--rw-r--r--   0        0        0     3098 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/core.yaml
--rw-r--r--   0        0        0     6210 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ctd.py
--rw-r--r--   0        0        0     6683 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ctd.yaml
--rw-r--r--   0        0        0     8825 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/diagnostic_procedure.py
--rw-r--r--   0        0        0     4774 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/diagnostic_procedure.yaml
--rw-r--r--   0        0        0     5466 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/drug.py
--rw-r--r--   0        0        0     1856 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/drug.yaml
--rw-r--r--   0        0        0     6092 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/environmental_sample.py
--rw-r--r--   0        0        0     2880 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/environmental_sample.yaml
--rw-r--r--   0        0        0     4709 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/gene_description_term.py
--rw-r--r--   0        0        0     1614 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/gene_description_term.yaml
--rw-r--r--   0        0        0     8172 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/gocam.py
--rw-r--r--   0        0        0     4871 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/gocam.yaml
--rw-r--r--   0        0        0     6813 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/halo.py
--rw-r--r--   0        0        0     2367 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/halo.yaml
--rw-r--r--   0        0        0     8165 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ibd.py
--rw-r--r--   0        0        0     4869 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ibd.yaml
--rw-r--r--   0        0        0     6097 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/mendelian_disease.py
--rw-r--r--   0        0        0     3130 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/mendelian_disease.yaml
--rw-r--r--   0        0        0     5384 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/metabolic_process.py
--rw-r--r--   0        0        0     1633 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/metabolic_process.yaml
--rw-r--r--   0        0        0     7156 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/metagenome_study.py
--rw-r--r--   0        0        0     3910 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/metagenome_study.yaml
--rw-r--r--   0        0        0     5072 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ontology_class.py
--rw-r--r--   0        0        0     2686 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ontology_class.yaml
--rw-r--r--   0        0        0     6136 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ontology_issue.py
--rw-r--r--   0        0        0     3383 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/ontology_issue.yaml
--rw-r--r--   0        0        0     4887 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/phenotype.py
--rw-r--r--   0        0        0     1532 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/phenotype.yaml
--rw-r--r--   0        0        0     7501 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/reaction.py
--rw-r--r--   0        0        0     3187 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/reaction.yaml
--rw-r--r--   0        0        0     7222 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/recipe.py
--rw-r--r--   0        0        0     5792 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/recipe.yaml
--rw-r--r--   0        0        0     7847 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/treatment.py
--rw-r--r--   0        0        0     4485 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/templates/treatment.yaml
--rw-r--r--   0        0        0        0 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/utils/__init__.py
--rw-r--r--   0        0        0     8788 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/utils/gene_set_utils.py
--rw-r--r--   0        0        0        0 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/webapp/__init__.py
--rw-r--r--   0        0        0      861 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/webapp/html/form.html
--rw-r--r--   0        0        0      201 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/webapp/html/results.html
--rw-r--r--   0        0        0      819 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/webapp/html/spindoctor/form.html
--rw-r--r--   0        0        0      205 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/webapp/html/spindoctor/results.html
--rw-r--r--   0        0        0     2767 2023-05-12 21:38:29.167860 ontogpt-0.2.5/src/ontogpt/webapp/main.py
--rw-r--r--   0        0        0    13948 1970-01-01 00:00:00.000000 ontogpt-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1485 2023-05-15 22:47:38.293546 ontogpt-0.2.6/LICENSE
+-rw-r--r--   0        0        0    13196 2023-05-15 22:47:38.293546 ontogpt-0.2.6/README.md
+-rw-r--r--   0        0        0     2417 2023-05-15 22:48:44.354069 ontogpt-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0      219 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/__init__.py
+-rw-r--r--   0        0        0    32676 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/cli.py
+-rw-r--r--   0        0        0      244 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/clients/__init__.py
+-rw-r--r--   0        0        0     6962 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/clients/openai_client.py
+-rw-r--r--   0        0        0     2921 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/clients/pubmed_client.py
+-rw-r--r--   0        0        0      617 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/clients/soup_client.py
+-rw-r--r--   0        0        0     1122 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/clients/wikipedia_client.py
+-rw-r--r--   0        0        0      684 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/conf/synonymizer-conf.yaml
+-rw-r--r--   0        0        0       81 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/converters/__init__.py
+-rw-r--r--   0        0        0     5289 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/converters/ontology_converter.py
+-rw-r--r--   0        0        0       59 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/__init__.py
+-rw-r--r--   0        0        0     3748 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/embedding_similarity_engine.py
+-rw-r--r--   0        0        0    12456 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/enrichment.py
+-rw-r--r--   0        0        0    19185 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/halo_engine.py
+-rw-r--r--   0        0        0    24196 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/knowledge_engine.py
+-rw-r--r--   0        0        0      752 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/resolver.py
+-rw-r--r--   0        0        0    18520 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/spires_engine.py
+-rw-r--r--   0        0        0      719 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/engines/synonym_engine.py
+-rw-r--r--   0        0        0       70 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/evaluation/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-15 22:47:38.337547 ontogpt-0.2.6/src/ontogpt/evaluation/ctd/__init__.py
+-rw-r--r--   0        0        0   425228 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz
+-rw-r--r--   0        0        0   409439 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz
+-rw-r--r--   0        0        0   413985 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ctd/database/synonyms.yaml
+-rw-r--r--   0        0        0    10390 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ctd/eval_ctd.py
+-rw-r--r--   0        0        0        0 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/drugmechdb/__init__.py
+-rw-r--r--   0        0        0     2145 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py
+-rw-r--r--   0        0        0     2027 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml
+-rw-r--r--   0        0        0    10670 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py
+-rw-r--r--   0        0        0        0 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/enrichment/__init__.py
+-rw-r--r--   0        0        0    13726 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/enrichment/eval_enrichment.py
+-rw-r--r--   0        0        0     2950 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/evaluation_engine.py
+-rw-r--r--   0        0        0     6164 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/go/eval_go.py
+-rw-r--r--   0        0        0        0 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/hpoa/__init__.py
+-rw-r--r--   0        0        0     8973 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/hpoa/eval_hpoa.py
+-rw-r--r--   0        0        0     1191 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt
+-rw-r--r--   0        0        0        0 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt~
+-rw-r--r--   0        0        0     4791 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml
+-rwxr-xr-x   0        0        0       95 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ibd/run.sh
+-rwxr-xr-x   0        0        0       99 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/ibd/run.sh~
+-rw-r--r--   0        0        0      586 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/evaluation/resolver.py
+-rw-r--r--   0        0        0        0 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/io/__init__.py
+-rw-r--r--   0        0        0      386 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/io/exporter.py
+-rw-r--r--   0        0        0     4329 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/io/html_exporter.py
+-rw-r--r--   0        0        0     3255 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/io/markdown_exporter.py
+-rw-r--r--   0        0        0     2350 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/io/owl_exporter.py
+-rw-r--r--   0        0        0     1440 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/io/rdf_exporter.py
+-rw-r--r--   0        0        0      899 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/io/yaml_wrapper.py
+-rw-r--r--   0        0        0        0 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/__init__.py
+-rw-r--r--   0        0        0      159 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/enrichment/__init__.py
+-rw-r--r--   0        0        0     1257 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2
+-rw-r--r--   0        0        0     1016 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2
+-rw-r--r--   0        0        0      993 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2
+-rw-r--r--   0        0        0      994 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2
+-rw-r--r--   0        0        0      995 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2
+-rw-r--r--   0        0        0      560 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/prompts/similarity/connections.jinja2
+-rw-r--r--   0        0        0     2354 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/streamlit/spindoctor.py
+-rw-r--r--   0        0        0       68 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/templates/__init__.py
+-rw-r--r--   0        0        0     5942 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/templates/biological_process.py
+-rw-r--r--   0        0        0     2027 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/templates/biological_process.yaml
+-rw-r--r--   0        0        0     2938 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/templates/class_enrichment.py
+-rw-r--r--   0        0        0     3192 2023-05-15 22:47:38.341547 ontogpt-0.2.6/src/ontogpt/templates/class_enrichment.yaml
+-rw-r--r--   0        0        0     4519 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/composite_disease.yaml
+-rw-r--r--   0        0        0     3593 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/core.py
+-rw-r--r--   0        0        0     3445 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/core.yaml
+-rw-r--r--   0        0        0     6210 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ctd.py
+-rw-r--r--   0        0        0     6683 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ctd.yaml
+-rw-r--r--   0        0        0     8878 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/diagnostic_procedure.py
+-rw-r--r--   0        0        0     4774 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/diagnostic_procedure.yaml
+-rw-r--r--   0        0        0     5466 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/drug.py
+-rw-r--r--   0        0        0     1856 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/drug.yaml
+-rw-r--r--   0        0        0     6092 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/environmental_sample.py
+-rw-r--r--   0        0        0     2900 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/environmental_sample.yaml
+-rw-r--r--   0        0        0     4709 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/gene_description_term.py
+-rw-r--r--   0        0        0     1614 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/gene_description_term.yaml
+-rw-r--r--   0        0        0     8172 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/gocam.py
+-rw-r--r--   0        0        0     4871 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/gocam.yaml
+-rw-r--r--   0        0        0     6813 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/halo.py
+-rw-r--r--   0        0        0     2367 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/halo.yaml
+-rw-r--r--   0        0        0     8165 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ibd.py
+-rw-r--r--   0        0        0     4869 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ibd.yaml
+-rw-r--r--   0        0        0     6097 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/mendelian_disease.py
+-rw-r--r--   0        0        0     3130 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/mendelian_disease.yaml
+-rw-r--r--   0        0        0     5384 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/metabolic_process.py
+-rw-r--r--   0        0        0     1633 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/metabolic_process.yaml
+-rw-r--r--   0        0        0     7156 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/metagenome_study.py
+-rw-r--r--   0        0        0     3910 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/metagenome_study.yaml
+-rw-r--r--   0        0        0     5072 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ontology_class.py
+-rw-r--r--   0        0        0     2686 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ontology_class.yaml
+-rw-r--r--   0        0        0     6136 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ontology_issue.py
+-rw-r--r--   0        0        0     3383 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/ontology_issue.yaml
+-rw-r--r--   0        0        0     4887 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/phenotype.py
+-rw-r--r--   0        0        0     1532 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/phenotype.yaml
+-rw-r--r--   0        0        0     7501 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/reaction.py
+-rw-r--r--   0        0        0     3187 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/reaction.yaml
+-rw-r--r--   0        0        0     7222 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/recipe.py
+-rw-r--r--   0        0        0     5792 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/recipe.yaml
+-rw-r--r--   0        0        0     7847 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/treatment.py
+-rw-r--r--   0        0        0     4485 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/templates/treatment.yaml
+-rw-r--r--   0        0        0        0 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/utils/__init__.py
+-rw-r--r--   0        0        0     8799 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/utils/gene_set_utils.py
+-rw-r--r--   0        0        0        0 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/webapp/__init__.py
+-rw-r--r--   0        0        0      861 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/webapp/html/form.html
+-rw-r--r--   0        0        0      201 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/webapp/html/results.html
+-rw-r--r--   0        0        0      819 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/webapp/html/spindoctor/form.html
+-rw-r--r--   0        0        0      205 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/webapp/html/spindoctor/results.html
+-rw-r--r--   0        0        0     2767 2023-05-15 22:47:38.345547 ontogpt-0.2.6/src/ontogpt/webapp/main.py
+-rw-r--r--   0        0        0    15658 1970-01-01 00:00:00.000000 ontogpt-0.2.6/PKG-INFO
```

### Comparing `ontogpt-0.2.5/LICENSE` & `ontogpt-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/README.md` & `ontogpt-0.2.6/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,64 +1,98 @@
-[![DOI](https://zenodo.org/badge/13996/monarch-initiative/ontogpt.svg)](https://zenodo.org/badge/latestdoi/13996/monarch-initiative/ontogpt)
-
 # OntoGPT
 
-Generation of Ontologies and Knowledge Bases using GPT
+[![DOI](https://zenodo.org/badge/13996/monarch-initiative/ontogpt.svg)](https://zenodo.org/badge/latestdoi/13996/monarch-initiative/ontogpt)
+![PyPI](https://img.shields.io/pypi/v/ontogpt)
+
+## Introduction
 
-A knowledge extraction tool that uses a large language model to extract semantic information from text.
+OntoGPT is a Python package for the generation of Ontologies and Knowledge Bases using GPT. It is a knowledge extraction tool that uses a Large Language Models (LLMs) to extract semantic information from text.
 
 This makes use of so-called *instruction prompts* in Large Language Models (LLMs) such as GPT-4.
 
-Currently there are two different pipelines implemented:
+Currently three different strategies for knowledge extraction have been implemented in the ontogpt package:
 
-- SPIRES: Structured Prompt Interrogation and Recursive Extraction of Semantics
-    - Zero-shot learning approach to extracting nested semantic structures from text
-    - Inputs: [LinkML](https://linkml.io/) schema + text
-    - Outputs: JSON, YAML, or RDF or OWL that conforms to the schema
-    - Uses text-davinci-003 or gpt-3.5-turbo (gtp-4 untested)
-- HALO: HAllucinating Latent Ontologies 
-    - Few-shot learning approach to generating/hallucinating a domain ontology given a few examples
-    - Uses code-davinci-002
-- SPINDOCTOR: Structured Prompt Interpolation of Narrative Descriptions Or Controlled Terms for Ontological Reporting
-    - Summarize gene set descriptions (pseudo gene-set enrichment)
-    - Uses text-davinci-003 or  gpt-3.5-turbo (gtp-4 untested)
+* SPIRES: *Structured Prompt Interrogation and Recursive Extraction of Semantics*
+  * Zero-shot learning (ZSL) approach to extracting nested semantic structures from text
+  * This approach takes two inputs - 1) LinkML schema 2) free text, and outputs knowledge in a structure conformant with the supplied schema in JSON, YAML, RDF or OWL formats
+  * Uses text-davinci-003 or gpt-3.5-turbo (gpt-4 untested)
+* HALO: *HAllucinating Latent Ontologies*
+  * Few-shot learning approach to generating/hallucinating a domain ontology given a few examples
+  * Uses code-davinci-002
+* SPINDOCTOR: *Structured Prompt Interpolation of Narrative Descriptions Or Controlled Terms for Ontological Reporting*
+  * Summarize gene set descriptions (pseudo gene-set enrichment)
+  * Uses text-davinci-003 or gpt-3.5-turbo (gpt-4 untested)
 
-SPIRES is described further in: Caufield JH, Hegde H, Emonet V, Harris NL, Joachimiak MP, Matentzoglu N, et al. Structured prompt interrogation and recursive extraction of semantics (SPIRES): A method for populating knowledge bases using zero-shot learning. arXiv [cs.AI]. 2023. http://arxiv.org/abs/2304.02711
 
-## Citation
+## Pre-requisites
+
+* Python 3.9+
+* OpenAI account
+* Optionally, [BioPortal](https://bioportal.bioontology.org/) account (for grounding)
+
+You will need to set both API keys using the [Ontology Access Kit](https://github.com/INCATools/ontology-access-kit)
+
+```bash
+poetry run runoak set-apikey -e openai <your openai api key>
+poetry run runoak set-apikey -e bioportal <your bioportal api key>
+```
+
+## Setup
+
+For feature development and contributing to the package:
+
+```bash
+git clone https://github.com/monarch-initiative/ontogpt.git
+cd ~/path/to/ontogpt
+poetry install
+```
 
- - https://arxiv.org/abs/2304.02711
+To simply start using the package in your workspace:
 
-## SPIRES: Usage
+```bash
+pip install ontogpt
+```
+
+## Examples
 
-Given a short text `abstract.txt` with content such as:
+### Strategy 1: Knowledge extraction using SPIRES
 
-   > The cGAS/STING-mediated DNA-sensing signaling pathway is crucial
-   for interferon (IFN) production and host antiviral
-   responses
-   > 
-   > ...
-   > [snip] 
-   > ...
-   > 
-   > The underlying mechanism was the
-   interaction of US3 with β-catenin and its hyperphosphorylation of
-   β-catenin at Thr556 to block its nuclear translocation
-   > ...
-   > ...
+#### Input
 
-(see [full input](tests/input/cases/gocam-betacat.txt))
+Consider some text from one of the input files being used in the ontogpt test suite. You can find the text file [here](tests/input/cases/gocam-betacat.txt). You can download the raw file from the GitHub link to that input text file, or copy its contents over into another file, say, `abstract.txt`. An excerpt 
 
-We can extract this into the [GO pathway datamodel](src/ontogpt/templates/gocam.yaml):
+  > The cGAS/STING-mediated DNA-sensing signaling pathway is crucial
+  for interferon (IFN) production and host antiviral
+  responses
+  > 
+  > ...
+  > [snip] 
+  > ...
+  > 
+  > The underlying mechanism was the
+  interaction of US3 with β-catenin and its hyperphosphorylation of
+  β-catenin at Thr556 to block its nuclear translocation
+  > ...
+  > ...
+
+We can extract knowledge from the above text this into the [GO pathway datamodel](src/ontogpt/templates/gocam.yaml) by running the following command:
+
+#### Command
 
 ```bash
-ontogpt extract -t gocam.GoCamAnnotations -i abstract.txt
+ontogpt extract -t gocam.GoCamAnnotations -i ~/path/to/abstract.txt
 ```
 
-Giving schema-compliant yaml such as:
+Note: The value accepted by the `-t` / `--template` argument is the base name of one of the LinkML schema / data model which can be found in the [templates](src/ontogpt/templates/) folder.
+
+#### Output
+
+The output returned from the above command is knowledge can be optionally redirected into an output file using the `-o` / `--output`.
+
+The following is a small part of what the larger schema-compliant output looks like:
 
 ```yaml
 genes:
 - HGNC:2514
 - HGNC:21367
 - HGNC:27962
 - US3
@@ -74,216 +108,198 @@
 - gene: HGNC:2514
   molecular_activity: Transcription
 - gene: HGNC:21367
   molecular_activity: Production
 ...
 ```
 
-See [full output](tests/output/gocam-betacat.yaml)
-
-Note in the above the grounding is very preliminary and can be improved. Ungrounded NamedEntities appear as text.
-
-## How it works
+#### Working Mechanism
 
 1. You provide an arbitrary data model, describing the structure you want to extract text into
-    - this can be nested (but see limitations below)
-2. Provide your preferred annotations for grounding NamedEntity fields
+    - This can be nested (but see limitations below)
+2. Provide your preferred annotations for grounding `NamedEntity` fields
 3. OntoGPT will:
-    - generate a prompt
-    - feed the prompt to a language model (currently OpenAI GPT models)
-    - parse the results into a dictionary structure
-    - ground the results using a preferred annotator
+    - Generate a prompt
+    - Feed the prompt to a language model (currently OpenAI GPT models)
+    - Parse the results into a dictionary structure
+    - Ground the results using a preferred annotator
 
-## Pre-requisites
+## Strategy 2: HALO
 
-- Python 3.9+
-- An OpenAI account
-- A [BioPortal](https://bioportal.bioontology.org/) account (optional, for grounding)
+*Documentation to come*
 
-You will need to set both API keys using the [Ontology Access Kit](https://github.com/INCATools/ontology-access-kit) (OAK, a dependency of this project)
+## Strategy 3: Gene Enrichment using SPINDOCTOR
 
-```
-poetry run runoak set-apikey -e openai <your openai api key>
-poetry run runoak set-apikey -e bioportal <your bioportal api key>
-```
+Given a set of genes, OntoGPT can find similarities among them.
 
-## How to define your own extraction data model
+Ex.:
 
-### Step 1: Define a schema
+```bash
+ontogpt enrichment -U tests/input/genesets/sensory-ataxia.yaml
+```
 
-See [src/ontogpt/templates/](src/ontogpt/templates/) for examples.
+The default is to use ontological gene function synopses (via the Alliance API).
 
-Define a schema (using a subset of [LinkML](https://linkml.io)) that describes the structure you want to extract from your text.
+* To use narrative/RefSeq summaries, use the `--no-ontological-synopses` flag
+* To run without any gene descriptions, use the `--no-annotations` flag
 
-```yaml
-classes:
-  MendelianDisease:
-    attributes:
-      name:
-        description: the name of the disease
-        examples:
-          - value: peroxisome biogenesis disorder
-        identifier: true  ## needed for inlining
-      description:
-        description: a description of the disease
-        examples:
-          - value: >-
-             Peroxisome biogenesis disorders, Zellweger syndrome spectrum (PBD-ZSS) is a group of autosomal recessive disorders affecting the formation of functional peroxisomes, characterized by sensorineural hearing loss, pigmentary retinal degeneration, multiple organ dysfunction and psychomotor impairment
-      synonyms:
-        multivalued: true
-        examples:
-          - value: Zellweger syndrome spectrum
-          - value: PBD-ZSS
-      subclass_of:
-        multivalued: true
-        range: MendelianDisease
-        examples:
-          - value: lysosomal disease
-          - value: autosomal recessive disorder
-      symptoms:
-        range: Symptom
-        multivalued: true
-        examples:
-          - value: sensorineural hearing loss
-          - value: pigmentary retinal degeneration
-      inheritance:
-        range: Inheritance
-        examples:
-          - value: autosomal recessive
-      genes:
-        range: Gene
-        multivalued: true
-        examples:
-          - value: PEX1
-          - value: PEX2
-          - value: PEX3
+## Features
 
-  Gene:
-    is_a: NamedThing
-    id_prefixes:
-      - HGNC
-    annotations:
-      annotators: gilda:, bioportal:hgnc-nr
+### Define your own extraction model using LinkML
 
-  Symptom:
-    is_a: NamedThing
-    id_prefixes:
-      - HP
-    annotations:
-      annotators: sqlite:obo:hp
+There are a number of pre-defined LinkML data models already developed here - [src/ontogpt/templates/](src/ontogpt/templates/) which you can use as reference when creating your own data models.
 
-  Inheritance:
-    is_a: NamedThing
-    annotations:
-      annotators: sqlite:obo:hp
-```
+Define a schema (using a subset of [LinkML](https://linkml.io)) that describes the structure in which you want to extract knowledge from your text.
 
-- the schema is defined in LinkML
-- prompt hints can be specified using the `prompt` annotation (otherwise description is used)
-- multivalued fields are supported
-- the default range is string - these are not grounded. E.g. disease name, synonyms
-- define a class for each NamedEntity
-- for any NamedEntity, you can specify a preferred annotator using the `annotators` annotation
+<details>
+  <summary>example custom linkml data model</summary>
+  ```yaml
+  classes:
+    MendelianDisease:
+      attributes:
+        name:
+          description: the name of the disease
+          examples:
+            - value: peroxisome biogenesis disorder
+          identifier: true  ## needed for inlining
+        description:
+          description: a description of the disease
+          examples:
+            - value: >-
+              Peroxisome biogenesis disorders, Zellweger syndrome spectrum (PBD-ZSS) is a group of autosomal recessive disorders affecting the formation of functional peroxisomes, characterized by sensorineural hearing loss, pigmentary retinal degeneration, multiple organ dysfunction and psychomotor impairment
+        synonyms:
+          multivalued: true
+          examples:
+            - value: Zellweger syndrome spectrum
+            - value: PBD-ZSS
+        subclass_of:
+          multivalued: true
+          range: MendelianDisease
+          examples:
+            - value: lysosomal disease
+            - value: autosomal recessive disorder
+        symptoms:
+          range: Symptom
+          multivalued: true
+          examples:
+            - value: sensorineural hearing loss
+            - value: pigmentary retinal degeneration
+        inheritance:
+          range: Inheritance
+          examples:
+            - value: autosomal recessive
+        genes:
+          range: Gene
+          multivalued: true
+          examples:
+            - value: PEX1
+            - value: PEX2
+            - value: PEX3
+
+    Gene:
+      is_a: NamedThing
+      id_prefixes:
+        - HGNC
+      annotations:
+        annotators: gilda:, bioportal:hgnc-nr
+
+    Symptom:
+      is_a: NamedThing
+      id_prefixes:
+        - HP
+      annotations:
+        annotators: sqlite:obo:hp
+
+    Inheritance:
+      is_a: NamedThing
+      annotations:
+        annotators: sqlite:obo:hp
+    ```
+</details>
+
+* Prompt hints can be specified using the `prompt` annotation (otherwise description is used)
+* Multivalued fields are supported
+* The default range is string — these are not grounded. Ex.: disease name, synonyms
+* Define a class for each `NamedEntity`
+* For any `NamedEntity`, you can specify a preferred annotator using the `annotators` annotation
 
 We recommend following an established schema like [BioLink Model](https://github.com/biolink/biolink-model), but you can define your own.
 
-### Step 2: Compile the schema
-
-Place the schema YAML in the directory `src/ontogpt/templates/`.
-
-Run the `make` command at the top level. This will compile the schema to Python (Pydantic classes).
+Next step is to compile the schema. For that, you should place the schema YAML in the directory [src/ontogpt/templates/](src/ontogpt/templates/). Then, run the `make` command at the top level. This will compile the schema to Python (Pydantic classes).
 
-### Step 3: Run the command line
+Once you have defined your own schema / data model and placed in the correct directory, you can run the `extract` command. 
 
-e.g.
+Ex.:
 
 ```
 ontogpt extract -t mendelian_disease.MendelianDisease -i marfan-wikipedia.txt
 ```
 
-## Web Application
-
-There is a bare bones web application for running OntoGPT and viewing results.
-
-Install the required dependencies first with the following command:
-```
-poetry install -E web
-```
-
-Then run the following command to start the web application:
-
-```
-poetry run web-ontogpt
-```
-
-Note that the agent running uvicorn must have the API key set, so for obvious reasons
-don't host this publicly without authentication, unless you want your credits drained.
-
-## Features
-
 ### Multiple levels of nesting
 
 Currently no more than two levels of nesting are recommended.
 
 If a field has a range which is itself a class and not a primitive, it will attempt to nest.
 
-E.g. the gocam schema has an attribute:
+Ex. the `gocam` schema has an attribute:
 
 ```yaml
   attributes:
       ...
       gene_functions:
         description: semicolon-separated list of gene to molecular activity relationships
         multivalued: true
         range: GeneMolecularActivityRelationship
 ```
 
-Because `GeneMolecularActivityRelationship` is *inlined* it will nest
+The range `GeneMolecularActivityRelationship` has been specified *inline*, so it will nest.
 
 The generated prompt is:
 
-`gene_functions : <semicolon-separated list of gene to molecular activities relationships>`
+```bash
+gene_functions : <semicolon-separated list of gene to molecular activities relationships>
+```
 
 The output of this is then passed through further SPIRES iterations.
 
 ### Text length limit
 
 Currently SPIRES must use text-davinci-003, which has a total 4k token limit (prompt + completion).
 
-You can pass in a parameter to split the text into chunks, results will be recombined automatically,
-but more experiments need to be done to determined how reliable this is.
+You can pass in a parameter to split the text into chunks. Returned results will be recombined automatically, but more experiments need to be done to determined how reliable this is.
+
+### Schema tips
 
-## Schema Tips
+It helps to have an understanding of the [LinkML](https://linkml.io) schema language, but it should be possible to define your own schemas using the examples in [src/ontogpt/templates](src/ontogpt/templates/) as a guide.
 
-It helps to have an understanding of the [LinkML](https://linkml.io) schema language, but it should be possible
-to define your own schemas using the examples as a guide.
+OntoGPT-specific extensions are specified as *annotations*.
 
-OntoGPT-specific extensions are specified as *annotations*
+You can specify a set of annotators for a field using the `annotators` annotation.
 
-You can specify a set of annotators for a field using the `annotators` annotation
+Ex.:
 
 ```yaml
   Gene:
     is_a: NamedThing
     id_prefixes:
       - HGNC
     annotations:
       annotators: gilda:, bioportal:hgnc-nr, obo:pr
 ```
 
 The annotators are applied in order.
 
 Additionally, when performing grounding, the following measures can be taken to improve accuracy:
 
-- specify the valid set of ID prefixes using `id_prefixes`
-- some vocabularies have structural IDs that are amenable to regexes, you can specify these using `pattern`
-- you can make use of `values_from` slot to specify a [Dynamic Value Set](https://linkml.io/linkml/schemas/enums.html#dynamic-enums)
-    - for example, you can constrain the set of valid locations for a gene product to be subclasses of `cellular_component` in GO or `cell` in CL.
+* Specify the valid set of ID prefixes using `id_prefixes`
+* Some vocabularies have structural IDs that are amenable to regexes, you can specify these using `pattern`
+* You can make use of `values_from` slot to specify a [Dynamic Value Set](https://linkml.io/linkml/schemas/enums.html#dynamic-enums)
+  * For example, you can constrain the set of valid locations for a gene product to be subclasses of `cellular_component` in GO or `cell` in CL
 
-For example:
+Ex.:
 
 ```yaml
 classes:
   ...
   GeneLocation:
     is_a: NamedEntity
     id_prefixes:
@@ -294,85 +310,87 @@
     slot_usage:
       id:
         values_from:
           - GOCellComponentType
           - CellType
 
 enums:
-
   GOCellComponentType:
     reachable_from:
       source_ontology: obo:go
       source_nodes:
         - GO:0005575 ## cellular_component
   CellType:
     reachable_from:
       source_ontology: obo:cl
       source_nodes:
         - CL:0000000 ## cell
-        
 ```
 
-## OWL Exports
+### OWL Exports
 
 The `extract` command will let you export the results as OWL axioms, utilizing [linkml-owl](https://linkml.io/linkml-owl) mappings in the schema.
 
-For example:
+Ex.:
 
 ```bash
 ontogpt extract -t recipe -i recipe-spaghetti.txt -o recipe-spaghetti.owl -O owl
 ```
 
-See [src/ontogpt/templates/recipe.yaml](src/ontogpt/templates/recipe.yaml) 
-for an example of a schema that uses linkml-owl mappings.
-
-See the Makefile for a full pipeline that involves using robot to extract a subset of FOODON
-and merge in the extracted results. This uses [recipe-scrapers](https://github.com/hhursev/recipe-scrapers)
+[src/ontogpt/templates/recipe.yaml](src/ontogpt/templates/recipe.yaml) is an example schema that uses linkml-owl mappings.
 
-Example output OWL here:
+See the [Makefile](Makefile) for a full pipeline that involves using robot to extract a subset of FOODON
+and merge in the extracted results. This uses [recipe-scrapers](https://github.com/hhursev/recipe-scrapers).
 
-- [recipe-all-merged.owl](https://github.com/monarch-initiative/ontogpt/blob/main/tests/output/owl/merged/recipe-all-merged.owl)
+OWL output: [recipe-all-merged.owl](tests/output/owl/merged/recipe-all-merged.owl)
 
-Example classification:
+Classification:
 
 <img width="1329" alt="image" src="https://user-images.githubusercontent.com/50745/230427663-20d845e9-f1d5-490e-b1ad-cdccdd0dca70.png">
 
+## Web Application Setup
 
-Contributions on recipes to test welcome from anyone! Just make a PR [here](https://github.com/monarch-initiative/ontogpt/blob/main/tests/input/recipe-urls.csv). See [this list](https://github.com/hhursev/recipe-scrapers) for accepted URLs
+There is a bare bones web application for running OntoGPT and viewing results.
 
+Install the required dependencies by running the following command:
 
-## HALO: Usage
+```bash
+poetry install -E web
+```
 
-TODO
+Then run this command to start the web application:
 
+```bash
+poetry run web-ontogpt
+```
 
+Note: The agent running uvicorn must have the API key set, so for obvious reasons don't host this publicly without authentication, unless you want your credits drained.
 
-## Gene Enrichment using SPINDOCTOR
+## OntoGPT Limitations
 
-Given a set of genes, OntoGPT can find similarities among them.
+1. Non-deterministic
+  * This relies on an existing LLM, and LLMs can be fickle in their responses
+2. Coupled to OpenAI
+  * You will need an OpenAI account to use their API. In theory any LLM can be used but in practice the parser is tuned for OpenAI's models
 
-Example:
+### SPINDOCTOR web app
+
+To start:
 
 ```
-ontogpt  enrichment -U tests/input/genesets/sensory-ataxia.yaml
+poetry run streamlit run src/ontogpt/streamlit/spindoctor.py
 ```
 
-The default is to use ontological gene function synopses (via the Alliance API).
-
-To use narrative/RefSeq summaries, use the `--no-ontological-synopses` flag.
 
-To run without any gene descriptions, use the `--no-annotations` flag.
-
-
-## OntoGPT Limitations
+## Citation
 
-### Non-deterministic
+SPIRES is described further in: Caufield JH, Hegde H, Emonet V, Harris NL, Joachimiak MP, Matentzoglu N, et al. Structured prompt interrogation and recursive extraction of semantics (SPIRES): A method for populating knowledge bases using zero-shot learning. 
 
-This relies on an existing LLM, and LLMs can be fickle in their responses.
+arXiv publication: http://arxiv.org/abs/2304.02711
 
-### Coupled to OpenAI
+## Contributing
 
-You will need an OpenAI account to use their API. In theory any LLM can be used but in practice the parser is tuned for OpenAI's models.
+Contributions on recipes to test welcome from anyone! Just make a PR [here](https://github.com/monarch-initiative/ontogpt/blob/main/tests/input/recipe-urls.csv). See [this list](https://github.com/hhursev/recipe-scrapers) for accepted URLs
 
 ## Acknowledgements
 
 We gratefully acknowledge [Bosch Research](https://www.bosch.com/research) for their support of this research project.
```

### Comparing `ontogpt-0.2.5/pyproject.toml` & `ontogpt-0.2.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "ontogpt"
-version = "0.2.5"
+version = "0.2.6"
 description = "OntoGPT"
 authors = ["Chris Mungall <cjmungall@lbl.gov>"]
 license = "BSD-3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
-python = "^3.9"
+python = ">=3.9,<3.9.7 || >3.9.7,<4.0"
 click = "^8.1.3"
 importlib = "^1.0.4"
 openai = "^0.27.4"
-oaklib = "^0.5.4"
+oaklib = "^0.5.6"
 gilda = "^0.10.3"
 jsonlines = "^3.1.0"
 python-multipart = "^0.0.5"
 linkml-owl = "^0.2.7"
 beautifulsoup4 = "^4.11.1"
 eutils = "^0.6.0"
 class-resolver = "*"
@@ -41,14 +41,16 @@
 sphinx-click = {version = "^4.3.0", extras = ["docs"], optional = true}
 myst-parser = {version = "^0.18.1", extras = ["docs"], optional = true}
 recipe-scrapers = {version = "^14.35.0", extras = ["recipes"], optional = true}
 cachier = "^2.1.0"
 wikipedia-api = "^0.5.8"
 rustsim = "^0.1.8"
 requests-cache = "^1.0.1"
+streamlit = "^1.22.0"
+gpt4 = "^0.0.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
 setuptools = ">=65.5.0"
 tox = "^3.25.1"
 mkdocs-mermaid2-plugin = "^0.6.0"
```

### Comparing `ontogpt-0.2.5/src/ontogpt/cli.py` & `ontogpt-0.2.6/src/ontogpt/cli.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/clients/openai_client.py` & `ontogpt-0.2.6/src/ontogpt/clients/openai_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/clients/pubmed_client.py` & `ontogpt-0.2.6/src/ontogpt/clients/pubmed_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/clients/soup_client.py` & `ontogpt-0.2.6/src/ontogpt/clients/soup_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/clients/wikipedia_client.py` & `ontogpt-0.2.6/src/ontogpt/clients/wikipedia_client.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/conf/synonymizer-conf.yaml` & `ontogpt-0.2.6/src/ontogpt/conf/synonymizer-conf.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/converters/ontology_converter.py` & `ontogpt-0.2.6/src/ontogpt/converters/ontology_converter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/engines/embedding_similarity_engine.py` & `ontogpt-0.2.6/src/ontogpt/engines/embedding_similarity_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/engines/enrichment.py` & `ontogpt-0.2.6/src/ontogpt/engines/enrichment.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from pathlib import Path
 from typing import Dict, List, Optional, Tuple, Union
 
 from jinja2 import Template
 from oaklib import BasicOntologyInterface, get_adapter
 from pydantic import BaseModel
 
-from ontogpt.engines.knowledge_engine import KnowledgeEngine, MODEL_GPT_4
+from ontogpt.engines.knowledge_engine import MODEL_GPT_4, KnowledgeEngine
 from ontogpt.prompts.enrichment import DEFAULT_ENRICHMENT_PROMPT
 from ontogpt.templates.class_enrichment import ClassEnrichmentResult
 from ontogpt.templates.gene_description_term import GeneDescriptionTerm
 from ontogpt.utils.gene_set_utils import (
     ENTITY_ID,
     GENE_TUPLE,
     GeneSet,
```

### Comparing `ontogpt-0.2.5/src/ontogpt/engines/halo_engine.py` & `ontogpt-0.2.6/src/ontogpt/engines/halo_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/engines/knowledge_engine.py` & `ontogpt-0.2.6/src/ontogpt/engines/knowledge_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -161,14 +161,18 @@
         self.api_key = self._get_openai_api_key()
         openai.api_key = self.api_key
         if self.mappers is None:
             logging.info("Using mappers (currently hardcoded)")
             self.mappers = [get_adapter("translator:")]
         self.encoding = tiktoken.encoding_for_model(self.client.model)
 
+    def set_api_key(self, key: str):
+        self.api_key = key
+        openai.api_key = key
+
     def extract_from_text(
         self, text: str, cls: ClassDefinition = None, object: OBJECT = None
     ) -> ExtractionResult:
         raise NotImplementedError
 
     def extract_from_file(self, file: Union[str, Path, TextIO]) -> pydantic.BaseModel:
         """
```

### Comparing `ontogpt-0.2.5/src/ontogpt/engines/resolver.py` & `ontogpt-0.2.6/src/ontogpt/engines/resolver.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/engines/spires_engine.py` & `ontogpt-0.2.6/src/ontogpt/engines/spires_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/engines/synonym_engine.py` & `ontogpt-0.2.6/src/ontogpt/engines/synonym_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz` & `ontogpt-0.2.6/src/ontogpt/evaluation/ctd/database/CDR_TestSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz` & `ontogpt-0.2.6/src/ontogpt/evaluation/ctd/database/CDR_TrainSet.BioC.xml.gz`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/evaluation/ctd/database/synonyms.yaml` & `ontogpt-0.2.6/src/ontogpt/evaluation/ctd/database/synonyms.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/evaluation/ctd/eval_ctd.py` & `ontogpt-0.2.6/src/ontogpt/evaluation/ctd/eval_ctd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py` & `ontogpt-0.2.6/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml` & `ontogpt-0.2.6/src/ontogpt/evaluation/drugmechdb/datamodel/drugmechdb.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py` & `ontogpt-0.2.6/src/ontogpt/evaluation/drugmechdb/eval_drugmechdb.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/evaluation/enrichment/eval_enrichment.py` & `ontogpt-0.2.6/src/ontogpt/evaluation/enrichment/eval_enrichment.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,20 @@
 from oaklib.interfaces.obograph_interface import OboGraphInterface
 from oaklib.parsers.association_parser_factory import get_association_parser
 from pydantic import BaseModel
 from tiktoken import Encoding
 
 from ontogpt.engines import create_engine
 from ontogpt.engines.enrichment import ENTITY_ID, EnrichmentEngine, EnrichmentPayload
-from ontogpt.engines.knowledge_engine import MODEL_GPT_3_5_TURBO, MODEL_NAME, MODEL_TEXT_DAVINCI_003, MODEL_GPT_4
+from ontogpt.engines.knowledge_engine import (
+    MODEL_GPT_3_5_TURBO,
+    MODEL_GPT_4,
+    MODEL_NAME,
+    MODEL_TEXT_DAVINCI_003,
+)
 from ontogpt.evaluation.evaluation_engine import EvaluationEngine
 from ontogpt.templates.class_enrichment import ClassEnrichmentResult
 from ontogpt.utils.gene_set_utils import SYMBOL, GeneSet, drop_genes_from_gene_set, gene_info
 
 THIS_DIR = Path(__file__).parent
 DATABASE_DIR = Path(__file__).parent / "database"
```

### Comparing `ontogpt-0.2.5/src/ontogpt/evaluation/evaluation_engine.py` & `ontogpt-0.2.6/src/ontogpt/evaluation/evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/evaluation/go/eval_go.py` & `ontogpt-0.2.6/src/ontogpt/evaluation/go/eval_go.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/evaluation/hpoa/eval_hpoa.py` & `ontogpt-0.2.6/src/ontogpt/evaluation/hpoa/eval_hpoa.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt` & `ontogpt-0.2.6/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.txt`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml` & `ontogpt-0.2.6/src/ontogpt/evaluation/ibd/PMC6386158_fig2_legend.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/evaluation/resolver.py` & `ontogpt-0.2.6/src/ontogpt/evaluation/resolver.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/io/html_exporter.py` & `ontogpt-0.2.6/src/ontogpt/io/html_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/io/markdown_exporter.py` & `ontogpt-0.2.6/src/ontogpt/io/markdown_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/io/owl_exporter.py` & `ontogpt-0.2.6/src/ontogpt/io/owl_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/io/rdf_exporter.py` & `ontogpt-0.2.6/src/ontogpt/io/rdf_exporter.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/io/yaml_wrapper.py` & `ontogpt-0.2.6/src/ontogpt/io/yaml_wrapper.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2` & `ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2` & `ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2` & `ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_0.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2` & `ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_1.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2` & `ontogpt-0.2.6/src/ontogpt/prompts/enrichment/gene_set_summarization_with_p_values_2.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/prompts/similarity/connections.jinja2` & `ontogpt-0.2.6/src/ontogpt/prompts/similarity/connections.jinja2`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/biological_process.py` & `ontogpt-0.2.6/src/ontogpt/templates/biological_process.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/biological_process.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/biological_process.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/class_enrichment.py` & `ontogpt-0.2.6/src/ontogpt/templates/class_enrichment.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/class_enrichment.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/class_enrichment.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/composite_disease.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/composite_disease.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/core.py` & `ontogpt-0.2.6/src/ontogpt/templates/core.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/core.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/core.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 id: http://w3id.org/ontogpt/core
 name: core
 title: AI core Template
 license: https://creativecommons.org/publicdomain/zero/1.0/
 prefixes:
   linkml: https://w3id.org/linkml/
   core: http://w3id.org/ontogpt/core/
+  NCIT: http://purl.obolibrary.org/obo/NCIT_
+  RO: http://purl.obolibrary.org/obo/RO_
 description: Core upper level
 
 default_prefix: core
 default_range: string
 
 imports:
   - linkml:types
@@ -123,7 +125,20 @@
           The full text of the publication
 
   AnnotatorResult:
     attributes:
       subject_text:
       object_id:
       object_text:
+
+enums:
+
+  NullDataOptions:
+    permissible_values:
+      UNSPECIFIED_METHOD_OF_ADMINISTRATION:
+        meaning: NCIT:C149701
+      NOT_APPLICABLE:
+        meaning: NCIT:C18902
+        aliases:
+          - "not applicable"
+          - "N/A"
+      NOT_MENTIONED:
```

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/ctd.py` & `ontogpt-0.2.6/src/ontogpt/templates/ctd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/ctd.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/ctd.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/diagnostic_procedure.py` & `ontogpt-0.2.6/src/ontogpt/templates/diagnostic_procedure.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,180 +1,199 @@
 from __future__ import annotations
-from datetime import datetime, date
+
+from datetime import date, datetime
 from enum import Enum
-from typing import List, Dict, Optional, Any, Union, Literal
-from pydantic import BaseModel as BaseModel, Field
+from typing import Any, Dict, List, Literal, Optional, Union
+
 from linkml_runtime.linkml_model import Decimal
+from pydantic import BaseModel as BaseModel
+from pydantic import Field
 
 metamodel_version = "None"
 version = "None"
 
+
 class WeakRefShimBaseModel(BaseModel):
-   __slots__ = '__weakref__'
-    
-class ConfiguredBaseModel(WeakRefShimBaseModel,
-                validate_assignment = True, 
-                validate_all = True, 
-                underscore_attrs_are_private = True, 
-                extra = 'forbid', 
-                arbitrary_types_allowed = True):
-    pass                    
+    __slots__ = "__weakref__"
+
+
+class ConfiguredBaseModel(
+    WeakRefShimBaseModel,
+    validate_assignment=True,
+    validate_all=True,
+    underscore_attrs_are_private=True,
+    extra="forbid",
+    arbitrary_types_allowed=True,
+):
+    pass
 
 
 class ExtractionResult(ConfiguredBaseModel):
     """
     A result of extracting knowledge on text
     """
+
     input_id: Optional[str] = Field(None)
     input_title: Optional[str] = Field(None)
     input_text: Optional[str] = Field(None)
     raw_completion_output: Optional[str] = Field(None)
     prompt: Optional[str] = Field(None)
-    extracted_object: Optional[Any] = Field(None, description="""The complex objects extracted from the text""")
-    named_entities: Optional[List[Any]] = Field(default_factory=list, description="""Named entities extracted from the text""")
-    
+    extracted_object: Optional[Any] = Field(
+        None, description="""The complex objects extracted from the text"""
+    )
+    named_entities: Optional[List[Any]] = Field(
+        default_factory=list, description="""Named entities extracted from the text"""
+    )
 
 
 class NamedEntity(ConfiguredBaseModel):
-    
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
-    
 
 
 class DiagnosticProcedure(NamedEntity):
-    
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
-    
 
 
 class Phenotype(NamedEntity):
-    
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
-    
 
 
 class ClinicalAttribute(NamedEntity):
-    
     unit: Optional[str] = Field(None, description="""the unit used to measure the attribute""")
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
-    
 
 
 class Quality(NamedEntity):
-    
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
-    
 
 
 class Unit(NamedEntity):
-    
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
-    
 
 
 class CompoundExpression(ConfiguredBaseModel):
-    
     None
-    
 
 
 class Triple(CompoundExpression):
     """
     Abstract parent for Relation Extraction tasks
     """
+
     subject: Optional[str] = Field(None)
     predicate: Optional[str] = Field(None)
     object: Optional[str] = Field(None)
-    qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
-    subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""")
-    object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""")
-    
+    qualifier: Optional[str] = Field(
+        None, description="""A qualifier for the statements, e.g. \"NOT\" for negation"""
+    )
+    subject_qualifier: Optional[str] = Field(
+        None,
+        description="""An optional qualifier or modifier for the subject of the statement, e.g. \"high dose\" or \"intravenously administered\"""",
+    )
+    object_qualifier: Optional[str] = Field(
+        None,
+        description="""An optional qualifier or modifier for the object of the statement, e.g. \"severe\" or \"with additional complications\"""",
+    )
 
 
 class DiagnosticProceduretoPhenotypeAssociation(Triple):
     """
     A triple representing a relationship between a diagnostic procedure and an associated phenotype, e.g., \"blood pressure measurement\" is associated with \"high blood pressure\".
     """
-    subject: Optional[str] = Field(None, description="""A diagnostic procedure yielding a result, which in turn may be interpreted as a phenotype. Procedures include \"heart rate measurement\", \"blood pressure measurement\", \"oxygen saturation measurement\", etc. In practice, procedures may be named based on what they measure, with the \"measurement\" part left implicit.""")
+
+    subject: Optional[str] = Field(
+        None,
+        description="""A diagnostic procedure yielding a result, which in turn may be interpreted as a phenotype. Procedures include \"heart rate measurement\", \"blood pressure measurement\", \"oxygen saturation measurement\", etc. In practice, procedures may be named based on what they measure, with the \"measurement\" part left implicit.""",
+    )
     predicate: Optional[str] = Field(None, description="""The relationship type, e.g. RELATED_TO""")
-    object: Optional[List[str]] = Field(default_factory=list, description="""The observable physical or biochemical characteristics of a patient. Not equivalent to a disease state, but may contribute to a diagnosis.""")
-    qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
-    subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the procedure.""")
-    object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the phenotype.""")
-    
+    object: Optional[List[str]] = Field(
+        default_factory=list,
+        description="""The observable physical or biochemical characteristics of a patient. Not equivalent to a disease state, but may contribute to a diagnosis.""",
+    )
+    qualifier: Optional[str] = Field(
+        None, description="""A qualifier for the statements, e.g. \"NOT\" for negation"""
+    )
+    subject_qualifier: Optional[str] = Field(
+        None, description="""An optional qualifier or modifier for the procedure."""
+    )
+    object_qualifier: Optional[str] = Field(
+        None, description="""An optional qualifier or modifier for the phenotype."""
+    )
 
 
 class DiagnosticProceduretoAttributeAssociation(Triple):
     """
     A triple representing a relationship between a diagnostic procedure and a measured attribute, e.g., \"blood pressure measurement\" is associated with \"blood pressure\" (or in OBA, something like OBA:VT0000183, \"blood pressure trait\").
     """
-    subject: Optional[str] = Field(None, description="""A diagnostic procedure yielding a result, which in turn may be interpreted as a phenotype. Procedures include \"heart rate measurement\", \"blood pressure measurement\", \"oxygen saturation measurement\", etc. In practice, procedures may be named based on what they measure, with the \"measurement\" part left implicit.""")
+
+    subject: Optional[str] = Field(
+        None,
+        description="""A diagnostic procedure yielding a result, which in turn may be interpreted as a phenotype. Procedures include \"heart rate measurement\", \"blood pressure measurement\", \"oxygen saturation measurement\", etc. In practice, procedures may be named based on what they measure, with the \"measurement\" part left implicit.""",
+    )
     predicate: Optional[str] = Field(None, description="""The relationship type, e.g. RELATED_TO""")
-    object: Optional[List[str]] = Field(default_factory=list, description="""Any measurable clinical attribute.""")
-    qualifier: Optional[str] = Field(None, description="""A qualifier for the statements, e.g. \"NOT\" for negation""")
-    subject_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the procedure.""")
-    object_qualifier: Optional[str] = Field(None, description="""An optional qualifier or modifier for the phenotype.""")
-    
+    object: Optional[List[str]] = Field(
+        default_factory=list, description="""Any measurable clinical attribute."""
+    )
+    qualifier: Optional[str] = Field(
+        None, description="""A qualifier for the statements, e.g. \"NOT\" for negation"""
+    )
+    subject_qualifier: Optional[str] = Field(
+        None, description="""An optional qualifier or modifier for the procedure."""
+    )
+    object_qualifier: Optional[str] = Field(
+        None, description="""An optional qualifier or modifier for the phenotype."""
+    )
 
 
 class TextWithTriples(ConfiguredBaseModel):
-    
     publication: Optional[Publication] = Field(None)
     triples: Optional[List[Triple]] = Field(default_factory=list)
-    
 
 
 class RelationshipType(NamedEntity):
-    
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
-    
 
 
 class ProcedureToPhenotypePredicate(RelationshipType):
     """
     A predicate for procedure to phenotype relationships, defining \"this procedure is intended to provide support for/against this phenotype\".
     """
+
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
-    
 
 
 class ProcedureToAttributePredicate(RelationshipType):
     """
     A predicate for procedure to attribute relationships, defining \"this procedure is a measurement of this attribute\".
     """
+
     id: Optional[str] = Field(None, description="""A unique identifier for the named entity""")
     label: Optional[str] = Field(None, description="""The label (name) of the named thing""")
-    
 
 
 class Publication(ConfiguredBaseModel):
-    
     id: Optional[str] = Field(None, description="""The publication identifier""")
     title: Optional[str] = Field(None, description="""The title of the publication""")
     abstract: Optional[str] = Field(None, description="""The abstract of the publication""")
     combined_text: Optional[str] = Field(None)
     full_text: Optional[str] = Field(None, description="""The full text of the publication""")
-    
 
 
 class AnnotatorResult(ConfiguredBaseModel):
-    
     subject_text: Optional[str] = Field(None)
     object_id: Optional[str] = Field(None)
     object_text: Optional[str] = Field(None)
-    
-
 
 
 # Update forward refs
 # see https://pydantic-docs.helpmanual.io/usage/postponed_annotations/
 ExtractionResult.update_forward_refs()
 NamedEntity.update_forward_refs()
 DiagnosticProcedure.update_forward_refs()
@@ -188,8 +207,7 @@
 DiagnosticProceduretoAttributeAssociation.update_forward_refs()
 TextWithTriples.update_forward_refs()
 RelationshipType.update_forward_refs()
 ProcedureToPhenotypePredicate.update_forward_refs()
 ProcedureToAttributePredicate.update_forward_refs()
 Publication.update_forward_refs()
 AnnotatorResult.update_forward_refs()
-
```

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/diagnostic_procedure.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/diagnostic_procedure.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/drug.py` & `ontogpt-0.2.6/src/ontogpt/templates/drug.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/drug.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/drug.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/environmental_sample.py` & `ontogpt-0.2.6/src/ontogpt/templates/environmental_sample.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/environmental_sample.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/environmental_sample.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 imports:
   - linkml:types
   - core
 
 classes:
   Study:
+    tree_root: true
     attributes:
       location:
         description: the sites at which the study was conducted
         annotations:
           prompt: semicolon-separated list of sites at which the study was conducted
         range: Location
         multivalued: true
```

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/gene_description_term.py` & `ontogpt-0.2.6/src/ontogpt/templates/gene_description_term.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/gene_description_term.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/gene_description_term.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/gocam.py` & `ontogpt-0.2.6/src/ontogpt/templates/gocam.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/gocam.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/gocam.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/halo.py` & `ontogpt-0.2.6/src/ontogpt/templates/halo.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/halo.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/halo.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/ibd.py` & `ontogpt-0.2.6/src/ontogpt/templates/ibd.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/ibd.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/ibd.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/mendelian_disease.py` & `ontogpt-0.2.6/src/ontogpt/templates/mendelian_disease.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/mendelian_disease.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/mendelian_disease.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/metabolic_process.py` & `ontogpt-0.2.6/src/ontogpt/templates/metabolic_process.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/metabolic_process.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/metabolic_process.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/metagenome_study.py` & `ontogpt-0.2.6/src/ontogpt/templates/metagenome_study.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/metagenome_study.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/metagenome_study.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/ontology_class.py` & `ontogpt-0.2.6/src/ontogpt/templates/ontology_class.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/ontology_class.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/ontology_class.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/ontology_issue.py` & `ontogpt-0.2.6/src/ontogpt/templates/ontology_issue.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/ontology_issue.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/ontology_issue.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/phenotype.py` & `ontogpt-0.2.6/src/ontogpt/templates/phenotype.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/phenotype.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/phenotype.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/reaction.py` & `ontogpt-0.2.6/src/ontogpt/templates/reaction.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/reaction.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/reaction.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/recipe.py` & `ontogpt-0.2.6/src/ontogpt/templates/recipe.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/recipe.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/recipe.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/treatment.py` & `ontogpt-0.2.6/src/ontogpt/templates/treatment.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/templates/treatment.yaml` & `ontogpt-0.2.6/src/ontogpt/templates/treatment.yaml`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/utils/gene_set_utils.py` & `ontogpt-0.2.6/src/ontogpt/utils/gene_set_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,17 +139,19 @@
             gene = Gene(id=id, symbol=sym)
             gene_set.gene_ids.append(id)
             gene_set.gene_symbols.append(sym)
             gene_set.gene_ids.append(id)
     return gene_set
 
 
-
 def load_gene_sets(
-    path: str, ontology_adapter: BasicOntologyInterface = None, strict=False, fill_missing=True,
+    path: str,
+    ontology_adapter: BasicOntologyInterface = None,
+    strict=False,
+    fill_missing=True,
 ) -> GeneSetCollection:
     """Load collection of gene sets from a folder.
 
     If ontology_adapter is provided, gene symbols will be converted to gene ids and vice versa.
     """
     gene_sets = []
     for input_path in glob.glob(f"{path}/*.yaml"):
```

### Comparing `ontogpt-0.2.5/src/ontogpt/webapp/html/form.html` & `ontogpt-0.2.6/src/ontogpt/webapp/html/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/webapp/html/spindoctor/form.html` & `ontogpt-0.2.6/src/ontogpt/webapp/html/spindoctor/form.html`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/src/ontogpt/webapp/main.py` & `ontogpt-0.2.6/src/ontogpt/webapp/main.py`

 * *Files identical despite different names*

### Comparing `ontogpt-0.2.5/PKG-INFO` & `ontogpt-0.2.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: ontogpt
-Version: 0.2.5
+Version: 0.2.6
 Summary: OntoGPT
 License: BSD-3
 Author: Chris Mungall
 Author-email: cjmungall@lbl.gov
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Provides-Extra: recipes
@@ -22,98 +22,134 @@
 Requires-Dist: bioc (>=2.0.post5,<3.0)
 Requires-Dist: cachier (>=2.1.0,<3.0.0)
 Requires-Dist: class-resolver
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Requires-Dist: eutils (>=0.6.0,<0.7.0)
 Requires-Dist: fastapi (>=0.88.0,<0.89.0) ; extra == "web"
 Requires-Dist: gilda (>=0.10.3,<0.11.0)
+Requires-Dist: gpt4 (>=0.0.1,<0.0.2)
 Requires-Dist: greenlet (!=2.0.2)
 Requires-Dist: httpx (>=0.23.3,<0.24.0)
 Requires-Dist: importlib (>=1.0.4,<2.0.0)
 Requires-Dist: inflect (>=6.0.2,<7.0.0)
 Requires-Dist: inflection (>=0.5.1,<0.6.0)
 Requires-Dist: jsonlines (>=3.1.0,<4.0.0)
 Requires-Dist: linkml (>=1.4.10,<2.0.0)
 Requires-Dist: linkml-owl (>=0.2.7,<0.3.0)
 Requires-Dist: linkml-runtime (>=1.4.9,<2.0.0)
 Requires-Dist: myst-parser[docs] (>=0.18.1,<0.19.0) ; extra == "docs"
 Requires-Dist: nlpcloud (>=1.0.39,<2.0.0)
-Requires-Dist: oaklib (>=0.5.4,<0.6.0)
+Requires-Dist: oaklib (>=0.5.6,<0.6.0)
 Requires-Dist: openai (>=0.27.4,<0.28.0)
 Requires-Dist: python-multipart (>=0.0.5,<0.0.6)
 Requires-Dist: recipe-scrapers[recipes] (>=14.35.0,<15.0.0) ; extra == "recipes"
 Requires-Dist: requests-cache (>=1.0.1,<2.0.0)
 Requires-Dist: rustsim (>=0.1.8,<0.2.0)
 Requires-Dist: sphinx-autodoc-typehints[docs] (>=1.19.4,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinx-click[docs] (>=4.3.0,<5.0.0) ; extra == "docs"
 Requires-Dist: sphinx-rtd-theme[docs] (>=1.0.0,<2.0.0) ; extra == "docs"
 Requires-Dist: sphinx[docs] (>=5.3.0,<6.0.0) ; extra == "docs"
+Requires-Dist: streamlit (>=1.22.0,<2.0.0)
 Requires-Dist: tiktoken (>=0.3.3,<0.4.0)
 Requires-Dist: uvicorn (>=0.20.0,<0.21.0) ; extra == "web"
 Requires-Dist: wikipedia (>=1.4.0,<2.0.0)
 Requires-Dist: wikipedia-api (>=0.5.8,<0.6.0)
 Description-Content-Type: text/markdown
 
-[![DOI](https://zenodo.org/badge/13996/monarch-initiative/ontogpt.svg)](https://zenodo.org/badge/latestdoi/13996/monarch-initiative/ontogpt)
-
 # OntoGPT
 
-Generation of Ontologies and Knowledge Bases using GPT
+[![DOI](https://zenodo.org/badge/13996/monarch-initiative/ontogpt.svg)](https://zenodo.org/badge/latestdoi/13996/monarch-initiative/ontogpt)
+![PyPI](https://img.shields.io/pypi/v/ontogpt)
+
+## Introduction
 
-A knowledge extraction tool that uses a large language model to extract semantic information from text.
+OntoGPT is a Python package for the generation of Ontologies and Knowledge Bases using GPT. It is a knowledge extraction tool that uses a Large Language Models (LLMs) to extract semantic information from text.
 
 This makes use of so-called *instruction prompts* in Large Language Models (LLMs) such as GPT-4.
 
-Currently there are two different pipelines implemented:
+Currently three different strategies for knowledge extraction have been implemented in the ontogpt package:
 
-- SPIRES: Structured Prompt Interrogation and Recursive Extraction of Semantics
-    - Zero-shot learning approach to extracting nested semantic structures from text
-    - Inputs: [LinkML](https://linkml.io/) schema + text
-    - Outputs: JSON, YAML, or RDF or OWL that conforms to the schema
-    - Uses text-davinci-003 or gpt-3.5-turbo (gtp-4 untested)
-- HALO: HAllucinating Latent Ontologies 
-    - Few-shot learning approach to generating/hallucinating a domain ontology given a few examples
-    - Uses code-davinci-002
-- SPINDOCTOR: Structured Prompt Interpolation of Narrative Descriptions Or Controlled Terms for Ontological Reporting
-    - Summarize gene set descriptions (pseudo gene-set enrichment)
-    - Uses text-davinci-003 or  gpt-3.5-turbo (gtp-4 untested)
+* SPIRES: *Structured Prompt Interrogation and Recursive Extraction of Semantics*
+  * Zero-shot learning (ZSL) approach to extracting nested semantic structures from text
+  * This approach takes two inputs - 1) LinkML schema 2) free text, and outputs knowledge in a structure conformant with the supplied schema in JSON, YAML, RDF or OWL formats
+  * Uses text-davinci-003 or gpt-3.5-turbo (gpt-4 untested)
+* HALO: *HAllucinating Latent Ontologies*
+  * Few-shot learning approach to generating/hallucinating a domain ontology given a few examples
+  * Uses code-davinci-002
+* SPINDOCTOR: *Structured Prompt Interpolation of Narrative Descriptions Or Controlled Terms for Ontological Reporting*
+  * Summarize gene set descriptions (pseudo gene-set enrichment)
+  * Uses text-davinci-003 or gpt-3.5-turbo (gpt-4 untested)
 
-SPIRES is described further in: Caufield JH, Hegde H, Emonet V, Harris NL, Joachimiak MP, Matentzoglu N, et al. Structured prompt interrogation and recursive extraction of semantics (SPIRES): A method for populating knowledge bases using zero-shot learning. arXiv [cs.AI]. 2023. http://arxiv.org/abs/2304.02711
 
-## Citation
+## Pre-requisites
+
+* Python 3.9+
+* OpenAI account
+* Optionally, [BioPortal](https://bioportal.bioontology.org/) account (for grounding)
+
+You will need to set both API keys using the [Ontology Access Kit](https://github.com/INCATools/ontology-access-kit)
+
+```bash
+poetry run runoak set-apikey -e openai <your openai api key>
+poetry run runoak set-apikey -e bioportal <your bioportal api key>
+```
+
+## Setup
+
+For feature development and contributing to the package:
+
+```bash
+git clone https://github.com/monarch-initiative/ontogpt.git
+cd ~/path/to/ontogpt
+poetry install
+```
 
- - https://arxiv.org/abs/2304.02711
+To simply start using the package in your workspace:
 
-## SPIRES: Usage
+```bash
+pip install ontogpt
+```
+
+## Examples
 
-Given a short text `abstract.txt` with content such as:
+### Strategy 1: Knowledge extraction using SPIRES
 
-   > The cGAS/STING-mediated DNA-sensing signaling pathway is crucial
-   for interferon (IFN) production and host antiviral
-   responses
-   > 
-   > ...
-   > [snip] 
-   > ...
-   > 
-   > The underlying mechanism was the
-   interaction of US3 with β-catenin and its hyperphosphorylation of
-   β-catenin at Thr556 to block its nuclear translocation
-   > ...
-   > ...
+#### Input
 
-(see [full input](tests/input/cases/gocam-betacat.txt))
+Consider some text from one of the input files being used in the ontogpt test suite. You can find the text file [here](tests/input/cases/gocam-betacat.txt). You can download the raw file from the GitHub link to that input text file, or copy its contents over into another file, say, `abstract.txt`. An excerpt 
 
-We can extract this into the [GO pathway datamodel](src/ontogpt/templates/gocam.yaml):
+  > The cGAS/STING-mediated DNA-sensing signaling pathway is crucial
+  for interferon (IFN) production and host antiviral
+  responses
+  > 
+  > ...
+  > [snip] 
+  > ...
+  > 
+  > The underlying mechanism was the
+  interaction of US3 with β-catenin and its hyperphosphorylation of
+  β-catenin at Thr556 to block its nuclear translocation
+  > ...
+  > ...
+
+We can extract knowledge from the above text this into the [GO pathway datamodel](src/ontogpt/templates/gocam.yaml) by running the following command:
+
+#### Command
 
 ```bash
-ontogpt extract -t gocam.GoCamAnnotations -i abstract.txt
+ontogpt extract -t gocam.GoCamAnnotations -i ~/path/to/abstract.txt
 ```
 
-Giving schema-compliant yaml such as:
+Note: The value accepted by the `-t` / `--template` argument is the base name of one of the LinkML schema / data model which can be found in the [templates](src/ontogpt/templates/) folder.
+
+#### Output
+
+The output returned from the above command is knowledge can be optionally redirected into an output file using the `-o` / `--output`.
+
+The following is a small part of what the larger schema-compliant output looks like:
 
 ```yaml
 genes:
 - HGNC:2514
 - HGNC:21367
 - HGNC:27962
 - US3
@@ -129,216 +165,198 @@
 - gene: HGNC:2514
   molecular_activity: Transcription
 - gene: HGNC:21367
   molecular_activity: Production
 ...
 ```
 
-See [full output](tests/output/gocam-betacat.yaml)
-
-Note in the above the grounding is very preliminary and can be improved. Ungrounded NamedEntities appear as text.
-
-## How it works
+#### Working Mechanism
 
 1. You provide an arbitrary data model, describing the structure you want to extract text into
-    - this can be nested (but see limitations below)
-2. Provide your preferred annotations for grounding NamedEntity fields
+    - This can be nested (but see limitations below)
+2. Provide your preferred annotations for grounding `NamedEntity` fields
 3. OntoGPT will:
-    - generate a prompt
-    - feed the prompt to a language model (currently OpenAI GPT models)
-    - parse the results into a dictionary structure
-    - ground the results using a preferred annotator
+    - Generate a prompt
+    - Feed the prompt to a language model (currently OpenAI GPT models)
+    - Parse the results into a dictionary structure
+    - Ground the results using a preferred annotator
 
-## Pre-requisites
+## Strategy 2: HALO
 
-- Python 3.9+
-- An OpenAI account
-- A [BioPortal](https://bioportal.bioontology.org/) account (optional, for grounding)
+*Documentation to come*
 
-You will need to set both API keys using the [Ontology Access Kit](https://github.com/INCATools/ontology-access-kit) (OAK, a dependency of this project)
+## Strategy 3: Gene Enrichment using SPINDOCTOR
 
-```
-poetry run runoak set-apikey -e openai <your openai api key>
-poetry run runoak set-apikey -e bioportal <your bioportal api key>
-```
+Given a set of genes, OntoGPT can find similarities among them.
 
-## How to define your own extraction data model
+Ex.:
 
-### Step 1: Define a schema
+```bash
+ontogpt enrichment -U tests/input/genesets/sensory-ataxia.yaml
+```
 
-See [src/ontogpt/templates/](src/ontogpt/templates/) for examples.
+The default is to use ontological gene function synopses (via the Alliance API).
 
-Define a schema (using a subset of [LinkML](https://linkml.io)) that describes the structure you want to extract from your text.
+* To use narrative/RefSeq summaries, use the `--no-ontological-synopses` flag
+* To run without any gene descriptions, use the `--no-annotations` flag
 
-```yaml
-classes:
-  MendelianDisease:
-    attributes:
-      name:
-        description: the name of the disease
-        examples:
-          - value: peroxisome biogenesis disorder
-        identifier: true  ## needed for inlining
-      description:
-        description: a description of the disease
-        examples:
-          - value: >-
-             Peroxisome biogenesis disorders, Zellweger syndrome spectrum (PBD-ZSS) is a group of autosomal recessive disorders affecting the formation of functional peroxisomes, characterized by sensorineural hearing loss, pigmentary retinal degeneration, multiple organ dysfunction and psychomotor impairment
-      synonyms:
-        multivalued: true
-        examples:
-          - value: Zellweger syndrome spectrum
-          - value: PBD-ZSS
-      subclass_of:
-        multivalued: true
-        range: MendelianDisease
-        examples:
-          - value: lysosomal disease
-          - value: autosomal recessive disorder
-      symptoms:
-        range: Symptom
-        multivalued: true
-        examples:
-          - value: sensorineural hearing loss
-          - value: pigmentary retinal degeneration
-      inheritance:
-        range: Inheritance
-        examples:
-          - value: autosomal recessive
-      genes:
-        range: Gene
-        multivalued: true
-        examples:
-          - value: PEX1
-          - value: PEX2
-          - value: PEX3
+## Features
 
-  Gene:
-    is_a: NamedThing
-    id_prefixes:
-      - HGNC
-    annotations:
-      annotators: gilda:, bioportal:hgnc-nr
+### Define your own extraction model using LinkML
 
-  Symptom:
-    is_a: NamedThing
-    id_prefixes:
-      - HP
-    annotations:
-      annotators: sqlite:obo:hp
+There are a number of pre-defined LinkML data models already developed here - [src/ontogpt/templates/](src/ontogpt/templates/) which you can use as reference when creating your own data models.
 
-  Inheritance:
-    is_a: NamedThing
-    annotations:
-      annotators: sqlite:obo:hp
-```
+Define a schema (using a subset of [LinkML](https://linkml.io)) that describes the structure in which you want to extract knowledge from your text.
 
-- the schema is defined in LinkML
-- prompt hints can be specified using the `prompt` annotation (otherwise description is used)
-- multivalued fields are supported
-- the default range is string - these are not grounded. E.g. disease name, synonyms
-- define a class for each NamedEntity
-- for any NamedEntity, you can specify a preferred annotator using the `annotators` annotation
+<details>
+  <summary>example custom linkml data model</summary>
+  ```yaml
+  classes:
+    MendelianDisease:
+      attributes:
+        name:
+          description: the name of the disease
+          examples:
+            - value: peroxisome biogenesis disorder
+          identifier: true  ## needed for inlining
+        description:
+          description: a description of the disease
+          examples:
+            - value: >-
+              Peroxisome biogenesis disorders, Zellweger syndrome spectrum (PBD-ZSS) is a group of autosomal recessive disorders affecting the formation of functional peroxisomes, characterized by sensorineural hearing loss, pigmentary retinal degeneration, multiple organ dysfunction and psychomotor impairment
+        synonyms:
+          multivalued: true
+          examples:
+            - value: Zellweger syndrome spectrum
+            - value: PBD-ZSS
+        subclass_of:
+          multivalued: true
+          range: MendelianDisease
+          examples:
+            - value: lysosomal disease
+            - value: autosomal recessive disorder
+        symptoms:
+          range: Symptom
+          multivalued: true
+          examples:
+            - value: sensorineural hearing loss
+            - value: pigmentary retinal degeneration
+        inheritance:
+          range: Inheritance
+          examples:
+            - value: autosomal recessive
+        genes:
+          range: Gene
+          multivalued: true
+          examples:
+            - value: PEX1
+            - value: PEX2
+            - value: PEX3
+
+    Gene:
+      is_a: NamedThing
+      id_prefixes:
+        - HGNC
+      annotations:
+        annotators: gilda:, bioportal:hgnc-nr
+
+    Symptom:
+      is_a: NamedThing
+      id_prefixes:
+        - HP
+      annotations:
+        annotators: sqlite:obo:hp
+
+    Inheritance:
+      is_a: NamedThing
+      annotations:
+        annotators: sqlite:obo:hp
+    ```
+</details>
+
+* Prompt hints can be specified using the `prompt` annotation (otherwise description is used)
+* Multivalued fields are supported
+* The default range is string — these are not grounded. Ex.: disease name, synonyms
+* Define a class for each `NamedEntity`
+* For any `NamedEntity`, you can specify a preferred annotator using the `annotators` annotation
 
 We recommend following an established schema like [BioLink Model](https://github.com/biolink/biolink-model), but you can define your own.
 
-### Step 2: Compile the schema
-
-Place the schema YAML in the directory `src/ontogpt/templates/`.
-
-Run the `make` command at the top level. This will compile the schema to Python (Pydantic classes).
+Next step is to compile the schema. For that, you should place the schema YAML in the directory [src/ontogpt/templates/](src/ontogpt/templates/). Then, run the `make` command at the top level. This will compile the schema to Python (Pydantic classes).
 
-### Step 3: Run the command line
+Once you have defined your own schema / data model and placed in the correct directory, you can run the `extract` command. 
 
-e.g.
+Ex.:
 
 ```
 ontogpt extract -t mendelian_disease.MendelianDisease -i marfan-wikipedia.txt
 ```
 
-## Web Application
-
-There is a bare bones web application for running OntoGPT and viewing results.
-
-Install the required dependencies first with the following command:
-```
-poetry install -E web
-```
-
-Then run the following command to start the web application:
-
-```
-poetry run web-ontogpt
-```
-
-Note that the agent running uvicorn must have the API key set, so for obvious reasons
-don't host this publicly without authentication, unless you want your credits drained.
-
-## Features
-
 ### Multiple levels of nesting
 
 Currently no more than two levels of nesting are recommended.
 
 If a field has a range which is itself a class and not a primitive, it will attempt to nest.
 
-E.g. the gocam schema has an attribute:
+Ex. the `gocam` schema has an attribute:
 
 ```yaml
   attributes:
       ...
       gene_functions:
         description: semicolon-separated list of gene to molecular activity relationships
         multivalued: true
         range: GeneMolecularActivityRelationship
 ```
 
-Because `GeneMolecularActivityRelationship` is *inlined* it will nest
+The range `GeneMolecularActivityRelationship` has been specified *inline*, so it will nest.
 
 The generated prompt is:
 
-`gene_functions : <semicolon-separated list of gene to molecular activities relationships>`
+```bash
+gene_functions : <semicolon-separated list of gene to molecular activities relationships>
+```
 
 The output of this is then passed through further SPIRES iterations.
 
 ### Text length limit
 
 Currently SPIRES must use text-davinci-003, which has a total 4k token limit (prompt + completion).
 
-You can pass in a parameter to split the text into chunks, results will be recombined automatically,
-but more experiments need to be done to determined how reliable this is.
+You can pass in a parameter to split the text into chunks. Returned results will be recombined automatically, but more experiments need to be done to determined how reliable this is.
+
+### Schema tips
 
-## Schema Tips
+It helps to have an understanding of the [LinkML](https://linkml.io) schema language, but it should be possible to define your own schemas using the examples in [src/ontogpt/templates](src/ontogpt/templates/) as a guide.
 
-It helps to have an understanding of the [LinkML](https://linkml.io) schema language, but it should be possible
-to define your own schemas using the examples as a guide.
+OntoGPT-specific extensions are specified as *annotations*.
 
-OntoGPT-specific extensions are specified as *annotations*
+You can specify a set of annotators for a field using the `annotators` annotation.
 
-You can specify a set of annotators for a field using the `annotators` annotation
+Ex.:
 
 ```yaml
   Gene:
     is_a: NamedThing
     id_prefixes:
       - HGNC
     annotations:
       annotators: gilda:, bioportal:hgnc-nr, obo:pr
 ```
 
 The annotators are applied in order.
 
 Additionally, when performing grounding, the following measures can be taken to improve accuracy:
 
-- specify the valid set of ID prefixes using `id_prefixes`
-- some vocabularies have structural IDs that are amenable to regexes, you can specify these using `pattern`
-- you can make use of `values_from` slot to specify a [Dynamic Value Set](https://linkml.io/linkml/schemas/enums.html#dynamic-enums)
-    - for example, you can constrain the set of valid locations for a gene product to be subclasses of `cellular_component` in GO or `cell` in CL.
+* Specify the valid set of ID prefixes using `id_prefixes`
+* Some vocabularies have structural IDs that are amenable to regexes, you can specify these using `pattern`
+* You can make use of `values_from` slot to specify a [Dynamic Value Set](https://linkml.io/linkml/schemas/enums.html#dynamic-enums)
+  * For example, you can constrain the set of valid locations for a gene product to be subclasses of `cellular_component` in GO or `cell` in CL
 
-For example:
+Ex.:
 
 ```yaml
 classes:
   ...
   GeneLocation:
     is_a: NamedEntity
     id_prefixes:
@@ -349,86 +367,88 @@
     slot_usage:
       id:
         values_from:
           - GOCellComponentType
           - CellType
 
 enums:
-
   GOCellComponentType:
     reachable_from:
       source_ontology: obo:go
       source_nodes:
         - GO:0005575 ## cellular_component
   CellType:
     reachable_from:
       source_ontology: obo:cl
       source_nodes:
         - CL:0000000 ## cell
-        
 ```
 
-## OWL Exports
+### OWL Exports
 
 The `extract` command will let you export the results as OWL axioms, utilizing [linkml-owl](https://linkml.io/linkml-owl) mappings in the schema.
 
-For example:
+Ex.:
 
 ```bash
 ontogpt extract -t recipe -i recipe-spaghetti.txt -o recipe-spaghetti.owl -O owl
 ```
 
-See [src/ontogpt/templates/recipe.yaml](src/ontogpt/templates/recipe.yaml) 
-for an example of a schema that uses linkml-owl mappings.
-
-See the Makefile for a full pipeline that involves using robot to extract a subset of FOODON
-and merge in the extracted results. This uses [recipe-scrapers](https://github.com/hhursev/recipe-scrapers)
+[src/ontogpt/templates/recipe.yaml](src/ontogpt/templates/recipe.yaml) is an example schema that uses linkml-owl mappings.
 
-Example output OWL here:
+See the [Makefile](Makefile) for a full pipeline that involves using robot to extract a subset of FOODON
+and merge in the extracted results. This uses [recipe-scrapers](https://github.com/hhursev/recipe-scrapers).
 
-- [recipe-all-merged.owl](https://github.com/monarch-initiative/ontogpt/blob/main/tests/output/owl/merged/recipe-all-merged.owl)
+OWL output: [recipe-all-merged.owl](tests/output/owl/merged/recipe-all-merged.owl)
 
-Example classification:
+Classification:
 
 <img width="1329" alt="image" src="https://user-images.githubusercontent.com/50745/230427663-20d845e9-f1d5-490e-b1ad-cdccdd0dca70.png">
 
+## Web Application Setup
 
-Contributions on recipes to test welcome from anyone! Just make a PR [here](https://github.com/monarch-initiative/ontogpt/blob/main/tests/input/recipe-urls.csv). See [this list](https://github.com/hhursev/recipe-scrapers) for accepted URLs
+There is a bare bones web application for running OntoGPT and viewing results.
 
+Install the required dependencies by running the following command:
 
-## HALO: Usage
+```bash
+poetry install -E web
+```
 
-TODO
+Then run this command to start the web application:
 
+```bash
+poetry run web-ontogpt
+```
 
+Note: The agent running uvicorn must have the API key set, so for obvious reasons don't host this publicly without authentication, unless you want your credits drained.
 
-## Gene Enrichment using SPINDOCTOR
+## OntoGPT Limitations
 
-Given a set of genes, OntoGPT can find similarities among them.
+1. Non-deterministic
+  * This relies on an existing LLM, and LLMs can be fickle in their responses
+2. Coupled to OpenAI
+  * You will need an OpenAI account to use their API. In theory any LLM can be used but in practice the parser is tuned for OpenAI's models
 
-Example:
+### SPINDOCTOR web app
+
+To start:
 
 ```
-ontogpt  enrichment -U tests/input/genesets/sensory-ataxia.yaml
+poetry run streamlit run src/ontogpt/streamlit/spindoctor.py
 ```
 
-The default is to use ontological gene function synopses (via the Alliance API).
-
-To use narrative/RefSeq summaries, use the `--no-ontological-synopses` flag.
 
-To run without any gene descriptions, use the `--no-annotations` flag.
-
-
-## OntoGPT Limitations
+## Citation
 
-### Non-deterministic
+SPIRES is described further in: Caufield JH, Hegde H, Emonet V, Harris NL, Joachimiak MP, Matentzoglu N, et al. Structured prompt interrogation and recursive extraction of semantics (SPIRES): A method for populating knowledge bases using zero-shot learning. 
 
-This relies on an existing LLM, and LLMs can be fickle in their responses.
+arXiv publication: http://arxiv.org/abs/2304.02711
 
-### Coupled to OpenAI
+## Contributing
 
-You will need an OpenAI account to use their API. In theory any LLM can be used but in practice the parser is tuned for OpenAI's models.
+Contributions on recipes to test welcome from anyone! Just make a PR [here](https://github.com/monarch-initiative/ontogpt/blob/main/tests/input/recipe-urls.csv). See [this list](https://github.com/hhursev/recipe-scrapers) for accepted URLs
 
 ## Acknowledgements
 
 We gratefully acknowledge [Bosch Research](https://www.bosch.com/research) for their support of this research project.
```

