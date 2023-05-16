# Comparing `tmp/qcew-1.0.3.tar.gz` & `tmp/qcew-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcew-1.0.3.tar", last modified: Fri May 12 17:36:52 2023, max compression
+gzip compressed data, was "qcew-1.0.4.tar", last modified: Tue May 16 17:46:28 2023, max compression
```

## Comparing `qcew-1.0.3.tar` & `qcew-1.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 17:36:52.246784 qcew-1.0.3/
--rw-r--r--   0 TrentThompson   (501) staff       (20)     1090 2023-05-12 11:30:42.000000 qcew-1.0.3/LICENSE
--rw-r--r--   0 TrentThompson   (501) staff       (20)     2856 2023-05-12 17:36:52.067532 qcew-1.0.3/PKG-INFO
--rw-r--r--   0 TrentThompson   (501) staff       (20)     2212 2023-05-12 17:36:17.000000 qcew-1.0.3/README.md
--rw-r--r--   0 TrentThompson   (501) staff       (20)       38 2023-05-12 17:36:52.246949 qcew-1.0.3/setup.cfg
--rw-r--r--   0 TrentThompson   (501) staff       (20)      980 2023-05-12 17:36:24.000000 qcew-1.0.3/setup.py
-drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 17:36:52.048755 qcew-1.0.3/src/
-drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-12 17:36:52.065751 qcew-1.0.3/src/qcew.egg-info/
--rw-r--r--   0 TrentThompson   (501) staff       (20)     2856 2023-05-12 17:36:52.000000 qcew-1.0.3/src/qcew.egg-info/PKG-INFO
--rw-r--r--   0 TrentThompson   (501) staff       (20)      166 2023-05-12 17:36:52.000000 qcew-1.0.3/src/qcew.egg-info/SOURCES.txt
--rw-r--r--   0 TrentThompson   (501) staff       (20)        1 2023-05-12 17:36:52.000000 qcew-1.0.3/src/qcew.egg-info/dependency_links.txt
--rw-r--r--   0 TrentThompson   (501) staff       (20)        5 2023-05-12 17:36:52.000000 qcew-1.0.3/src/qcew.egg-info/top_level.txt
--rw-r--r--   0 TrentThompson   (501) staff       (20)    12840 2023-05-12 17:34:42.000000 qcew-1.0.3/src/qcew.py
+drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-16 17:46:28.272284 qcew-1.0.4/
+-rw-r--r--   0 TrentThompson   (501) staff       (20)     1090 2023-05-16 14:13:08.000000 qcew-1.0.4/LICENSE
+-rw-r--r--   0 TrentThompson   (501) staff       (20)     3420 2023-05-16 17:46:28.270654 qcew-1.0.4/PKG-INFO
+-rw-r--r--   0 TrentThompson   (501) staff       (20)     2796 2023-05-16 17:44:58.000000 qcew-1.0.4/README.md
+-rw-r--r--   0 TrentThompson   (501) staff       (20)       38 2023-05-16 17:46:28.272436 qcew-1.0.4/setup.cfg
+-rw-r--r--   0 TrentThompson   (501) staff       (20)      980 2023-05-16 17:46:12.000000 qcew-1.0.4/setup.py
+drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-16 17:46:28.266975 qcew-1.0.4/src/
+-rw-r--r--   0 TrentThompson   (501) staff       (20)        0 2023-05-16 14:13:08.000000 qcew-1.0.4/src/__init__.py
+drwxr-xr-x   0 TrentThompson   (501) staff       (20)        0 2023-05-16 17:46:28.270024 qcew-1.0.4/src/qcew.egg-info/
+-rw-r--r--   0 TrentThompson   (501) staff       (20)     3420 2023-05-16 17:46:28.000000 qcew-1.0.4/src/qcew.egg-info/PKG-INFO
+-rw-r--r--   0 TrentThompson   (501) staff       (20)      182 2023-05-16 17:46:28.000000 qcew-1.0.4/src/qcew.egg-info/SOURCES.txt
+-rw-r--r--   0 TrentThompson   (501) staff       (20)        1 2023-05-16 17:46:28.000000 qcew-1.0.4/src/qcew.egg-info/dependency_links.txt
+-rw-r--r--   0 TrentThompson   (501) staff       (20)       14 2023-05-16 17:46:28.000000 qcew-1.0.4/src/qcew.egg-info/top_level.txt
+-rw-r--r--   0 TrentThompson   (501) staff       (20)    16699 2023-05-16 14:13:08.000000 qcew-1.0.4/src/qcew.py
```

### Comparing `qcew-1.0.3/LICENSE` & `qcew-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qcew-1.0.3/PKG-INFO` & `qcew-1.0.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcew
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for retrieving Quarterly Census of Employment and Wages (QCEW) data.
 Home-page: https://github.com/TrentLThompson/qcew
 Author: Trent Thompson
 Author-email: 808trent@gmail.com
 Keywords: QCEW,BLS,employment,wages,statistics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -42,15 +42,15 @@
     year="2020",
     annual=False,
     fields=None
 )
 
 # Get annual average employment and pay data for the United States from 2001 to 2021.
 data = qcew.get_qcew_data_slice(
-    area_slice=True,
+    slice_type="area",
     qcew_codes=["US000"],
     years=[str(i) for i in range(2001, 2022)],
     annual_data=True,
     fields=[
         "area_fips",
         "own_code",
         "industry_code",
@@ -59,15 +59,15 @@
         "annual_avg_emplvl",
         "avg_annual_pay"
         ]
     )
 
 # Get monthly employment data for the state of Hawaii as well as Honolulu County, HI in 2020.
 data = qcew.get_qcew_data_slice(
-    area_slice=True,
+    slice_type="area",
     qcew_codes=[
         "15000", # Hawaii -- Statewide
         "15003", # Honolulu County, HI
         ],
     years=["2020"],
     annual_data=False,
     fields=[
@@ -81,27 +81,49 @@
         "month2_emplvl",
         "month3_emplvl"
         ]
     )
 
 # Get annual average employment and pay data for the manufacturing sector as a whole from 2010 to 2020.
 data = qcew.get_qcew_data_slice(
-    area_slice=False,
+    slice_type="industry",
     qcew_codes=[
         "31-33", # NAICS code for manufacturing sector.
         ],
     years=[str(i) for i in range(2010, 2021)],
-    annual_data=False,
+    annual_data=True,
     fields=[
         "area_fips",
         "own_code",
         "industry_code",
         "year",
         "disclosure_code",
         "annual_avg_emplvl",
         "avg_annual_pay"
         ]
     )
+
+# Get monthly employment data for establishments with fewer than 5 employees in the first quarter of 2021.
+data = qcew.get_qcew_data_slice(
+    slice_type="size",
+    qcew_codes=[
+        "1", # Size code for establishments with fewer than 5 employees.
+        ],
+    years=["2021"],
+    annual_data=False,
+    fields=[
+        "area_fips",
+        "own_code",
+        "industry_code",
+        "size_code",
+        "year",
+        "qtr",
+        "disclosure_code",
+        "month1_emplvl",
+        "month2_emplvl",
+        "month3_emplvl"
+        ]
+    )
 ```
 
 ## License
 Distributed under the MIT license. See [LICENSE](/LICENSE) for more information.
```

### Comparing `qcew-1.0.3/README.md` & `qcew-1.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     year="2020",
     annual=False,
     fields=None
 )
 
 # Get annual average employment and pay data for the United States from 2001 to 2021.
 data = qcew.get_qcew_data_slice(
-    area_slice=True,
+    slice_type="area",
     qcew_codes=["US000"],
     years=[str(i) for i in range(2001, 2022)],
     annual_data=True,
     fields=[
         "area_fips",
         "own_code",
         "industry_code",
@@ -40,15 +40,15 @@
         "annual_avg_emplvl",
         "avg_annual_pay"
         ]
     )
 
 # Get monthly employment data for the state of Hawaii as well as Honolulu County, HI in 2020.
 data = qcew.get_qcew_data_slice(
-    area_slice=True,
+    slice_type="area",
     qcew_codes=[
         "15000", # Hawaii -- Statewide
         "15003", # Honolulu County, HI
         ],
     years=["2020"],
     annual_data=False,
     fields=[
@@ -62,27 +62,49 @@
         "month2_emplvl",
         "month3_emplvl"
         ]
     )
 
 # Get annual average employment and pay data for the manufacturing sector as a whole from 2010 to 2020.
 data = qcew.get_qcew_data_slice(
-    area_slice=False,
+    slice_type="industry",
     qcew_codes=[
         "31-33", # NAICS code for manufacturing sector.
         ],
     years=[str(i) for i in range(2010, 2021)],
-    annual_data=False,
+    annual_data=True,
     fields=[
         "area_fips",
         "own_code",
         "industry_code",
         "year",
         "disclosure_code",
         "annual_avg_emplvl",
         "avg_annual_pay"
         ]
     )
+
+# Get monthly employment data for establishments with fewer than 5 employees in the first quarter of 2021.
+data = qcew.get_qcew_data_slice(
+    slice_type="size",
+    qcew_codes=[
+        "1", # Size code for establishments with fewer than 5 employees.
+        ],
+    years=["2021"],
+    annual_data=False,
+    fields=[
+        "area_fips",
+        "own_code",
+        "industry_code",
+        "size_code",
+        "year",
+        "qtr",
+        "disclosure_code",
+        "month1_emplvl",
+        "month2_emplvl",
+        "month3_emplvl"
+        ]
+    )
 ```
 
 ## License
-Distributed under the MIT license. See [LICENSE](/LICENSE) for more information.
+Distributed under the MIT license. See [LICENSE](/LICENSE) for more information.
```

### Comparing `qcew-1.0.3/setup.py` & `qcew-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup
 from pathlib import Path
 
-VERSION = "1.0.3"
+VERSION = "1.0.4"
 DESCRIPTION = "A package for retrieving Quarterly Census of Employment and Wages (QCEW) data."
 
 setup(
     name="qcew",
     version=VERSION,
     description=DESCRIPTION,
     author="Trent Thompson",
```

### Comparing `qcew-1.0.3/src/qcew.egg-info/PKG-INFO` & `qcew-1.0.4/src/qcew.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcew
-Version: 1.0.3
+Version: 1.0.4
 Summary: A package for retrieving Quarterly Census of Employment and Wages (QCEW) data.
 Home-page: https://github.com/TrentLThompson/qcew
 Author: Trent Thompson
 Author-email: 808trent@gmail.com
 Keywords: QCEW,BLS,employment,wages,statistics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
@@ -42,15 +42,15 @@
     year="2020",
     annual=False,
     fields=None
 )
 
 # Get annual average employment and pay data for the United States from 2001 to 2021.
 data = qcew.get_qcew_data_slice(
-    area_slice=True,
+    slice_type="area",
     qcew_codes=["US000"],
     years=[str(i) for i in range(2001, 2022)],
     annual_data=True,
     fields=[
         "area_fips",
         "own_code",
         "industry_code",
@@ -59,15 +59,15 @@
         "annual_avg_emplvl",
         "avg_annual_pay"
         ]
     )
 
 # Get monthly employment data for the state of Hawaii as well as Honolulu County, HI in 2020.
 data = qcew.get_qcew_data_slice(
-    area_slice=True,
+    slice_type="area",
     qcew_codes=[
         "15000", # Hawaii -- Statewide
         "15003", # Honolulu County, HI
         ],
     years=["2020"],
     annual_data=False,
     fields=[
@@ -81,27 +81,49 @@
         "month2_emplvl",
         "month3_emplvl"
         ]
     )
 
 # Get annual average employment and pay data for the manufacturing sector as a whole from 2010 to 2020.
 data = qcew.get_qcew_data_slice(
-    area_slice=False,
+    slice_type="industry",
     qcew_codes=[
         "31-33", # NAICS code for manufacturing sector.
         ],
     years=[str(i) for i in range(2010, 2021)],
-    annual_data=False,
+    annual_data=True,
     fields=[
         "area_fips",
         "own_code",
         "industry_code",
         "year",
         "disclosure_code",
         "annual_avg_emplvl",
         "avg_annual_pay"
         ]
     )
+
+# Get monthly employment data for establishments with fewer than 5 employees in the first quarter of 2021.
+data = qcew.get_qcew_data_slice(
+    slice_type="size",
+    qcew_codes=[
+        "1", # Size code for establishments with fewer than 5 employees.
+        ],
+    years=["2021"],
+    annual_data=False,
+    fields=[
+        "area_fips",
+        "own_code",
+        "industry_code",
+        "size_code",
+        "year",
+        "qtr",
+        "disclosure_code",
+        "month1_emplvl",
+        "month2_emplvl",
+        "month3_emplvl"
+        ]
+    )
 ```
 
 ## License
 Distributed under the MIT license. See [LICENSE](/LICENSE) for more information.
```

### Comparing `qcew-1.0.3/src/qcew.py` & `qcew-1.0.4/src/qcew.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,14 +29,15 @@
     "lq_avg_annual_pay": float,
     "lq_avg_wkly_wage": float,
     "lq_disclosure_code": str,
     "lq_month1_emplvl": float,
     "lq_month2_emplvl": float,
     "lq_month3_emplvl": float,
     "lq_qtrly_contributions": float,
+    "lq_qtrly_estabs": float,
     "lq_qtrly_estabs_count": float,
     "lq_taxable_annual_wages": float,
     "lq_taxable_qtrly_wages": float,
     "lq_total_annual_wages": float,
     "lq_total_qtrly_wages": float,
     "month1_emplvl": int,
     "month2_emplvl": int,
@@ -63,14 +64,16 @@
     "oty_month2_emplvl_pct_chg": float,
     "oty_month3_emplvl_chg": int,
     "oty_month3_emplvl_pct": float,
     "oty_month3_emplvl_pct_chg": float,
     "oty_qtrly_contributions_chg": int,
     "oty_qtrly_contributions_pct": float,
     "oty_qtrly_contributions_pct_chg": float,
+    "oty_qtrly_estabs_chg": int,
+    "oty_qtrly_estabs_pct_chg": float,
     "oty_qtrly_estabs_count_chg": int,
     "oty_qtrly_estabs_count_pct_chg": float,
     "oty_taxable_annual_wages_chg": int,
     "oty_taxable_annual_wages_pct_chg": float,
     "oty_taxable_qtrly_wages_chg": int,
     "oty_taxable_qtrly_wages_pct": float,
     "oty_taxable_qtrly_wages_pct_chg": float,
@@ -79,198 +82,199 @@
     "oty_total_qtrly_wages_chg": int,
     "oty_total_qtrly_wages_pct": float,
     "oty_total_qtrly_wages_pct_chg": float,
     "own_code": str,
     "own_title": str,
     "qtr": str,
     "qtrly_contributions": int,
+    "qtrly_estabs": int,
     "qtrly_estabs_count": int,
     "size_code": str,
     "size_title": str,
     "taxable_annual_wages": int,
     "taxable_qtrly_wages": int,
     "total_annual_wages": int,
     "total_qtrly_wages": int,
     "year": str,
-}
+    }
 
 
-def slice_qcew(area_slice: bool, qcew_codes: list, year: str, annual_data: bool=True, 
-               fields: Union[list, None]=None) -> list:
+def get_qcew_data(year: str, annual: bool=False, fields: Union[list, None]=None) -> list:
     '''
-    Returns a slice of QCEW data for a given area or industry, for a given `year`. Data are read 
-    into memory from the web, without being stored on disk.
+    Returns all annual or quarterly QCEW data for a given `year`.
 
     ### Parameters
-    `area_slice` : bool
-        True for QCEW area-based data. False for QCEW industry-based data.
-    `qcew_codes` : list[str]
-        The QCEW area or industry code(s) of interest. Valid codes can be found at: 
-        https://www.bls.gov/cew/classifications/.
     `year` : str
-        Reference year. NOTE: QCEW data are only available from 1975 onward and data for 1975-1989
-        are only available for industry "10" (total, all industries).
-    `annual_data` : bool (default: True)
-        True for annual-interval data. False for quarterly-interval data. Defaults to True.
-    `fields`: list[str] or None (default: None)
+        Reference year. NOTE: QCEW data are only available from 1990 onward.
+    `annual` : bool (default: False)
+        True for annual data. False for quarterly data. Defaults to False.
+    `fields`: str or None (default: None)
         Names of fields to keep. Use None if keeping all fields. Defaults to None. NOTE: Specifying 
         fields will decrease memory usage and improve performance. Quarterly fields can be found at:
         https://www.bls.gov/cew/about-data/downloadable-file-layouts/quarterly/naics-based-quarterly-layout.htm
         Annual fields can be found at: https://www.bls.gov/cew/about-data/downloadable-file-layouts/annual/naics-based-annual-layout.htm
 
     ### Returns
-    list[dict] : A slice of QCEW data.
+    list[dict] : Annual or quarterly QCEW data for a single year.
     '''
-    if int(year) < 1975:
-        raise ValueError('Invalid year arg. QCEW data are only available from 1975 onward.')
-    if int(year) in range(1975, 1990) and (area_slice or qcew_codes != ["10"]):
-        raise ValueError((
-            'Invalid area_slice and/or qcew_codes arg(s). QCEW data from 1975 to 1989 are only'
-            ' available for industry "10" (total, all industries). Try area_slice = False and'
-            ' qcew_codes = ["10"].'
-        ))
+    if int(year) < 1990:
+        raise ValueError('Invalid year arg. Data are only accessible from 1990 onward.')
+    
+    interval = "annual" if annual else "qtrly"
+    url = f"https://data.bls.gov/cew/data/files/{year}/csv/{year}_{interval}_singlefile.zip"
     
-    interval = "annual" if annual_data else "qtrly"
-    slice_type = "area" if area_slice else "industry"
-    if int(year) in range(1975, 1990):
-        url = f"https://data.bls.gov/cew/data/files/{year}/csv/{year}_{interval}_naics10_totals.zip"
-    else:
-        url = f"https://data.bls.gov/cew/data/files/{year}/csv/{year}_{interval}_by_{slice_type}.zip"
-
     try:
-        request = urlopen(url).read()
+        response = urlopen(url)
     except:
         raise ValueError((
             f'Cannot find URL: "{url}". These data may have not yet been published by BLS. For more'
             ' information, please see: https://www.bls.gov/cew/downloadable-data-files.htm.'
         ))
     else:
-        zip = ZipFile(BytesIO(request), "r")
-        
-        files, codes_without_data = [], []
-        for qcew_code in qcew_codes:
-            code_not_found = True
-            for file in zip.namelist():
-                if f" {qcew_code} " in file:
-                    files.append(file)
-                    code_not_found = False
-            if code_not_found:
-                codes_without_data.append(qcew_code)
-
-        qcew_slice = []
-        for file in files:
-            with zip.open(file) as input:
-                field_names = parse_line(input.readline()) # Parse first line, which contains field names.
-                keep_fields = fields if fields else field_names # Get the list of fields to keep
-                field_types = { # Get the types of each kept field as well as their row index.
-                    f: {"type": FIELD_TYPES[f], "index": field_names.index(f)} for f in keep_fields
-                }
-                for line in input.readlines():
-                    row = parse_line(line)
-                    qcew_slice.append({k: v["type"](row[v["index"]]) for k, v in field_types.items()})
-        
-        for qcew_code in codes_without_data:
-            print(f"No {interval} data for {slice_type} {qcew_code} in {year}.")
-
-        return(qcew_slice)
+        zip = ZipFile(BytesIO(response.read()), "r")
+        qcew_data = []
+        with zip.open(zip.namelist()[0]) as input:
+            field_names = parse_line(input.readline()) # Parse first line, which contains field names.
+            keep_fields = fields if fields else field_names # Get the list of fields to keep
+            field_types = { # Get the types of each kept field as well as their row index.
+                f: {"type": FIELD_TYPES[f], "index": field_names.index(f)} for f in keep_fields
+            }
+            for line in input.readlines():
+                row = parse_line(line)
+                qcew_data.append({k: v["type"](row[v["index"]]) for k, v in field_types.items()})
+        return(qcew_data)
 
 
-def get_qcew_data_slice(area_slice: bool, qcew_codes: list, years: list, annual_data: bool=True, 
+def get_qcew_data_slice(slice_type: str, qcew_codes: list, years: list, annual_data: bool=False, 
                         fields: Union[list, None]=None) -> list:
     '''
-    Returns a slice of QCEW data for a given area or industry, for a range of years.
+    Returns a slice of QCEW data for a given area/industry/establishment size, for a range of years.
     
     NOTE: Yearly data slices are wrangled in parallel processes and then concatenated in order to 
     boost performance.
     
     ### Parameters
-    `area_slice` : bool
-        True for QCEW area-based data. False for QCEW industry-based data.
+    `slice_type` : str
+        Type of QCEW data, either: "area", "industry", or "size". Use "area" to get QCEW data for
+        one or more areas. Use "industry" to get QCEW data for one or more industries. Use "size" to 
+        get QCEW data for one or more establishment sizes.
     `qcew_codes` : list[str]
-        The QCEW area or industry code(s) of interest. Valid codes can be found at: 
+        The QCEW area/industry/establishment size code(s) of interest. Valid codes can be found at: 
         https://www.bls.gov/cew/classifications/.
     `years` : list[str]
         Reference year(s). NOTE: QCEW data are only available from 1975 onward, and data for 
         1975-1989 are only available for industry "10" (total, all industries).
-    `annual_data` : bool (default: True)
-        True for annual-interval data. False for quarterly-interval data. Defaults to True.
+    `annual_data` : bool (default: False)
+        True for annual-interval data. False for quarterly-interval data. Defaults to False. NOTE: 
+        QCEW data by establishment size are only available at the quarterly-interval.
     `fields`: str or None (default: None)
         Names of fields to keep. Use None if keeping all fields. Defaults to None. NOTE: Specifying 
         fields will decrease memory usage and improve performance. Quarterly fields can be found at:
         https://www.bls.gov/cew/about-data/downloadable-file-layouts/quarterly/naics-based-quarterly-layout.htm
         Annual fields can be found at: https://www.bls.gov/cew/about-data/downloadable-file-layouts/annual/naics-based-annual-layout.htm
 
     ### Returns
     list[dict] : A slice of QCEW data.
     '''
-    for year in years:
-        if int(year) < 1975:
-            raise ValueError('Invalid years arg. QCEW data are only available from 1975 onward.')
-        if int(year) in range(1975, 1990) and (area_slice or qcew_codes != ["10"]):
-            raise ValueError((
-                'Invalid area_slice and/or qcew_codes arg(s). QCEW data from 1975 to 1989 are only'
-                ' available for industry "10" (total, all industries). Try area_slice = False and'
-                ' qcew_codes = ["10"].'
-            ))
-    
-    processes = [(slice_qcew, area_slice, qcew_codes, y, annual_data, fields) for y in years]
+    check_args(slice_type, qcew_codes, years, annual_data, fields)
+
+    processes = [(slice_qcew, slice_type, qcew_codes, y, annual_data, fields) for y in years]
     with ProcessPoolExecutor() as multiprocessor:
         futures = [multiprocessor.submit(*process) for process in processes]
     
     qcew_data = []
     for future in futures:
         qcew_data += future.result()
     
     return(qcew_data)
 
 
-def get_qcew_data(year: str, annual: bool=True, fields: Union[list, None]=None) -> list:
+def slice_qcew(slice_type: str, qcew_codes: list, year: str, annual_data: bool=False, 
+               fields: Union[list, None]=None) -> list:
     '''
-    Returns all annual or quarterly QCEW data for a given `year`.
+    Returns a slice of QCEW data for a given area/industry/establishment size, for a given `year`. 
+    Data are read into memory from the web, without being stored on disk.
 
     ### Parameters
+    `slice_type` : str
+        Type of QCEW data, either: "area", "industry", or "size". Use "area" to get QCEW data for
+        one or more areas. Use "industry" to get QCEW data for one or more industries. Use "size" to 
+        get QCEW data for one or more establishment sizes.
+    `qcew_codes` : list[str]
+        The QCEW area/industry/establishment size code(s) of interest. Valid codes can be found at: 
+        https://www.bls.gov/cew/classifications/.
     `year` : str
-        Reference year. NOTE: QCEW data are only available from 1990 onward.
-    `annual` : bool (default: True)
-        True for annual data. False for quarterly data. Defaults to True.
+        Reference year. NOTE: QCEW data are only available from 1975 onward, and data for 1975-1989 
+        are only available for industry "10" (total, all industries).
+    `annual_data` : bool (default: False)
+        True for annual-interval data. False for quarterly-interval data. Defaults to False. NOTE: 
+        QCEW data by establishment size are only available at the quarterly-interval.
     `fields`: str or None (default: None)
         Names of fields to keep. Use None if keeping all fields. Defaults to None. NOTE: Specifying 
         fields will decrease memory usage and improve performance. Quarterly fields can be found at:
         https://www.bls.gov/cew/about-data/downloadable-file-layouts/quarterly/naics-based-quarterly-layout.htm
         Annual fields can be found at: https://www.bls.gov/cew/about-data/downloadable-file-layouts/annual/naics-based-annual-layout.htm
 
     ### Returns
-    list[dict] : Annual or quarterly QCEW data for a single year.
+    list[dict] : A slice of QCEW data.
     '''
-    if int(year) < 1990:
-        raise ValueError('Invalid year arg. Data are only accessible from 1990 onward.')
-    
-    interval = "annual" if annual else "qtrly"
-    url = f"https://data.bls.gov/cew/data/files/{year}/csv/{year}_{interval}_singlefile.zip"
+    check_args(slice_type, qcew_codes, [year], annual_data, fields)
     
+    interval = "annual" if annual_data else "qtrly"
+    if int(year) in range(1975, 1990):
+        url = f"https://data.bls.gov/cew/data/files/{year}/csv/{year}_{interval}_naics10_totals.zip"
+    else:
+        if slice_type == "size":
+            url = f"https://data.bls.gov/cew/data/files/{year}/csv/{year}_q1_by_size.zip"
+        else:
+            url = f"https://data.bls.gov/cew/data/files/{year}/csv/{year}_{interval}_by_{slice_type}.zip"
+
     try:
-        request = urlopen(url).read()
+        response = urlopen(url)
     except:
         raise ValueError((
             f'Cannot find URL: "{url}". These data may have not yet been published by BLS. For more'
             ' information, please see: https://www.bls.gov/cew/downloadable-data-files.htm.'
         ))
     else:
-        zip = ZipFile(BytesIO(request), "r")
-        qcew_data = []
-        with zip.open(zip.namelist()[0]) as input:
-            field_names = parse_line(input.readline()) # Parse first line, which contains field names.
-            keep_fields = fields if fields else field_names # Get the list of fields to keep
-            field_types = { # Get the types of each kept field as well as their row index.
-                f: {"type": FIELD_TYPES[f], "index": field_names.index(f)} for f in keep_fields
-            }
-            for line in input.readlines():
-                row = parse_line(line)
-                qcew_data.append({k: v["type"](row[v["index"]]) for k, v in field_types.items()})
-        return(qcew_data)
+        zip = ZipFile(BytesIO(response.read()), "r")
+        
+        files, codes_without_data = [], []
+        if slice_type == "size":
+            for file in zip.namelist():
+                files.append(file)
+        else:
+            for qcew_code in qcew_codes:
+                code_not_found = True
+                for file in zip.namelist():
+                    if f" {qcew_code} " in file:
+                        files.append(file)
+                        code_not_found = False
+                if code_not_found:
+                    codes_without_data.append(qcew_code)
+
+        qcew_slice = []
+        for file in files:
+            with zip.open(file) as input:
+                field_names = parse_line(input.readline()) # Parse first line, which contains field names.
+                keep_fields = fields if fields else field_names # Get the list of fields to keep
+                field_types = { # Get the types of each kept field as well as their row index.
+                    f: {"type": FIELD_TYPES[f], "index": field_names.index(f)} for f in keep_fields
+                }
+                for line in input.readlines():
+                    row = parse_line(line)
+                    qcew_slice.append({k: v["type"](row[v["index"]]) for k, v in field_types.items()})
+        
+        if slice_type == "size":
+            qcew_slice = [d for d in qcew_slice if d["size_code"] in qcew_codes]
+        
+        for qcew_code in codes_without_data:
+            print(f"No {interval} data for {slice_type} {qcew_code} in {year}.")
+
+        return(qcew_slice)
 
 
 def parse_line(line: bytes) -> list:
     '''
     Returns a parsed list of values from a given `line` of bytes.
 
     ### Parameters
@@ -285,7 +289,75 @@
     row = row.replace('"', '') # Remove double quotes.
     row = row.replace('\r\n','') # Remove escape characters.
     row = row.split(',') # Split the row at commas into a list of values.
     row = [v.replace('|', ',') for v in row] # Replace pipes back with commas.
     return(row)
 
 
+def check_args(slice_type: str, qcew_codes: list, years: list, annual_data: bool, 
+               fields: Union[list, None]) -> None:
+    '''
+    Runs a check on passed arguments.
+
+    ### Parameters
+    `slice_type` : str
+        Type of QCEW data, either: "area", "industry", or "size". Use "area" to get QCEW data for
+        one or more areas. Use "industry" to get QCEW data for one or more industries. Use "size" to 
+        get QCEW data for one or more establishment sizes.
+    `qcew_codes` : list[str]
+        The QCEW area/industry/establishment size code(s) of interest. Valid codes can be found at: 
+        https://www.bls.gov/cew/classifications/.
+    `years` : list[str]
+        Reference year(s). NOTE: QCEW data are only available from 1975 onward, and data for 
+        1975-1989 are only available for industry "10" (total, all industries).
+    `annual_data` : bool (default: True)
+        True for annual-interval data. False for quarterly-interval data. Defaults to True. NOTE: 
+        QCEW data by establishment size are only available at the quarterly-interval.
+    `fields`: str or None (default: None)
+        Names of fields to keep. Use None if keeping all fields. Specifying fields will improve
+        performance. Defaults to None.
+
+    ### Raises
+    ValueError if:
+        - `slice_type` requested is not one of: ["area", "industry", "size"].
+        - Any year in `years` precedes 1975.
+        - Area data are requested for any year between 1975 and 1989.
+        - Size data are requested for any year between 1975 and 1989.
+        - Industry data for any industry other than industry "10" are requested for any year between 1975 and 1989.
+        - Annual-interval size data are requested.
+        - If size data are requested for any size code other than "1", "2", "3", "4", "5", "6", "7", "8", and/or "9".
+
+    ### Returns
+    None
+    '''
+    if slice_type not in ['area', 'industry', 'size']:
+        raise ValueError(
+            'Invalid slice_type arg. Expected one of: ["area", "industry", "size"].'
+        )
+    for year in years:
+        if int(year) < 1975:
+            raise ValueError('Invalid years arg. QCEW data are only available from 1975 onward.')
+        if int(year) in range(1975, 1990) and (slice_type != "industry" or qcew_codes != ["10"]):
+            raise ValueError((
+                'Invalid slice_type and/or qcew_codes arg(s). QCEW data from 1975 to 1989 are only'
+                ' available for industry "10" (total, all industries). Try slice_type = "industry"'
+                ' and qcew_codes = ["10"].'
+            ))
+    if slice_type == "size":
+        if annual_data:
+            raise ValueError((
+                'Invalid annual_data arg. QCEW data by establishment size are only available at the'
+                ' quarterly interval. Try annual_data = False.'
+            ))
+        for qcew_code in qcew_codes:
+            if qcew_code not in ["1", "2", "3", "4", "5", "6", "7", "8", "9"]:
+                raise ValueError((
+                    'Invalid qcew_codes arg. QCEW size codes allowable include: ["1", "2", "3",'
+                    ' "4", "5", "6", "7", "8", "9"].'
+                ))
+        if fields and "size_code" not in fields:
+            raise ValueError((
+                'Invalid fields arg. The "size_code" field is needed in order to slice QCEW data'
+                ' by establishment size. Specify the fields argument as a list with "size_code"'
+                ' included or try fields = None.'
+            ))
+
```

