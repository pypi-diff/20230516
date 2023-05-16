# Comparing `tmp/factorioBlueprintAnalyser-1.3.3.tar.gz` & `tmp/factorioBlueprintAnalyser-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factorioBlueprintAnalyser-1.3.3.tar", last modified: Wed Oct 26 20:21:43 2022, max compression
+gzip compressed data, was "factorioBlueprintAnalyser-1.3.4.tar", last modified: Tue May 16 20:34:00 2023, max compression
```

## Comparing `factorioBlueprintAnalyser-1.3.3.tar` & `factorioBlueprintAnalyser-1.3.4.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 20:21:43.846500 factorioBlueprintAnalyser-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-10-26 20:21:43.846500 factorioBlueprintAnalyser-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5122 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 20:21:43.842500 factorioBlueprintAnalyser-1.3.3/factorioBlueprintAnalyser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      281 2022-10-26 20:21:43.000000 factorioBlueprintAnalyser-1.3.3/factorioBlueprintAnalyser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-10-26 20:21:43.000000 factorioBlueprintAnalyser-1.3.3/factorioBlueprintAnalyser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 20:21:43.000000 factorioBlueprintAnalyser-1.3.3/factorioBlueprintAnalyser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       44 2022-10-26 20:21:43.000000 factorioBlueprintAnalyser-1.3.3/factorioBlueprintAnalyser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-10-26 20:21:43.000000 factorioBlueprintAnalyser-1.3.3/factorioBlueprintAnalyser.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 20:21:43.846500 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 20:21:43.842500 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/assets/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-26 20:21:43.846500 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/assets/factorio_raw/
--rw-r--r--   0 runner    (1001) docker     (121)   329732 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/assets/factorio_raw/factorio_raw_min.json
--rw-r--r--   0 runner    (1001) docker     (121)    14576 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (121)      853 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/blueprint_analyser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3041 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/config.py
--rw-r--r--   0 runner    (1001) docker     (121)    23350 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/entity.py
--rw-r--r--   0 runner    (1001) docker     (121)     1615 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/factorio.py
--rw-r--r--   0 runner    (1001) docker     (121)     1863 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/item.py
--rw-r--r--   0 runner    (1001) docker     (121)    19160 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/network.py
--rw-r--r--   0 runner    (1001) docker     (121)    22956 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/node.py
--rw-r--r--   0 runner    (1001) docker     (121)     2088 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/options.py
--rw-r--r--   0 runner    (1001) docker     (121)     3438 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/recipe.py
--rw-r--r--   0 runner    (1001) docker     (121)      805 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      254 2022-10-26 20:21:43.846500 factorioBlueprintAnalyser-1.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      565 2022-10-26 20:21:39.000000 factorioBlueprintAnalyser-1.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:34:00.787774 factorioBlueprintAnalyser-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-16 20:34:00.787774 factorioBlueprintAnalyser-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5122 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:34:00.787774 factorioBlueprintAnalyser-1.3.4/factorioBlueprintAnalyser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-16 20:34:00.000000 factorioBlueprintAnalyser-1.3.4/factorioBlueprintAnalyser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-16 20:34:00.000000 factorioBlueprintAnalyser-1.3.4/factorioBlueprintAnalyser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:34:00.000000 factorioBlueprintAnalyser-1.3.4/factorioBlueprintAnalyser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-16 20:34:00.000000 factorioBlueprintAnalyser-1.3.4/factorioBlueprintAnalyser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 20:34:00.000000 factorioBlueprintAnalyser-1.3.4/factorioBlueprintAnalyser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:34:00.787774 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:34:00.787774 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 20:34:00.787774 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/assets/factorio_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   329732 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/assets/factorio_raw/factorio_raw_min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14576 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/blueprint_analyser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3041 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22560 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/factorio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19160 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22956 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-16 20:34:00.787774 factorioBlueprintAnalyser-1.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-16 20:33:55.000000 factorioBlueprintAnalyser-1.3.4/setup.py
```

### Comparing `factorioBlueprintAnalyser-1.3.3/LICENCE` & `factorioBlueprintAnalyser-1.3.4/LICENCE`

 * *Files identical despite different names*

### Comparing `factorioBlueprintAnalyser-1.3.3/README.md` & `factorioBlueprintAnalyser-1.3.4/README.md`

 * *Files identical despite different names*

### Comparing `factorioBlueprintAnalyser-1.3.3/factorioBlueprintAnalyser.egg-info/SOURCES.txt` & `factorioBlueprintAnalyser-1.3.4/factorioBlueprintAnalyser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/assets/factorio_raw/factorio_raw_min.json` & `factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/assets/factorio_raw/factorio_raw_min.json`

 * *Files identical despite different names*

### Comparing `factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/blueprint.py` & `factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/blueprint.py`

 * *Files identical despite different names*

### Comparing `factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/blueprint_analyser.py` & `factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/blueprint_analyser.py`

 * *Files identical despite different names*

### Comparing `factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/config.py` & `factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/config.py`

 * *Files identical despite different names*

### Comparing `factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/entity.py` & `factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/entity.py`

 * *Files 2% similar despite different names*

```diff
@@ -396,32 +396,14 @@
             # Define the required items per second
             # to have the assembling machine working at 100%
             self.required_items_per_second = {}
             for item in self.recipe.ingredients:
                 self.required_items_per_second[item.name] = item.amount / \
                     time_per_item
 
-    def get_usage_ratio(self, ingredients_amount):
-        # Calculate the number of items produced per second
-        # according to an ingredients amount dictionary
-
-        if self.recipe is None or not self.recipe.all_ingredients_required(ingredients_amount.keys()):
-            return 0
-
-        lowest_ingredient_requierment_ratio = None
-        for ingredient in ingredients_amount:
-
-            completion_ratio = ingredients_amount[ingredient] / \
-                self.required_items_per_second[ingredient]
-
-            if lowest_ingredient_requierment_ratio is None or \
-                    completion_ratio < lowest_ingredient_requierment_ratio:
-                lowest_ingredient_requierment_ratio = completion_ratio
-
-        return min(1.0, lowest_ingredient_requierment_ratio)
 
     def to_char(self, coords=None):
         color = "white"
         if self.name == "assembling-machine-2":
             color = "blue"
         if self.name == "assembling-machine-3":
             color = "yellow"
```

### Comparing `factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/factorio.py` & `factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/factorio.py`

 * *Files identical despite different names*

### Comparing `factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/item.py` & `factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/item.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-
 # -----------------------------------------------------------
 # Items class
 # Used to calculate bottleneck
 # -----------------------------------------------------------
 
 
 class Item:
@@ -16,15 +15,15 @@
 
     def get_ingame_image_path(self):
         # Item image url
         # To display the entity game image, we will the images
         # from : https://wiki.factorio.com/Category:Game_images
 
         # We need to transform the entity name to a valid url
-        entity_wiki_name = self.name.capitalize().replace('-', '_')
+        entity_wiki_name = self.name.capitalize().replace("-", "_")
 
         return f"https://wiki.factorio.com/images/{entity_wiki_name}.png"
 
 
 class Flow:
     def __init__(self):
         self.items = {}
@@ -46,21 +45,27 @@
         if item not in self.items:
             self.items[item] = amount
         else:
             self.items[item] += amount
 
     def reduce(self, item, amount):
         if item not in self.items:
-            raise Exception("Item not in flow")
+            print(f"/!\ Warning, item {item} not in flow")
+            # raise Exception("Item not in flow")
+            return
 
         self.items[item] -= amount
         if self.items[item] <= 0:
             del self.items[item]
 
     @property
     def total_amount(self):
         if len(self.items) == 0:
             return 0
         return sum(self.items.values())
 
     def __str__(self) -> str:
-        return "[" + ", ".join([f"{item}: {amount}" for item, amount in self.items.items()]) + "]"
+        return (
+            "["
+            + ", ".join([f"{item}: {amount}" for item, amount in self.items.items()])
+            + "]"
+        )
```

### Comparing `factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/network.py` & `factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/network.py`

 * *Files identical despite different names*

### Comparing `factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/node.py` & `factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/node.py`

 * *Files identical despite different names*

### Comparing `factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/options.py` & `factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/options.py`

 * *Files identical despite different names*

### Comparing `factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/recipe.py` & `factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/recipe.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 utils.warning(f"Something went wrong with the recipe {name}")
                 self.exists = False
                 return
 
         # Get production time
         self.time = factorio_recipe["energy_required"] \
             if "energy_required" in factorio_recipe \
-            else 1
+            else 0.5
 
     def ingredient_required(self, ingredient_name):
         for ingredient in self.ingredients:
             if ingredient.name == ingredient_name:
                 return True
 
         return False
```

### Comparing `factorioBlueprintAnalyser-1.3.3/factorio_blueprint_analyser/utils.py` & `factorioBlueprintAnalyser-1.3.4/factorio_blueprint_analyser/utils.py`

 * *Files identical despite different names*

### Comparing `factorioBlueprintAnalyser-1.3.3/setup.py` & `factorioBlueprintAnalyser-1.3.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='factorioBlueprintAnalyser',
-    version='1.3.3',
+    version='1.3.4',
     description="A python library analyse Factorio Blueprints and find bottlenecks.",
     url="https://github.com/tomansion/factorio_blueprint_analyser_app/",
     author="Tom Mansion",
     license="MIT License",
     install_requires=["termcolor==2.0.1", "PyYAML==5.4.1", "pyvis==0.3.0"],
     package_data={
         "factorio_blueprint_analyser": [
```

