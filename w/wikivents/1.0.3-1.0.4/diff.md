# Comparing `tmp/wikivents-1.0.3.tar.gz` & `tmp/wikivents-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wikivents-1.0.3.tar", last modified: Fri Apr  9 17:10:35 2021, max compression
+gzip compressed data, was "wikivents-1.0.4.tar", last modified: Tue May 16 17:57:34 2023, max compression
```

## Comparing `wikivents-1.0.3.tar` & `wikivents-1.0.4.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwx------   0 gberna02  (1000) gberna02  (1000)        0 2021-04-09 17:10:35.934011 wikivents-1.0.3/
--rw-------   0 gberna02  (1000) gberna02  (1000)        0 2020-10-21 20:18:20.000000 wikivents-1.0.3/MANIFEST.in
--rw-------   0 gberna02  (1000) gberna02  (1000)    13868 2021-04-09 17:10:35.934011 wikivents-1.0.3/PKG-INFO
--rw-------   0 gberna02  (1000) gberna02  (1000)    10463 2021-04-09 07:01:51.000000 wikivents-1.0.3/README.md
--rw-------   0 gberna02  (1000) gberna02  (1000)       79 2021-04-09 17:10:35.935011 wikivents-1.0.3/setup.cfg
--rwx------   0 gberna02  (1000) gberna02  (1000)     1781 2021-04-09 07:01:51.000000 wikivents-1.0.3/setup.py
-drwx------   0 gberna02  (1000) gberna02  (1000)        0 2021-04-09 17:10:35.932011 wikivents-1.0.3/tests/
--rw-r--r--   0 gberna02  (1000) gberna02  (1000)        0 2020-11-05 09:47:11.000000 wikivents-1.0.3/tests/__init__.py
--rw-------   0 gberna02  (1000) gberna02  (1000)     2995 2021-04-09 07:01:51.000000 wikivents-1.0.3/tests/entity_factory_test.py
--rw-------   0 gberna02  (1000) gberna02  (1000)     2624 2021-04-09 07:01:51.000000 wikivents-1.0.3/tests/entity_type_test.py
--rw-------   0 gberna02  (1000) gberna02  (1000)     6040 2021-04-09 07:01:51.000000 wikivents-1.0.3/tests/event_factory_test.py
-drwx------   0 gberna02  (1000) gberna02  (1000)        0 2021-04-09 17:10:35.932011 wikivents-1.0.3/wikivents/
--rw-------   0 gberna02  (1000) gberna02  (1000)      912 2021-04-09 17:07:00.000000 wikivents-1.0.3/wikivents/__init__.py
-drwx------   0 gberna02  (1000) gberna02  (1000)        0 2021-04-09 17:10:35.933011 wikivents-1.0.3/wikivents/cache/
--rw-------   0 gberna02  (1000) gberna02  (1000)     2863 2021-04-09 07:01:51.000000 wikivents-1.0.3/wikivents/cache/__init__.py
--rw-------   0 gberna02  (1000) gberna02  (1000)      882 2021-04-09 07:01:51.000000 wikivents-1.0.3/wikivents/exc.py
-drwx------   0 gberna02  (1000) gberna02  (1000)        0 2021-04-09 17:10:35.933011 wikivents-1.0.3/wikivents/factories/
--rw-------   0 gberna02  (1000) gberna02  (1000)     4009 2021-04-09 07:01:51.000000 wikivents-1.0.3/wikivents/factories/__init__.py
--rw-------   0 gberna02  (1000) gberna02  (1000)     6297 2021-04-09 16:56:01.000000 wikivents-1.0.3/wikivents/factories/wikimedia.py
--rw-------   0 gberna02  (1000) gberna02  (1000)     4628 2021-04-09 09:37:08.000000 wikivents-1.0.3/wikivents/model_encoders.py
--rw-------   0 gberna02  (1000) gberna02  (1000)    10813 2021-04-09 07:01:51.000000 wikivents-1.0.3/wikivents/models.py
-drwx------   0 gberna02  (1000) gberna02  (1000)        0 2021-04-09 17:10:35.934011 wikivents-1.0.3/wikivents/ontology/
--rw-------   0 gberna02  (1000) gberna02  (1000)     4974 2021-04-09 07:01:51.000000 wikivents-1.0.3/wikivents/ontology/__init__.py
--rw-------   0 gberna02  (1000) gberna02  (1000)      836 2021-04-09 07:01:51.000000 wikivents-1.0.3/wikivents/ontology/exc.py
--rw-------   0 gberna02  (1000) gberna02  (1000)    25659 2021-04-09 07:01:51.000000 wikivents-1.0.3/wikivents/ontology/wikidata.py
-drwx------   0 gberna02  (1000) gberna02  (1000)        0 2021-04-09 17:10:35.934011 wikivents-1.0.3/wikivents/resource/
--rw-------   0 gberna02  (1000) gberna02  (1000)     1486 2021-04-09 07:01:51.000000 wikivents-1.0.3/wikivents/resource/__init__.py
--rw-------   0 gberna02  (1000) gberna02  (1000)      887 2021-04-09 07:01:51.000000 wikivents-1.0.3/wikivents/resource/exc.py
--rw-------   0 gberna02  (1000) gberna02  (1000)    11271 2021-04-09 12:17:09.000000 wikivents-1.0.3/wikivents/resource/wikipedia.py
-drwx------   0 gberna02  (1000) gberna02  (1000)        0 2021-04-09 17:10:35.933011 wikivents-1.0.3/wikivents.egg-info/
--rw-------   0 gberna02  (1000) gberna02  (1000)    13868 2021-04-09 17:10:35.000000 wikivents-1.0.3/wikivents.egg-info/PKG-INFO
--rw-------   0 gberna02  (1000) gberna02  (1000)      662 2021-04-09 17:10:35.000000 wikivents-1.0.3/wikivents.egg-info/SOURCES.txt
--rw-------   0 gberna02  (1000) gberna02  (1000)        1 2021-04-09 17:10:35.000000 wikivents-1.0.3/wikivents.egg-info/dependency_links.txt
--rw-------   0 gberna02  (1000) gberna02  (1000)       68 2021-04-09 17:10:35.000000 wikivents-1.0.3/wikivents.egg-info/requires.txt
--rw-------   0 gberna02  (1000) gberna02  (1000)       16 2021-04-09 17:10:35.000000 wikivents-1.0.3/wikivents.egg-info/top_level.txt
+drwx------   0 gbernard  (1000) gbernard  (1000)        0 2023-05-16 17:57:34.652292 wikivents-1.0.4/
+-rw-------   0 gbernard  (1000) gbernard  (1000)       49 2023-05-16 17:43:01.000000 wikivents-1.0.4/AUTHORS
+-rw-------   0 gbernard  (1000) gbernard  (1000)    35149 2023-05-16 17:43:01.000000 wikivents-1.0.4/LICENSE
+-rw-------   0 gbernard  (1000) gbernard  (1000)        0 2023-05-16 17:43:01.000000 wikivents-1.0.4/MANIFEST.in
+-rw-------   0 gbernard  (1000) gbernard  (1000)    11265 2023-05-16 17:57:34.652292 wikivents-1.0.4/PKG-INFO
+-rw-------   0 gbernard  (1000) gbernard  (1000)    10463 2023-05-16 17:43:01.000000 wikivents-1.0.4/README.md
+-rw-------   0 gbernard  (1000) gbernard  (1000)       79 2023-05-16 17:57:34.652292 wikivents-1.0.4/setup.cfg
+-rwx------   0 gbernard  (1000) gbernard  (1000)     1782 2023-05-16 17:43:01.000000 wikivents-1.0.4/setup.py
+drwx------   0 gbernard  (1000) gbernard  (1000)        0 2023-05-16 17:57:34.650292 wikivents-1.0.4/tests/
+-rw-------   0 gbernard  (1000) gbernard  (1000)        0 2023-05-16 17:43:01.000000 wikivents-1.0.4/tests/__init__.py
+-rw-------   0 gbernard  (1000) gbernard  (1000)     2995 2023-05-16 17:43:01.000000 wikivents-1.0.4/tests/entity_factory_test.py
+-rw-------   0 gbernard  (1000) gbernard  (1000)     2623 2023-05-16 17:43:01.000000 wikivents-1.0.4/tests/entity_type_test.py
+-rw-------   0 gbernard  (1000) gbernard  (1000)     6000 2023-05-16 17:43:01.000000 wikivents-1.0.4/tests/event_factory_test.py
+drwx------   0 gbernard  (1000) gbernard  (1000)        0 2023-05-16 17:57:34.650292 wikivents-1.0.4/wikivents/
+-rw-------   0 gbernard  (1000) gbernard  (1000)      912 2023-05-16 17:54:13.000000 wikivents-1.0.4/wikivents/__init__.py
+drwx------   0 gbernard  (1000) gbernard  (1000)        0 2023-05-16 17:57:34.651292 wikivents-1.0.4/wikivents/cache/
+-rw-------   0 gbernard  (1000) gbernard  (1000)     2859 2023-05-16 17:43:01.000000 wikivents-1.0.4/wikivents/cache/__init__.py
+-rw-------   0 gbernard  (1000) gbernard  (1000)      882 2023-05-16 17:43:01.000000 wikivents-1.0.4/wikivents/exc.py
+drwx------   0 gbernard  (1000) gbernard  (1000)        0 2023-05-16 17:57:34.651292 wikivents-1.0.4/wikivents/factories/
+-rw-------   0 gbernard  (1000) gbernard  (1000)     3981 2023-05-16 17:43:01.000000 wikivents-1.0.4/wikivents/factories/__init__.py
+-rw-------   0 gbernard  (1000) gbernard  (1000)     6335 2023-05-16 17:43:01.000000 wikivents-1.0.4/wikivents/factories/wikimedia.py
+-rw-------   0 gbernard  (1000) gbernard  (1000)     4397 2023-05-16 17:43:01.000000 wikivents-1.0.4/wikivents/model_encoders.py
+-rw-------   0 gbernard  (1000) gbernard  (1000)    12110 2023-05-16 17:43:01.000000 wikivents-1.0.4/wikivents/models.py
+drwx------   0 gbernard  (1000) gbernard  (1000)        0 2023-05-16 17:57:34.651292 wikivents-1.0.4/wikivents/ontology/
+-rw-------   0 gbernard  (1000) gbernard  (1000)     4990 2023-05-16 17:43:01.000000 wikivents-1.0.4/wikivents/ontology/__init__.py
+-rw-------   0 gbernard  (1000) gbernard  (1000)      836 2023-05-16 17:43:01.000000 wikivents-1.0.4/wikivents/ontology/exc.py
+-rw-------   0 gbernard  (1000) gbernard  (1000)    26701 2023-05-16 17:43:01.000000 wikivents-1.0.4/wikivents/ontology/wikidata.py
+drwx------   0 gbernard  (1000) gbernard  (1000)        0 2023-05-16 17:57:34.652292 wikivents-1.0.4/wikivents/resource/
+-rw-------   0 gbernard  (1000) gbernard  (1000)     1502 2023-05-16 17:43:01.000000 wikivents-1.0.4/wikivents/resource/__init__.py
+-rw-------   0 gbernard  (1000) gbernard  (1000)      887 2023-05-16 17:43:01.000000 wikivents-1.0.4/wikivents/resource/exc.py
+-rw-------   0 gbernard  (1000) gbernard  (1000)    11642 2023-05-16 17:43:01.000000 wikivents-1.0.4/wikivents/resource/wikipedia.py
+drwx------   0 gbernard  (1000) gbernard  (1000)        0 2023-05-16 17:57:34.651292 wikivents-1.0.4/wikivents.egg-info/
+-rw-------   0 gbernard  (1000) gbernard  (1000)    11265 2023-05-16 17:57:34.000000 wikivents-1.0.4/wikivents.egg-info/PKG-INFO
+-rw-------   0 gbernard  (1000) gbernard  (1000)      678 2023-05-16 17:57:34.000000 wikivents-1.0.4/wikivents.egg-info/SOURCES.txt
+-rw-------   0 gbernard  (1000) gbernard  (1000)        1 2023-05-16 17:57:34.000000 wikivents-1.0.4/wikivents.egg-info/dependency_links.txt
+-rw-------   0 gbernard  (1000) gbernard  (1000)       68 2023-05-16 17:57:34.000000 wikivents-1.0.4/wikivents.egg-info/requires.txt
+-rw-------   0 gbernard  (1000) gbernard  (1000)       16 2023-05-16 17:57:34.000000 wikivents-1.0.4/wikivents.egg-info/top_level.txt
```

### Comparing `wikivents-1.0.3/PKG-INFO` & `wikivents-1.0.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,346 +1,347 @@
 Metadata-Version: 2.1
 Name: wikivents
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple Python package to represent events from Wikipedia and Wikidata resources.
 Home-page: https://gitlab.com/guilieb/wikivents
 Author: Guillaume Bernard
 Author-email: contact@guillaume-bernard.fr
 License: GPLv3 License
-Description: # `wikivents`
-        
-        This Python package is used to represent events based on both ontologies and semi-structured databases. Up to now, only Wikidata and Wikipedia are implemented and provide these data. The name of this package, `wikivents` show this legacy.
-        
-        ### Events
-        
-        An event is an ontology entity. For Wikidata, an event is an instance of an [occurrence (Q1190554)](https://www.wikidata.org/wiki/Q1190554) or of an [event (Q1656682)](https://www.wikidata.org/wiki/Q1656682).
-        
-        A **event** is defined by few characteristics:
-         * **A type**: on Wikidata, this defines the type of the event. For instance, [rebellion (Q124734)](https://www.wikidata.org/wiki/Q124734) on Wikidata. This information is provided by the `wd:P31` or `rdf:type`, depending on the source.
-         * **Date** of occurrence, converted if necessary in the Gregorian calendar.
-         * **Location where the event happened**.
-         * The entities related to the event. The extraction process is based on semi-strucuted databases, which are processed in search of entities (people involved, places, etc). Entities are counted. This index shows the relevance of the entity in relation to the event. We assume the entities found in multiple lead sections are important entities in the event description.
-        
-        ## Usage
-        
-        The process of gathering data from multiple APIs (ontologies and semi-structured databases) can take a long time. We implemented a cache which speeds up queries and prevents from querying twice the same data.
-        
-        Up to now, the only implemented toolchain is based on Wikimedia foundation projects: Wikidata for the ontology and Wikipedia articles for semi-structured databases. Then it is possible to get the representation of an event using the `WikimediaFactory` object, as in the example below:
-        
-        ```python
-        from wikivents.factories.wikimedia import WikimediaFactory
-        from wikivents.models import EntityId
-        
-        easter_rising_entity_id = EntityId("Q193689")
-        easter_rising_event = WikimediaFactory.create_event(easter_rising_entity_id)
-        ```
-        
-        The previous code takes the [Easter Rising event](https://en.wikipedia.org/wiki/Easter_Rising) entity id (`Q193689`)' as input. If using another `Factory` which processes other ontologies, the entry point will obviously not be the same.
-        
-        From the `easter_rising_event` object, it is possible to access multiple attributes:
-        
-        * The **event identifier**, which comes from the ontology itself:
-        ```python
-        easter_rising_event.id
-        Out[5]: 'Q193689'
-        ```
-        
-        * The **event label**, in any possible language. If unavailable, will return an empty string.
-        ```python
-        easter_rising_event.label("fr")
-        Out[7]: 'Insurrection de Pâques 1916'
-        ```
-        
-        * The **event alternative names**, which means all the names that are used in a specific language to speak about the event.
-        ```python
-        easter_rising_event.names("de")
-        Out[8]: {'Easter Rising', 'Irischer Osteraufstand 1916', 'Osteraufstand'}
-        ```
-        
-        * The **event description**, in plain text.
-        ```python
-        easter_rising_event.description("en")
-        Out[9]: 'an armed insurrection in Ireland during Easter Week, 1916'
-        ```
-        
-        * The **event boundary dates**, beginning and end.
-        ```python
-        easter_rising_event.beginning, easter_rising_event.end
-        Out[12]: (datetime.datetime(1916, 4, 24, 0, 0, tzinfo=datetime.timezone.utc),  datetime.datetime(1916, 4, 30, 0, 0, tzinfo=datetime.timezone.utc))
-        ```
-        
-        * The entities involved, accessible using the `gpe` property for **GPE**, `org` property for **ORG** and `per` property for **PER** entities.
-        ```python
-        easter_rising_event.gpe
-        Out[13]: [ParticipatingEntity(entity=<Entity(Q1761, Dublin)>, count=8),ParticipatingEntity(entity=<Entity(Q27, Ireland)>, count=5)]
-        ```
-        
-        ## Encode events in reusable formats
-        
-        The `wikivents` library also provides encoders which are used to transform the event object into other formats, easier to manipulate. From now on, we provide a `DictEncoder` which make it easy to create a JSON file from it.
-        
-        ```python
-        from wikivents.model_encoders import EventToDictEncoder
-        from wikivents.models import ISO6391LanguageCode
-        
-        encoder = EventToDictEncoder(easter_rising_event, ISO6391LanguageCode("en"))
-        encoder.encode()
-        ```
-        
-        The purpose of encoders is to provide all the possible knowledge acquired about events and to show involved entities. It is also possible to add a parameter to the `encode()` method, `participating_entities_ratio_to_keep` to indicate which entities will be kept. It is a value comprised between 0 and 1. `1` means to keep all the participating entities, `0.5` to keep them only if they were found in at least 50% of the total number of processed semi-structured databases.
-        
-        Below is an example, and the associated JSON output:
-        
-        ```python
-        import json
-        
-        with open("easter_rising_event.json", mode="w") as easter_rising_json_file:
-            json.dump(encoder.encode(), easter_rising_json_file)
-        ```
-        
-        ```json
-        [
-          {
-            "Q193689": {
-              "iso_639_1_language_code": "en",
-              "id": "Q193689",
-              "type": "EVENT",
-              "label": "Easter Rising",
-              "description": "an armed insurrection in Ireland during Easter Week, 1916",
-              "names": [
-                "1916 Rising",
-                "Easter Rebellion",
-                "Easter Rising"
-              ],
-              "processed_languages": [
-                "de",
-                "it",
-                "es",
-                "fr",
-                "en"
-              ],
-              "entities_kept_if_mentioned_in_more_at_least_X_languages": 2.5,
-              "start": "1916-04-24T00:00:00+00:00",
-              "end": "1916-04-30T00:00:00+00:00",
-              "entities": {
-                "per": [
-                  {
-                    "id": "Q213374",
-                    "type": [
-                      "PERSON"
-                    ],
-                    "label": "James Connolly",
-                    "description": "James Connolly",
-                    "names": [
-                      "James Connolly"
-                    ],
-                    "count": 3
-                  },
-                  {
-                    "id": "Q274143",
-                    "type": [
-                      "PERSON"
-                    ],
-                    "label": "Patrick Pearse",
-                    "description": "Patrick Pearse",
-                    "names": [
-                      "Patrick Henry Pearse",
-                      "Patrick Pearse",
-                      "Padraig Pearse"
-                    ],
-                    "count": 3
-                  }
-                ],
-                "gpe": [
-                  {
-                    "id": "Q1761",
-                    "type": [
-                      "GPE"
-                    ],
-                    "label": "Dublin",
-                    "description": "Dublin",
-                    "names": [
-                      "City of Dublin",
-                      "Baile Átha Cliath",
-                      "Dublin",
-                      "Dublin city"
-                    ],
-                    "count": 8
-                  },
-                  {
-                    "id": "Q27",
-                    "type": [
-                      "GPE",
-                      "ORG"
-                    ],
-                    "label": "Ireland",
-                    "description": "Ireland",
-                    "names": [
-                      "🇮🇪",
-                      "Eire",
-                      "Éire",
-                      "Ireland",
-                      "ie",
-                      "ireland",
-                      "IRL",
-                      "Ireland, Republic of",
-                      "Republic of Ireland",
-                      "Hibernia",
-                      "IE",
-                      "Southern Ireland"
-                    ],
-                    "count": 5
-                  },
-                  {
-                    "id": "Q145",
-                    "type": [
-                      "GPE",
-                      "ORG"
-                    ],
-                    "label": "United Kingdom",
-                    "description": "United Kingdom",
-                    "names": [
-                      "G.B.",
-                      "GBR",
-                      "United Kingdom",
-                      "U. K.",
-                      "U K",
-                      "GB",
-                      "UK",
-                      "United Kingdom of Great Britain and Northern Ireland",
-                      "G B R",
-                      "Marea Britanie",
-                      "G. B. R.",
-                      "G B",
-                      "G. B.",
-                      "G.B.R.",
-                      "🇬🇧",
-                      "U.K.",
-                      "Great Britain"
-                    ],
-                    "count": 3
-                  }
-                ],
-                "org": [
-                  {
-                    "id": "Q27",
-                    "type": [
-                      "GPE",
-                      "ORG"
-                    ],
-                    "label": "Ireland",
-                    "description": "Ireland",
-                    "names": [
-                      "🇮🇪",
-                      "Eire",
-                      "Éire",
-                      "Ireland",
-                      "ie",
-                      "ireland",
-                      "IRL",
-                      "Ireland, Republic of",
-                      "Republic of Ireland",
-                      "Hibernia",
-                      "IE",
-                      "Southern Ireland"
-                    ],
-                    "count": 5
-                  },
-                  {
-                    "id": "Q1074958",
-                    "type": [
-                      "ORG"
-                    ],
-                    "label": "Irish Volunteers",
-                    "description": "Irish Volunteers",
-                    "names": [
-                      "Irish Volunteers",
-                      "Irish Volunteer Army",
-                      "Irish Volunteer Force"
-                    ],
-                    "count": 3
-                  },
-                  {
-                    "id": "Q145",
-                    "type": [
-                      "GPE",
-                      "ORG"
-                    ],
-                    "label": "United Kingdom",
-                    "description": "United Kingdom",
-                    "names": [
-                      "G.B.",
-                      "GBR",
-                      "United Kingdom",
-                      "U. K.",
-                      "U K",
-                      "GB",
-                      "UK",
-                      "United Kingdom of Great Britain and Northern Ireland",
-                      "G B R",
-                      "Marea Britanie",
-                      "G. B. R.",
-                      "G B",
-                      "G. B.",
-                      "G.B.R.",
-                      "🇬🇧",
-                      "U.K.",
-                      "Great Britain"
-                    ],
-                    "count": 3
-                  },
-                  {
-                    "id": "Q222595",
-                    "type": [
-                      "ORG"
-                    ],
-                    "label": "British Army",
-                    "description": "British Army",
-                    "names": [
-                      "British Army",
-                      "army of the United Kingdom"
-                    ],
-                    "count": 3
-                  },
-                  {
-                    "id": "Q1190570",
-                    "type": [
-                      "ORG"
-                    ],
-                    "label": "Irish Citizen Army",
-                    "description": "Irish Citizen Army",
-                    "names": [
-                      "Irish Citizen Army"
-                    ],
-                    "count": 3
-                  },
-                  {
-                    "id": "Q427496",
-                    "type": [
-                      "ORG"
-                    ],
-                    "label": "Cumann na mBan",
-                    "description": "Cumann na mBan",
-                    "names": [
-                      "Cumann na mBan",
-                      "CnamB",
-                      "The Irishwomen's Council"
-                    ],
-                    "count": 3
-                  }
-                ]
-              }
-            }
-          }
-        ]
-        ```
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+# `wikivents`
+
+This Python package is used to represent events based on both ontologies and semi-structured databases. Up to now, only Wikidata and Wikipedia are implemented and provide these data. The name of this package, `wikivents` show this legacy.
+
+### Events
+
+An event is an ontology entity. For Wikidata, an event is an instance of an [occurrence (Q1190554)](https://www.wikidata.org/wiki/Q1190554) or of an [event (Q1656682)](https://www.wikidata.org/wiki/Q1656682).
+
+A **event** is defined by few characteristics:
+ * **A type**: on Wikidata, this defines the type of the event. For instance, [rebellion (Q124734)](https://www.wikidata.org/wiki/Q124734) on Wikidata. This information is provided by the `wd:P31` or `rdf:type`, depending on the source.
+ * **Date** of occurrence, converted if necessary in the Gregorian calendar.
+ * **Location where the event happened**.
+ * The entities related to the event. The extraction process is based on semi-strucuted databases, which are processed in search of entities (people involved, places, etc). Entities are counted. This index shows the relevance of the entity in relation to the event. We assume the entities found in multiple lead sections are important entities in the event description.
+
+## Usage
+
+The process of gathering data from multiple APIs (ontologies and semi-structured databases) can take a long time. We implemented a cache which speeds up queries and prevents from querying twice the same data.
+
+Up to now, the only implemented toolchain is based on Wikimedia foundation projects: Wikidata for the ontology and Wikipedia articles for semi-structured databases. Then it is possible to get the representation of an event using the `WikimediaFactory` object, as in the example below:
+
+```python
+from wikivents.factories.wikimedia import WikimediaFactory
+from wikivents.models import EntityId
+
+easter_rising_entity_id = EntityId("Q193689")
+easter_rising_event = WikimediaFactory.create_event(easter_rising_entity_id)
+```
+
+The previous code takes the [Easter Rising event](https://en.wikipedia.org/wiki/Easter_Rising) entity id (`Q193689`)' as input. If using another `Factory` which processes other ontologies, the entry point will obviously not be the same.
+
+From the `easter_rising_event` object, it is possible to access multiple attributes:
+
+* The **event identifier**, which comes from the ontology itself:
+```python
+easter_rising_event.id
+Out[5]: 'Q193689'
+```
+
+* The **event label**, in any possible language. If unavailable, will return an empty string.
+```python
+easter_rising_event.label("fr")
+Out[7]: 'Insurrection de Pâques 1916'
+```
+
+* The **event alternative names**, which means all the names that are used in a specific language to speak about the event.
+```python
+easter_rising_event.names("de")
+Out[8]: {'Easter Rising', 'Irischer Osteraufstand 1916', 'Osteraufstand'}
+```
+
+* The **event description**, in plain text.
+```python
+easter_rising_event.description("en")
+Out[9]: 'an armed insurrection in Ireland during Easter Week, 1916'
+```
+
+* The **event boundary dates**, beginning and end.
+```python
+easter_rising_event.beginning, easter_rising_event.end
+Out[12]: (datetime.datetime(1916, 4, 24, 0, 0, tzinfo=datetime.timezone.utc),  datetime.datetime(1916, 4, 30, 0, 0, tzinfo=datetime.timezone.utc))
+```
+
+* The entities involved, accessible using the `gpe` property for **GPE**, `org` property for **ORG** and `per` property for **PER** entities.
+```python
+easter_rising_event.gpe
+Out[13]: [ParticipatingEntity(entity=<Entity(Q1761, Dublin)>, count=8),ParticipatingEntity(entity=<Entity(Q27, Ireland)>, count=5)]
+```
+
+## Encode events in reusable formats
+
+The `wikivents` library also provides encoders which are used to transform the event object into other formats, easier to manipulate. From now on, we provide a `DictEncoder` which make it easy to create a JSON file from it.
+
+```python
+from wikivents.model_encoders import EventToDictEncoder
+from wikivents.models import ISO6391LanguageCode
+
+encoder = EventToDictEncoder(easter_rising_event, ISO6391LanguageCode("en"))
+encoder.encode()
+```
+
+The purpose of encoders is to provide all the possible knowledge acquired about events and to show involved entities. It is also possible to add a parameter to the `encode()` method, `participating_entities_ratio_to_keep` to indicate which entities will be kept. It is a value comprised between 0 and 1. `1` means to keep all the participating entities, `0.5` to keep them only if they were found in at least 50% of the total number of processed semi-structured databases.
+
+Below is an example, and the associated JSON output:
+
+```python
+import json
+
+with open("easter_rising_event.json", mode="w") as easter_rising_json_file:
+    json.dump(encoder.encode(), easter_rising_json_file)
+```
+
+```json
+[
+  {
+    "Q193689": {
+      "iso_639_1_language_code": "en",
+      "id": "Q193689",
+      "type": "EVENT",
+      "label": "Easter Rising",
+      "description": "an armed insurrection in Ireland during Easter Week, 1916",
+      "names": [
+        "1916 Rising",
+        "Easter Rebellion",
+        "Easter Rising"
+      ],
+      "processed_languages": [
+        "de",
+        "it",
+        "es",
+        "fr",
+        "en"
+      ],
+      "entities_kept_if_mentioned_in_more_at_least_X_languages": 2.5,
+      "start": "1916-04-24T00:00:00+00:00",
+      "end": "1916-04-30T00:00:00+00:00",
+      "entities": {
+        "per": [
+          {
+            "id": "Q213374",
+            "type": [
+              "PERSON"
+            ],
+            "label": "James Connolly",
+            "description": "James Connolly",
+            "names": [
+              "James Connolly"
+            ],
+            "count": 3
+          },
+          {
+            "id": "Q274143",
+            "type": [
+              "PERSON"
+            ],
+            "label": "Patrick Pearse",
+            "description": "Patrick Pearse",
+            "names": [
+              "Patrick Henry Pearse",
+              "Patrick Pearse",
+              "Padraig Pearse"
+            ],
+            "count": 3
+          }
+        ],
+        "gpe": [
+          {
+            "id": "Q1761",
+            "type": [
+              "GPE"
+            ],
+            "label": "Dublin",
+            "description": "Dublin",
+            "names": [
+              "City of Dublin",
+              "Baile Átha Cliath",
+              "Dublin",
+              "Dublin city"
+            ],
+            "count": 8
+          },
+          {
+            "id": "Q27",
+            "type": [
+              "GPE",
+              "ORG"
+            ],
+            "label": "Ireland",
+            "description": "Ireland",
+            "names": [
+              "🇮🇪",
+              "Eire",
+              "Éire",
+              "Ireland",
+              "ie",
+              "ireland",
+              "IRL",
+              "Ireland, Republic of",
+              "Republic of Ireland",
+              "Hibernia",
+              "IE",
+              "Southern Ireland"
+            ],
+            "count": 5
+          },
+          {
+            "id": "Q145",
+            "type": [
+              "GPE",
+              "ORG"
+            ],
+            "label": "United Kingdom",
+            "description": "United Kingdom",
+            "names": [
+              "G.B.",
+              "GBR",
+              "United Kingdom",
+              "U. K.",
+              "U K",
+              "GB",
+              "UK",
+              "United Kingdom of Great Britain and Northern Ireland",
+              "G B R",
+              "Marea Britanie",
+              "G. B. R.",
+              "G B",
+              "G. B.",
+              "G.B.R.",
+              "🇬🇧",
+              "U.K.",
+              "Great Britain"
+            ],
+            "count": 3
+          }
+        ],
+        "org": [
+          {
+            "id": "Q27",
+            "type": [
+              "GPE",
+              "ORG"
+            ],
+            "label": "Ireland",
+            "description": "Ireland",
+            "names": [
+              "🇮🇪",
+              "Eire",
+              "Éire",
+              "Ireland",
+              "ie",
+              "ireland",
+              "IRL",
+              "Ireland, Republic of",
+              "Republic of Ireland",
+              "Hibernia",
+              "IE",
+              "Southern Ireland"
+            ],
+            "count": 5
+          },
+          {
+            "id": "Q1074958",
+            "type": [
+              "ORG"
+            ],
+            "label": "Irish Volunteers",
+            "description": "Irish Volunteers",
+            "names": [
+              "Irish Volunteers",
+              "Irish Volunteer Army",
+              "Irish Volunteer Force"
+            ],
+            "count": 3
+          },
+          {
+            "id": "Q145",
+            "type": [
+              "GPE",
+              "ORG"
+            ],
+            "label": "United Kingdom",
+            "description": "United Kingdom",
+            "names": [
+              "G.B.",
+              "GBR",
+              "United Kingdom",
+              "U. K.",
+              "U K",
+              "GB",
+              "UK",
+              "United Kingdom of Great Britain and Northern Ireland",
+              "G B R",
+              "Marea Britanie",
+              "G. B. R.",
+              "G B",
+              "G. B.",
+              "G.B.R.",
+              "🇬🇧",
+              "U.K.",
+              "Great Britain"
+            ],
+            "count": 3
+          },
+          {
+            "id": "Q222595",
+            "type": [
+              "ORG"
+            ],
+            "label": "British Army",
+            "description": "British Army",
+            "names": [
+              "British Army",
+              "army of the United Kingdom"
+            ],
+            "count": 3
+          },
+          {
+            "id": "Q1190570",
+            "type": [
+              "ORG"
+            ],
+            "label": "Irish Citizen Army",
+            "description": "Irish Citizen Army",
+            "names": [
+              "Irish Citizen Army"
+            ],
+            "count": 3
+          },
+          {
+            "id": "Q427496",
+            "type": [
+              "ORG"
+            ],
+            "label": "Cumann na mBan",
+            "description": "Cumann na mBan",
+            "names": [
+              "Cumann na mBan",
+              "CnamB",
+              "The Irishwomen's Council"
+            ],
+            "count": 3
+          }
+        ]
+      }
+    }
+  }
+]
+```
```

### Comparing `wikivents-1.0.3/README.md` & `wikivents-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `wikivents-1.0.3/setup.py` & `wikivents-1.0.4/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,53 +3,53 @@
 import os
 import re
 from datetime import datetime
 from typing import List
 
 from setuptools import find_packages, setup
 
-with open(os.path.join(os.path.dirname(__file__), 'README.md'), encoding='utf-8') as readme:
+with open(os.path.join(os.path.dirname(__file__), "README.md"), encoding="utf-8") as readme:
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 
 def get_requirements() -> List[str]:
     req = list()
-    with open('requirements.txt') as requirements:
+    with open("requirements.txt") as requirements:
         pattern = re.compile(r"^.*#egg=([\w]+)$")
         for line in requirements.read().splitlines():
             if pattern.match(line):
                 req.append(pattern.findall(line)[0])
             else:
                 req.append(line)
     return req
 
 
-exec(open('wikivents/__init__.py').read())
+exec(open("wikivents/__init__.py").read())
 
 # noinspection PyUnresolvedReferences
 setup(
-    name='wikivents',
+    name="wikivents",
     version=__version__,
     packages=find_packages(),
     include_package_data=True,
-    license='GPLv3 License',
-    description='A simple Python package to represent events from Wikipedia and Wikidata resources.',
+    license="GPLv3 License",
+    description="A simple Python package to represent events from Wikipedia and Wikidata resources.",
     long_description=README,
     long_description_content_type="text/markdown",
-    url='https://gitlab.com/guilieb/wikivents',
-    author='Guillaume Bernard',
-    author_email='contact@guillaume-bernard.fr',
+    url="https://gitlab.com/guilieb/wikivents",
+    author="Guillaume Bernard",
+    author_email="contact@guillaume-bernard.fr",
     classifiers=[
-        'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
-        'Intended Audience :: Developers',
-        'Intended Audience :: Education',
-        'Topic :: Scientific/Engineering :: Information Analysis',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
+        "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+        "Intended Audience :: Developers",
+        "Intended Audience :: Education",
+        "Topic :: Scientific/Engineering :: Information Analysis",
+        "Operating System :: OS Independent",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
     ],
-    install_requires=get_requirements()
+    install_requires=get_requirements(),
 )
```

### Comparing `wikivents-1.0.3/tests/entity_factory_test.py` & `wikivents-1.0.4/tests/entity_factory_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,26 +19,25 @@
 
 from wikivents.factories.wikimedia import WikimediaFactory
 from wikivents.models import EntityId, EntityType, ISO6391LanguageCode
 from wikivents.ontology.wikidata import WikidataOntologyRepository
 
 
 class EntityFactoryTest(unittest.TestCase):
-
     def setUp(self) -> None:
         self.san_francisco_wikidata_id = EntityId("Q62")
         self.easter_rising_wikidata_id = EntityId("Q193689")
 
     def test_san_francisco_entity_labels_and_names(self):
         san_francisco_entity = WikimediaFactory.create_entity(self.san_francisco_wikidata_id)
         self.assertEqual("San Francisco", san_francisco_entity.label(ISO6391LanguageCode("en")))
         self.assertIsInstance(san_francisco_entity.names(ISO6391LanguageCode("en")), set)
         self.assertEqual(
             "consolidated city-county in California, United States",
-            san_francisco_entity.description(ISO6391LanguageCode("en"))
+            san_francisco_entity.description(ISO6391LanguageCode("en")),
         )
 
     def test_san_francisco_entity_type_is_gpe(self):
         san_francisco_entity = WikimediaFactory.create_entity(self.san_francisco_wikidata_id)
         self.assertIn(EntityType.GPE, san_francisco_entity.types())
 
     def test_easter_rising_types_contain_rebellion_and_occurrence(self):
@@ -55,9 +54,9 @@
         easter_rising_entity = WikimediaFactory.create_entity(self.easter_rising_wikidata_id)
         self.assertEqual(1, len(easter_rising_entity.types_as_entities()))
 
         rebellion_wikidata_id = EntityId("Q124734")
         self.assertEqual(rebellion_wikidata_id, list(easter_rising_entity.types_as_entities())[0].id)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `wikivents-1.0.3/tests/entity_type_test.py` & `wikivents-1.0.4/tests/entity_type_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 #
 import unittest
 
 from wikivents.models import EntityType, EntityId
 
 
 class TestEntityType(unittest.TestCase):
-
     def setUp(self) -> None:
         self.human_wikidata_id = EntityId("Q5")
         self.organisation_wikidata_id = EntityId("Q43229")
         self.position_wikidata_id = EntityId("Q4164871")
         self.locality_wikidata_id = EntityId("Q3257686")
         self.country_wikidata_id = EntityId("Q6256")
         self.territorial_entity_wikidata_id = EntityId("Q56061")
@@ -56,9 +55,9 @@
     def test_entity_type_Q1190554_occurrence_is_an_event(self):
         self.assertIn(EntityType.EVENT, EntityType.get_types({self.occurrence_wikidata_id}))
 
     def test_entity_type_Q56061_event_is_an_event(self):
         self.assertIn(EntityType.EVENT, EntityType.get_types({self.event_wikidata_id}))
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `wikivents-1.0.3/tests/event_factory_test.py` & `wikivents-1.0.4/tests/event_factory_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,38 +19,35 @@
 
 from wikivents.factories import CallbackMessageHandler, LoggingCallbackMessageHandler
 from wikivents.factories.wikimedia import WikimediaFactory
 from wikivents.models import EntityId, ISO6391LanguageCode
 
 
 class FactoriesTest(unittest.TestCase):
-
     def setUp(self) -> None:
         self.san_francisco_wikidata_id = EntityId("Q62")
         self.easter_rising_wikidata_id = EntityId("Q193689")
         self.russian_revolution_wikidata_id = EntityId("Q8729")
 
     def test_easter_rising_labels_and_names(self):
         easter_rising = WikimediaFactory.create_event(self.easter_rising_wikidata_id)
         self.assertEqual("Easter Rising", easter_rising.label(ISO6391LanguageCode("en")))
         self.assertEqual("Insurrection de Pâques 1916", easter_rising.label(ISO6391LanguageCode("fr")))
         self.assertEqual(
             "an armed insurrection in Ireland during Easter Week, 1916",
-            easter_rising.description(ISO6391LanguageCode("en"))
+            easter_rising.description(ISO6391LanguageCode("en")),
         )
         self.assertEqual(
             "Ribellione avvenuta in Irlanda durante la settimana di Pasqua del 1916",
-            easter_rising.description(ISO6391LanguageCode("it"))
+            easter_rising.description(ISO6391LanguageCode("it")),
         )
 
     def test_easter_rising_places(self):
         easter_rising = WikimediaFactory.create_event(self.easter_rising_wikidata_id)
-        places_labels = {
-            place_label.id for place_label in easter_rising.places()
-        }
+        places_labels = {place_label.id for place_label in easter_rising.places()}
         united_kingdom_of_great_britain_and_ireland, dublin = EntityId("Q174193"), EntityId("Q1761")
         self.assertIn(united_kingdom_of_great_britain_and_ireland, places_labels)
         self.assertIn(dublin, places_labels)
 
     def test_easter_rising_participants(self):
         easter_rising = WikimediaFactory.create_event(self.easter_rising_wikidata_id)
         self.assertIsInstance(easter_rising.participants(), set)
@@ -69,41 +66,39 @@
 
     def test_russian_revolution_labels_and_names(self):
         russian_revolution = WikimediaFactory.create_event(self.russian_revolution_wikidata_id)
         self.assertEqual("Russian Revolution", russian_revolution.label(ISO6391LanguageCode("en")))
         self.assertEqual("Revolución rusa", russian_revolution.label(ISO6391LanguageCode("es")))
         self.assertEqual(
             "20th-century revolution leading to the downfall of the Russian monarchy",
-            russian_revolution.description(ISO6391LanguageCode("en"))
+            russian_revolution.description(ISO6391LanguageCode("en")),
         )
         self.assertEqual(
             "révolution du XXe siècle marquant l'arrivée au pouvoir des communistes",
-            russian_revolution.description(ISO6391LanguageCode("fr"))
+            russian_revolution.description(ISO6391LanguageCode("fr")),
         )
 
     def test_russian_revolution_places(self):
         russian_revolution = WikimediaFactory.create_event(self.russian_revolution_wikidata_id)
-        places_labels = {
-            place_label.id for place_label in russian_revolution.places()
-        }
+        places_labels = {place_label.id for place_label in russian_revolution.places()}
         russian_empire = EntityId("Q34266")
         self.assertIn(russian_empire, places_labels)
 
     def test_russian_revolution_participants(self):
         russian_revolution = WikimediaFactory.create_event(self.russian_revolution_wikidata_id)
         self.assertIsInstance(russian_revolution.participants(), set)
         self.assertIsInstance(russian_revolution.gpe, list)
         self.assertIsInstance(russian_revolution.per, list)
         self.assertIsInstance(russian_revolution.org, list)
 
     def test_russian_revolution_processed_languages(self):
         russian_revolution = WikimediaFactory.create_event(self.russian_revolution_wikidata_id)
         self.assertEqual(
             {"es", "it", "en", "fr", "de", "ru", "fi", "pl", "sv"},
-            russian_revolution.processed_languages_iso_639_1_codes
+            russian_revolution.processed_languages_iso_639_1_codes,
         )
 
     def test_russian_revolution_dates(self):
         russian_revolution = WikimediaFactory.create_event(self.russian_revolution_wikidata_id)
         self.assertEqual("1917-01-01T00:00:00+00:00", russian_revolution.beginning.isoformat())
         with self.assertRaises(ValueError):
             russian_revolution.end
@@ -121,9 +116,9 @@
             self.count += 1
 
         self.count = 0
         WikimediaFactory.create_event(EntityId("Q193689"), LoggingCallbackMessageHandler(callback))
         self.assertEqual(self.count, 9)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `wikivents-1.0.3/wikivents/__init__.py` & `wikivents-1.0.4/wikivents/resource/exc.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,17 +11,16 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
+from wikivents.exc import WikiventsError
 
-__version_info__ = {
-    "number": {
-        "major": "1",
-        "minor": "0",
-        "revision": "3",
-    }
-}
 
-__version__ = ".".join(list(__version_info__.get("number").values()))
+class ResourceInLanguageDoesNotExist(WikiventsError):
+    pass
+
+
+class ResourceDoesNotExist(WikiventsError):
+    pass
```

### Comparing `wikivents-1.0.3/wikivents/cache/__init__.py` & `wikivents-1.0.4/wikivents/cache/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,26 +23,24 @@
 # The security risk is taken into account, this means ignored.
 import dill  # nosec
 
 from wikivents.exc import NotInCacheException
 
 
 class AbstractCachePath(abc.ABC):
-
     @abc.abstractmethod
     def get_filepath(self, path_directories_and_filename: Tuple[str]) -> Path:
         pass
 
     @abc.abstractmethod
     def expire(self):
         pass
 
 
 class CachePath(AbstractCachePath):
-
     def __init__(self, specific_cache_directory_name: str, suffix: str):
         self.__base_path = Path.home().joinpath(".cache", "wikivents", specific_cache_directory_name)
         self.__suffix = suffix
         if self.__base_path.exists():
             self.__base_path.mkdir(parents=True, exist_ok=True)
 
     def get_filepath(self, path_directories_and_filename: List[str]) -> Path:
@@ -51,26 +49,24 @@
         return file_path.with_suffix(self.__suffix)
 
     def expire(self):
         shutil.rmtree(self.__base_path)
 
 
 class Cache(abc.ABC):
-
     @abc.abstractmethod
     def _get_data_else_raise_exception(self, data_identifiers: List[str]) -> Any:
         pass
 
     @abc.abstractmethod
     def _set_data(self, data_identifiers: List[str], data: Any):
         pass
 
 
 class DillCache(Cache):
-
     def __init__(self, specific_cache_directory_name: str):
         self.__cache_path = CachePath(specific_cache_directory_name, ".dill")
 
     def _get_data_else_raise_exception(self, data_identifiers: List[str]) -> Any:
         input_path_file = self.__cache_path.get_filepath(data_identifiers)
         if input_path_file.exists():
             with open(input_path_file, mode="rb") as input_file:
```

### Comparing `wikivents-1.0.3/wikivents/exc.py` & `wikivents-1.0.4/wikivents/exc.py`

 * *Files identical despite different names*

### Comparing `wikivents-1.0.3/wikivents/factories/__init__.py` & `wikivents-1.0.4/wikivents/factories/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 from progress.bar import IncrementalBar
 
 from wikivents.models import EntityId, Entity, Event
 
 
 class Factory(abc.ABC):
-
     @classmethod
     @abc.abstractmethod
     def create_entity(cls, entity_id: EntityId) -> Entity:
         pass
 
     @classmethod
     @abc.abstractmethod
@@ -39,15 +38,14 @@
     @staticmethod
     @abc.abstractmethod
     def get_instance() -> "Factory":
         pass
 
 
 class MessageHandler(abc.ABC):
-
     @property
     def number_of_steps(self) -> int:
         return self._number_of_steps
 
     def add_number_of_steps(self, number_of_steps: int):
         if number_of_steps > 0:
             self._number_of_steps += number_of_steps
@@ -62,69 +60,63 @@
 
     @abc.abstractmethod
     def debug(self, message: str):
         pass
 
 
 class LoggingMessageHandler(MessageHandler):
-
     def __init__(self):
         super().__init__()
         self._logger = logging.getLogger(__name__)
         console_handler = logging.StreamHandler()
-        console_handler.setFormatter(logging.Formatter(
-            "%(asctime)s - %(name)s - %(levelname)s - %(funcName)s in %(module)s − %(message)s")
+        console_handler.setFormatter(
+            logging.Formatter("%(asctime)s - %(name)s - %(levelname)s - %(funcName)s in %(module)s − %(message)s")
         )
         self._logger.addHandler(console_handler)
         self._logger.setLevel(logging.DEBUG)
 
     def info(self, message: str):
         self._logger.info("%s: %d/%d", message, self._step_process_number, self._number_of_steps)
         self._step_process_number += 1
 
     def debug(self, message: str):
         self._logger.debug("%s: %d/%d", message, self._step_process_number, self._number_of_steps)
 
 
 class CallbackMessageHandler(MessageHandler):
-
     def __init__(self, callback: Callable[[str, int, int], None] = lambda *args, **kwargs: None):
         super().__init__()
         self._callback = callback
 
     def info(self, message: str):
         self._callback(message, self._step_process_number, self._number_of_steps)
         self._step_process_number += 1
 
     def debug(self, message: str):
         pass
 
 
 class LoggingCallbackMessageHandler(LoggingMessageHandler, CallbackMessageHandler):
-
     def __init__(self, callback: Callable[[str, int, int], None] = lambda *args, **kwargs: None):
         LoggingMessageHandler.__init__(self)
         CallbackMessageHandler.__init__(self, callback)
 
     def info(self, message: str):
         self._callback(message, self._step_process_number, self._number_of_steps)
         self._logger.info("%s: %d/%d", message, self._step_process_number, self._number_of_steps)
         self._step_process_number += 1
 
     def debug(self, message: str):
         self._logger.debug("%s: %d/%d", message, self._step_process_number, self._number_of_steps)
 
 
 class ProgressBarHandler(MessageHandler):
-
     def __init__(self):
         super().__init__()
-        self._bar = IncrementalBar(
-            "Event definition progress", max=self.number_of_steps, suffix="%(percent)d%%"
-        )
+        self._bar = IncrementalBar("Event definition progress", max=self.number_of_steps, suffix="%(percent)d%%")
 
     def info(self, message: str):
         self._bar.max = self.number_of_steps
         self._bar.next()
 
     def debug(self, message: str):
         pass
```

### Comparing `wikivents-1.0.3/wikivents/factories/wikimedia.py` & `wikivents-1.0.4/wikivents/factories/wikimedia.py`

 * *Files 9% similar despite different names*

```diff
@@ -11,31 +11,36 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
+from collections import defaultdict
 from typing import Set
 
 from wikivents.factories import Factory, MessageHandler, LoggingMessageHandler
 from wikivents.ontology.wikidata import WikidataOntologyRepository
 from wikivents.models import Entity, EntityId, ISO6391LanguageCode, Event, Resource, ParticipatingEntity
 from wikivents.ontology import EventData
 from wikivents.resource.exc import ResourceInLanguageDoesNotExist
 from wikivents.resource.wikipedia import WikipediaResourceRepository
 
 
 class WikimediaFactory(Factory):
 
-    __DEFAULT_LANGUAGES = frozenset([
-        ISO6391LanguageCode("en"), ISO6391LanguageCode("fr"),
-        ISO6391LanguageCode("de"), ISO6391LanguageCode("it"),
-        ISO6391LanguageCode("es")
-    ])
+    __DEFAULT_LANGUAGES = frozenset(
+        [
+            ISO6391LanguageCode("en"),
+            ISO6391LanguageCode("fr"),
+            ISO6391LanguageCode("de"),
+            ISO6391LanguageCode("it"),
+            ISO6391LanguageCode("es"),
+        ]
+    )
 
     repository = WikidataOntologyRepository()
     resources_repositories = dict()
 
     @staticmethod
     def get_instance() -> "Factory":
         return WikimediaFactory()
@@ -53,17 +58,15 @@
         message_handler.info("Retrieving entity data from the repository")
         languages = cls.repository.get_official_languages_spoken_where_event_happened(event_data.id)
         cls.__initialize_resource_repositories(languages)
 
         message_handler.info("Retrieving connected entity resources to get more information about the event")
         resources = cls.__get_event_resources(event_data, languages)
         message_handler.add_number_of_steps(len(resources))
-        message_handler.debug(
-            f"There are {len(resources)} resources found for the event ‘{event_data.id}’."
-        )
+        message_handler.debug(f"There are {len(resources)} resources found for the event ‘{event_data.id}’.")
 
         entity = Entity(event_data, resources)
 
         message_handler.info("Retrieving event participants")
         participants = cls.__get_event_participants(resources, message_handler)
         message_handler.info(f"There are {len(participants)} participants found for this event")
 
@@ -82,30 +85,30 @@
 
     @classmethod
     def __initialize_resource_repositories(cls, spoken_languages_iso_639_1_codes: Set[ISO6391LanguageCode]):
         for spoken_language_iso_639_1_code in spoken_languages_iso_639_1_codes | cls.__DEFAULT_LANGUAGES:
             try:
                 if spoken_language_iso_639_1_code not in cls.resources_repositories:
                     cls.resources_repositories[
-                        ISO6391LanguageCode(spoken_language_iso_639_1_code)] = WikipediaResourceRepository(
-                        spoken_language_iso_639_1_code, cls.repository
-                    )
+                        ISO6391LanguageCode(spoken_language_iso_639_1_code)
+                    ] = WikipediaResourceRepository(spoken_language_iso_639_1_code, cls.repository)
             except ResourceInLanguageDoesNotExist:
                 pass
 
     @classmethod
     def __get_event_places(cls, event_data: EventData) -> Set[Entity]:
         places = set()
         for event_place_id in event_data.places:
             places.add(cls.create_entity(event_place_id))
         return places
 
     @classmethod
-    def __get_event_resources(cls, event_data: EventData,
-                              spoken_languages_iso_639_1_codes: Set[ISO6391LanguageCode]) -> Set[Resource]:
+    def __get_event_resources(
+        cls, event_data: EventData, spoken_languages_iso_639_1_codes: Set[ISO6391LanguageCode]
+    ) -> Set[Resource]:
         resources = set()
         site_links = event_data.resource_names
         for spoken_language_iso_639_1_code in spoken_languages_iso_639_1_codes | cls.__DEFAULT_LANGUAGES:
             wiki_language = ISO6391LanguageCode(f"{spoken_language_iso_639_1_code}wiki")
             if wiki_language in site_links:
                 resources.add(
                     cls.resources_repositories.get(spoken_language_iso_639_1_code).get_resource_from_label(
@@ -116,25 +119,28 @@
 
     @classmethod
     def __get_event_participants(cls, resources: Set[Resource], logger: MessageHandler) -> Set[ParticipatingEntity]:
         participating_entities_with_duplicates = set()
         for resource in resources:
             logger.info(f"Retrieving participating entities for resource ’{resource}’.")
             participating_entities_with_duplicates.update(
-                cls.resources_repositories[resource.iso_639_1_language()].get_participating_entities(resource)
+                cls.resources_repositories[resource.iso_639_1_language()].get_participating_entities_count_by_language(
+                    resource
+                )
+            )
+            logger.debug(
+                f"There are now {len(participating_entities_with_duplicates)} entities " f"participating in the event"
             )
-            logger.debug(f"There are now {len(participating_entities_with_duplicates)} entities "
-                         f"participating in the event")
 
-        participating_entities_count = dict()
+        participating_entities_found_in_languages = defaultdict(set)
         for participating_entity in participating_entities_with_duplicates:
             entity = participating_entity.entity
-            if entity not in participating_entities_count:
-                participating_entities_count[entity] = participating_entity.count
-            else:
-                participating_entities_count[entity] += participating_entity.count
+            participating_entities_found_in_languages[entity].add(participating_entity.language)
 
         participating_entities = set()
-        for entity, entity_count in participating_entities_count.items():
-            participating_entities.add(ParticipatingEntity(entity, entity_count))
+        for (
+            entity,
+            entity_language_list,
+        ) in participating_entities_found_in_languages.items():
+            participating_entities.add(ParticipatingEntity(entity, len(entity_language_list)))
 
         return participating_entities
```

### Comparing `wikivents-1.0.3/wikivents/model_encoders.py` & `wikivents-1.0.4/wikivents/model_encoders.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,21 +18,20 @@
 import abc
 from typing import Dict, Any
 
 from wikivents.models import ParticipatingEntity, ISO6391LanguageCode, EntityType, Event
 
 
 class EventEncoder(abc.ABC):
-
     def __init__(self, event: Event, iso_639_1_language_code: ISO6391LanguageCode):
         self.event = event
         self.iso_639_1_language_code = iso_639_1_language_code
 
     @abc.abstractmethod
-    def encode(self, participating_entities_ratio_to_keep: float = 0.5) -> Dict[str, Dict[str, Any]]:
+    def encode(self, keep_entities_if_present_in_at_least_x_languages: int = 2) -> Dict[str, Dict[str, Any]]:
         pass
 
     def _get_start_date_or_empty(self) -> str:
         try:
             beginning = self.event.beginning.isoformat()
         except ValueError:
             beginning = str()
@@ -43,60 +42,59 @@
             end = self.event.end.isoformat()
         except ValueError:
             end = str()
         return end
 
 
 class EventToDictEncoder(EventEncoder):
-
-    def encode(self, participating_entities_ratio_to_keep: float = 0.5) -> Dict[str, Dict[str, Any]]:
-        if participating_entities_ratio_to_keep < 0 or participating_entities_ratio_to_keep > 1.0:
-            raise ValueError(f"The participating entities ratio to keep should be comprised between 0 and 1"
-                             f" ({participating_entities_ratio_to_keep}) given.")
+    def encode(self, keep_entities_if_present_in_at_least_x_languages: int = 2) -> Dict[str, Dict[str, Any]]:
         return {
             self.event.id: {
                 "iso_639_1_language_code": self.iso_639_1_language_code,
                 "id": self.event.id,
                 "type": EntityType.EVENT.name,
                 "label": self.event.label(self.iso_639_1_language_code),
                 "description": self.event.description(self.iso_639_1_language_code),
                 "names": list(self.event.names(self.iso_639_1_language_code)),
                 "processed_languages": list(self.event.processed_languages_iso_639_1_codes),
-                "entities_kept_if_mentioned_in_more_at_least_X_languages":
-                    self.event.nb_of_processed_languages * participating_entities_ratio_to_keep,
+                "entities_kept_if_in_more_than_X_languages": keep_entities_if_present_in_at_least_x_languages,
                 "start": self._get_start_date_or_empty(),
                 "end": self._get_end_date_or_empty(),
                 "entities": {
                     "per": [
                         self.__get_participating_dict(participating_per, self.iso_639_1_language_code)
                         for participating_per in self.event.entities(
-                            EntityType.PERSON, participating_entities_ratio_to_keep
+                            EntityType.PERSON,
+                            keep_entities_if_present_in_at_least_x_languages,
                         )
                     ],
                     "gpe": [
                         self.__get_participating_dict(participating_gpe, self.iso_639_1_language_code)
                         for participating_gpe in self.event.entities(
-                            EntityType.GPE, participating_entities_ratio_to_keep
+                            EntityType.GPE,
+                            keep_entities_if_present_in_at_least_x_languages,
                         )
                     ],
                     "org": [
                         self.__get_participating_dict(participating_org, self.iso_639_1_language_code)
                         for participating_org in self.event.entities(
-                            EntityType.ORG, participating_entities_ratio_to_keep
+                            EntityType.ORG,
+                            keep_entities_if_present_in_at_least_x_languages,
                         )
                     ],
-                }
+                },
             }
         }
 
     # pylint: disable=no-self-use
     # noinspection PyMethodMayBeStatic
-    def __get_participating_dict(self, participating_entity: ParticipatingEntity,
-                                 iso_639_1_language_code: ISO6391LanguageCode) -> Dict[str, Any]:
+    def __get_participating_dict(
+        self, participating_entity: ParticipatingEntity, iso_639_1_language_code: ISO6391LanguageCode
+    ) -> Dict[str, Any]:
         return {
             "id": participating_entity.entity.id,
             "type": [entity_type.name for entity_type in participating_entity.entity.types()],
             "label": participating_entity.entity.label(iso_639_1_language_code),
             "description": participating_entity.entity.label(iso_639_1_language_code),
             "names": list(participating_entity.entity.names(iso_639_1_language_code)),
-            "count": participating_entity.count
+            "count": participating_entity.count,
         }
```

### Comparing `wikivents-1.0.3/wikivents/models.py` & `wikivents-1.0.4/wikivents/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,49 +28,41 @@
 EntityId = NewType("EntityId", str)
 PropertyId = NewType("PropertyId", str)
 
 DEFAULT_LANGUAGE = ISO6391LanguageCode("en")
 
 
 class EntityType(Enum):
-    PERSON = {
-        "Q5"  # Human
-    }
+    PERSON = {"Q5"}  # Human
     ORG = {
         "Q43229",  # Organisation
         "Q4164871",  # Position
     }
     GPE = {
         "Q3257686",  # Locality
         "Q6256",  # Country
         "Q56061",  # Territorial Entity
     }
-    EVENT = {
-        "Q1190554",  # Occurrence
-        "Q1656682"  # Event
-    }
+    EVENT = {"Q1190554", "Q1656682"}  # Occurrence  # Event
     UNKNOWN = set()
 
     @staticmethod
     def get_types(entity_id_set: Set[EntityId]) -> Set["EntityType"]:
         """
         :param entity_id_set: the set of Entity ids which all define the same EntityType. For instance {"Q1190554"},
                               {"Q1656682"} or {"Q1190554", "Q1656682"} are EntityType.OCCURRENCE.
 
         """
-        return {
-            entity_type for entity_type in EntityType if entity_type.value.intersection(entity_id_set)
-        }
+        return {entity_type for entity_type in EntityType if entity_type.value.intersection(entity_id_set)}
 
     def __str__(self) -> str:
         return str(self.name)
 
 
 class SingleValueMultilingualText(collections.abc.Mapping):
-
     @abc.abstractmethod
     def __getitem__(self, iso_639_1_language_code: ISO6391LanguageCode) -> str:
         """Get the single value associated with the input language code"""
 
     @abc.abstractmethod
     def __iter__(self):
         pass
@@ -85,15 +77,14 @@
 
     @abc.abstractmethod
     def __str__(self) -> str:
         pass
 
 
 class MultipleValuesMultilingualText(collections.abc.Mapping):
-
     @abc.abstractmethod
     def __getitem__(self, iso_639_1_language_code: ISO6391LanguageCode) -> Set[str]:
         """Get the multiple values associated with the input language code"""
 
     @abc.abstractmethod
     def __iter__(self):
         pass
@@ -108,15 +99,14 @@
 
     @abc.abstractmethod
     def __str__(self) -> str:
         pass
 
 
 class SingleValueMultiLingualTextFromDict(SingleValueMultilingualText):
-
     def __init__(self, multiple_values_dict: Dict[ISO6391LanguageCode, str]):
         self.__multiple_values_dict = multiple_values_dict
 
     def __getitem__(self, iso_639_1_language_code: ISO6391LanguageCode) -> str:
         return self.__multiple_values_dict.get(iso_639_1_language_code, str())
 
     def __len__(self) -> int:
@@ -134,15 +124,14 @@
             return self.__multiple_values_dict.get(ISO6391LanguageCode(DEFAULT_LANGUAGE))
         if len(self.__multiple_values_dict) > 0:
             return next(iter(self.__multiple_values_dict))
         return "SingleValueMultiLingualTextFromDict()"
 
 
 class MultipleValuesMultiLingualTextFromDict(MultipleValuesMultilingualText):
-
     def __init__(self, multiple_values_dict: Dict[ISO6391LanguageCode, Set[str]]):
         self.__multiple_values_dict = multiple_values_dict
 
     def __getitem__(self, iso_639_1_language_code: ISO6391LanguageCode) -> Set[str]:
         return self.__multiple_values_dict.get(iso_639_1_language_code, set())
 
     def __len__(self) -> int:
@@ -160,15 +149,14 @@
             return repr(self.__multiple_values_dict.get(ISO6391LanguageCode(DEFAULT_LANGUAGE)))
         if len(self.__multiple_values_dict) > 0:
             return next(iter(self.__multiple_values_dict))
         return "MultipleValuesMultiLingualTextFromDict()"
 
 
 class Resource(abc.ABC):
-
     @abc.abstractmethod
     def content(self) -> str:
         pass
 
     @abc.abstractmethod
     def entities(self) -> Dict[str, int]:
         pass
@@ -182,17 +170,60 @@
         pass
 
     @abc.abstractmethod
     def __str__(self):
         pass
 
 
-class Entity:
+class InformativeEntity(abc.ABC):
+
+    # pylint: disable=invalid-name
+    @property
+    def id(self):
+        pass
+
+    @abc.abstractmethod
+    def label(self, iso_639_1_language_code: ISO6391LanguageCode) -> str:
+        pass
+
+    @abc.abstractmethod
+    def names(self, iso_639_1_language_code: ISO6391LanguageCode) -> Set[str]:
+        pass
+
+    @abc.abstractmethod
+    def description(self, iso_639_1_language_code: ISO6391LanguageCode) -> str:
+        pass
+
+    @abc.abstractmethod
+    def types(self) -> Set[EntityType]:
+        pass
+
+    @abc.abstractmethod
+    def types_as_entities(self) -> Set["Entity"]:
+        pass
+
+    @abc.abstractmethod
+    def __eq__(self, other) -> bool:
+        return self.id == other.id
+
+    def __ne__(self, other) -> bool:
+        return not self == other
+
+    def __repr__(self) -> str:
+        return self.__str__()
+
+    def __str__(self):
+        return f"<{self.__class__.__name__}({self.id}, {self.label(ISO6391LanguageCode(DEFAULT_LANGUAGE))})>"
+
+    def __hash__(self):
+        return hash(self.id)
+
 
-    def __init__(self, entity_data: 'EntityData', resources: Set[Resource] = None):  # noqa: F821
+class Entity(InformativeEntity):
+    def __init__(self, entity_data: "EntityData", resources: Set[Resource] = None):  # noqa: F821
         self.__id = entity_data.id
         self.__types = EntityType.get_types(entity_data.hierarchical_instance_of_ids)
         self.__types_entities = {Entity(type_entity_data) for type_entity_data in entity_data.instance_of}
         self.__label = entity_data.labels
         self.__description = entity_data.descriptions
         self.__names = entity_data.names
         self.__resources = resources or set()
@@ -210,15 +241,15 @@
 
     def description(self, iso_639_1_language_code: ISO6391LanguageCode) -> str:
         return self.__description.get(iso_639_1_language_code)
 
     def types(self) -> Set[EntityType]:
         return self.__types
 
-    def types_as_entities(self) -> Set['Entity']:
+    def types_as_entities(self) -> Set["Entity"]:
         return self.__types_entities
 
     def resources(self) -> Set[Resource]:
         return self.__resources
 
     def __eq__(self, other) -> bool:
         return self.id == other.id
@@ -229,25 +260,29 @@
     def __repr__(self) -> str:
         return self.__str__()
 
     def __str__(self):
         return f"<{self.__class__.__name__}({self.id}, {self.label(ISO6391LanguageCode(DEFAULT_LANGUAGE))})>"
 
     def __hash__(self):
-        return hash(self.id)
+        return hash(f"entity_{self.id}")
 
 
 @dataclass(eq=True, unsafe_hash=True, frozen=True)
 class ParticipatingEntity:
     entity: Entity
     count: int
 
 
-class Event:
+@dataclass(eq=True, unsafe_hash=True, frozen=True)
+class EntityCountByLanguage(ParticipatingEntity):
+    language: ISO6391LanguageCode
+
 
+class Event(InformativeEntity):
     @property
     def gpe(self) -> List[ParticipatingEntity]:
         return self.entities(EntityType.GPE, 1)
 
     @property
     def org(self) -> List[ParticipatingEntity]:
         return self.entities(EntityType.ORG, 1)
@@ -272,16 +307,21 @@
             return self.__end_date
         raise ValueError(f"There is no known end date for event {self.label(DEFAULT_LANGUAGE)}")
 
     @property
     def processed_languages_iso_639_1_codes(self) -> Set[str]:
         return {resource.iso_639_1_language() for resource in self.__entity.resources()}
 
-    def __init__(self, entity: Entity, dates: Tuple[datetime, datetime],
-                 participants: Set[ParticipatingEntity], places: Set[Entity]):
+    def __init__(
+        self,
+        entity: Entity,
+        dates: Tuple[datetime, datetime],
+        participants: Set[ParticipatingEntity],
+        places: Set[Entity],
+    ):
         if EntityType.EVENT not in entity.types():
             raise EntityIsNotAnEventError(
                 "The entity given to initialise the event is not declared as an event for Wikidata."
             )
         self.__entity = entity
         self.__participants = participants
         self.__places = places
@@ -300,26 +340,32 @@
 
     def description(self, iso_639_1_language_code: ISO6391LanguageCode) -> str:
         return self.__entity.description(iso_639_1_language_code)
 
     def places(self) -> Set[Entity]:
         return self.__places
 
+    def types(self) -> Set[EntityType]:
+        return self.__entity.types()
+
+    def types_as_entities(self) -> Set["Entity"]:
+        return self.__entity.types_as_entities()
+
     def participants(self) -> Set[ParticipatingEntity]:
         return self.__participants
 
-    def entities(self, entity_type: EntityType,
-                 participating_entities_ratio_to_keep: float = 0.5) -> List[ParticipatingEntity]:
-        participating_entities_count_to_keep = self.nb_of_processed_languages * participating_entities_ratio_to_keep
+    def entities(
+        self, entity_type: EntityType, keep_if_participating_entity_in_at_least_x_languages: int = 1
+    ) -> List[ParticipatingEntity]:
         participating_entities = {
             participating_entity
             for participating_entity in self.__participants
             if (
-                entity_type in participating_entity.entity.types() and
-                participating_entity.count >= participating_entities_count_to_keep
+                entity_type in participating_entity.entity.types()
+                and participating_entity.count >= keep_if_participating_entity_in_at_least_x_languages
             )
         }
         return sorted(
             participating_entities, key=lambda participating_entity: participating_entity.count, reverse=True
         )
 
     def __eq__(self, other) -> bool:
@@ -331,8 +377,8 @@
     def __repr__(self):
         return self.__str__()
 
     def __str__(self):
         return f"<{self.__class__.__name__}({self.id}, {self.label(ISO6391LanguageCode(DEFAULT_LANGUAGE))})>"
 
     def __hash__(self):
-        return hash(self.id)
+        return hash(f"event_{self.id}")
```

### Comparing `wikivents-1.0.3/wikivents/ontology/__init__.py` & `wikivents-1.0.4/wikivents/ontology/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,16 +16,21 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 import abc
 import collections.abc
 from datetime import datetime
 from typing import Set, Dict, Iterator, List
 
-from wikivents.models import EntityId, ISO6391LanguageCode, SingleValueMultilingualText, \
-    MultipleValuesMultilingualText, PropertyId
+from wikivents.models import (
+    EntityId,
+    ISO6391LanguageCode,
+    SingleValueMultilingualText,
+    MultipleValuesMultilingualText,
+    PropertyId,
+)
 
 
 class EntityData(collections.abc.Mapping):
 
     # pylint: disable=invalid-name
     @property
     @abc.abstractmethod
@@ -106,15 +111,14 @@
     @abc.abstractmethod
     def __hash__(self) -> int:
         pass
 
 
 # pylint: disable=too-many-ancestors
 class EventData(EntityData, abc.ABC):
-
     @property
     @abc.abstractmethod
     def start_date(self) -> datetime.date:
         pass
 
     @property
     @abc.abstractmethod
@@ -124,15 +128,14 @@
     @property
     @abc.abstractmethod
     def places(self) -> Set[EntityId]:
         pass
 
 
 class EntityOntologyRepository(abc.ABC):
-
     @abc.abstractmethod
     def get_entity_data_from_id(self, entity_id: EntityId) -> EntityData:
         pass
 
     @abc.abstractmethod
     def get_event_data_from_id(self, event_id: EntityId) -> EventData:
         pass
@@ -151,15 +154,14 @@
 
     @abc.abstractmethod
     def get_languages_spoken_where_event_happened(self, event_id: EntityId) -> Set[ISO6391LanguageCode]:
         pass
 
 
 class EntityOntologyCache(EntityOntologyRepository, abc.ABC):
-
     @abc.abstractmethod
     def set_entity_data_from_id(self, entity_id: EntityId, entity_data: EntityData):
         pass
 
     @abc.abstractmethod
     def set_event_data_from_id(self, event_id: EntityId, event_data: EventData):
         pass
```

### Comparing `wikivents-1.0.3/wikivents/ontology/exc.py` & `wikivents-1.0.4/wikivents/ontology/exc.py`

 * *Files identical despite different names*

### Comparing `wikivents-1.0.3/wikivents/ontology/wikidata.py` & `wikivents-1.0.4/wikivents/ontology/wikidata.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,23 +16,31 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 from collections import defaultdict
 from datetime import datetime, timedelta
 from threading import Lock
 from typing import Set, Any, Mapping, Dict, List, Iterator
 
+import requests
 from SPARQLWrapper import SPARQLWrapper, JSON
 from wikidata.client import Client
 from wikidata.entity import EntityId as WikidataEntityId
 
 from wikivents.cache import DillCache
 from wikivents.exc import NotInCacheException
-from wikivents.models import EntityId, ISO6391LanguageCode, SingleValueMultilingualText, \
-    SingleValueMultiLingualTextFromDict, MultipleValuesMultiLingualTextFromDict, MultipleValuesMultilingualText, \
-    PropertyId, EntityType
+from wikivents.models import (
+    EntityId,
+    ISO6391LanguageCode,
+    SingleValueMultilingualText,
+    SingleValueMultiLingualTextFromDict,
+    MultipleValuesMultiLingualTextFromDict,
+    MultipleValuesMultilingualText,
+    PropertyId,
+    EntityType,
+)
 from wikivents.ontology import EntityOntologyAPI, EntityOntologyCache, EntityOntologyRepository, EntityData, EventData
 from wikivents.ontology.exc import EntityDataDoesNotMatchAnEventError
 
 
 class WikidataEntityData(EntityData):
     __ID_OF_INSTANCE_OF_HIERARCHICAL = "P31-hierarchical"
 
@@ -101,17 +109,15 @@
             ).items()
         }
 
     @property
     def aliases(self) -> Dict[ISO6391LanguageCode, List[str]]:
         return {
             ISO6391LanguageCode(iso_639_1_language_code): [item.get("value") for item in language_value_list]
-            for iso_639_1_language_code, language_value_list in self.__wikidata_api_data.get(
-                "aliases", dict()
-            ).items()
+            for iso_639_1_language_code, language_value_list in self.__wikidata_api_data.get("aliases", dict()).items()
         }
 
     @property
     def instance_of_ids(self) -> Set[EntityId]:
         return {
             entity_type_dict.get("mainsnak").get("datavalue").get("value").get("id")
             for entity_type_dict in self.__claims.get("P31", dict())
@@ -130,21 +136,17 @@
             self.__claims[self.__ID_OF_INSTANCE_OF_HIERARCHICAL].append(
                 {
                     "mainsnak": {
                         "snaktype": "value",
                         "property": "P31",
                         "datatype": "wikibase-item",
                         "datavalue": {
-                            "value": {
-                                "entity-type": "item",
-                                "numeric-id": entity_id[1:],
-                                "id": entity_id
-                            },
-                            "type": "wikibase-entityid"
-                        }
+                            "value": {"entity-type": "item", "numeric-id": entity_id[1:], "id": entity_id},
+                            "type": "wikibase-entityid",
+                        },
                     }
                 }
             )
 
     @property
     def instance_of(self) -> Set["EntityData"]:
         return self.__instance_of_entities_data
@@ -176,15 +178,14 @@
 
     def __hash__(self) -> int:
         return hash(self.id)
 
 
 # pylint: disable=too-many-ancestors
 class WikidataEventData(EventData):
-
     def __init__(self, entity_data: EntityData):
         self.__entity_data = entity_data
         if not self.__entity_data.hierarchical_instance_of_ids & EntityType.EVENT.value:
             raise EntityDataDoesNotMatchAnEventError(
                 f"The given entity data ({self.__entity_data.id}) given is not event data. They are not instances "
                 f"of {EntityType.EVENT.value}. {self.__entity_data.hierarchical_instance_of_ids} instead."
             )
@@ -219,30 +220,31 @@
         # TODO: select the most relevant date if multiple
         if len(event_ending_dates) > 0:
             return self.__get_datetime_from_wikidata_date_format(*event_ending_dates[0])
         raise ValueError("This entity does not provide any end time information")
 
     # noinspection PyMethodMayBeStatic
     # pylint: disable=no-self-use
-    def __get_datetime_from_wikidata_date_format(self, wikidata_time_format: str,
-                                                 calendar_model: EntityId) -> datetime.date:
+    def __get_datetime_from_wikidata_date_format(
+        self, wikidata_time_format: str, calendar_model: EntityId
+    ) -> datetime.date:
         # https://www.wikidata.org/wiki/Help:Dates
         for date_format in [
             "+%Y-%m-%dT%H:%M:%S%z",  # day precision
             "+%Y-%m-00T%H:%M:%S%z",  # month precision
             "+%Y-00-00T%H:%M:%S%z",  # year precision
         ]:
             try:
                 gregorian_date = original_date = datetime.strptime(wikidata_time_format, date_format)
             except ValueError:
                 pass
             else:
                 # Julian date that needs conversion to gregorian
                 julian_calendar = EntityId("Q1985786")
-                if calendar_model == julian_calendar:
+                if julian_calendar in calendar_model:
                     # FIXME: AC and BC dates are not both supported.
                     # FIXME: Julian date to Gregorian is not appropriate
                     gregorian_date = original_date + timedelta(days=13)  # The delta in the 20th century
                 return gregorian_date  # Keep only the first date
 
     @property
     def places(self) -> Set[EntityId]:
@@ -374,80 +376,103 @@
         )
         return wikidata_api_data
 
     def get_event_data_from_id(self, event_id: EntityId) -> EventData:
         return WikidataEventData(self.get_entity_data_from_id(event_id))
 
     def get_official_languages_spoken_where_event_happened(self, event_id: EntityId) -> Set[ISO6391LanguageCode]:
-        self.__sparql_wrapper.setQuery(f"""
+        self.__sparql_wrapper.setQuery(
+            f"""
             SELECT DISTINCT ?language_code WHERE {{
               {{
                 wd:{event_id} wdt:P17 ?country.
                 ?country wdt:P37 ?official_language.
                 ?official_language wdt:P424 ?language_code.
               }}
               UNION
               {{
                 wd:{event_id} wdt:P17 ?country.
                 ?country wdt:P37 ?official_language.
                 ?official_language wdt:P4913 ?language_dialect.
                 ?language_dialect wdt:P424 ?language_code.
               }}
             }}
-        """)
-        return {
-            ISO6391LanguageCode(language_codes_dict.get("language_code").get("value"))
-            for language_codes_dict in self.__sparql_wrapper.query().convert().get("results").get("bindings")
-        }
+        """
+        )
+        return self.__filter_only_existing_wikipedia_projects_from_language_codes(
+            {
+                ISO6391LanguageCode(language_codes_dict.get("language_code").get("value"))
+                for language_codes_dict in self.__sparql_wrapper.query().convert().get("results").get("bindings")
+            }
+        )
 
     def get_languages_spoken_where_event_happened(self, event_id: EntityId) -> Set[ISO6391LanguageCode]:
-        self.__sparql_wrapper.setQuery(f"""
+        self.__sparql_wrapper.setQuery(
+            f"""
             SELECT DISTINCT ?language_code WHERE {{
               {{
                 wd:{event_id} wdt:P17 ?country.
                 ?country wdt:P37 | wdt:P2936 ?language.
                 ?language wdt:P424 ?language_code.
               }}
             UNION
               {{
                 wd:{event_id} wdt:P17 ?country.
                 ?country wdt:P37 ?language.
                 ?language wdt:P4913 ?language_dialect.
                 ?language_dialect wdt:P424 ?language_code.
               }}
             }}
-        """)
-        return {
-            ISO6391LanguageCode(language_codes_dict.get("language_code").get("value"))
-            for language_codes_dict in self.__sparql_wrapper.query().convert().get("results").get("bindings")
-        }
+        """
+        )
+        return self.__filter_only_existing_wikipedia_projects_from_language_codes(
+            {
+                ISO6391LanguageCode(language_codes_dict.get("language_code").get("value"))
+                for language_codes_dict in self.__sparql_wrapper.query().convert().get("results").get("bindings")
+            }
+        )
 
+    # pylint: disable=no-self-use
+    # noinspection PyMethodMayBeStatic
+    def __filter_only_existing_wikipedia_projects_from_language_codes(
+        self, iso_639_1_language_codes: Set[ISO6391LanguageCode]
+    ):
+        """
+        Keep only, from a list of language codes, them with an associated Wikipedia version. For instance
+        ‘fr’ has the https://fr.wikipedia.org, as well as ‘en’ with https://en.wikipedia.org while ‘en-us’
+        does not have one, as https://en-us.wikipedia.org does not exist.
+        """
+        existing_wikipedia_projects_language_codes = set()
+        for iso_639_1_language_code in iso_639_1_language_codes:
+            try:
+                response = requests.get(f"https://{iso_639_1_language_code}.wikipedia.org")
+                if response.status_code == 200:
+                    existing_wikipedia_projects_language_codes.add(iso_639_1_language_code)
+            except requests.exceptions.RequestException:
+                pass  # no project exists
+        return existing_wikipedia_projects_language_codes
 
-class _WikidataAPICache(EntityOntologyCache, DillCache):
 
+class _WikidataAPICache(EntityOntologyCache, DillCache):
     def __init__(self):
         super().__init__("wikidata")
 
     def get_entity_data_from_id(self, entity_id: EntityId) -> EntityData:
-        return self._get_data_else_raise_exception(
-            self.__get_entity_data_from_id_identifiers(entity_id)
-        )
+        return self._get_data_else_raise_exception(self.__get_entity_data_from_id_identifiers(entity_id))
 
     def set_entity_data_from_id(self, entity_id: EntityId, entity_data: EntityData):
         self._set_data(self.__get_entity_data_from_id_identifiers(entity_id), entity_data)
 
     # noinspection PyMethodMayBeStatic
     # pylint: disable=no-self-use
     def __get_entity_data_from_id_identifiers(self, entity_id: EntityId) -> List[str]:
         return ["entity_data", f"{entity_id}"]
 
     def get_event_data_from_id(self, event_id: EntityId) -> EventData:
-        return self._get_data_else_raise_exception(
-            self.__get_event_data_from_id_identifiers(event_id)
-        )
+        return self._get_data_else_raise_exception(self.__get_event_data_from_id_identifiers(event_id))
 
     def set_event_data_from_id(self, event_id: EntityId, event_data: EventData):
         self._set_data(self.__get_event_data_from_id_identifiers(event_id), event_data)
 
     # noinspection PyMethodMayBeStatic
     # pylint: disable=no-self-use
     def __get_event_data_from_id_identifiers(self, event_id: EntityId) -> List[str]:
@@ -478,38 +503,39 @@
     # pylint: disable=no-self-use
     def __get_all_entities_id_the_entity_is_an_instance_of_identifiers(self, entity_id: EntityId) -> List[str]:
         return ["all_entities_instance", f"{entity_id}"]
 
     def get_official_languages_spoken_where_event_happened(self, event_id: EntityId) -> Set[ISO6391LanguageCode]:
         return self._get_data_else_raise_exception(self.__get_official_languages_spoken_identifiers(event_id))
 
-    def set_official_languages_spoken_where_event_happened(self, event_id: EntityId,
-                                                           official_languages: Set[ISO6391LanguageCode]):
+    def set_official_languages_spoken_where_event_happened(
+        self, event_id: EntityId, official_languages: Set[ISO6391LanguageCode]
+    ):
         self._set_data(self.__get_official_languages_spoken_identifiers(event_id), official_languages)
 
     # noinspection PyMethodMayBeStatic
     # pylint: disable=no-self-use
     def __get_official_languages_spoken_identifiers(self, event_id) -> List[str]:
         return ["official_spoken_languages", f"{event_id}"]
 
     def get_languages_spoken_where_event_happened(self, event_id: EntityId) -> Set[ISO6391LanguageCode]:
         return self._get_data_else_raise_exception(self.__get_languages_spoken_identifiers(event_id))
 
-    def set_languages_spoken_where_event_happened(self, event_id: EntityId,
-                                                  spoken_languages: Set[ISO6391LanguageCode]):
+    def set_languages_spoken_where_event_happened(
+        self, event_id: EntityId, spoken_languages: Set[ISO6391LanguageCode]
+    ):
         self._set_data(self.__get_languages_spoken_identifiers(event_id), spoken_languages)
 
     # noinspection PyMethodMayBeStatic
     # pylint: disable=no-self-use
     def __get_languages_spoken_identifiers(self, event_id) -> List[str]:
         return ["all_spoken_languages", f"{event_id}"]
 
 
 class WikidataOntologyRepository(EntityOntologyRepository):
-
     def __init__(self):
         self.__event_ontology_api = _WikidataAPI()
         self.__event_ontology_cache = _WikidataAPICache()
         self.__entity_id_locks = defaultdict(Lock)
 
     def get_entity_data_from_id(self, entity_id: EntityId) -> EntityData:
         with self.__entity_id_locks[("entity_data", entity_id)]:
```

### Comparing `wikivents-1.0.3/wikivents/resource/__init__.py` & `wikivents-1.0.4/wikivents/resource/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,26 +18,24 @@
 import abc
 from typing import Set
 
 from wikivents.models import ParticipatingEntity, Resource
 
 
 class EntityResourceRepository(abc.ABC):
-
     @abc.abstractmethod
     def get_resource_from_label(self, label: str) -> Resource:
         pass
 
     @abc.abstractmethod
-    def get_participating_entities(self, resource: Resource) -> Set[ParticipatingEntity]:
+    def get_participating_entities_count_by_language(self, resource: Resource) -> Set[ParticipatingEntity]:
         pass
 
 
 class EntityResourceCache(EntityResourceRepository, abc.ABC):
-
     @abc.abstractmethod
     def set_resource_from_label(self, label: str, resource: Resource):
         pass
 
     @abc.abstractmethod
     def set_participating_entities(self, resource: Resource, participating_entities: Set[ParticipatingEntity]):
         pass
```

### Comparing `wikivents-1.0.3/wikivents/resource/wikipedia.py` & `wikivents-1.0.4/wikivents/resource/wikipedia.py`

 * *Files 14% similar despite different names*

```diff
@@ -22,22 +22,21 @@
 
 import mwclient
 import requests
 from mwclient.page import Page
 
 from wikivents.cache import DillCache
 from wikivents.exc import NotInCacheException
-from wikivents.models import ParticipatingEntity, EntityId, ISO6391LanguageCode, Entity
+from wikivents.models import ParticipatingEntity, EntityId, ISO6391LanguageCode, Entity, EntityCountByLanguage
 from wikivents.ontology import EntityOntologyRepository
 from wikivents.resource import Resource, EntityResourceAPI, EntityResourceRepository, EntityResourceCache
 from wikivents.resource.exc import ResourceInLanguageDoesNotExist, ResourceDoesNotExist
 
 
 class WikipediaArticle(Resource):
-
     def __init__(self, wikipedia_page: Page):
         self._wikipedia_page = wikipedia_page
         self._article_name = wikipedia_page.page_title
         self._iso_639_1_language_code = wikipedia_page.pagelanguage
 
     def content(self) -> str:
         return self._wikipedia_page.text()
@@ -84,41 +83,39 @@
         return len(self._wikipedia_page.text(section=self.__MEDIA_WIKI_API_INDEX_FOR_INTRODUCTION_SECTION))
 
     def __str__(self):
         return f"WikipediaArticleLeadSection({self._wikipedia_page.page_title}, {self._wikipedia_page.pagelanguage})"
 
 
 class _WikipediaResourceCache(EntityResourceCache, DillCache):
-
     def __init__(self, iso_639_1_language_code: str, wikidata_ontology_repository: EntityOntologyRepository):
         super().__init__("wikipedia")
         self.__entity_ontology_repository = wikidata_ontology_repository
         self.__iso_639_1_language_code = iso_639_1_language_code
 
     def get_resource_from_label(self, label: str) -> Resource:
         return self._get_data_else_raise_exception(self.__get_resource_from_label_identifiers(label))
 
     def set_resource_from_label(self, label: str, resource: Resource):
         self._set_data(self.__get_resource_from_label_identifiers(label), resource)
 
     def __get_resource_from_label_identifiers(self, label: str) -> List[str]:
         return ["resource", f"wikipedia_{self.__iso_639_1_language_code}_{label}"]
 
-    def get_participating_entities(self, resource: Resource) -> Set[ParticipatingEntity]:
+    def get_participating_entities_count_by_language(self, resource: Resource) -> Set[ParticipatingEntity]:
         return self._get_data_else_raise_exception(self.__get_participating_entities_identifiers(resource))
 
     def set_participating_entities(self, resource: Resource, participating_entities: Set[ParticipatingEntity]):
         self._set_data(self.__get_participating_entities_identifiers(resource), participating_entities)
 
     def __get_participating_entities_identifiers(self, resource: Resource) -> List[str]:
         return ["participating_entities", f"{self.__iso_639_1_language_code}_{resource}"]
 
 
 class _WikipediaResourceAPI(EntityResourceAPI):
-
     def __init__(self, iso_639_1_language_code: str, wikidata_ontology_repository: EntityOntologyRepository):
         self.__entity_ontology_repository = wikidata_ontology_repository
         self.__iso_639_1_language_code = iso_639_1_language_code
         try:
             self._site = mwclient.Site(f"{self.__iso_639_1_language_code}.wikipedia.org")
         except (mwclient.InvalidResponse, requests.exceptions.ConnectionError) as connection_error:
             raise ResourceInLanguageDoesNotExist(
@@ -136,26 +133,31 @@
             resource = WikipediaArticleLeadSection(self._site.pages[label])
         except KeyError:
             raise ResourceDoesNotExist(
                 f"No resource found for entity ‘{label}’ in language ‘{self.__iso_639_1_language_code}’"
             )
         return resource
 
-    def get_participating_entities(self, resource: Resource) -> Set[ParticipatingEntity]:
+    def get_participating_entities_count_by_language(self, resource: Resource) -> Set[EntityCountByLanguage]:
         participating_entities = dict()
         for entity_name, entity_count in resource.entities().items():
             if entity_name not in participating_entities:
                 try:
                     entity_id = self.__get_entity_id_from_label(entity_name)
                 except ValueError:
                     #  No page exist for the label on this site
                     pass
                 else:
                     entity_data = self.__entity_ontology_repository.get_entity_data_from_id(entity_id)
-                    participating_entities[entity_name] = ParticipatingEntity(Entity(entity_data), entity_count)
+                    entity = Entity(entity_data)
+                    participating_entities[entity_name] = EntityCountByLanguage(
+                        entity,
+                        entity_count,
+                        resource.iso_639_1_language(),
+                    )
         return set(participating_entities.values())
 
     def __get_entity_id_from_label(self, label: str) -> EntityId:
         """
         :raises ValueError: when no page exists for the given label or nothing is returned by the API.
 
         .. seealso:: https://en.wikipedia.org/wiki/Wikipedia:Finding_a_Wikidata_ID
@@ -182,29 +184,31 @@
                         }
                     }
                 }
             }
 
         """
         response = self._site.get(
-            action="query", format="json", titles=label,
+            action="query",
+            format="json",
+            titles=label,
             prop="pageprops",  # query “page properties”
-            redirects=""  # redirects is the page has move or has been rewritten
+            redirects="",  # redirects is the page has move or has been rewritten
         )
         wikipedia_pages_response = response.get("query").get("pages")
 
-        if (
-            not wikipedia_pages_response or
-            not self.__wikipedia_page_response_has_pages_properties(wikipedia_pages_response)
+        if not wikipedia_pages_response or not self.__wikipedia_page_response_has_pages_properties(
+            wikipedia_pages_response
         ):
             raise ValueError(f"No page exist for {label} on ’{self._site.host}’")
 
         entity_id = EntityId(
             self.__get_wikidata_pages_response_linked_wikidata_entity(wikipedia_pages_response)
-                .get("pageprops").get("wikibase_item")
+            .get("pageprops")
+            .get("wikibase_item")
         )
 
         if entity_id is None:
             raise ValueError(f"No entity identifier found for entity with label {label}.")
 
         return entity_id
 
@@ -214,30 +218,33 @@
     # noinspection PyMethodMayBeStatic
     # pylint: disable=no-self-use
     def __get_wikidata_pages_response_linked_wikidata_entity(self, wikipedia_pages_response: Dict[EntityId, Dict]):
         return next(iter(wikipedia_pages_response.values()))
 
 
 class WikipediaResourceRepository(EntityResourceRepository):
-
     def __init__(self, iso_639_1_language_code: str, wikidata_ontology_repository: EntityOntologyRepository):
         self.__entity_resource_api = _WikipediaResourceAPI(iso_639_1_language_code, wikidata_ontology_repository)
         self.__entity_resource_cache = _WikipediaResourceCache(iso_639_1_language_code, wikidata_ontology_repository)
         self.__resource_locks = defaultdict(Lock)
 
     def get_resource_from_label(self, label: str) -> Resource:
         with self.__resource_locks[("resource_from_label", label)]:
             try:
                 resource = self.__entity_resource_cache.get_resource_from_label(label)
             except NotInCacheException:
                 resource = self.__entity_resource_api.get_resource_from_label(label)
                 self.__entity_resource_cache.set_resource_from_label(label, resource)
             return resource
 
-    def get_participating_entities(self, resource: Resource) -> Set[ParticipatingEntity]:
+    def get_participating_entities_count_by_language(self, resource: Resource) -> Set[ParticipatingEntity]:
         with self.__resource_locks["participating_entities", resource.content()[:50]]:
             try:
-                participating_entities = self.__entity_resource_cache.get_participating_entities(resource)
+                participating_entities = self.__entity_resource_cache.get_participating_entities_count_by_language(
+                    resource
+                )
             except NotInCacheException:
-                participating_entities = self.__entity_resource_api.get_participating_entities(resource)
+                participating_entities = self.__entity_resource_api.get_participating_entities_count_by_language(
+                    resource
+                )
                 self.__entity_resource_cache.set_participating_entities(resource, participating_entities)
             return participating_entities
```

### Comparing `wikivents-1.0.3/wikivents.egg-info/PKG-INFO` & `wikivents-1.0.4/wikivents.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,346 +1,347 @@
 Metadata-Version: 2.1
 Name: wikivents
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple Python package to represent events from Wikipedia and Wikidata resources.
 Home-page: https://gitlab.com/guilieb/wikivents
 Author: Guillaume Bernard
 Author-email: contact@guillaume-bernard.fr
 License: GPLv3 License
-Description: # `wikivents`
-        
-        This Python package is used to represent events based on both ontologies and semi-structured databases. Up to now, only Wikidata and Wikipedia are implemented and provide these data. The name of this package, `wikivents` show this legacy.
-        
-        ### Events
-        
-        An event is an ontology entity. For Wikidata, an event is an instance of an [occurrence (Q1190554)](https://www.wikidata.org/wiki/Q1190554) or of an [event (Q1656682)](https://www.wikidata.org/wiki/Q1656682).
-        
-        A **event** is defined by few characteristics:
-         * **A type**: on Wikidata, this defines the type of the event. For instance, [rebellion (Q124734)](https://www.wikidata.org/wiki/Q124734) on Wikidata. This information is provided by the `wd:P31` or `rdf:type`, depending on the source.
-         * **Date** of occurrence, converted if necessary in the Gregorian calendar.
-         * **Location where the event happened**.
-         * The entities related to the event. The extraction process is based on semi-strucuted databases, which are processed in search of entities (people involved, places, etc). Entities are counted. This index shows the relevance of the entity in relation to the event. We assume the entities found in multiple lead sections are important entities in the event description.
-        
-        ## Usage
-        
-        The process of gathering data from multiple APIs (ontologies and semi-structured databases) can take a long time. We implemented a cache which speeds up queries and prevents from querying twice the same data.
-        
-        Up to now, the only implemented toolchain is based on Wikimedia foundation projects: Wikidata for the ontology and Wikipedia articles for semi-structured databases. Then it is possible to get the representation of an event using the `WikimediaFactory` object, as in the example below:
-        
-        ```python
-        from wikivents.factories.wikimedia import WikimediaFactory
-        from wikivents.models import EntityId
-        
-        easter_rising_entity_id = EntityId("Q193689")
-        easter_rising_event = WikimediaFactory.create_event(easter_rising_entity_id)
-        ```
-        
-        The previous code takes the [Easter Rising event](https://en.wikipedia.org/wiki/Easter_Rising) entity id (`Q193689`)' as input. If using another `Factory` which processes other ontologies, the entry point will obviously not be the same.
-        
-        From the `easter_rising_event` object, it is possible to access multiple attributes:
-        
-        * The **event identifier**, which comes from the ontology itself:
-        ```python
-        easter_rising_event.id
-        Out[5]: 'Q193689'
-        ```
-        
-        * The **event label**, in any possible language. If unavailable, will return an empty string.
-        ```python
-        easter_rising_event.label("fr")
-        Out[7]: 'Insurrection de Pâques 1916'
-        ```
-        
-        * The **event alternative names**, which means all the names that are used in a specific language to speak about the event.
-        ```python
-        easter_rising_event.names("de")
-        Out[8]: {'Easter Rising', 'Irischer Osteraufstand 1916', 'Osteraufstand'}
-        ```
-        
-        * The **event description**, in plain text.
-        ```python
-        easter_rising_event.description("en")
-        Out[9]: 'an armed insurrection in Ireland during Easter Week, 1916'
-        ```
-        
-        * The **event boundary dates**, beginning and end.
-        ```python
-        easter_rising_event.beginning, easter_rising_event.end
-        Out[12]: (datetime.datetime(1916, 4, 24, 0, 0, tzinfo=datetime.timezone.utc),  datetime.datetime(1916, 4, 30, 0, 0, tzinfo=datetime.timezone.utc))
-        ```
-        
-        * The entities involved, accessible using the `gpe` property for **GPE**, `org` property for **ORG** and `per` property for **PER** entities.
-        ```python
-        easter_rising_event.gpe
-        Out[13]: [ParticipatingEntity(entity=<Entity(Q1761, Dublin)>, count=8),ParticipatingEntity(entity=<Entity(Q27, Ireland)>, count=5)]
-        ```
-        
-        ## Encode events in reusable formats
-        
-        The `wikivents` library also provides encoders which are used to transform the event object into other formats, easier to manipulate. From now on, we provide a `DictEncoder` which make it easy to create a JSON file from it.
-        
-        ```python
-        from wikivents.model_encoders import EventToDictEncoder
-        from wikivents.models import ISO6391LanguageCode
-        
-        encoder = EventToDictEncoder(easter_rising_event, ISO6391LanguageCode("en"))
-        encoder.encode()
-        ```
-        
-        The purpose of encoders is to provide all the possible knowledge acquired about events and to show involved entities. It is also possible to add a parameter to the `encode()` method, `participating_entities_ratio_to_keep` to indicate which entities will be kept. It is a value comprised between 0 and 1. `1` means to keep all the participating entities, `0.5` to keep them only if they were found in at least 50% of the total number of processed semi-structured databases.
-        
-        Below is an example, and the associated JSON output:
-        
-        ```python
-        import json
-        
-        with open("easter_rising_event.json", mode="w") as easter_rising_json_file:
-            json.dump(encoder.encode(), easter_rising_json_file)
-        ```
-        
-        ```json
-        [
-          {
-            "Q193689": {
-              "iso_639_1_language_code": "en",
-              "id": "Q193689",
-              "type": "EVENT",
-              "label": "Easter Rising",
-              "description": "an armed insurrection in Ireland during Easter Week, 1916",
-              "names": [
-                "1916 Rising",
-                "Easter Rebellion",
-                "Easter Rising"
-              ],
-              "processed_languages": [
-                "de",
-                "it",
-                "es",
-                "fr",
-                "en"
-              ],
-              "entities_kept_if_mentioned_in_more_at_least_X_languages": 2.5,
-              "start": "1916-04-24T00:00:00+00:00",
-              "end": "1916-04-30T00:00:00+00:00",
-              "entities": {
-                "per": [
-                  {
-                    "id": "Q213374",
-                    "type": [
-                      "PERSON"
-                    ],
-                    "label": "James Connolly",
-                    "description": "James Connolly",
-                    "names": [
-                      "James Connolly"
-                    ],
-                    "count": 3
-                  },
-                  {
-                    "id": "Q274143",
-                    "type": [
-                      "PERSON"
-                    ],
-                    "label": "Patrick Pearse",
-                    "description": "Patrick Pearse",
-                    "names": [
-                      "Patrick Henry Pearse",
-                      "Patrick Pearse",
-                      "Padraig Pearse"
-                    ],
-                    "count": 3
-                  }
-                ],
-                "gpe": [
-                  {
-                    "id": "Q1761",
-                    "type": [
-                      "GPE"
-                    ],
-                    "label": "Dublin",
-                    "description": "Dublin",
-                    "names": [
-                      "City of Dublin",
-                      "Baile Átha Cliath",
-                      "Dublin",
-                      "Dublin city"
-                    ],
-                    "count": 8
-                  },
-                  {
-                    "id": "Q27",
-                    "type": [
-                      "GPE",
-                      "ORG"
-                    ],
-                    "label": "Ireland",
-                    "description": "Ireland",
-                    "names": [
-                      "🇮🇪",
-                      "Eire",
-                      "Éire",
-                      "Ireland",
-                      "ie",
-                      "ireland",
-                      "IRL",
-                      "Ireland, Republic of",
-                      "Republic of Ireland",
-                      "Hibernia",
-                      "IE",
-                      "Southern Ireland"
-                    ],
-                    "count": 5
-                  },
-                  {
-                    "id": "Q145",
-                    "type": [
-                      "GPE",
-                      "ORG"
-                    ],
-                    "label": "United Kingdom",
-                    "description": "United Kingdom",
-                    "names": [
-                      "G.B.",
-                      "GBR",
-                      "United Kingdom",
-                      "U. K.",
-                      "U K",
-                      "GB",
-                      "UK",
-                      "United Kingdom of Great Britain and Northern Ireland",
-                      "G B R",
-                      "Marea Britanie",
-                      "G. B. R.",
-                      "G B",
-                      "G. B.",
-                      "G.B.R.",
-                      "🇬🇧",
-                      "U.K.",
-                      "Great Britain"
-                    ],
-                    "count": 3
-                  }
-                ],
-                "org": [
-                  {
-                    "id": "Q27",
-                    "type": [
-                      "GPE",
-                      "ORG"
-                    ],
-                    "label": "Ireland",
-                    "description": "Ireland",
-                    "names": [
-                      "🇮🇪",
-                      "Eire",
-                      "Éire",
-                      "Ireland",
-                      "ie",
-                      "ireland",
-                      "IRL",
-                      "Ireland, Republic of",
-                      "Republic of Ireland",
-                      "Hibernia",
-                      "IE",
-                      "Southern Ireland"
-                    ],
-                    "count": 5
-                  },
-                  {
-                    "id": "Q1074958",
-                    "type": [
-                      "ORG"
-                    ],
-                    "label": "Irish Volunteers",
-                    "description": "Irish Volunteers",
-                    "names": [
-                      "Irish Volunteers",
-                      "Irish Volunteer Army",
-                      "Irish Volunteer Force"
-                    ],
-                    "count": 3
-                  },
-                  {
-                    "id": "Q145",
-                    "type": [
-                      "GPE",
-                      "ORG"
-                    ],
-                    "label": "United Kingdom",
-                    "description": "United Kingdom",
-                    "names": [
-                      "G.B.",
-                      "GBR",
-                      "United Kingdom",
-                      "U. K.",
-                      "U K",
-                      "GB",
-                      "UK",
-                      "United Kingdom of Great Britain and Northern Ireland",
-                      "G B R",
-                      "Marea Britanie",
-                      "G. B. R.",
-                      "G B",
-                      "G. B.",
-                      "G.B.R.",
-                      "🇬🇧",
-                      "U.K.",
-                      "Great Britain"
-                    ],
-                    "count": 3
-                  },
-                  {
-                    "id": "Q222595",
-                    "type": [
-                      "ORG"
-                    ],
-                    "label": "British Army",
-                    "description": "British Army",
-                    "names": [
-                      "British Army",
-                      "army of the United Kingdom"
-                    ],
-                    "count": 3
-                  },
-                  {
-                    "id": "Q1190570",
-                    "type": [
-                      "ORG"
-                    ],
-                    "label": "Irish Citizen Army",
-                    "description": "Irish Citizen Army",
-                    "names": [
-                      "Irish Citizen Army"
-                    ],
-                    "count": 3
-                  },
-                  {
-                    "id": "Q427496",
-                    "type": [
-                      "ORG"
-                    ],
-                    "label": "Cumann na mBan",
-                    "description": "Cumann na mBan",
-                    "names": [
-                      "Cumann na mBan",
-                      "CnamB",
-                      "The Irishwomen's Council"
-                    ],
-                    "count": 3
-                  }
-                ]
-              }
-            }
-          }
-        ]
-        ```
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
+License-File: LICENSE
+License-File: AUTHORS
+
+# `wikivents`
+
+This Python package is used to represent events based on both ontologies and semi-structured databases. Up to now, only Wikidata and Wikipedia are implemented and provide these data. The name of this package, `wikivents` show this legacy.
+
+### Events
+
+An event is an ontology entity. For Wikidata, an event is an instance of an [occurrence (Q1190554)](https://www.wikidata.org/wiki/Q1190554) or of an [event (Q1656682)](https://www.wikidata.org/wiki/Q1656682).
+
+A **event** is defined by few characteristics:
+ * **A type**: on Wikidata, this defines the type of the event. For instance, [rebellion (Q124734)](https://www.wikidata.org/wiki/Q124734) on Wikidata. This information is provided by the `wd:P31` or `rdf:type`, depending on the source.
+ * **Date** of occurrence, converted if necessary in the Gregorian calendar.
+ * **Location where the event happened**.
+ * The entities related to the event. The extraction process is based on semi-strucuted databases, which are processed in search of entities (people involved, places, etc). Entities are counted. This index shows the relevance of the entity in relation to the event. We assume the entities found in multiple lead sections are important entities in the event description.
+
+## Usage
+
+The process of gathering data from multiple APIs (ontologies and semi-structured databases) can take a long time. We implemented a cache which speeds up queries and prevents from querying twice the same data.
+
+Up to now, the only implemented toolchain is based on Wikimedia foundation projects: Wikidata for the ontology and Wikipedia articles for semi-structured databases. Then it is possible to get the representation of an event using the `WikimediaFactory` object, as in the example below:
+
+```python
+from wikivents.factories.wikimedia import WikimediaFactory
+from wikivents.models import EntityId
+
+easter_rising_entity_id = EntityId("Q193689")
+easter_rising_event = WikimediaFactory.create_event(easter_rising_entity_id)
+```
+
+The previous code takes the [Easter Rising event](https://en.wikipedia.org/wiki/Easter_Rising) entity id (`Q193689`)' as input. If using another `Factory` which processes other ontologies, the entry point will obviously not be the same.
+
+From the `easter_rising_event` object, it is possible to access multiple attributes:
+
+* The **event identifier**, which comes from the ontology itself:
+```python
+easter_rising_event.id
+Out[5]: 'Q193689'
+```
+
+* The **event label**, in any possible language. If unavailable, will return an empty string.
+```python
+easter_rising_event.label("fr")
+Out[7]: 'Insurrection de Pâques 1916'
+```
+
+* The **event alternative names**, which means all the names that are used in a specific language to speak about the event.
+```python
+easter_rising_event.names("de")
+Out[8]: {'Easter Rising', 'Irischer Osteraufstand 1916', 'Osteraufstand'}
+```
+
+* The **event description**, in plain text.
+```python
+easter_rising_event.description("en")
+Out[9]: 'an armed insurrection in Ireland during Easter Week, 1916'
+```
+
+* The **event boundary dates**, beginning and end.
+```python
+easter_rising_event.beginning, easter_rising_event.end
+Out[12]: (datetime.datetime(1916, 4, 24, 0, 0, tzinfo=datetime.timezone.utc),  datetime.datetime(1916, 4, 30, 0, 0, tzinfo=datetime.timezone.utc))
+```
+
+* The entities involved, accessible using the `gpe` property for **GPE**, `org` property for **ORG** and `per` property for **PER** entities.
+```python
+easter_rising_event.gpe
+Out[13]: [ParticipatingEntity(entity=<Entity(Q1761, Dublin)>, count=8),ParticipatingEntity(entity=<Entity(Q27, Ireland)>, count=5)]
+```
+
+## Encode events in reusable formats
+
+The `wikivents` library also provides encoders which are used to transform the event object into other formats, easier to manipulate. From now on, we provide a `DictEncoder` which make it easy to create a JSON file from it.
+
+```python
+from wikivents.model_encoders import EventToDictEncoder
+from wikivents.models import ISO6391LanguageCode
+
+encoder = EventToDictEncoder(easter_rising_event, ISO6391LanguageCode("en"))
+encoder.encode()
+```
+
+The purpose of encoders is to provide all the possible knowledge acquired about events and to show involved entities. It is also possible to add a parameter to the `encode()` method, `participating_entities_ratio_to_keep` to indicate which entities will be kept. It is a value comprised between 0 and 1. `1` means to keep all the participating entities, `0.5` to keep them only if they were found in at least 50% of the total number of processed semi-structured databases.
+
+Below is an example, and the associated JSON output:
+
+```python
+import json
+
+with open("easter_rising_event.json", mode="w") as easter_rising_json_file:
+    json.dump(encoder.encode(), easter_rising_json_file)
+```
+
+```json
+[
+  {
+    "Q193689": {
+      "iso_639_1_language_code": "en",
+      "id": "Q193689",
+      "type": "EVENT",
+      "label": "Easter Rising",
+      "description": "an armed insurrection in Ireland during Easter Week, 1916",
+      "names": [
+        "1916 Rising",
+        "Easter Rebellion",
+        "Easter Rising"
+      ],
+      "processed_languages": [
+        "de",
+        "it",
+        "es",
+        "fr",
+        "en"
+      ],
+      "entities_kept_if_mentioned_in_more_at_least_X_languages": 2.5,
+      "start": "1916-04-24T00:00:00+00:00",
+      "end": "1916-04-30T00:00:00+00:00",
+      "entities": {
+        "per": [
+          {
+            "id": "Q213374",
+            "type": [
+              "PERSON"
+            ],
+            "label": "James Connolly",
+            "description": "James Connolly",
+            "names": [
+              "James Connolly"
+            ],
+            "count": 3
+          },
+          {
+            "id": "Q274143",
+            "type": [
+              "PERSON"
+            ],
+            "label": "Patrick Pearse",
+            "description": "Patrick Pearse",
+            "names": [
+              "Patrick Henry Pearse",
+              "Patrick Pearse",
+              "Padraig Pearse"
+            ],
+            "count": 3
+          }
+        ],
+        "gpe": [
+          {
+            "id": "Q1761",
+            "type": [
+              "GPE"
+            ],
+            "label": "Dublin",
+            "description": "Dublin",
+            "names": [
+              "City of Dublin",
+              "Baile Átha Cliath",
+              "Dublin",
+              "Dublin city"
+            ],
+            "count": 8
+          },
+          {
+            "id": "Q27",
+            "type": [
+              "GPE",
+              "ORG"
+            ],
+            "label": "Ireland",
+            "description": "Ireland",
+            "names": [
+              "🇮🇪",
+              "Eire",
+              "Éire",
+              "Ireland",
+              "ie",
+              "ireland",
+              "IRL",
+              "Ireland, Republic of",
+              "Republic of Ireland",
+              "Hibernia",
+              "IE",
+              "Southern Ireland"
+            ],
+            "count": 5
+          },
+          {
+            "id": "Q145",
+            "type": [
+              "GPE",
+              "ORG"
+            ],
+            "label": "United Kingdom",
+            "description": "United Kingdom",
+            "names": [
+              "G.B.",
+              "GBR",
+              "United Kingdom",
+              "U. K.",
+              "U K",
+              "GB",
+              "UK",
+              "United Kingdom of Great Britain and Northern Ireland",
+              "G B R",
+              "Marea Britanie",
+              "G. B. R.",
+              "G B",
+              "G. B.",
+              "G.B.R.",
+              "🇬🇧",
+              "U.K.",
+              "Great Britain"
+            ],
+            "count": 3
+          }
+        ],
+        "org": [
+          {
+            "id": "Q27",
+            "type": [
+              "GPE",
+              "ORG"
+            ],
+            "label": "Ireland",
+            "description": "Ireland",
+            "names": [
+              "🇮🇪",
+              "Eire",
+              "Éire",
+              "Ireland",
+              "ie",
+              "ireland",
+              "IRL",
+              "Ireland, Republic of",
+              "Republic of Ireland",
+              "Hibernia",
+              "IE",
+              "Southern Ireland"
+            ],
+            "count": 5
+          },
+          {
+            "id": "Q1074958",
+            "type": [
+              "ORG"
+            ],
+            "label": "Irish Volunteers",
+            "description": "Irish Volunteers",
+            "names": [
+              "Irish Volunteers",
+              "Irish Volunteer Army",
+              "Irish Volunteer Force"
+            ],
+            "count": 3
+          },
+          {
+            "id": "Q145",
+            "type": [
+              "GPE",
+              "ORG"
+            ],
+            "label": "United Kingdom",
+            "description": "United Kingdom",
+            "names": [
+              "G.B.",
+              "GBR",
+              "United Kingdom",
+              "U. K.",
+              "U K",
+              "GB",
+              "UK",
+              "United Kingdom of Great Britain and Northern Ireland",
+              "G B R",
+              "Marea Britanie",
+              "G. B. R.",
+              "G B",
+              "G. B.",
+              "G.B.R.",
+              "🇬🇧",
+              "U.K.",
+              "Great Britain"
+            ],
+            "count": 3
+          },
+          {
+            "id": "Q222595",
+            "type": [
+              "ORG"
+            ],
+            "label": "British Army",
+            "description": "British Army",
+            "names": [
+              "British Army",
+              "army of the United Kingdom"
+            ],
+            "count": 3
+          },
+          {
+            "id": "Q1190570",
+            "type": [
+              "ORG"
+            ],
+            "label": "Irish Citizen Army",
+            "description": "Irish Citizen Army",
+            "names": [
+              "Irish Citizen Army"
+            ],
+            "count": 3
+          },
+          {
+            "id": "Q427496",
+            "type": [
+              "ORG"
+            ],
+            "label": "Cumann na mBan",
+            "description": "Cumann na mBan",
+            "names": [
+              "Cumann na mBan",
+              "CnamB",
+              "The Irishwomen's Council"
+            ],
+            "count": 3
+          }
+        ]
+      }
+    }
+  }
+]
+```
```

### Comparing `wikivents-1.0.3/wikivents.egg-info/SOURCES.txt` & `wikivents-1.0.4/wikivents.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+AUTHORS
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 tests/__init__.py
 tests/entity_factory_test.py
 tests/entity_type_test.py
```

