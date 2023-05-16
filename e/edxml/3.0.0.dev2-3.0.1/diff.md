# Comparing `tmp/edxml-3.0.0.dev2.tar.gz` & `tmp/edxml-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edxml-3.0.0.dev2.tar", last modified: Tue Apr 26 14:06:55 2022, max compression
+gzip compressed data, was "edxml-3.0.1.tar", last modified: Tue May 16 14:13:56 2023, max compression
```

## Comparing `edxml-3.0.0.dev2.tar` & `edxml-3.0.1.tar`

### file list

```diff
@@ -1,122 +1,125 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:06:55.055395 edxml-3.0.0.dev2/
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-04-26 14:06:55.055395 edxml-3.0.0.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1376 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:06:55.043395 edxml-3.0.0.dev2/edxml/
--rw-r--r--   0 runner    (1001) docker     (121)     1921 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:06:55.047395 edxml-3.0.0.dev2/edxml/cli/
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3305 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/cli/edxml_cat.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    14836 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/cli/edxml_ddgen.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5181 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/cli/edxml_diff.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5638 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/cli/edxml_filter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2908 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/cli/edxml_hash.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8488 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/cli/edxml_merge.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     7660 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/cli/edxml_mine.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8021 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/cli/edxml_replay.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    13812 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/cli/edxml_stats.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4752 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/cli/edxml_template_tester.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8946 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/cli/edxml_to_delimited.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3311 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/cli/edxml_to_text.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3086 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/cli/edxml_validate.py
--rw-r--r--   0 runner    (1001) docker     (121)     2126 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/error.py
--rw-r--r--   0 runner    (1001) docker     (121)    54811 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/event.py
--rw-r--r--   0 runner    (1001) docker     (121)     8904 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/event_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)     7998 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/event_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:06:55.047395 edxml-3.0.0.dev2/edxml/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/brick_register.py
--rw-r--r--   0 runner    (1001) docker     (121)      522 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/define_parent_declarative.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/event_collection.py
--rw-r--r--   0 runner    (1001) docker     (121)      308 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/event_representation_attachments_dict.py
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/event_representation_properties_dict_read.py
--rw-r--r--   0 runner    (1001) docker     (121)      391 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/event_representation_properties_dict_write.py
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/event_type_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)      671 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/event_writer.py
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/mining_knowledge_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/parser_pull.py
--rw-r--r--   0 runner    (1001) docker     (121)      866 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/transcoder_harness.py
--rw-r--r--   0 runner    (1001) docker     (121)      479 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/transcoder_object.py
--rw-r--r--   0 runner    (1001) docker     (121)     1047 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/transcoder_object_mediator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1215 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/examples/transcoder_xml_mediator.py
--rw-r--r--   0 runner    (1001) docker     (121)     4126 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/filter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:06:55.051395 edxml-3.0.0.dev2/edxml/miner/
--rw-r--r--   0 runner    (1001) docker     (121)     1236 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/miner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:06:55.051395 edxml-3.0.0.dev2/edxml/miner/graph/
--rw-r--r--   0 runner    (1001) docker     (121)     1169 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/miner/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7325 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/miner/graph/construct.py
--rw-r--r--   0 runner    (1001) docker     (121)    16629 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/miner/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     9730 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/miner/graph/visualize.py
--rw-r--r--   0 runner    (1001) docker     (121)     5998 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/miner/inference.py
--rw-r--r--   0 runner    (1001) docker     (121)    11843 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/miner/knowledge.py
--rw-r--r--   0 runner    (1001) docker     (121)     4217 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/miner/miner.py
--rw-r--r--   0 runner    (1001) docker     (121)    14978 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/miner/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     2691 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/miner/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    16725 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/miner/result.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:06:55.055395 edxml-3.0.0.dev2/edxml/ontology/
--rw-r--r--   0 runner    (1001) docker     (121)     3043 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3598 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/brick.py
--rw-r--r--   0 runner    (1001) docker     (121)      425 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/brick.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    14626 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/concept.py
--rw-r--r--   0 runner    (1001) docker     (121)     1935 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/concept.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    57241 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/data_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     5456 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/data_type.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    11136 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/description.py
--rw-r--r--   0 runner    (1001) docker     (121)    33505 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_property.py
--rw-r--r--   0 runner    (1001) docker     (121)     5038 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_property.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    15434 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_property_concept.py
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_property_concept.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    23092 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_property_relation.py
--rw-r--r--   0 runner    (1001) docker     (121)     2226 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_property_relation.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     9105 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_source.py
--rw-r--r--   0 runner    (1001) docker     (121)     1529 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_source.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    69084 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     6718 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_type.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    14804 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_type_attachment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1793 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_type_attachment.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    38798 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_type_factory.py
--rw-r--r--   0 runner    (1001) docker     (121)    13557 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_type_parent.py
--rw-r--r--   0 runner    (1001) docker     (121)     1681 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/event_type_parent.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    27697 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/object_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     3178 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/object_type.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    36134 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/ontology.py
--rw-r--r--   0 runner    (1001) docker     (121)     4211 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/ontology.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     5032 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/ontology_element.py
--rw-r--r--   0 runner    (1001) docker     (121)      802 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/ontology_element.pyi
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     9406 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/ontology/visualization.py
--rw-r--r--   0 runner    (1001) docker     (121)    28502 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    38214 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/template.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:06:55.055395 edxml-3.0.0.dev2/edxml/transcode/
--rw-r--r--   0 runner    (1001) docker     (121)     1517 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/transcode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21962 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/transcode/mediator.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:06:55.055395 edxml-3.0.0.dev2/edxml/transcode/object/
--rw-r--r--   0 runner    (1001) docker     (121)     1631 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/transcode/object/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3864 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/transcode/object/object_test_harness.py
--rw-r--r--   0 runner    (1001) docker     (121)     7696 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/transcode/object/object_transcoder.py
--rw-r--r--   0 runner    (1001) docker     (121)     6252 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/transcode/object/object_transcoder_mediator.py
--rw-r--r--   0 runner    (1001) docker     (121)     6976 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/transcode/test_harness.py
--rw-r--r--   0 runner    (1001) docker     (121)     8637 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/transcode/transcoder.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:06:55.055395 edxml-3.0.0.dev2/edxml/transcode/xml/
--rw-r--r--   0 runner    (1001) docker     (121)     1613 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/transcode/xml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4488 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/transcode/xml/xml_test_harness.py
--rw-r--r--   0 runner    (1001) docker     (121)    13399 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/transcode/xml/xml_transcoder.py
--rw-r--r--   0 runner    (1001) docker     (121)    18463 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/transcode/xml/xml_transcoder_mediator.py
--rw-r--r--   0 runner    (1001) docker     (121)     1770 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/util.py
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/version.py
--rw-r--r--   0 runner    (1001) docker     (121)    17582 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/edxml/writer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:06:55.043395 edxml-3.0.0.dev2/edxml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      725 2022-04-26 14:06:54.000000 edxml-3.0.0.dev2/edxml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3232 2022-04-26 14:06:55.000000 edxml-3.0.0.dev2/edxml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-26 14:06:54.000000 edxml-3.0.0.dev2/edxml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      589 2022-04-26 14:06:54.000000 edxml-3.0.0.dev2/edxml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-04-26 14:06:54.000000 edxml-3.0.0.dev2/edxml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-04-26 14:06:54.000000 edxml-3.0.0.dev2/edxml.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      138 2022-04-26 14:06:55.059395 edxml-3.0.0.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4158 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-26 14:06:55.055395 edxml-3.0.0.dev2/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1092 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2598 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/tests/assertions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1840 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/tests/test_event_source.py
--rw-r--r--   0 runner    (1001) docker     (121)    12047 2022-04-26 14:06:23.000000 edxml-3.0.0.dev2/tests/test_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:13:56.508234 edxml-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1150 2023-05-16 14:13:53.000000 edxml-3.0.1/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-16 14:13:56.508234 edxml-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-05-16 14:13:53.000000 edxml-3.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:13:56.500234 edxml-3.0.1/edxml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:13:56.500234 edxml-3.0.1/edxml/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3305 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/cli/edxml_cat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14836 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/cli/edxml_ddgen.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5181 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/cli/edxml_diff.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5638 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/cli/edxml_filter.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2908 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/cli/edxml_hash.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8502 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/cli/edxml_merge.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7702 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/cli/edxml_mine.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8021 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/cli/edxml_replay.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13819 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/cli/edxml_stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4752 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/cli/edxml_template_tester.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8946 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/cli/edxml_to_delimited.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3311 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/cli/edxml_to_text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3086 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/cli/edxml_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54811 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8165 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/event.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8911 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/event_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8005 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/event_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:13:56.504234 edxml-3.0.1/edxml/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/brick_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)      522 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/define_parent_declarative.py
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/event_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/event_representation_attachments_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/event_representation_properties_dict_read.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/event_representation_properties_dict_write.py
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/event_type_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/event_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/mining_knowledge_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/parser_pull.py
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/transcoder_harness.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/transcoder_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/transcoder_object_mediator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/examples/transcoder_xml_mediator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4126 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/filter.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:13:56.504234 edxml-3.0.1/edxml/miner/
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/miner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:13:56.504234 edxml-3.0.1/edxml/miner/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/miner/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/miner/graph/construct.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16636 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/miner/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9730 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/miner/graph/visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/miner/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11850 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/miner/knowledge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/miner/miner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14999 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/miner/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2698 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/miner/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/miner/result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:13:56.508234 edxml-3.0.1/edxml/ontology/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3598 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/brick.py
+-rw-r--r--   0 runner    (1001) docker     (123)      425 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/brick.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14731 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/concept.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/concept.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    57241 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/data_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5456 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/data_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/description.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33674 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_property.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15902 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_property_concept.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_property_concept.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    23062 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_property_relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_property_relation.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9112 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_source.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    68704 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6718 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14947 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_type_attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1793 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_type_attachment.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    38798 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_type_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13557 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_type_parent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/event_type_parent.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27717 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/object_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3178 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/object_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    36141 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/ontology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/ontology.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/ontology_element.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/ontology_element.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9406 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/ontology/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28614 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/parser.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    38228 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:13:56.508234 edxml-3.0.1/edxml/transcode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/transcode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21976 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/transcode/mediator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:13:56.508234 edxml-3.0.1/edxml/transcode/object/
+-rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/transcode/object/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/transcode/object/object_test_harness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7696 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/transcode/object/object_transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/transcode/object/object_transcoder_mediator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/transcode/test_harness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8637 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/transcode/transcoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:13:56.508234 edxml-3.0.1/edxml/transcode/xml/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/transcode/xml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4488 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/transcode/xml/xml_test_harness.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13406 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/transcode/xml/xml_transcoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18463 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/transcode/xml/xml_transcoder_mediator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17589 2023-05-16 14:13:53.000000 edxml-3.0.1/edxml/writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:13:56.500234 edxml-3.0.1/edxml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2151 2023-05-16 14:13:56.000000 edxml-3.0.1/edxml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-05-16 14:13:56.000000 edxml-3.0.1/edxml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 14:13:56.000000 edxml-3.0.1/edxml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-16 14:13:56.000000 edxml-3.0.1/edxml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-16 14:13:56.000000 edxml-3.0.1/edxml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 14:13:56.000000 edxml-3.0.1/edxml.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-16 14:13:56.508234 edxml-3.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-05-16 14:13:53.000000 edxml-3.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 14:13:56.508234 edxml-3.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-16 14:13:53.000000 edxml-3.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-05-16 14:13:53.000000 edxml-3.0.1/tests/assertions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-16 14:13:53.000000 edxml-3.0.1/tests/test_event_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-05-16 14:13:53.000000 edxml-3.0.1/tests/test_writer.py
```

### Comparing `edxml-3.0.0.dev2/LICENSE.rst` & `edxml-3.0.1/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/__init__.py` & `edxml-3.0.1/edxml/__init__.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/cli/__init__.py` & `edxml-3.0.1/edxml/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/cli/edxml_cat.py` & `edxml-3.0.1/edxml/cli/edxml_cat.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/cli/edxml_ddgen.py` & `edxml-3.0.1/edxml/cli/edxml_ddgen.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/cli/edxml_diff.py` & `edxml-3.0.1/edxml/cli/edxml_diff.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/cli/edxml_filter.py` & `edxml-3.0.1/edxml/cli/edxml_filter.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/cli/edxml_hash.py` & `edxml-3.0.1/edxml/cli/edxml_hash.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/cli/edxml_merge.py` & `edxml-3.0.1/edxml/cli/edxml_merge.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,17 +22,17 @@
 #  Note that, unless buffering is used, this script needs to store one event for each
 #  sticky hash of the input events in RAM. For large event streams that contain events
 #  with many sticky hashes, it will eventually run out of memory.
 
 import argparse
 import sys
 import time
-from typing import Dict, List
+from typing import Dict, List # noqa
 
-from edxml import EDXMLEvent
+from edxml import EDXMLEvent # noqa
 from edxml.cli import configure_logger
 from edxml.filter import EDXMLPullFilter, EDXMLPushFilter
 from edxml.error import EDXMLValidationError
 from edxml.logger import log
 
 
 class EDXMLEventMerger(EDXMLPullFilter):
```

### Comparing `edxml-3.0.0.dev2/edxml/cli/edxml_mine.py` & `edxml-3.0.1/edxml/cli/edxml_mine.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
 import logging
 import sys
 from collections import defaultdict
 
 from edxml.cli import configure_logger
 from edxml.miner.graph.visualize import graphviz_nodes, graphviz_concepts
 from edxml.miner.inference import RelationInference
-from edxml.miner.knowledge import KnowledgePullParser, KnowledgeBase
+from edxml.miner.parser import KnowledgePullParser
+from edxml.miner.knowledge import KnowledgeBase
 
 
 def parse_args():
     parser = argparse.ArgumentParser(
         description="This utility performs concept mining on EDXML data received on standard input or from a file."
     )
 
@@ -94,26 +95,26 @@
 
     ontology = parser._ontology
 
     found_concepts = set()
     instance_concepts = defaultdict(set)
 
     while True:
-        seed = parser._graph.find_optimal_seed()
+        seed = parser.miner._graph.find_optimal_seed()
 
         if seed is None:
             # When the best seed we can find
             # is tainted, all nodes have been
             # used and we are done.
             break
 
         seed_dn = seed.concept_association.get_attribute_display_name_singular()
         logging.info(f"Selected seed: {seed_dn} = {seed.value}")
 
-        parser.mine(seed, min_confidence=min_confidence, max_depth=max_depth)
+        parser.miner.mine(seed, min_confidence=min_confidence, max_depth=max_depth)
         results = knowledge_base.concept_collection
         # Find the ID of the newly created concept and report it.
         concept_id = next(iter(set(results.concepts.keys()) - found_concepts))
         concept = results.concepts[concept_id]
         if args.tell:
             instance_concepts[seed.id] = {(seed.concept_association.get_concept_name())}
             instance_concepts = report_new_concept(ontology, seed.id, concept, instance_concepts, args.with_reasons)
```

### Comparing `edxml-3.0.0.dev2/edxml/cli/edxml_replay.py` & `edxml-3.0.1/edxml/cli/edxml_replay.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/cli/edxml_stats.py` & `edxml-3.0.1/edxml/cli/edxml_stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #  URLs, and so on.
 
 import argparse
 import logging
 import operator
 import sys
 from collections import defaultdict
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional # noqa
 
 from dateutil.parser import parse
 from edxml.cli import configure_logger
 from edxml.parser import EDXMLPullParser
 
 
 class StatsParser(EDXMLPullParser):
```

### Comparing `edxml-3.0.0.dev2/edxml/cli/edxml_template_tester.py` & `edxml-3.0.1/edxml/cli/edxml_template_tester.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/cli/edxml_to_delimited.py` & `edxml-3.0.1/edxml/cli/edxml_to_delimited.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/cli/edxml_to_text.py` & `edxml-3.0.1/edxml/cli/edxml_to_text.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/cli/edxml_validate.py` & `edxml-3.0.1/edxml/cli/edxml_validate.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/error.py` & `edxml-3.0.1/edxml/error.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/event.py` & `edxml-3.0.1/edxml/event.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/event_collection.py` & `edxml-3.0.1/edxml/event_collection.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #                       and is released under the MIT License:                           =
 #                         https://opensource.org/licenses/MIT                            =
 #                                                                                        =
 # ========================================================================================
 
 from io import BytesIO
 from collections import defaultdict
-from typing import Dict, List
+from typing import Dict, List # noqa
 
 from edxml import EDXMLWriter, EDXMLPullParser, EDXMLEvent
 from edxml.ontology import Ontology
 
 
 class EventCollection(List[EDXMLEvent]):
     """
```

### Comparing `edxml-3.0.0.dev2/edxml/event_validator.py` & `edxml-3.0.1/edxml/event_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #                                                                                        =
 #             This file is part of the EDXML Software Development Kit (SDK)              =
 #                       and is released under the MIT License:                           =
 #                         https://opensource.org/licenses/MIT                            =
 #                                                                                        =
 # ========================================================================================
 from lxml import etree
-from typing import Dict, Optional
+from typing import Dict, Optional # noqa
 
 import edxml
 from edxml.error import EDXMLEventValidationError
 
 
 class EventValidatorError:
     """
```

### Comparing `edxml-3.0.0.dev2/edxml/examples/__init__.py` & `edxml-3.0.1/edxml/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/examples/define_parent_declarative.py` & `edxml-3.0.1/edxml/examples/define_parent_declarative.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/examples/event_writer.py` & `edxml-3.0.1/edxml/examples/event_writer.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/examples/transcoder_harness.py` & `edxml-3.0.1/edxml/examples/transcoder_harness.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/examples/transcoder_object_mediator.py` & `edxml-3.0.1/edxml/examples/transcoder_object_mediator.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/examples/transcoder_xml_mediator.py` & `edxml-3.0.1/edxml/examples/transcoder_xml_mediator.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/filter.py` & `edxml-3.0.1/edxml/filter.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/logger.py` & `edxml-3.0.1/edxml/logger.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/miner/__init__.py` & `edxml-3.0.1/edxml/miner/__init__.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/miner/graph/__init__.py` & `edxml-3.0.1/edxml/miner/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/miner/graph/construct.py` & `edxml-3.0.1/edxml/miner/graph/construct.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/miner/graph/graph.py` & `edxml-3.0.1/edxml/miner/graph/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #                       and is released under the MIT License:                           =
 #                         https://opensource.org/licenses/MIT                            =
 #                                                                                        =
 # ========================================================================================
 
 from collections import defaultdict
 from functools import reduce
-from typing import Dict, Set, Iterable
+from typing import Dict, Set, Iterable # noqa
 
 from edxml.ontology import Ontology
 from edxml.miner.node import Node, EventObjectHub, EventObjectNode
 from edxml.miner.result import MinedConceptAttribute, MinedConceptInstance, MinedConceptInstanceCollection
 
 
 class ConceptInstanceGraph(object):
```

### Comparing `edxml-3.0.0.dev2/edxml/miner/graph/visualize.py` & `edxml-3.0.1/edxml/miner/graph/visualize.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/miner/inference.py` & `edxml-3.0.1/edxml/miner/inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #                                                                                        =
 #             This file is part of the EDXML Software Development Kit (SDK)              =
 #                       and is released under the MIT License:                           =
 #                         https://opensource.org/licenses/MIT                            =
 #                                                                                        =
 # ========================================================================================
 
-import edxml.miner
+import edxml.miner # noqa
 
 
 class Inference(object):
     """
 
     An edge in a concept instance graph representing the
     inference of a relation between two nodes.
```

### Comparing `edxml-3.0.0.dev2/edxml/miner/knowledge.py` & `edxml-3.0.1/edxml/miner/knowledge.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ..  autoclass:: KnowledgeBase
     :members:
     :show-inheritance:
 """
 import json
 from collections import defaultdict
 
-import edxml
+import edxml # noqa
 
 from edxml.miner.result import ConceptInstanceCollection
 from edxml.miner.result import from_json as concept_collection_from_json
 from edxml.ontology import Ontology
 
 
 class KnowledgeBase:
```

### Comparing `edxml-3.0.0.dev2/edxml/miner/miner.py` & `edxml-3.0.1/edxml/miner/miner.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #                         https://opensource.org/licenses/MIT                            =
 #                                                                                        =
 # ========================================================================================
 
 from edxml import EDXMLEvent
 from edxml.miner.graph.construct import GraphConstructor
 from edxml.miner.graph import ConceptInstanceGraph
-from edxml.miner.knowledge import KnowledgeBase
+from edxml.miner.knowledge import KnowledgeBase # noqa
 from edxml.ontology import Ontology
 
 
 class Miner:
     """
     Class combining an ontology, concept graph and a knowledge
     base to mine concepts and universals.
```

### Comparing `edxml-3.0.0.dev2/edxml/miner/node.py` & `edxml-3.0.1/edxml/miner/node.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 #                                   http://edxml.org                                     =
 #                                                                                        =
 #             This file is part of the EDXML Software Development Kit (SDK)              =
 #                       and is released under the MIT License:                           =
 #                         https://opensource.org/licenses/MIT                            =
 #                                                                                        =
 # ========================================================================================
-from datetime import datetime
+from datetime import datetime # noqa
 from functools import reduce
 from itertools import groupby
 from operator import mul
-from typing import Dict, Set, Optional, MutableMapping, List
+from typing import Dict, Set, Optional, MutableMapping, List # noqa
 from collections import defaultdict, UserDict
 
-from edxml.miner.inference import Inference
+from edxml.miner.inference import Inference # noqa
 from edxml.ontology import Concept
 
 import edxml.miner.inference
 
 
 def is_intra_edge(edge):
     return isinstance(edge, edxml.miner.inference.RelationInference) and edge.relation.get_type() != 'inter'
```

### Comparing `edxml-3.0.0.dev2/edxml/miner/parser.py` & `edxml-3.0.1/edxml/miner/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     :members:
     :show-inheritance:
 
 ..  autoclass:: KnowledgePushParser
     :members:
     :show-inheritance:
 """
-import edxml
+import edxml # noqa
 from edxml import EDXMLPullParser, EDXMLPushParser
 from edxml.miner import Miner
 
 
 class KnowledgeParserBase:
     def __init__(self, knowledge_base):
         """
```

### Comparing `edxml-3.0.0.dev2/edxml/miner/result.py` & `edxml-3.0.1/edxml/miner/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # ========================================================================================
 
 import json
 
 from collections import defaultdict
 from functools import reduce
 from operator import mul
-from typing import List, Dict, Optional
+from typing import List, Dict, Optional # noqa
 from dateutil.parser import parse
 
 from edxml.miner.node import NodeCollection
 
 
 class ConceptAttribute:
     """
```

### Comparing `edxml-3.0.0.dev2/edxml/ontology/__init__.py` & `edxml-3.0.1/edxml/ontology/__init__.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/brick.py` & `edxml-3.0.1/edxml/ontology/brick.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/concept.py` & `edxml-3.0.1/edxml/ontology/concept.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 # ========================================================================================
 
 import copy
 import re
 
 from lxml import etree
 
-import edxml.ontology
+import edxml.ontology # noqa
 
 from edxml.error import EDXMLOntologyValidationError
 from edxml.ontology import VersionedOntologyElement, normalize_xml_token
 from edxml.ontology.ontology_element import ontology_element_upgrade_error
 
 
 class Concept(VersionedOntologyElement):
     """
     Class representing an EDXML concept
     """
 
-    NAME_PATTERN = re.compile('^[a-z0-9.-]{1,255}$')
+    NAME_PATTERN = re.compile('^[a-z][a-z0-9-]*(\\.[a-z][a-z0-9-]*)*$')
 
     def __init__(self, ontology, name, display_name_singular=None, display_name_plural=None, description=None):
 
         display_name_singular = display_name_singular or name.replace('.', ' ')
         display_name_plural = display_name_plural or display_name_singular + 's'
 
         self._attr = {
@@ -234,15 +234,18 @@
         Returns:
           edxml.ontology.Concept: The Concept instance
         """
         new_version = copy.deepcopy(self).set_version(self._attr['version'] + 1)
         if new_version > self.__versions[self._attr['version']]:
             self.set_version(self._attr['version'] + 1)
         else:
-            raise Exception('Cannot upgrade when current version is not greater than previous version.')
+            raise Exception(
+                'Cannot upgrade concept. '
+                'Apparently no changes were made since the last time the version number changed.'
+            )
 
         return self
 
     def validate(self):
         """
 
         Checks if the concept is valid. It only looks
```

### Comparing `edxml-3.0.0.dev2/edxml/ontology/concept.pyi` & `edxml-3.0.1/edxml/ontology/concept.pyi`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/data_type.py` & `edxml-3.0.1/edxml/ontology/data_type.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/data_type.pyi` & `edxml-3.0.1/edxml/ontology/data_type.pyi`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/description.py` & `edxml-3.0.1/edxml/ontology/description.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,24 +60,24 @@
                     event_type_dn.append(ontology.get_event_type(event_type_name).get_display_name_plural())
                 description += _list_strings(event_type_dn) + ')'
 
     if relates_intra:
         description += f"\n\nThe {producer_name} enhances `concept mining <http://edxml.org/concept-mining>`_ " \
                        "by expanding knowledge about:\n"
 
-    expansions = defaultdict(set)
-    for concept_name, attribute_names in relates_intra.items():
-        concept_dn = ontology.get_concept(concept_name).get_display_name_plural()
-        expansions[concept_dn].update(attribute_names)
+        expansions = defaultdict(set)
+        for concept_name, attribute_names in relates_intra.items():
+            concept_dn = ontology.get_concept(concept_name).get_display_name_plural()
+            expansions[concept_dn].update(attribute_names)
 
-    for concept_dn, object_types in expansions.items():
-        description += f"\n:{concept_dn.capitalize()}: Discovering new " + _list_strings(object_types)
+        for concept_dn, attribute_names in sorted(expansions.items()):
+            description += f"\n:{concept_dn.capitalize()}: Discovering new " + _list_strings(attribute_names)
 
     if concept_combinations:
-        description += f"\n\nThe {producer_name} identifies:\n" + '\n'.join(set(concept_combinations.values()))
+        description += f"\n\nThe {producer_name} identifies:\n" + '\n'.join(sorted(set(concept_combinations.values())))
 
     value_names = set()
     value_descriptions = set()
     value_containers = set()
     for event_type in ontology.get_event_types().values():
         for relation in event_type.get_property_relations(relation_type='name').values():
             value_names.add(
@@ -136,35 +136,35 @@
     for object_type in ontology.get_object_types().values():
         object_type_names.append(f"{object_type.get_name()} ({object_type.get_display_name_singular()})")
     return object_type_names
 
 
 def _describe_event_types(ontology: Ontology):
     type_names = []
-    for event_type_name in ontology.get_event_type_names():
+    for event_type_name in sorted(ontology.get_event_type_names()):
         type_names.append(ontology.get_event_type(event_type_name).get_display_name_plural())
     return _list_strings(type_names)
 
 
 def _describe_inter_concept_relations(ontology: Ontology):
     relations = defaultdict(lambda: defaultdict(set))
-    for event_type_name in ontology.get_event_type_names():
+    for event_type_name in sorted(ontology.get_event_type_names()):
         event_type = ontology.get_event_type(event_type_name)
-        for relation in event_type.relations:
+        for relation in sorted(event_type.relations, key=lambda rel: rel.get_persistent_id()):
             if relation.get_type() != 'inter':
                 continue
             relations[relation.get_source_concept()][relation.get_target_concept()].add(event_type_name)
     return relations
 
 
 def _describe_intra_concept_relations(ontology: Ontology):
     relations = defaultdict(set)
-    for event_type_name in ontology.get_event_type_names():
+    for event_type_name in sorted(ontology.get_event_type_names()):
         event_type = ontology.get_event_type(event_type_name)
-        for relation in event_type.relations:
+        for relation in sorted(event_type.relations, key=lambda rel: rel.get_persistent_id()):
             if relation.get_type() != 'intra':
                 continue
             relations[relation.get_source_concept()].add(
                 event_type[relation.get_source()].get_concept_associations()[relation.get_source_concept()]
                 .get_attribute_display_name_plural(),
             )
             relations[relation.get_target_concept()].add(
@@ -221,12 +221,13 @@
                     'concept_target': target_concept.get_display_name_plural()
                 })
 
     return descriptions
 
 
 def _list_strings(strings):
+    strings = sorted(strings)
     if len(strings) > 1:
         last = strings.pop()
         return ', '.join(strings) + ' and ' + last
     else:
         return ' and '.join(strings)
```

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_property.py` & `edxml-3.0.1/edxml/ontology/event_property.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 # ========================================================================================
 
 import re
 import edxml.ontology
 
 from edxml.error import EDXMLOntologyValidationError
 from lxml import etree
-from typing import Dict
+from typing import Dict # noqa
 from edxml.ontology import OntologyElement, normalize_xml_token
 from edxml.ontology.ontology_element import event_type_element_upgrade_error
 
 
 class EventProperty(OntologyElement):
     """
     Class representing an EDXML event property
     """
 
-    EDXML_PROPERTY_NAME_PATTERN = re.compile('^[a-z0-9-]+(.[a-z0-9-]+)*$')
+    NAME_PATTERN = re.compile('^[a-z][a-z0-9-]*(\\.[a-z][a-z0-9-]*)*$')
 
     MERGE_MATCH = 'match'
     """Merge strategy 'match'"""
     MERGE_ANY = 'any'
     """Merge strategy 'any'"""
     MERGE_ADD = 'add'
     """Merge strategy 'add'"""
@@ -675,23 +675,27 @@
           edxml.ontology.EventProperty: The EventProperty instance
         """
         self.set_merge_strategy('max')
         return self
 
     def _validate_attributes(self):
 
-        if not re.match(self.EDXML_PROPERTY_NAME_PATTERN, self.__attr['name']):
+        if not re.match(self.NAME_PATTERN, self.__attr['name']):
             raise EDXMLOntologyValidationError(
-                'Invalid property name in property definition: "%s"' % self.__attr['name']
+                'Property "%s" has an invalid name.' % self.__attr['name']
             )
 
         if len(self.__attr['name']) > 64:
             raise EDXMLOntologyValidationError(
                 'Property name is too long: "%s"' % self.__attr['name'])
 
+        if self.__attr['name'].startswith('xml'):
+            raise EDXMLOntologyValidationError(
+                'Property name must not be a reserved XML tag name: "%s"' % self.__attr['name'])
+
         if not re.match(edxml.ontology.ObjectType.NAME_PATTERN, self.__attr['object-type']):
             raise EDXMLOntologyValidationError(
                 'Invalid object type name in property definition: "%s"' % self.__attr['object-type'])
 
         if not len(self.__attr['description']) <= 128:
             raise EDXMLOntologyValidationError(
                 'Property description is too long: "%s"' % self.__attr['description'])
```

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_property.pyi` & `edxml-3.0.1/edxml/ontology/event_property.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from typing import Dict
 
 from edxml.ontology import OntologyElement, PropertyConcept
 
 
 class EventProperty(OntologyElement):
 
-    EDXML_PROPERTY_NAME_PATTERN = ...
+    NAME_PATTERN = ...
 
     MERGE_MATCH = ...
     """Merge strategy 'match'"""
     MERGE_ANY = ...
     """Merge strategy 'any'"""
     MERGE_ADD = ...
     """Merge strategy 'add'"""
```

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_property_concept.py` & `edxml-3.0.1/edxml/ontology/event_property_concept.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,16 @@
 #                                                                                        =
 # ========================================================================================
 
 from lxml import etree
 
 
 from edxml.error import EDXMLOntologyValidationError
-from edxml.ontology import OntologyElement, EventType, EventProperty, normalize_xml_token
+from edxml.ontology import EventType, EventProperty # noqa
+from edxml.ontology import OntologyElement, normalize_xml_token
 from edxml.ontology.ontology_element import event_type_element_upgrade_error
 
 
 class PropertyConcept(OntologyElement):
     """
     Class representing an association between a property and a concept
     """
@@ -260,14 +261,22 @@
             raise EDXMLOntologyValidationError(
                 'The property / concept association between property %s in event type %s and concept %s has '
                 'a custom display name which contains illegal whitespace characters: "%s"' %
                 (self.__event_type.get_name(), self.__property.get_name(), self.__attr['name'],
                  self.__attr['attr-display-name-plural'])
             )
 
+        if len(self.__attr['attr-extension']) > 16:
+            raise EDXMLOntologyValidationError(
+                'The property / concept association between property %s in event type %s and concept %s has '
+                'an attribute extension that is too long: "%s"' %
+                (self.__event_type.get_name(), self.__property.get_name(), self.__attr['name'],
+                 self.__attr['attr-extension'])
+            )
+
         return self
 
     @classmethod
     def create_from_xml(cls, concept_element, event_type, property):
         try:
             association = cls(
                 event_type,
```

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_property_concept.pyi` & `edxml-3.0.1/edxml/ontology/event_property_concept.pyi`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_property_relation.py` & `edxml-3.0.1/edxml/ontology/event_property_relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,19 +267,19 @@
 
         Raises:
           EDXMLOntologyValidationError
         Returns:
           edxml.ontology.PropertyRelation: The PropertyRelation instance
 
         """
-        if not re.match(edxml.ontology.EventProperty.EDXML_PROPERTY_NAME_PATTERN, self.__attr['source']):
+        if not re.match(edxml.ontology.EventProperty.NAME_PATTERN, self.__attr['source']):
             raise EDXMLOntologyValidationError(
                 'Invalid property name in property relation: "%s"' % self.__attr['source'])
 
-        if not re.match(edxml.ontology.EventProperty.EDXML_PROPERTY_NAME_PATTERN, self.__attr['target']):
+        if not re.match(edxml.ontology.EventProperty.NAME_PATTERN, self.__attr['target']):
             raise EDXMLOntologyValidationError(
                 'Invalid property name in property relation: "%s"' % self.__attr['target'])
 
         if self.__attr['description'] is not None:
             if not len(self.__attr['description']) <= 255:
                 raise EDXMLOntologyValidationError(
                     'Property relation description is too long: "%s"' % self.__attr['description']
```

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_property_relation.pyi` & `edxml-3.0.1/edxml/ontology/event_property_relation.pyi`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_source.py` & `edxml-3.0.1/edxml/ontology/event_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # ========================================================================================
 
 import re
 from datetime import datetime
 
 from lxml import etree
 
-import edxml.ontology
+import edxml.ontology # noqa
 
 from edxml.error import EDXMLOntologyValidationError
 from edxml.ontology import VersionedOntologyElement
 from edxml.ontology.ontology_element import ontology_element_upgrade_error
 
 
 class EventSource(VersionedOntologyElement):
```

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_source.pyi` & `edxml-3.0.1/edxml/ontology/event_source.pyi`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_type.py` & `edxml-3.0.1/edxml/ontology/event_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #                         https://opensource.org/licenses/MIT                            =
 #                                                                                        =
 # ========================================================================================
 
 import base64
 import binascii
 from decimal import Decimal
-from typing import Dict
+from typing import Dict # noqa
 
 import re
 
 from io import BytesIO
 from collections import defaultdict
 from collections.abc import MutableMapping
 from lxml import etree
@@ -124,16 +124,15 @@
     """
     Class representing an EDXML event type. The class provides
     access to event properties by means of a dictionary interface.
     For each of the properties there is a key matching the name of
     the event property, the value is the property itself.
     """
 
-    NAME_PATTERN = re.compile("^[a-z0-9.-]*$")
-    CLASS_LIST_PATTERN = re.compile("^[a-z0-9, ]*$")
+    NAME_PATTERN = re.compile("^[a-z][a-z0-9-]*(\\.[a-z][a-z0-9-]*)*$")
 
     def __init__(self, ontology, name, display_name_singular=None, display_name_plural=None, description=None,
                  summary='no description available', story='no description available', parent=None):
 
         display_name_singular = display_name_singular or name.replace('.', ' ')
         display_name_plural = display_name_plural or display_name_singular + 's'
 
@@ -1823,16 +1822,11 @@
             property_object_sets = defaultdict(set)
             for event in version_events:
                 for property_name in self.__properties.keys():
                     property_object_sets[property_name].add(tuple(sorted(event[property_name])))
             # Now we check for each property if the object sets of all
             # events that share a version are mutually consistent.
             for property_name, object_sets in property_object_sets.items():
-                strategy = self.__properties[property_name].get_merge_strategy()
-                if strategy in [EventProperty.MERGE_MATCH, EventProperty.MERGE_ANY]:
-                    # No conflict possible because the object values are either identical (match)
-                    # or any differences are insignificant (drop)
-                    continue
                 if len(object_sets) > 1:
                     # There is more than one unique set of object values
                     # for this property.
                     raise EDXMLMergeConflictError(version_events)
```

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_type.pyi` & `edxml-3.0.1/edxml/ontology/event_type.pyi`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_type_attachment.py` & `edxml-3.0.1/edxml/ontology/event_type_attachment.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 
 class EventTypeAttachment(OntologyElement):
     """
     Class representing an EDXML event attachment definition
     """
 
-    NAME_PATTERN = re.compile("^[a-z0-9-]*$")
+    NAME_PATTERN = re.compile("^[a-z][a-z0-9-]*$")
     DISPLAY_NAME_PATTERN = re.compile("^[ a-zA-Z0-9]*/[ a-zA-Z0-9]*$")
 
     def __init__(self, event_type, name='default', media_type='text/plain', display_name_singular=None,
                  display_name_plural=None, description=None, encode_base64=False):
         """
 
         Creates a new event attachment definition.
@@ -265,19 +265,21 @@
         Returns:
           edxml.ontology.EventTypeAttachment: The EventTypeAttachment instance
 
         """
 
         if not 1 <= len(self._attr['name']) <= 64:
             raise EDXMLOntologyValidationError(
-                'Event type "%s" has an invalid name.' % self._attr['name']
+                'An attachment of event type "%s" has an invalid name: "%s"' %
+                (self._event_type.get_name(), self._attr['name'])
             )
         if not re.match(self.NAME_PATTERN, self._attr['name']):
             raise EDXMLOntologyValidationError(
-                'Event type "%s" has an invalid name.' % self._attr['name']
+                'An attachment of event type "%s" has an invalid name: "%s"' %
+                (self._event_type.get_name(), self._attr['name'])
             )
 
         if not 1 <= len(self._attr['description']) <= 128:
             raise EDXMLOntologyValidationError(
                 'An attachment definition contains a description attribute that is either empty or too long: "%s"'
                 % self._attr['description']
             )
```

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_type_attachment.pyi` & `edxml-3.0.1/edxml/ontology/event_type_attachment.pyi`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_type_factory.py` & `edxml-3.0.1/edxml/ontology/event_type_factory.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_type_parent.py` & `edxml-3.0.1/edxml/ontology/event_type_parent.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/event_type_parent.pyi` & `edxml-3.0.1/edxml/ontology/event_type_parent.pyi`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/object_type.py` & `edxml-3.0.1/edxml/ontology/object_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,32 +13,31 @@
 
 import copy
 import re
 import sre_constants
 
 from lxml import etree
 
-import edxml.ontology
+import edxml.ontology # noqa
 
 from edxml.error import EDXMLEventValidationError, EDXMLOntologyValidationError
 
 from .data_type import DataType
 from .ontology_element import VersionedOntologyElement, ontology_element_upgrade_error
 from .util import normalize_xml_token
 
 
 class ObjectType(VersionedOntologyElement):
     """
     Class representing an EDXML object type
     """
 
-    NAME_PATTERN = re.compile('^[a-z0-9.-]{1,64}$')
+    NAME_PATTERN = re.compile('^[a-z][a-z0-9-]*(\\.[a-z][a-z0-9-]*)*$')
     DISPLAY_NAME_PATTERN = re.compile("^[ a-zA-Z0-9]*/[ a-zA-Z0-9]*$")
-    FUZZY_MATCHING_PATTERN = re.compile(
-        r"^|(phonetic)|(substring:.*)|(\[[0-9]{1,2}:\])|(\[:[0-9]{1,2}\])$")
+    FUZZY_MATCHING_PATTERN = re.compile(r"^|(phonetic)|(substring:.*)|(\[[0-9]{1,2}:\\])|(\[:[0-9]{1,2}\\])$")
 
     def __init__(self, ontology, name, display_name_singular=None, display_name_plural=None, description=None,
                  data_type='string:0:mc:u', unit_name=None, unit_symbol=None, prefix_radix=None, compress=False,
                  xref=None, fuzzy_matching=None, regex_hard=None, regex_soft=None):
 
         display_name_singular = display_name_singular or name.replace('.', ' ')
         display_name_plural = display_name_plural or display_name_singular + 's'
```

### Comparing `edxml-3.0.0.dev2/edxml/ontology/object_type.pyi` & `edxml-3.0.1/edxml/ontology/object_type.pyi`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/ontology.py` & `edxml-3.0.1/edxml/ontology/ontology.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #                                                                                        =
 #             This file is part of the EDXML Software Development Kit (SDK)              =
 #                       and is released under the MIT License:                           =
 #                         https://opensource.org/licenses/MIT                            =
 #                                                                                        =
 # ========================================================================================
 
-from typing import Dict
+from typing import Dict # noqa
 
 from lxml import etree
 from edxml.error import EDXMLOntologyValidationError
 from .object_type import ObjectType
 from .concept import Concept
 from .event_type import EventType
 from .event_source import EventSource
```

### Comparing `edxml-3.0.0.dev2/edxml/ontology/ontology.pyi` & `edxml-3.0.1/edxml/ontology/ontology.pyi`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/ontology_element.py` & `edxml-3.0.1/edxml/ontology/ontology_element.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/ontology_element.pyi` & `edxml-3.0.1/edxml/ontology/ontology_element.pyi`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/util.py` & `edxml-3.0.1/edxml/ontology/util.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/ontology/visualization.py` & `edxml-3.0.1/edxml/ontology/visualization.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/parser.py` & `edxml-3.0.1/edxml/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,20 @@
 #                         https://opensource.org/licenses/MIT                            =
 #                                                                                        =
 # ========================================================================================
 
 """
 This module offers various classes for incremental parsing of EDXML data streams.
 """
+import copy
 import re
 import edxml_schema
 
 from lxml.etree import XMLSyntaxError
-from typing import Dict, List, Any
+from typing import Dict, List, Any # noqa
 
 from collections import defaultdict
 from lxml import etree
 
 from edxml.error import EDXMLValidationError, EDXMLEventValidationError, EDXMLOntologyValidationError
 from edxml import ParsedEvent
 from edxml.event_validator import EventValidator
@@ -270,30 +271,33 @@
         if self.__root_element is None:
             # The root element is set as soon as the opening <edxml> tag
             # is parsed. If it is not set, we either did not receive any
             # XML tags or the input is not valid EDXML.
             raise EDXMLValidationError('Failed to parse EDXML data. Either the data is not EDXML or it is empty.')
 
         try:
-            self.__schema.assertValid(self.__root_element)
+            # We are specifically aiming to find ontology validation problems,
+            # so we generate a minimal XML tree containing just ontology elements.
+            ontology_tree = copy.copy(self.__root_element)
+            for element in ontology_tree.findall('./*'):
+                if element.tag != '{http://edxml.org/edxml}ontology':
+                    element.getparent().remove(element)
+            self.__schema.assertValid(ontology_tree)
         except (etree.DocumentInvalid, etree.XMLSyntaxError) as validation_error:
-            # XML syntax is incorrect or the structure does not validate against the RelaxNG schema.
-            if isinstance(validation_error, etree.DocumentInvalid):
-                # Document is not valid according to schema. This is most likely
-                # due to a problem with an <ontology> element. See if we have
-                # an ontology element in the tree and try to process it. That
-                # will yield a better exception message than the errors
-                # produced by the RelaxNG validator.
-                if not self.__schema.error_log.last_error.path.startswith('/ontology/'):
-                    # Ontology appears to be fine. In that case the validation error can
-                    # be caused by incomplete input. Since parsing is incremental, there
-                    # may be an incomplete <event> element in the tree.
-                    return
-                for ontology_element in self.__root_element.iterfind('{http://edxml.org/edxml}ontology'):
-                    self.__process_ontology(ontology_element)
+            # Document is not valid according to schema. This is most likely
+            # due to a problem with an <ontology> element. See if we have
+            # an ontology element in the tree and try to process it. That
+            # will yield a better exception message than the errors
+            # produced by the RelaxNG validator.
+            for ontology_element in self.__root_element.iterfind('{http://edxml.org/edxml}ontology'):
+                self.__process_ontology(ontology_element)
+
+            # And if we did not identify the problem, we have no choice
+            # but throw an exception showing the schema validation error.
+            raise EDXMLOntologyValidationError("An EDXML validation error occurred: " + str(validation_error))
 
     def __process_ontology(self, ontology_element):
         if self._ontology is None:
             self._ontology = Ontology()
 
         try:
             self._ontology.update(ontology_element)
```

### Comparing `edxml-3.0.0.dev2/edxml/template.py` & `edxml-3.0.1/edxml/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,17 +8,17 @@
 #             This file is part of the EDXML Software Development Kit (SDK)              =
 #                       and is released under the MIT License:                           =
 #                         https://opensource.org/licenses/MIT                            =
 #                                                                                        =
 # ========================================================================================
 
 import re
-from typing import Dict
+from typing import Dict # noqa
 
-import edxml
+import edxml # noqa
 from .ontology.event_type import EventType
 from dateutil import relativedelta
 from dateutil.parser import parse, ParserError
 from edxml.error import EDXMLOntologyValidationError
 from termcolor import colored
```

### Comparing `edxml-3.0.0.dev2/edxml/transcode/__init__.py` & `edxml-3.0.1/edxml/transcode/__init__.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/transcode/mediator.py` & `edxml-3.0.1/edxml/transcode/mediator.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 #                                                                                        =
 #             This file is part of the EDXML Software Development Kit (SDK)              =
 #                       and is released under the MIT License:                           =
 #                         https://opensource.org/licenses/MIT                            =
 #                                                                                        =
 # ========================================================================================
 
-from typing import Dict, Optional
+from typing import Dict, Optional # noqa
 from graphviz import Digraph
 
-import edxml
+import edxml # noqa
 from edxml.logger import log
 from edxml.transcode import RecordTranscoder, NullTranscoder
 from edxml.ontology import Ontology
 from edxml.ontology.visualization import generate_graph_property_concepts
 from edxml.ontology.description import describe_producer_rst
 from edxml.error import EDXMLValidationError
 from edxml.writer import EDXMLWriter
```

### Comparing `edxml-3.0.0.dev2/edxml/transcode/object/__init__.py` & `edxml-3.0.1/edxml/transcode/object/__init__.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/transcode/object/object_test_harness.py` & `edxml-3.0.1/edxml/transcode/object/object_test_harness.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/transcode/object/object_transcoder.py` & `edxml-3.0.1/edxml/transcode/object/object_transcoder.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/transcode/object/object_transcoder_mediator.py` & `edxml-3.0.1/edxml/transcode/object/object_transcoder_mediator.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/transcode/test_harness.py` & `edxml-3.0.1/edxml/transcode/test_harness.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/transcode/transcoder.py` & `edxml-3.0.1/edxml/transcode/transcoder.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/transcode/xml/__init__.py` & `edxml-3.0.1/edxml/transcode/xml/__init__.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/transcode/xml/xml_test_harness.py` & `edxml-3.0.1/edxml/transcode/xml/xml_test_harness.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/transcode/xml/xml_transcoder.py` & `edxml-3.0.1/edxml/transcode/xml/xml_transcoder.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 #                         https://opensource.org/licenses/MIT                            =
 #                                                                                        =
 # ========================================================================================
 
 import re
 import unicodedata
 
-from typing import Dict
+from typing import Dict # noqa
 
 import edxml.transcode
 
 from edxml import EventElement
 from lxml import etree
 from lxml.etree import XPathSyntaxError
```

### Comparing `edxml-3.0.0.dev2/edxml/transcode/xml/xml_transcoder_mediator.py` & `edxml-3.0.1/edxml/transcode/xml/xml_transcoder_mediator.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/util.py` & `edxml-3.0.1/edxml/util.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/edxml/version.py` & `edxml-3.0.1/edxml/version.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,10 +12,10 @@
 # ========================================================================================
 
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
 #
-# Version 3.0.0.dev0:
-__version_info__ = ('3', '0', '0', 'dev2')
+# Version 3.0.1:
+__version_info__ = ('3', '0', '1')
 __version__ = '.'.join(__version_info__)
```

### Comparing `edxml-3.0.0.dev2/edxml/writer.py` & `edxml-3.0.1/edxml/writer.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 to generate EDXML streams.
 
 """
 import edxml_schema
 import sys
 
 from collections import deque
-from typing import Optional
+from typing import Optional # noqa
 from lxml import etree
 from copy import deepcopy
 
 from edxml.error import EDXMLEventValidationError, EDXMLOntologyValidationError
 from edxml.event_validator import EventValidator
 from edxml.ontology import Ontology
 from edxml.logger import log
```

### Comparing `edxml-3.0.0.dev2/edxml.egg-info/SOURCES.txt` & `edxml-3.0.1/edxml.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 LICENSE.rst
 README.rst
 setup.cfg
 setup.py
 edxml/__init__.py
 edxml/error.py
 edxml/event.py
+edxml/event.pyi
 edxml/event_collection.py
 edxml/event_validator.py
 edxml/filter.py
+edxml/filter.pyi
 edxml/logger.py
 edxml/parser.py
+edxml/parser.pyi
 edxml/template.py
 edxml/util.py
 edxml/version.py
 edxml/writer.py
 edxml.egg-info/PKG-INFO
 edxml.egg-info/SOURCES.txt
 edxml.egg-info/dependency_links.txt
```

### Comparing `edxml-3.0.0.dev2/edxml.egg-info/entry_points.txt` & `edxml-3.0.1/edxml.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/setup.py` & `edxml-3.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 from os import path
 
 here = path.abspath(path.dirname(__file__))
-# Get the long description from the relevant file
-# with open(path.join(here, 'DESCRIPTION.rst'), encoding='utf-8') as f:
-#  long_description = f.read()
+
+with open("README.rst", "r") as fh:
+    long_description = fh.read()
 
 # Explicitly state a version to please flake8
 __version__ = 1.0
 # This will read __version__ from edxml/version.py
 exec(compile(open('edxml/version.py', "rb").read(), 'edxml/version.py', 'exec'))
 
 setup(
     name='edxml',
     version=__version__,
 
     # A description of your project
     description='The EDXML Software Development Kit',
-    long_description='Python implementation of the EDXML specification and tools for application development',
+    long_description=long_description,
+    long_description_content_type='text/x-rst',
 
     # The project's main homepage
     url='https://github.com/edxml/sdk',
 
     # Author details
     author='Dik Takken',
     author_email='dik.takken@edxml.org',
@@ -85,21 +86,22 @@
     },
 
     # List run-time dependencies here. These will be installed by pip when your
     # project is installed.
     # See https://pip.pypa.io/en/latest/reference/pip_install.html#requirements-file-format
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/technical.html#install-requires-vs-requirements-files
-    install_requires=['lxml>=3.8', 'python-dateutil', 'edxml-schema==3.0.0.dev3',
-                      'iso3166', 'pytz', 'termcolor', 'graphviz', 'typing', 'pytest',
-                      'ipy', 'coverage', 'edxml-test-corpus==3.0.0.dev4', 'edxml-bricks-computing>=3.0.0.dev0',
-                      'edxml-bricks-computing-networking>=3.0.0.dev0', 'edxml-bricks-generic>=3.0.0.dev0'],
+    install_requires=['lxml>=3.8', 'python-dateutil', 'edxml-schema~=3.0.0',
+                      'pytz', 'termcolor', 'graphviz', 'pytest',
+                      'ipy', 'coverage', 'edxml-test-corpus~=3.0.0'],
 
     # Specify additional packages that are only installed for specific purposes,
     # like building documentation.
     extras_require={
         'doc': [
-            'sphinx',
-            'sphinxcontrib-napoleon'
+            'sphinx<7.0',
+            'edxml-bricks-computing~=3.0.0',
+            'edxml-bricks-computing-networking~=3.0.0',
+            'edxml-bricks-generic~=3.0.0'
         ]
     }
 )
```

### Comparing `edxml-3.0.0.dev2/tests/__init__.py` & `edxml-3.0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/tests/assertions.py` & `edxml-3.0.1/tests/assertions.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/tests/test_event_source.py` & `edxml-3.0.1/tests/test_event_source.py`

 * *Files identical despite different names*

### Comparing `edxml-3.0.0.dev2/tests/test_writer.py` & `edxml-3.0.1/tests/test_writer.py`

 * *Files identical despite different names*

