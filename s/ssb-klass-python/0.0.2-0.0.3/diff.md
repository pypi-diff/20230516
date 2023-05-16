# Comparing `tmp/ssb_klass_python-0.0.2.tar.gz` & `tmp/ssb_klass_python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_klass_python-0.0.2.tar", max compression
+gzip compressed data, was "ssb_klass_python-0.0.3.tar", max compression
```

## Comparing `ssb_klass_python-0.0.2.tar` & `ssb_klass_python-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1076 2023-05-11 17:02:17.238198 ssb_klass_python-0.0.2/LICENSE.md
--rw-r--r--   0        0        0      856 2023-05-11 17:02:17.238198 ssb_klass_python-0.0.2/README.md
--rw-r--r--   0        0        0     1487 2023-05-11 17:02:36.694235 ssb_klass_python-0.0.2/klass/__init__.py
--rw-r--r--   0        0        0        0 2023-05-11 17:02:17.238198 ssb_klass_python-0.0.2/klass/classes/__init__.py
--rw-r--r--   0        0        0     3229 2023-05-11 17:02:17.238198 ssb_klass_python-0.0.2/klass/classes/classification.py
--rw-r--r--   0        0        0     3857 2023-05-11 17:02:17.238198 ssb_klass_python-0.0.2/klass/classes/codes.py
--rw-r--r--   0        0        0     2233 2023-05-11 17:02:36.694235 ssb_klass_python-0.0.2/klass/classes/correspondance.py
--rw-r--r--   0        0        0      704 2023-05-11 17:02:17.238198 ssb_klass_python-0.0.2/klass/classes/family.py
--rw-r--r--   0        0        0     3172 2023-05-11 17:02:36.694235 ssb_klass_python-0.0.2/klass/classes/search.py
--rw-r--r--   0        0        0     2293 2023-05-11 17:02:17.238198 ssb_klass_python-0.0.2/klass/classes/variant.py
--rw-r--r--   0        0        0     1831 2023-05-11 17:02:17.238198 ssb_klass_python-0.0.2/klass/classes/version.py
--rw-r--r--   0        0        0      522 2023-05-11 17:02:17.238198 ssb_klass_python-0.0.2/klass/klass_config.py
--rw-r--r--   0        0        0        0 2023-05-11 17:02:17.238198 ssb_klass_python-0.0.2/klass/requests/__init__.py
--rw-r--r--   0        0        0    11092 2023-05-11 17:02:36.694235 ssb_klass_python-0.0.2/klass/requests/klass_requests.py
--rw-r--r--   0        0        0      530 2023-05-11 17:02:36.698235 ssb_klass_python-0.0.2/klass/requests/sections.py
--rw-r--r--   0        0        0     3120 2023-05-11 17:02:36.698235 ssb_klass_python-0.0.2/klass/requests/validate.py
--rw-r--r--   0        0        0        0 2023-05-11 17:02:17.238198 ssb_klass_python-0.0.2/klass/samples/__init__.py
--rw-r--r--   0        0        0      180 2023-05-11 17:02:17.238198 ssb_klass_python-0.0.2/klass/utility/classification.py
--rw-r--r--   0        0        0      244 2023-05-11 17:02:17.238198 ssb_klass_python-0.0.2/klass/utility/codes.py
--rw-r--r--   0        0        0        0 2023-05-11 17:02:17.238198 ssb_klass_python-0.0.2/klass/widgets/__init__.py
--rw-r--r--   0        0        0     2410 2023-05-11 17:02:36.698235 ssb_klass_python-0.0.2/klass/widgets/search_ipywidget.py
--rw-r--r--   0        0        0     1091 2023-05-11 17:02:36.698235 ssb_klass_python-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1527 1970-01-01 00:00:00.000000 ssb_klass_python-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/LICENSE.md
+-rw-r--r--   0        0        0     1556 2023-05-16 11:03:15.361497 ssb_klass_python-0.0.3/README.md
+-rw-r--r--   0        0        0     1487 2023-05-16 11:03:15.361497 ssb_klass_python-0.0.3/klass/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/classes/__init__.py
+-rw-r--r--   0        0        0     3229 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/classes/classification.py
+-rw-r--r--   0        0        0     3857 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/classes/codes.py
+-rw-r--r--   0        0        0     2233 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/classes/correspondance.py
+-rw-r--r--   0        0        0      704 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/classes/family.py
+-rw-r--r--   0        0        0     3810 2023-05-16 11:03:15.361497 ssb_klass_python-0.0.3/klass/classes/search.py
+-rw-r--r--   0        0        0     2293 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/classes/variant.py
+-rw-r--r--   0        0        0     1831 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/classes/version.py
+-rw-r--r--   0        0        0      551 2023-05-16 11:03:15.361497 ssb_klass_python-0.0.3/klass/klass_config.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/requests/__init__.py
+-rw-r--r--   0        0        0    11092 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/requests/klass_requests.py
+-rw-r--r--   0        0        0      530 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/requests/sections.py
+-rw-r--r--   0        0        0     3121 2023-05-16 11:03:15.361497 ssb_klass_python-0.0.3/klass/requests/validate.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/samples/__init__.py
+-rw-r--r--   0        0        0      180 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/utility/classification.py
+-rw-r--r--   0        0        0      244 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/utility/codes.py
+-rw-r--r--   0        0        0        0 2023-05-16 11:03:01.124208 ssb_klass_python-0.0.3/klass/widgets/__init__.py
+-rw-r--r--   0        0        0     3078 2023-05-16 11:03:15.361497 ssb_klass_python-0.0.3/klass/widgets/search_ipywidget.py
+-rw-r--r--   0        0        0     1156 2023-05-16 11:03:15.361497 ssb_klass_python-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2220 1970-01-01 00:00:00.000000 ssb_klass_python-0.0.3/PKG-INFO
```

### Comparing `ssb_klass_python-0.0.2/LICENSE.md` & `ssb_klass_python-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.2/klass/__init__.py` & `ssb_klass_python-0.0.3/klass/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from importlib import import_module
 
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 __all__ = []
 
 # Everything we want to be directly importable from under "klass"-package
 local_imports = {
     "requests.klass_requests": [
         "classifications",
         "classification_search",
```

### Comparing `ssb_klass_python-0.0.2/klass/classes/classification.py` & `ssb_klass_python-0.0.3/klass/classes/classification.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.2/klass/classes/codes.py` & `ssb_klass_python-0.0.3/klass/classes/codes.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.2/klass/classes/correspondance.py` & `ssb_klass_python-0.0.3/klass/classes/correspondance.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.2/klass/classes/family.py` & `ssb_klass_python-0.0.3/klass/classes/family.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.2/klass/classes/search.py` & `ssb_klass_python-0.0.3/klass/classes/search.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,64 +1,79 @@
 from ..requests.klass_requests import classification_search, classificationfamilies
 from .classification import KlassClassification
 
 
 class KlassSearchClassifications:
     def __init__(
-        self, query: str = "", include_codelists: bool = False, ssbsection: str = ""
+        self,
+        query: str = "",
+        include_codelists: bool = True,  # Opposite default of API, cause why not
+        ssbsection: str = "",
+        no_dupes=False,
     ):
         self.query = query
         self.include_codelists = include_codelists
         self.ssbsection = ssbsection
-        
+
         # If you enter a number, replace with name of the classification
         if query.isdigit() and query != "":
             result = KlassClassification(query)
             print(result.name)
             self.query = "".join([c for c in result.name if c.isalnum() or c == " "])
         elif not self.query and self.ssbsection:
-            self.query= " "
-        
-        print(self.query, self.ssbsection)
-        
+            self.query = " "
+
         result = classification_search(
             query=self.query,
             include_codelists=self.include_codelists,
             ssbsection=self.ssbsection,
         )
-        print(result)
         if "_embedded" in result.keys():
             self.classifications = result["_embedded"]["searchResults"]
         elif "searchResults" in result.keys():
             self.classifications = result["searchResults"]
         else:
-            self.classifications = [result]
+            self.classifications = []
 
         self.links = result["_links"]
-        classification_replace = []
-        for cl in self.classifications:
-            cl = {
-                "classification_id": int(cl["_links"]["self"]["href"].split("/")[-1]),
-                **cl,
-            }
-            classification_replace.append(cl)
-
-        self.classifications = classification_replace
+        print(self.classifications)
+        if len(self.classifications):
+            classification_replace = []
+            for cl in self.classifications:
+                cl = {
+                    "classification_id": int(
+                        cl["_links"]["self"]["href"].split("/")[-1]
+                    ),
+                    **cl,
+                }
+                classification_replace.append(cl)
+            self.classifications = classification_replace
+            if no_dupes:
+                classification_replace = []
+                seen = []
+                for cl in self.classifications:
+                    if cl["classification_id"] not in seen:
+                        classification_replace.append(cl)
+                        seen.append(cl["classification_id"])
+                self.classifications = classification_replace
 
     @staticmethod
     def get_classification(classification_id: str) -> KlassClassification:
         return KlassClassification(classification_id)
 
     def __str__(self):
         return str(self.__dict__)
 
     def simple_search_result(self):
         result = ""
-        for cl in self.classifications:
-            result += f'{cl["classification_id"]}: {cl["name"]}\n'
+        if len(self.classifications):
+            for cl in self.classifications:
+                result += f'{cl["classification_id"]}: {cl["name"]}\n'
+        else:
+            result = "Found no classifications"
         return result
 
 
 class KlassSearchFamilies:
     def __init__(
         self,
         ssbsection: str = "",
```

### Comparing `ssb_klass_python-0.0.2/klass/classes/variant.py` & `ssb_klass_python-0.0.3/klass/classes/variant.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.2/klass/classes/version.py` & `ssb_klass_python-0.0.3/klass/classes/version.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.2/klass/klass_config.py` & `ssb_klass_python-0.0.3/klass/klass_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -12,7 +12,8 @@
     def singleton_init(self):
         self.LANGUAGES = ["nb", "nn", "en"]
         self.BASE_URL = "https://data.ssb.no/api/klass/v1/"
         self.HEADERS = {
             "Accept": 'application/json',
         }
         self.TESTING = False
+        self.MOCKING = False
```

### Comparing `ssb_klass_python-0.0.2/klass/requests/klass_requests.py` & `ssb_klass_python-0.0.3/klass/requests/klass_requests.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.2/klass/requests/sections.py` & `ssb_klass_python-0.0.3/klass/requests/sections.py`

 * *Files identical despite different names*

### Comparing `ssb_klass_python-0.0.2/klass/requests/validate.py` & `ssb_klass_python-0.0.3/klass/requests/validate.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     if not check.isalpha():
         raise ValueError("Unexpected characters in presentation name pattern.")
     return pattern
 
 
 def validate_alnum_spaces(variant_name: str) -> str:
     check = variant_name.replace(" ", "")
-    print(f"{check=}")
+    #print(f"{check=}")
     if not check in ["", " "] and not check.isalnum() :
         raise ValueError(
             "Expecting variant name to only include numbers, characters and spaces..."
         )
     return variant_name
```

### Comparing `ssb_klass_python-0.0.2/klass/widgets/search_ipywidget.py` & `ssb_klass_python-0.0.3/klass/widgets/search_ipywidget.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,58 +1,77 @@
 import ipywidgets as widgets
-from IPython.display import display, clear_output, HTML
-from klass import KlassSearchClassifications, KlassSearchFamilies, sections_dict
+from IPython.display import HTML, display
 
-def search_classification():
+from klass import KlassSearchClassifications, sections_dict
+
+
+def search_classification(no_dupes=True):
     def do_search(btn):
         nonlocal search_term
         nonlocal section_dropdown
         nonlocal search_result
-        
-        if section_dropdown.value != "Choose...":
-            search_class = KlassSearchClassifications(search_term.value, ssbsection=section_dropdown.value)
-        else:
-            search_class = KlassSearchClassifications(search_term.value)
-        search_content = ""
-        for cl in search_class.classifications:
-            var_name = (cl["name"]
+
+        with search_result:
+            search_result.clear_output()
+            display("Searching...")
+            # Add loading-gif?
+
+        try:
+            if section_dropdown.value != "Choose...":
+                search_class = KlassSearchClassifications(
+                    search_term.value,
+                    ssbsection=section_dropdown.value,
+                    include_codelists=True,
+                    no_dupes=no_dupes,
+                )
+            else:
+                search_class = KlassSearchClassifications(
+                    search_term.value, include_codelists=True, no_dupes=no_dupes
+                )
+            search_content = ""
+            print(f"{search_class.classifications=}")
+            if len(search_class.classifications):
+                for cl in search_class.classifications:
+                    var_name = (
+                        cl["name"]
                         .split(":")[0]
                         .lower()
                         .replace(" ", "_")
                         .replace("(", "")
                         .replace(")", "")
                         .replace("æ", "ae")
                         .replace("ø", "oe")
                         .replace("å", "aa")
-                        .strip())
-            text = f'''from klass import KlassClassification\\n{var_name} = KlassClassification({cl["classification_id"]})\\n{var_name}.get_codes().data'''
-            var_name = "klass" + str(cl["classification_id"])
-            script_var = f"<script>var {var_name} = '{text}'</script>"
-            search_content += f'''<button onclick="navigator.clipboard.writeText('{text}')">Copy code</button> {cl["classification_id"]} - {cl["name"]}<br />'''
-
+                        .strip()
+                    )
+                    text = f"""from klass import KlassClassification\\n{var_name} = KlassClassification({cl["classification_id"]})\\n{var_name}.get_codes().data"""
+                    var_name = "klass" + str(cl["classification_id"])
+                    search_content += f"""<button class="classification_copy_code" onclick="navigator.clipboard.writeText('{text}')">Copy code</button> {cl["classification_id"]} - {cl["name"]}<br />"""
+            else:
+                search_content = "Found no matching classifications."
+        except Exception as e:
+            search_content = str(e)
 
-        
         with search_result:
             search_result.clear_output()
             display(HTML(search_content))
-    
-    
-    search_term = widgets.Text(value="",
-                              placeholder="Searchterm",
-                              description="Type searchterm:")
+
+    search_term = widgets.Text(
+        value="", placeholder="Searchterm", description="Type searchterm:"
+    )
     sections = ["Choose..."] + list(sections_dict().keys())
-    section_dropdown = widgets.Dropdown(options=sections,
-                                            value=sections[0],
-                                            description="Section:",
-                                            disabled=False)
+    section_dropdown = widgets.Dropdown(
+        options=sections, value=sections[0], description="Section:", disabled=False
+    )
     search_button = widgets.Button(description="Search")
     search_button.on_click(do_search)
-    
+    html_header = widgets.HTML(
+        value="<style>button.classification_copy_code:active {opacity: 30%;} button.classification_copy_code:hover {opacity: 80%;}</style>"
+    )
     search_result = widgets.Output()
-    #display(search_result)
-    
-    return widgets.VBox([
-        widgets.HBox([search_term, section_dropdown, search_button]),
-        widgets.HBox([search_result])
-    ])
-
 
+    return widgets.VBox(
+        [
+            widgets.HBox([html_header, search_term, section_dropdown, search_button]),
+            widgets.HBox([search_result]),
+        ]
+    )
```

### Comparing `ssb_klass_python-0.0.2/pyproject.toml` & `ssb_klass_python-0.0.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "ssb-klass-python"
-version = "0.0.2"
+version = "0.0.3"
 description = "A Python package built on top of KLASS's API for retrieving classifications, codes, correspondances etc."
 authors = ["Carl Corneil <cfc@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "klass"}]
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.11"
 dapla-toolbelt = "^1.3.2"
 python-dateutil = "^2.8.2"
 toml = "^0.10.2"
 ipywidgets = "^8.0.6"
-pandas = "^2.0.1"
+pandas = "1.5.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.3"
 ipykernel = "^6.15.3"
 pre-commit = "^2.20.0"
 autoflake = "^1.7.6"
 pep8-naming = "^0.13.2"
@@ -31,14 +31,17 @@
 flake8-bugbear = "^22.9.23"
 flake8 = "^5.0.4"
 bump2version = "^1.0.1"
 pytest-cov = "^4.0.0"
 mypy = "^0.982"
 pyproject-flake8 = "^5.0.4.post1"
 
+[tool.poetry.group.dev.dependencies]
+pre-commit-hooks = "^4.4.0"
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
 profile = "black"
 skip_gitignore = true
```

### Comparing `ssb_klass_python-0.0.2/PKG-INFO` & `ssb_klass_python-0.0.3/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,49 +1,39 @@
-Metadata-Version: 2.1
-Name: ssb-klass-python
-Version: 0.0.2
-Summary: A Python package built on top of KLASS's API for retrieving classifications, codes, correspondances etc.
-License: MIT
-Author: Carl Corneil
-Author-email: cfc@ssb.no
-Requires-Python: >=3.10,<3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: dapla-toolbelt (>=1.3.2,<2.0.0)
-Requires-Dist: ipywidgets (>=8.0.6,<9.0.0)
-Requires-Dist: pandas (>=2.0.1,<3.0.0)
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
-Description-Content-Type: text/markdown
-
 # ssb-klass-python
 
-A Python package built on top of KLASS's API for retrieving classifications, codes, correspondances etc.
+A Python package built on top of Statistics Norway's code- and classification-system "KLASS". \
+The package aims to make Klass's API for retrieving data easier to use by re-representing Klass's internal hierarchy as python-classes. Containing methods for easier traversal down, search classes and widgets, reasonable defaults to parameters etc.
+Where data is possible to fit into pandas DataFrames, this will be preferred, but hirerachical data will be kept as json / dict structure.
 
 
-## Example usage
+## Example usages
 
-```python
-from klass import KlassClassification as KC # Import the class for KlassClassifications
-nus = KC(36)  # Use ID for classification
-codes = nus.get_codes() # codes from current date
-print(codes)
-codes.data  # Pandas dataframe available
 
+```python
+from klass import search_classification
+# Opens a ipywidget in notebooks for searching for classifications and copying code, to get started
+search_classification(no_dupes=True)
 ```
 
 ```python
 from klass import get_classification # Import the utility-function
 nus = get_classification(36)
+```
 
+```python
+# Does the same as the code above, but does not shy away from using the class directly
+from klass import KlassClassification # Import the class for KlassClassifications
+nus = KlassClassification(36)  # Use ID for classification
+codes = nus.get_codes() # codes from current date
+print(codes)
+codes.data  # Pandas dataframe available under the .data attribute
 ```
 
 
+
 ## Technical notes
 Documentation for the [endpoints we are using can be found on Statistics Norways pages.](https://data.ssb.no/api/klass/v1/api-guide.html)
 
-Technical architecture of the API we are interacting with is detailed in [Statistics Norway's internal wiki](https://wiki.ssb.no/display/KP/Teknisk+arkitektur#Tekniskarkitektur-GSIM).
+Technical architecture of the API we are interacting with is detailed in [Statistics Norway's **internal** wiki](https://wiki.ssb.no/display/KP/Teknisk+arkitektur#Tekniskarkitektur-GSIM).
 
 
 ---
-
```

