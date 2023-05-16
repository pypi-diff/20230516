# Comparing `tmp/skelly_synchronize-2023.5.1014.tar.gz` & `tmp/skelly_synchronize-2023.5.1015.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skelly_synchronize-2023.5.1014.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "skelly_synchronize-2023.5.1015.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `skelly_synchronize-2023.5.1014.tar` & `skelly_synchronize-2023.5.1015.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0       65 2023-05-16 20:30:38.970420 skelly_synchronize-2023.5.1014/.gitattributes
--rw-r--r--   0        0        0      146 2023-05-16 20:30:38.970420 skelly_synchronize-2023.5.1014/.github/workflows/lint-with-black.yml
--rw-r--r--   0        0        0     1087 2023-05-16 20:30:38.970420 skelly_synchronize-2023.5.1014/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
--rw-r--r--   0        0        0     1025 2023-05-16 20:30:38.970420 skelly_synchronize-2023.5.1014/.github/workflows/python-testing.yml
--rw-r--r--   0        0        0     2783 2023-05-16 20:30:38.970420 skelly_synchronize-2023.5.1014/.gitignore
--rw-r--r--   0        0        0    34523 2023-05-16 20:30:38.970420 skelly_synchronize-2023.5.1014/LICENSE
--rw-r--r--   0        0        0     3030 2023-05-16 20:30:38.970420 skelly_synchronize-2023.5.1014/README.md
--rw-r--r--   0        0        0     1608 2023-05-16 20:30:38.970420 skelly_synchronize-2023.5.1014/pyproject.toml
--rw-r--r--   0        0        0      123 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/requirements.txt
--rw-r--r--   0        0        0       50 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/setup.py
--rw-r--r--   0        0        0     1056 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/__init__.py
--rw-r--r--   0        0        0      333 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/__main__.py
--rw-r--r--   0        0        0     2192 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/core_processes/audio_utilities.py
--rw-r--r--   0        0        0     2758 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/core_processes/correlation_functions.py
--rw-r--r--   0        0        0      821 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/core_processes/debug_output.py
--rw-r--r--   0        0        0     1557 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
--rw-r--r--   0        0        0     2699 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
--rw-r--r--   0        0        0     4510 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/core_processes/video_functions/video_utilities.py
--rw-r--r--   0        0        0     1821 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/gui/skelly_synchronize_gui.py
--rw-r--r--   0        0        0      420 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/gui/widgets/run_button_widget.py
--rw-r--r--   0        0        0     4763 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/skelly_synchronize.py
--rw-r--r--   0        0        0        0 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/system/__init__.py
--rw-r--r--   0        0        0     1479 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/system/default_paths.py
--rw-r--r--   0        0        0     1402 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/system/logging_configuration.py
--rw-r--r--   0        0        0      323 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/system/paths_and_file_names.py
--rw-r--r--   0        0        0     1085 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/tests/conftest.py
--rw-r--r--   0        0        0      656 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/tests/test_normalize_lag_dict.py
--rw-r--r--   0        0        0      847 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/tests/test_trim_single_video_deffcode.py
--rw-r--r--   0        0        0      577 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
--rw-r--r--   0        0        0      262 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
--rw-r--r--   0        0        0     1263 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
--rw-r--r--   0        0        0     1061 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/tests/utilities/load_sample_data.py
--rw-r--r--   0        0        0     2048 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
--rw-r--r--   0        0        0     1340 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/utils/get_video_files.py
--rw-r--r--   0        0        0     1569 2023-05-16 20:30:38.974420 skelly_synchronize-2023.5.1014/skelly_synchronize/utils/path_handling_utilities.py
--rw-r--r--   0        0        0     3917 1970-01-01 00:00:00.000000 skelly_synchronize-2023.5.1014/PKG-INFO
+-rw-r--r--   0        0        0       65 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/.gitattributes
+-rw-r--r--   0        0        0      146 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/.github/workflows/lint-with-black.yml
+-rw-r--r--   0        0        0     1087 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml
+-rw-r--r--   0        0        0     1025 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/.github/workflows/python-testing.yml
+-rw-r--r--   0        0        0     2783 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/.gitignore
+-rw-r--r--   0        0        0    34523 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/LICENSE
+-rw-r--r--   0        0        0     3030 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/README.md
+-rw-r--r--   0        0        0     1626 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/pyproject.toml
+-rw-r--r--   0        0        0      132 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/requirements.txt
+-rw-r--r--   0        0        0       50 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/setup.py
+-rw-r--r--   0        0        0     1056 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/skelly_synchronize/__init__.py
+-rw-r--r--   0        0        0      333 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/skelly_synchronize/__main__.py
+-rw-r--r--   0        0        0     2192 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/skelly_synchronize/core_processes/audio_utilities.py
+-rw-r--r--   0        0        0     2758 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/skelly_synchronize/core_processes/correlation_functions.py
+-rw-r--r--   0        0        0      821 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/skelly_synchronize/core_processes/debug_output.py
+-rw-r--r--   0        0        0     1557 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/skelly_synchronize/core_processes/video_functions/deffcode_functions.py
+-rw-r--r--   0        0        0     2699 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py
+-rw-r--r--   0        0        0     4510 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/skelly_synchronize/core_processes/video_functions/video_utilities.py
+-rw-r--r--   0        0        0     1821 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/skelly_synchronize/gui/skelly_synchronize_gui.py
+-rw-r--r--   0        0        0      420 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/skelly_synchronize/gui/widgets/run_button_widget.py
+-rw-r--r--   0        0        0     4763 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/skelly_synchronize/skelly_synchronize.py
+-rw-r--r--   0        0        0        0 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/skelly_synchronize/system/__init__.py
+-rw-r--r--   0        0        0     1479 2023-05-16 20:32:50.855021 skelly_synchronize-2023.5.1015/skelly_synchronize/system/default_paths.py
+-rw-r--r--   0        0        0     1402 2023-05-16 20:32:50.859022 skelly_synchronize-2023.5.1015/skelly_synchronize/system/logging_configuration.py
+-rw-r--r--   0        0        0      323 2023-05-16 20:32:50.859022 skelly_synchronize-2023.5.1015/skelly_synchronize/system/paths_and_file_names.py
+-rw-r--r--   0        0        0     1085 2023-05-16 20:32:50.859022 skelly_synchronize-2023.5.1015/skelly_synchronize/tests/conftest.py
+-rw-r--r--   0        0        0      656 2023-05-16 20:32:50.859022 skelly_synchronize-2023.5.1015/skelly_synchronize/tests/test_normalize_lag_dict.py
+-rw-r--r--   0        0        0      847 2023-05-16 20:32:50.859022 skelly_synchronize-2023.5.1015/skelly_synchronize/tests/test_trim_single_video_deffcode.py
+-rw-r--r--   0        0        0      577 2023-05-16 20:32:50.859022 skelly_synchronize-2023.5.1015/skelly_synchronize/tests/utilities/check_list_values_are_equal.py
+-rw-r--r--   0        0        0      262 2023-05-16 20:32:50.859022 skelly_synchronize-2023.5.1015/skelly_synchronize/tests/utilities/find_frame_count_of_video.py
+-rw-r--r--   0        0        0     1263 2023-05-16 20:32:50.859022 skelly_synchronize-2023.5.1015/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py
+-rw-r--r--   0        0        0     1061 2023-05-16 20:32:50.859022 skelly_synchronize-2023.5.1015/skelly_synchronize/tests/utilities/load_sample_data.py
+-rw-r--r--   0        0        0     2048 2023-05-16 20:32:50.859022 skelly_synchronize-2023.5.1015/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py
+-rw-r--r--   0        0        0     1340 2023-05-16 20:32:50.859022 skelly_synchronize-2023.5.1015/skelly_synchronize/utils/get_video_files.py
+-rw-r--r--   0        0        0     1569 2023-05-16 20:32:50.859022 skelly_synchronize-2023.5.1015/skelly_synchronize/utils/path_handling_utilities.py
+-rw-r--r--   0        0        0     3935 1970-01-01 00:00:00.000000 skelly_synchronize-2023.5.1015/PKG-INFO
```

### Comparing `skelly_synchronize-2023.5.1014/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml` & `skelly_synchronize-2023.5.1015/.github/workflows/publish_to_pypi_when_new_tag_is_pushed_to_main.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/.github/workflows/python-testing.yml` & `skelly_synchronize-2023.5.1015/.github/workflows/python-testing.yml`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/.gitignore` & `skelly_synchronize-2023.5.1015/.gitignore`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/LICENSE` & `skelly_synchronize-2023.5.1015/LICENSE`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/README.md` & `skelly_synchronize-2023.5.1015/README.md`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/pyproject.toml` & `skelly_synchronize-2023.5.1015/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -28,28 +28,28 @@
 dependencies = [
 "pytest",
 "librosa",
 "PyQt6",
 "numpy",
 "scipy",
 "setuptools",
-"opencv-python",
+"opencv-contrib-python==4.6.0.66",
 "deffcode",
 "toml",
 ] #add additional dependencies here - try to pin versions as minimally as possible
 
 requires-python = ">=3.8"
 
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver] #bump the version by entering `bumpver update` in the terminal
-current_version = "v2023.05.1014"
+current_version = "v2023.05.1015"
 version_pattern = "vYYYY.0M.BUILD[-TAG]"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/__init__.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level package for basic_template_repo."""
 
 __package_name__ = "skelly_synchronize"
-__version__ = "v2023.05.1014"
+__version__ = "v2023.05.1015"
 
 __author__ = """Philip Queen"""
 __email__ = "info@freemocap.org"
 __repo_owner_github_user_name__ = "freemocap"
 __repo_url__ = (
     f"https://github.com/{__repo_owner_github_user_name__}/{__package_name__}/"
 )
```

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/core_processes/audio_utilities.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/core_processes/audio_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/core_processes/correlation_functions.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/core_processes/correlation_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/core_processes/debug_output.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/core_processes/debug_output.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/core_processes/video_functions/deffcode_functions.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/core_processes/video_functions/deffcode_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/core_processes/video_functions/ffmpeg_functions.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/core_processes/video_functions/video_utilities.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/core_processes/video_functions/video_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/gui/skelly_synchronize_gui.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/gui/skelly_synchronize_gui.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/skelly_synchronize.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/skelly_synchronize.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/system/default_paths.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/system/default_paths.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/system/logging_configuration.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/system/logging_configuration.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/tests/conftest.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/tests/test_normalize_lag_dict.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/tests/test_normalize_lag_dict.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/tests/test_trim_single_video_deffcode.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/tests/test_trim_single_video_deffcode.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/tests/utilities/check_list_values_are_equal.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/tests/utilities/check_list_values_are_equal.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/tests/utilities/get_number_of_frames_of_videos_in_a_folder.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/tests/utilities/load_sample_data.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/tests/utilities/load_sample_data.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/utils/check_if_video_has_reversed_metadata.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/utils/get_video_files.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/utils/get_video_files.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/skelly_synchronize/utils/path_handling_utilities.py` & `skelly_synchronize-2023.5.1015/skelly_synchronize/utils/path_handling_utilities.py`

 * *Files identical despite different names*

### Comparing `skelly_synchronize-2023.5.1014/PKG-INFO` & `skelly_synchronize-2023.5.1015/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: skelly_synchronize
-Version: 2023.5.1014
+Version: 2023.5.1015
 Summary: Basic template of a python repository
 Keywords: basic,template,python,repository
 Author-email: skelly_synchronize <info@freemocap.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: pytest
 Requires-Dist: librosa
 Requires-Dist: PyQt6
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: setuptools
-Requires-Dist: opencv-python
+Requires-Dist: opencv-contrib-python==4.6.0.66
 Requires-Dist: deffcode
 Requires-Dist: toml
 Requires-Dist: black ; extra == "dev"
 Requires-Dist: bumpver ; extra == "dev"
 Requires-Dist: isort ; extra == "dev"
 Requires-Dist: pip-tools ; extra == "dev"
 Requires-Dist: pytest ; extra == "dev"
```

