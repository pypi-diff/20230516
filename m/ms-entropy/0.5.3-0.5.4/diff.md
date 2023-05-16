# Comparing `tmp/ms_entropy-0.5.3.tar.gz` & `tmp/ms_entropy-0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_entropy-0.5.3.tar", last modified: Thu May 11 18:19:14 2023, max compression
+gzip compressed data, was "ms_entropy-0.5.4.tar", last modified: Tue May 16 04:51:28 2023, max compression
```

## Comparing `ms_entropy-0.5.3.tar` & `ms_entropy-0.5.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/
--rw-r--r--   0 yli       (1000) yli       (1000)    11357 2023-03-18 01:04:19.000000 ms_entropy-0.5.3/LICENSE
--rw-rw-r--   0 yli       (1000) yli       (1000)       68 2023-05-10 07:52:05.000000 ms_entropy-0.5.3/MANIFEST.in
--rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)     3264 2023-03-29 23:15:55.000000 ms_entropy-0.5.3/README.md
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/ms_entropy/
--rw-rw-r--   0 yli       (1000) yli       (1000)      155 2023-05-10 07:39:51.000000 ms_entropy-0.5.3/ms_entropy/__init__.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/ms_entropy/entropy_search/
--rw-rw-r--   0 yli       (1000) yli       (1000)      196 2023-05-10 21:32:05.000000 ms_entropy-0.5.3/ms_entropy/entropy_search/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)    20245 2023-05-10 07:39:35.000000 ms_entropy-0.5.3/ms_entropy/entropy_search/flash_entropy_search.py
--rw-rw-r--   0 yli       (1000) yli       (1000)    27891 2023-05-10 07:39:35.000000 ms_entropy-0.5.3/ms_entropy/entropy_search/flash_entropy_search_core.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     5661 2023-05-10 07:39:35.000000 ms_entropy-0.5.3/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/ms_entropy/file_io/
--rw-rw-r--   0 yli       (1000) yli       (1000)       62 2023-05-10 23:13:55.000000 ms_entropy-0.5.3/ms_entropy/file_io/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     2047 2023-05-10 07:39:40.000000 ms_entropy-0.5.3/ms_entropy/file_io/lbm2_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     1690 2023-05-10 07:39:40.000000 ms_entropy-0.5.3/ms_entropy/file_io/mgf_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     1930 2023-05-10 07:39:40.000000 ms_entropy-0.5.3/ms_entropy/file_io/msp_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     1974 2023-05-10 07:39:40.000000 ms_entropy-0.5.3/ms_entropy/file_io/mzml_file.py
--rw-rw-r--   0 yli       (1000) yli       (1000)      920 2023-05-10 07:39:40.000000 ms_entropy-0.5.3/ms_entropy/file_io/shared.py
--rw-rw-r--   0 yli       (1000) yli       (1000)     5718 2023-05-10 23:12:41.000000 ms_entropy-0.5.3/ms_entropy/file_io/spec_file.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/ms_entropy/tools/
--rw-rw-r--   0 yli       (1000) yli       (1000)      118 2023-05-10 07:39:45.000000 ms_entropy-0.5.3/ms_entropy/tools/__init__.py
--rw-rw-r--   0 yli       (1000) yli       (1000)   903746 2023-05-10 07:43:19.000000 ms_entropy-0.5.3/ms_entropy/tools/fast_entropy.c
--rw-rw-r--   0 yli       (1000) yli       (1000)     3183 2023-05-10 07:39:45.000000 ms_entropy-0.5.3/ms_entropy/tools/fast_entropy.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)   895888 2023-05-10 07:43:20.000000 ms_entropy-0.5.3/ms_entropy/tools/fast_spectrum.c
--rw-rw-r--   0 yli       (1000) yli       (1000)     4978 2023-05-10 07:39:45.000000 ms_entropy-0.5.3/ms_entropy/tools/fast_spectrum.pyx
--rw-rw-r--   0 yli       (1000) yli       (1000)     4318 2023-05-10 07:39:45.000000 ms_entropy-0.5.3/ms_entropy/tools/tools.py
-drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/ms_entropy.egg-info/
--rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-11 18:19:14.000000 ms_entropy-0.5.3/ms_entropy.egg-info/PKG-INFO
--rw-rw-r--   0 yli       (1000) yli       (1000)     1404 2023-05-11 18:19:14.000000 ms_entropy-0.5.3/ms_entropy.egg-info/SOURCES.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-05-11 18:19:14.000000 ms_entropy-0.5.3/ms_entropy.egg-info/dependency_links.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)       84 2023-05-11 18:19:14.000000 ms_entropy-0.5.3/ms_entropy.egg-info/requires.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-05-11 18:19:14.000000 ms_entropy-0.5.3/ms_entropy.egg-info/top_level.txt
--rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-03-24 01:05:23.000000 ms_entropy-0.5.3/pyproject.toml
--rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-05-11 18:19:14.539361 ms_entropy-0.5.3/setup.cfg
--rw-rw-r--   0 yli       (1000) yli       (1000)     1648 2023-05-11 18:17:51.000000 ms_entropy-0.5.3/setup.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 04:51:28.015557 ms_entropy-0.5.4/
+-rw-r--r--   0 yli       (1000) yli       (1000)    11357 2023-03-18 01:04:19.000000 ms_entropy-0.5.4/LICENSE
+-rw-rw-r--   0 yli       (1000) yli       (1000)       68 2023-05-10 07:52:05.000000 ms_entropy-0.5.4/MANIFEST.in
+-rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-16 04:51:28.015557 ms_entropy-0.5.4/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3264 2023-03-29 23:15:55.000000 ms_entropy-0.5.4/README.md
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 04:51:28.011557 ms_entropy-0.5.4/ms_entropy/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      177 2023-05-13 02:10:56.000000 ms_entropy-0.5.4/ms_entropy/__init__.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 04:51:28.011557 ms_entropy-0.5.4/ms_entropy/entropy_search/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      196 2023-05-10 21:32:05.000000 ms_entropy-0.5.4/ms_entropy/entropy_search/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    20160 2023-05-15 19:49:33.000000 ms_entropy-0.5.4/ms_entropy/entropy_search/flash_entropy_search.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)    27891 2023-05-10 07:39:35.000000 ms_entropy-0.5.4/ms_entropy/entropy_search/flash_entropy_search_core.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     5661 2023-05-10 07:39:35.000000 ms_entropy-0.5.4/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 04:51:28.015557 ms_entropy-0.5.4/ms_entropy/file_io/
+-rw-rw-r--   0 yli       (1000) yli       (1000)       62 2023-05-10 23:13:55.000000 ms_entropy-0.5.4/ms_entropy/file_io/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     2047 2023-05-10 07:39:40.000000 ms_entropy-0.5.4/ms_entropy/file_io/lbm2_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1690 2023-05-10 07:39:40.000000 ms_entropy-0.5.4/ms_entropy/file_io/mgf_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1930 2023-05-10 07:39:40.000000 ms_entropy-0.5.4/ms_entropy/file_io/msp_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     2208 2023-05-15 18:02:39.000000 ms_entropy-0.5.4/ms_entropy/file_io/mzml_file.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)      920 2023-05-10 07:39:40.000000 ms_entropy-0.5.4/ms_entropy/file_io/shared.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)     5722 2023-05-15 19:09:34.000000 ms_entropy-0.5.4/ms_entropy/file_io/spec_file.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 04:51:28.015557 ms_entropy-0.5.4/ms_entropy/tools/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      118 2023-05-10 07:39:45.000000 ms_entropy-0.5.4/ms_entropy/tools/__init__.py
+-rw-rw-r--   0 yli       (1000) yli       (1000)   903746 2023-05-10 07:43:19.000000 ms_entropy-0.5.4/ms_entropy/tools/fast_entropy.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     3183 2023-05-10 07:39:45.000000 ms_entropy-0.5.4/ms_entropy/tools/fast_entropy.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)   895888 2023-05-10 07:43:20.000000 ms_entropy-0.5.4/ms_entropy/tools/fast_spectrum.c
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4978 2023-05-10 07:39:45.000000 ms_entropy-0.5.4/ms_entropy/tools/fast_spectrum.pyx
+-rw-rw-r--   0 yli       (1000) yli       (1000)     4318 2023-05-10 07:39:45.000000 ms_entropy-0.5.4/ms_entropy/tools/tools.py
+drwxrwxr-x   0 yli       (1000) yli       (1000)        0 2023-05-16 04:51:28.015557 ms_entropy-0.5.4/ms_entropy.egg-info/
+-rw-rw-r--   0 yli       (1000) yli       (1000)      402 2023-05-16 04:51:27.000000 ms_entropy-0.5.4/ms_entropy.egg-info/PKG-INFO
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1404 2023-05-16 04:51:27.000000 ms_entropy-0.5.4/ms_entropy.egg-info/SOURCES.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)        1 2023-05-16 04:51:27.000000 ms_entropy-0.5.4/ms_entropy.egg-info/dependency_links.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)       84 2023-05-16 04:51:27.000000 ms_entropy-0.5.4/ms_entropy.egg-info/requires.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)       11 2023-05-16 04:51:27.000000 ms_entropy-0.5.4/ms_entropy.egg-info/top_level.txt
+-rw-rw-r--   0 yli       (1000) yli       (1000)      111 2023-03-24 01:05:23.000000 ms_entropy-0.5.4/pyproject.toml
+-rw-rw-r--   0 yli       (1000) yli       (1000)      128 2023-05-16 04:51:28.015557 ms_entropy-0.5.4/setup.cfg
+-rw-rw-r--   0 yli       (1000) yli       (1000)     1648 2023-05-16 04:51:21.000000 ms_entropy-0.5.4/setup.py
```

### Comparing `ms_entropy-0.5.3/LICENSE` & `ms_entropy-0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.3/README.md` & `ms_entropy-0.5.4/README.md`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.3/ms_entropy/entropy_search/flash_entropy_search.py` & `ms_entropy-0.5.4/ms_entropy/entropy_search/flash_entropy_search.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,17 +232,15 @@
                                                                precursor_mz=spec["precursor_mz"],
                                                                precursor_ions_removal_da=precursor_ions_removal_da,
                                                                noise_threshold=noise_threshold,
                                                                min_ms2_difference_in_da=min_ms2_difference_in_da,
                                                                max_peak_num=max_peak_num)
             if len(spec["peaks"]) > 0:
                 all_spectra_list.append(spec)
-                metadata = copy.copy(spec)
-                metadata.pop("peaks")
-                all_metadata_list.append(pickle.dumps(metadata))
+                all_metadata_list.append(pickle.dumps(spec))
 
         # Extract precursor m/z array
         self.precursor_mz_array = np.array([spec["precursor_mz"] for spec in all_spectra_list], dtype=np.float32)
 
         # Extract metadata array
         all_metadata_len = np.array([0]+[len(metadata) for metadata in all_metadata_list], dtype=np.uint64)
         self.metadata_loc = np.cumsum(all_metadata_len).astype(np.uint64)
```

### Comparing `ms_entropy-0.5.3/ms_entropy/entropy_search/flash_entropy_search_core.py` & `ms_entropy-0.5.4/ms_entropy/entropy_search/flash_entropy_search_core.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.3/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py` & `ms_entropy-0.5.4/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.3/ms_entropy/file_io/lbm2_file.py` & `ms_entropy-0.5.4/ms_entropy/file_io/lbm2_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.3/ms_entropy/file_io/mgf_file.py` & `ms_entropy-0.5.4/ms_entropy/file_io/mgf_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.3/ms_entropy/file_io/msp_file.py` & `ms_entropy-0.5.4/ms_entropy/file_io/msp_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.3/ms_entropy/file_io/mzml_file.py` & `ms_entropy-0.5.4/ms_entropy/file_io/mzml_file.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,14 +17,20 @@
             "_ms_level": raw_spectrum_info.ms_level,
             "_scan_number": _scan_number + 1,
             "peaks": np.asarray(raw_spectrum_info.peaks("centroided"), dtype=np.float32, order="C"),
             'rt': raw_spectrum_info.scan_time_in_minutes() * 60,
             'precursor_mz': raw_spectrum_info.selected_precursors[0].get('mz', None) if len(raw_spectrum_info.selected_precursors) > 0 else None,
             'precursor_charge': raw_spectrum_info.selected_precursors[0].get('charge', None) if len(raw_spectrum_info.selected_precursors) > 0 else None,
         }
+        try:
+            spectrum_title = raw_spectrum_info.get_element_by_name("spectrum title")
+            spectrum_info["name"] = spectrum_title.attrib["value"]
+        except:
+            spectrum_info["name"] = ""
+            
         if spectrum_info["precursor_charge"] is None:
             if raw_spectrum_info["negative scan"]:
                 spectrum_info["precursor_charge"] = -1
             elif raw_spectrum_info["positive scan"]:
                 spectrum_info["precursor_charge"] = 1
         else:
             try:
@@ -34,8 +40,8 @@
                 elif raw_spectrum_info["positive scan"]:
                     spectrum_info["precursor_charge"] = abs(spectrum_info["precursor_charge"])
             except ValueError:
                 print("Warning: precursor charge is not an integer: {}".format(spectrum_info["precursor_charge"]))
 
         yield spectrum_info
 
-    run.close()
+    run.close()
```

### Comparing `ms_entropy-0.5.3/ms_entropy/file_io/shared.py` & `ms_entropy-0.5.4/ms_entropy/file_io/shared.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.3/ms_entropy/file_io/spec_file.py` & `ms_entropy-0.5.4/ms_entropy/file_io/spec_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,16 +33,16 @@
                         spec_result[key_target] = cast_type(spectrum_dict.pop(key_candidate))
                     break
                 except:
                     continue
         else:
             spec_result[key_target] = value_default
 
-        for key_candidate in key_all_candidates:
-            spectrum_dict.pop(key_candidate, None)
+        # for key_candidate in key_all_candidates:
+        #     spectrum_dict.pop(key_candidate, None)
     return spec_result
 
 
 def read_one_spectrum(file_input: Union[str, Path],
                       file_type: object = None,
                       **kwargs) -> dict:
     """
```

### Comparing `ms_entropy-0.5.3/ms_entropy/tools/fast_entropy.c` & `ms_entropy-0.5.4/ms_entropy/tools/fast_entropy.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.3/ms_entropy/tools/fast_entropy.pyx` & `ms_entropy-0.5.4/ms_entropy/tools/fast_entropy.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.3/ms_entropy/tools/fast_spectrum.c` & `ms_entropy-0.5.4/ms_entropy/tools/fast_spectrum.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.3/ms_entropy/tools/fast_spectrum.pyx` & `ms_entropy-0.5.4/ms_entropy/tools/fast_spectrum.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.3/ms_entropy/tools/tools.py` & `ms_entropy-0.5.4/ms_entropy/tools/tools.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.3/ms_entropy.egg-info/SOURCES.txt` & `ms_entropy-0.5.4/ms_entropy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ms_entropy-0.5.3/setup.py` & `ms_entropy-0.5.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import os
 
 
 os.environ['CFLAGS'] = '-O3 -Wno-cpp -Wno-unused-function'
 
 setup(
     name='ms_entropy',
-    version='0.5.3',
+    version='0.5.4',
     license='Apache License 2.0',
     author='Yuanyue Li',
     url='https://github.com/YuanyueLi/SpectralEntropy',
     packages=find_packages(where='.', exclude=['tests', 'docs', 'examples', 'manuscript', 'dist', 'build']),
     python_requires='>=3.8',
     install_requires=[
         "numpy >= 1.18",
```

