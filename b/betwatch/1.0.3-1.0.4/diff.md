# Comparing `tmp/betwatch-1.0.3.tar.gz` & `tmp/betwatch-1.0.4.tar.gz`

## Comparing `betwatch-1.0.3.tar` & `betwatch-1.0.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.0.3/Makefile
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.0.3/.github/dependabot.yml
--rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.0.3/.github/workflows/test.yml
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.0.3/betwatch/__about__.py
--rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.0.3/betwatch/__init__.py
--rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.0.3/betwatch/client.py
--rw-r--r--   0        0        0    26499 2020-02-02 00:00:00.000000 betwatch-1.0.3/betwatch/client_async.py
--rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.0.3/betwatch/queries.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.0.3/betwatch/types/__init__.py
--rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 betwatch-1.0.3/betwatch/types/bookmakers.py
--rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 betwatch-1.0.3/betwatch/types/filters.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.0.3/betwatch/types/markets.py
--rw-r--r--   0        0        0    11720 2020-02-02 00:00:00.000000 betwatch-1.0.3/betwatch/types/race.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.0.3/betwatch/types/updates.py
--rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 betwatch-1.0.3/examples/get_race_prices.py
--rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.0.3/examples/get_race_prices_async.py
--rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.0.3/examples/get_races.py
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.0.3/examples/get_races_async.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 betwatch-1.0.3/examples/subscriptions.py
--rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.0.3/examples/update_rated_prices.py
--rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.0.3/tests/__init__.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.0.3/tests/test_check_last_updated.py
--rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.0.3/tests/test_get_race.py
--rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.0.3/tests/test_get_race_async.py
--rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.0.3/tests/test_get_races.py
--rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.0.3/tests/test_get_races_async.py
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 betwatch-1.0.3/.gitignore
--rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.0.3/LICENSE.txt
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.0.3/README.md
--rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 betwatch-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      138 2020-02-02 00:00:00.000000 betwatch-1.0.4/Makefile
+-rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 betwatch-1.0.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      795 2020-02-02 00:00:00.000000 betwatch-1.0.4/.github/workflows/test.yml
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/__about__.py
+-rw-r--r--   0        0        0     1000 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/__init__.py
+-rw-r--r--   0        0        0     8765 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/client.py
+-rw-r--r--   0        0        0    26499 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/client_async.py
+-rw-r--r--   0        0        0     5029 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/queries.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/types/__init__.py
+-rw-r--r--   0        0        0     2305 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/types/bookmakers.py
+-rw-r--r--   0        0        0     4458 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/types/filters.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/types/markets.py
+-rw-r--r--   0        0        0    12489 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/types/race.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 betwatch-1.0.4/betwatch/types/updates.py
+-rw-r--r--   0        0        0     2651 2020-02-02 00:00:00.000000 betwatch-1.0.4/examples/get_race_prices.py
+-rw-r--r--   0        0        0     1417 2020-02-02 00:00:00.000000 betwatch-1.0.4/examples/get_race_prices_async.py
+-rw-r--r--   0        0        0     2240 2020-02-02 00:00:00.000000 betwatch-1.0.4/examples/get_races.py
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 betwatch-1.0.4/examples/get_races_async.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 betwatch-1.0.4/examples/subscriptions.py
+-rw-r--r--   0        0        0     1280 2020-02-02 00:00:00.000000 betwatch-1.0.4/examples/update_rated_prices.py
+-rw-r--r--   0        0        0      105 2020-02-02 00:00:00.000000 betwatch-1.0.4/tests/__init__.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 betwatch-1.0.4/tests/test_check_last_updated.py
+-rw-r--r--   0        0        0      782 2020-02-02 00:00:00.000000 betwatch-1.0.4/tests/test_get_race.py
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 betwatch-1.0.4/tests/test_get_race_async.py
+-rw-r--r--   0        0        0      759 2020-02-02 00:00:00.000000 betwatch-1.0.4/tests/test_get_races.py
+-rw-r--r--   0        0        0      663 2020-02-02 00:00:00.000000 betwatch-1.0.4/tests/test_get_races_async.py
+-rw-r--r--   0        0        0     1867 2020-02-02 00:00:00.000000 betwatch-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1097 2020-02-02 00:00:00.000000 betwatch-1.0.4/LICENSE.txt
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 betwatch-1.0.4/README.md
+-rw-r--r--   0        0        0     2143 2020-02-02 00:00:00.000000 betwatch-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 betwatch-1.0.4/PKG-INFO
```

### Comparing `betwatch-1.0.3/.github/workflows/test.yml` & `betwatch-1.0.4/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/betwatch/__init__.py` & `betwatch-1.0.4/betwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/betwatch/client.py` & `betwatch-1.0.4/betwatch/client.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/betwatch/client_async.py` & `betwatch-1.0.4/betwatch/client_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/betwatch/queries.py` & `betwatch-1.0.4/betwatch/queries.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/betwatch/types/bookmakers.py` & `betwatch-1.0.4/betwatch/types/bookmakers.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/betwatch/types/filters.py` & `betwatch-1.0.4/betwatch/types/filters.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,17 +37,16 @@
         self.limit = limit
         self.offset = offset
         self.types = types if types else []
         self.tracks = tracks if tracks else []
 
         # if locations is a string, convert to a list
         # this is to simplify filtering for Australian races
-        if isinstance(locations, str):
-            if locations == "Australia":
-                locations = get_australian_states()
+        if locations == ["Australia"]:
+            locations = get_australian_states()
 
         self.locations = locations if locations else []
         self.has_bookmakers = has_bookmakers if has_bookmakers else []
         self.has_runners = has_runners if has_runners else []
         self.has_trainers = has_trainers if has_trainers else []
         self.has_riders = has_riders if has_riders else []
```

### Comparing `betwatch-1.0.3/betwatch/types/markets.py` & `betwatch-1.0.4/betwatch/types/markets.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/betwatch/types/race.py` & `betwatch-1.0.4/betwatch/types/race.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from dataclasses import dataclass, field
-from datetime import datetime
+import dataclasses
+from datetime import date, datetime, time, timedelta
 from enum import Enum
+import json
 from typing import List, Literal, Optional, Union
 
 import dateutil.parser
 
 from betwatch.types.markets import (
     BetfairMarket,
     Bookmaker,
@@ -251,14 +253,28 @@
     status: RaceStatus
     _start_time: str = field(metadata={"name": "startTime"})
 
     def __post_init__(self):
         self.start_time = dateutil.parser.isoparse(self._start_time)
 
 
+class EnhancedJSONEncoder(json.JSONEncoder):
+    # Create a custom encoder to handle nested dataclasses
+    # and convert them to dicts. Also handles datetime objects
+    def default(self, o):
+        if dataclasses.is_dataclass(o):
+            return dataclasses.asdict(o)
+        if isinstance(o, (datetime, date, time)):
+            return o.isoformat()
+        elif isinstance(o, timedelta):
+            return (datetime.min + o).time().isoformat()
+        elif isinstance(o, Enum):
+            return o.value
+        return super().default(o)
+
 @dataclass
 class Race:
     id: str
 
     status: Optional[RaceStatus] = None
 
     runners: Optional[List[Runner]] = None
@@ -302,14 +318,17 @@
             if self.start_time
             else ""
         )
 
         if self.meeting is None:
             return f"R{self.number} [{st}]"
         return f"({self.meeting.type}) {self.meeting.track} R{self.number}{st}"
+    
+    def __repr__(self) -> str:
+        return str(self)
 
     def get_bookmaker_link(
         self, bookmaker: Union[Bookmaker, str]
     ) -> Optional[RaceLink]:
         """Returns the link for the given bookmaker"""
         # parse bookmaker if string
         if isinstance(bookmaker, str):
@@ -317,14 +336,17 @@
 
         if not self.links:
             return None
         for link in self.links:
             if link.bookmaker == bookmaker:
                 return link
         return None
+    
+    def to_dict(self) -> dict:
+        return json.loads(json.dumps(self, cls=EnhancedJSONEncoder))
 
     def get_runners_by_price(
         self,
         market_type: MarketPriceType,
         bookmakers: Optional[List[Bookmaker]] = None,
     ) -> List[Runner]:
         """Sorts the runners by the given market types best price"""
```

### Comparing `betwatch-1.0.3/examples/get_race_prices.py` & `betwatch-1.0.4/examples/get_race_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/examples/get_race_prices_async.py` & `betwatch-1.0.4/examples/get_race_prices_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/examples/get_races.py` & `betwatch-1.0.4/examples/get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/examples/get_races_async.py` & `betwatch-1.0.4/examples/get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/examples/subscriptions.py` & `betwatch-1.0.4/examples/subscriptions.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/examples/update_rated_prices.py` & `betwatch-1.0.4/examples/update_rated_prices.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/tests/test_get_race.py` & `betwatch-1.0.4/tests/test_get_race.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/tests/test_get_race_async.py` & `betwatch-1.0.4/tests/test_get_race_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/tests/test_get_races.py` & `betwatch-1.0.4/tests/test_get_races.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/tests/test_get_races_async.py` & `betwatch-1.0.4/tests/test_get_races_async.py`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/.gitignore` & `betwatch-1.0.4/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -129,7 +129,8 @@
 # mypy
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
+demos/
```

### Comparing `betwatch-1.0.3/LICENSE.txt` & `betwatch-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/README.md` & `betwatch-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/pyproject.toml` & `betwatch-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `betwatch-1.0.3/PKG-INFO` & `betwatch-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betwatch
-Version: 1.0.3
+Version: 1.0.4
 Summary: A Python package for interacting with the Betwatch.com API
 Project-URL: Documentation, https://github.com/betwatch/betwatch-sdk-python#readme
 Project-URL: Issues, https://github.com/betwatch/betwatch-sdk-python/issues
 Project-URL: Source, https://github.com/betwatch/betwatch-sdk-python
 Project-URL: Betwatch.com, https://betwatch.com
 Author-email: Jamie Watts <jamie@betwatch.com>
 License-File: LICENSE.txt
```

