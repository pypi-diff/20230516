# Comparing `tmp/pypet2bids-1.1.2.tar.gz` & `tmp/pypet2bids-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypet2bids-1.1.2.tar", max compression
+gzip compressed data, was "pypet2bids-1.2.2.tar", max compression
```

## Comparing `pypet2bids-1.1.2.tar` & `pypet2bids-1.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0      428 2022-11-30 20:30:12.412732 pypet2bids-1.1.2/pypet2bids/Pipfile
--rw-r--r--   0        0        0     9755 2022-11-30 20:30:12.413053 pypet2bids-1.1.2/pypet2bids/README.md
--rw-r--r--   0        0        0        0 2022-11-30 20:30:12.413084 pypet2bids-1.1.2/pypet2bids/__init__.py
--rw-r--r--   0        0        0    37643 2022-11-30 20:30:12.413624 pypet2bids-1.1.2/pypet2bids/convert_pmod_to_blood.py
--rw-r--r--   0        0        0    62353 2023-05-04 17:10:47.656853 pypet2bids-1.1.2/pypet2bids/dcm2niix4pet.py
--rwxr-xr-x   0        0        0    18241 2022-11-30 20:30:12.414789 pypet2bids-1.1.2/pypet2bids/dicom_convert.py
--rw-r--r--   0        0        0    14006 2023-01-20 20:54:10.147427 pypet2bids-1.1.2/pypet2bids/ecat.py
--rw-r--r--   0        0        0    10704 2023-01-20 20:54:10.147812 pypet2bids-1.1.2/pypet2bids/ecat2nii.py
--rw-r--r--   0        0        0     9516 2022-11-30 20:30:12.415581 pypet2bids-1.1.2/pypet2bids/ecat_cli.py
--rw-r--r--   0        0        0   162568 2022-11-30 20:30:12.416153 pypet2bids-1.1.2/pypet2bids/ecat_headers.json
--rw-r--r--   0        0        0     4996 2022-11-30 20:30:12.416272 pypet2bids-1.1.2/pypet2bids/golden_ecat.py
--rw-r--r--   0        0        0    33773 2023-02-22 18:22:21.292332 pypet2bids-1.1.2/pypet2bids/helper_functions.py
--rw-r--r--   0        0        0     6763 2023-03-21 20:12:05.711580 pypet2bids-1.1.2/pypet2bids/is_pet.py
--rw-r--r--   0        0        0     1386 2023-05-04 17:35:51.289125 pypet2bids-1.1.2/pypet2bids/metadata/PET_Radionuclide.mkd
--rw-r--r--   0        0        0     1710 2023-05-04 17:35:51.290897 pypet2bids-1.1.2/pypet2bids/metadata/PET_metadata.json
--rw-r--r--   0        0        0     3377 2023-05-04 17:35:51.289555 pypet2bids-1.1.2/pypet2bids/metadata/PET_reconstruction_methods.json
--rw-r--r--   0        0        0      384 2023-05-04 17:35:51.288683 pypet2bids-1.1.2/pypet2bids/metadata/blood_metadata.json
--rw-r--r--   0        0        0     1182 2023-05-04 17:35:51.290656 pypet2bids-1.1.2/pypet2bids/metadata/definitions.json
--rw-r--r--   0        0        0     2667 2023-05-04 17:35:51.288365 pypet2bids-1.1.2/pypet2bids/metadata/dicom2bids.json
--rw-r--r--   0        0        0     3915 2022-11-30 20:30:12.417192 pypet2bids-1.1.2/pypet2bids/metadata_spreadsheet_example_reader.py
--rw-r--r--   0        0        0     8569 2022-12-27 23:28:49.169202 pypet2bids-1.1.2/pypet2bids/multiple_spreadsheets.py
--rw-r--r--   0        0        0     1542 2023-05-04 17:35:51.294584 pypet2bids-1.1.2/pypet2bids/pyproject.toml
--rw-r--r--   0        0        0    17315 2022-11-30 20:30:12.417834 pypet2bids-1.1.2/pypet2bids/read_ecat.py
--rw-r--r--   0        0        0     3298 2022-11-30 20:30:12.418133 pypet2bids-1.1.2/pypet2bids/sidecar.py
--rw-r--r--   0        0        0     8484 2022-11-30 20:30:12.418396 pypet2bids-1.1.2/pypet2bids/single_spreadsheet.py
--rw-r--r--   0        0        0       95 2022-11-30 20:30:12.418472 pypet2bids-1.1.2/pypet2bids/template.env
--rw-r--r--   0        0        0    12798 2022-11-30 20:30:12.418809 pypet2bids-1.1.2/pypet2bids/write_ecat.py
--rw-r--r--   0        0        0     1542 2023-05-04 17:19:08.656037 pypet2bids-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     3372 1970-01-01 00:00:00.000000 pypet2bids-1.1.2/setup.py
--rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 pypet2bids-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      428 2022-11-30 20:30:12.412732 pypet2bids-1.2.2/pypet2bids/Pipfile
+-rw-r--r--   0        0        0     9755 2022-11-30 20:30:12.413053 pypet2bids-1.2.2/pypet2bids/README.md
+-rw-r--r--   0        0        0        0 2022-11-30 20:30:12.413084 pypet2bids-1.2.2/pypet2bids/__init__.py
+-rw-r--r--   0        0        0    37643 2022-11-30 20:30:12.413624 pypet2bids-1.2.2/pypet2bids/convert_pmod_to_blood.py
+-rw-r--r--   0        0        0    63381 2023-05-15 21:59:10.624742 pypet2bids-1.2.2/pypet2bids/dcm2niix4pet.py
+-rwxr-xr-x   0        0        0    18241 2022-11-30 20:30:12.414789 pypet2bids-1.2.2/pypet2bids/dicom_convert.py
+-rw-r--r--   0        0        0    14006 2023-01-20 20:54:10.147427 pypet2bids-1.2.2/pypet2bids/ecat.py
+-rw-r--r--   0        0        0    10704 2023-01-20 20:54:10.147812 pypet2bids-1.2.2/pypet2bids/ecat2nii.py
+-rw-r--r--   0        0        0     9726 2023-05-11 00:46:54.200694 pypet2bids-1.2.2/pypet2bids/ecat_cli.py
+-rw-r--r--   0        0        0   162568 2022-11-30 20:30:12.416153 pypet2bids-1.2.2/pypet2bids/ecat_headers.json
+-rw-r--r--   0        0        0     4996 2022-11-30 20:30:12.416272 pypet2bids-1.2.2/pypet2bids/golden_ecat.py
+-rw-r--r--   0        0        0    34202 2023-05-15 21:59:10.625273 pypet2bids-1.2.2/pypet2bids/helper_functions.py
+-rw-r--r--   0        0        0     6763 2023-03-21 20:12:05.711580 pypet2bids-1.2.2/pypet2bids/is_pet.py
+-rw-r--r--   0        0        0     1386 2023-05-15 21:59:17.386254 pypet2bids-1.2.2/pypet2bids/metadata/PET_Radionuclide.mkd
+-rw-r--r--   0        0        0     1710 2023-05-15 21:59:17.387413 pypet2bids-1.2.2/pypet2bids/metadata/PET_metadata.json
+-rw-r--r--   0        0        0     3377 2023-05-15 21:59:17.386514 pypet2bids-1.2.2/pypet2bids/metadata/PET_reconstruction_methods.json
+-rw-r--r--   0        0        0      384 2023-05-15 21:59:17.386071 pypet2bids-1.2.2/pypet2bids/metadata/blood_metadata.json
+-rw-r--r--   0        0        0     1182 2023-05-15 21:59:17.387100 pypet2bids-1.2.2/pypet2bids/metadata/definitions.json
+-rw-r--r--   0        0        0     2667 2023-05-15 21:59:17.385733 pypet2bids-1.2.2/pypet2bids/metadata/dicom2bids.json
+-rw-r--r--   0        0        0     3915 2022-11-30 20:30:12.417192 pypet2bids-1.2.2/pypet2bids/metadata_spreadsheet_example_reader.py
+-rw-r--r--   0        0        0     8569 2022-12-27 23:28:49.169202 pypet2bids-1.2.2/pypet2bids/multiple_spreadsheets.py
+-rw-r--r--   0        0        0     1542 2023-05-15 21:59:17.390056 pypet2bids-1.2.2/pypet2bids/pyproject.toml
+-rw-r--r--   0        0        0    17315 2022-11-30 20:30:12.417834 pypet2bids-1.2.2/pypet2bids/read_ecat.py
+-rw-r--r--   0        0        0     3298 2022-11-30 20:30:12.418133 pypet2bids-1.2.2/pypet2bids/sidecar.py
+-rw-r--r--   0        0        0     8483 2023-05-15 21:59:10.625535 pypet2bids-1.2.2/pypet2bids/single_spreadsheet.py
+-rw-r--r--   0        0        0       95 2022-11-30 20:30:12.418472 pypet2bids-1.2.2/pypet2bids/template.env
+-rw-r--r--   0        0        0    12798 2022-11-30 20:30:12.418809 pypet2bids-1.2.2/pypet2bids/write_ecat.py
+-rw-r--r--   0        0        0     1542 2023-05-15 21:59:10.625753 pypet2bids-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3372 1970-01-01 00:00:00.000000 pypet2bids-1.2.2/setup.py
+-rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 pypet2bids-1.2.2/PKG-INFO
```

### Comparing `pypet2bids-1.1.2/pypet2bids/README.md` & `pypet2bids-1.2.2/pypet2bids/README.md`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/convert_pmod_to_blood.py` & `pypet2bids-1.2.2/pypet2bids/convert_pmod_to_blood.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/dcm2niix4pet.py` & `pypet2bids-1.2.2/pypet2bids/dcm2niix4pet.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,33 +16,33 @@
 import os
 import textwrap
 from json_maj.main import JsonMAJ, load_json_or_dict
 from platform import system
 import subprocess
 import pandas as pd
 from os.path import join
-from os import listdir, walk, makedirs
+from os import listdir, walk
 from pathlib import Path
 import json
 import pydicom
 import re
 from tempfile import TemporaryDirectory
 import shutil
 from dateutil import parser
 from termcolor import colored
 import argparse
 import importlib
 import dotenv
-import logging
 
 try:
     import helper_functions
+    import is_pet
 except ModuleNotFoundError:
     import pypet2bids.helper_functions as helper_functions
-
+    import pypet2bids.is_pet as is_pet
 
 logger = helper_functions.logger
 
 # fields to check for
 module_folder = Path(__file__).parent.resolve()
 python_folder = module_folder.parent
 pet2bids_folder = python_folder.parent
@@ -225,15 +225,16 @@
         else:
             pass
 
     if missing_values.get('ScanStart', None):
         if missing_values.get('ScanStart')['key'] is False or missing_values.get('ScanStart')['value'] is False:
             json_updater.update({'ScanStart': 0})
     if missing_values.get('InjectionStart', None):
-        if missing_values.get('InjectionStart')['key'] is False or missing_values.get('InjectionStart')['value'] is False:
+        if missing_values.get('InjectionStart')['key'] is False \
+                or missing_values.get('InjectionStart')['value'] is False:
             json_updater.update({'InjectionStart': 0})
 
     # check to see if units are BQML
     json_updater = JsonMAJ(str(path_to_json), bids_null=True)
     if json_updater.get('Units') == 'BQML':
         json_updater.update({'Units': 'Bq/mL'})
 
@@ -249,15 +250,15 @@
     updated_values = json.load(open(path_to_json, 'r'))
     for key, value in paired_fields.items():
         try:
             json_field = updated_values.get(key)
             dicom_field = dicom_header.__getattr__(key)
             if json_field != dicom_field:
                 logger.info(f"WARNING!!!! JSON Field {key} with value {json_field} does not match dicom value "
-                              f"of {dicom_field}")
+                            f"of {dicom_field}")
         except AttributeError:
             pass
 
 
 def dicom_datetime_to_dcm2niix_time(dicom=None, date='', time=''):
     """
     Dcm2niix provides the option of outputing the scan data and time into the .nii and .json filename at the time of
@@ -343,15 +344,15 @@
         :param metadata_path: path to excel, csv, or text file with PET metadata (radioligand, blood, etc etc)
         :param metadata_translation_script: python file to extract and transform data contained in the metadata_path
         :param file_format: the file format that we want dcm2niix to use, by default %p_%i_%t_%s
         %p -> protocol
         %i -> ID of patient
         %t -> time
         %s -> series number
-        :param additional_arguments: user supplied key value pairs, E.g. TimeZero=12:12:12, InjectedRadioactivity=1
+        :param additional_arguments: user supplied key value pairs, E.g. TimeZero=\"12:12:12\", InjectedRadioactivity=1
         this key value pair will overwrite any fields in the dcm2niix produced nifti sidecar.json as it is assumed that
         the user knows more about converting their data than the heuristics within dcm2niix, this library, or even the
         dicom header
         :param silent: silence missing sidecar metadata messages, default is False and very verbose
         """
 
         # check to see if dcm2niix is installed
@@ -367,15 +368,15 @@
         version_string = subprocess.run([self.dcm2niix_path, '-v'], capture_output=True)
         version = re.search(r"v[0-9].[0-9].{8}[0-9]", str(version_string.stdout))
 
         if version:
             # compare with minimum version
             if version[0] < minimum_version:
                 logger.warning(f"Minimum version {minimum_version} of dcm2niix is recommended, found "
-                                f"installed version {version[0]} at {self.dcm2niix_path}.")
+                               f"installed version {version[0]} at {self.dcm2niix_path}.")
 
         self.image_folder = Path(image_folder)
         if destination_path:
             self.destination_path = Path(destination_path)
         else:
             self.destination_path = self.image_folder
 
@@ -414,19 +415,41 @@
             self.metadata_translation_script = Path(metadata_translation_script)
 
             if self.metadata_path.exists() and self.metadata_translation_script.exists():
                 # load the spreadsheet into a dataframe
                 self.extract_metadata()
                 # next we use the loaded python script to extract the information we need
                 self.load_spread_sheet_data()
-        elif metadata_path and not metadata_translation_script:
-            spread_sheet_values = \
-                helper_functions.single_spreadsheet_reader(metadata_path,
-                                                           dicom_metadata=self.dicom_headers[next(iter(self.dicom_headers))],
-                                                           **self.additional_arguments)
+        elif metadata_path and not metadata_translation_script or metadata_path == "":
+            spread_sheet_values = {}
+
+            if Path(metadata_path).is_file():
+                spread_sheet_values = helper_functions.single_spreadsheet_reader(
+                    metadata_path,
+                    dicom_metadata=self.dicom_headers[next(iter(self.dicom_headers))],
+                    **self.additional_arguments)
+
+            if Path(metadata_path).is_dir() or metadata_path == "":
+                # we accept folder input as well as no input, in the
+                # event of no input we search for spreadsheets in the
+                # image folder
+                if metadata_path == "":
+                    metadata_path = self.image_folder
+
+                spreadsheets = helper_functions.collect_spreadsheets(metadata_path)
+                pet_spreadsheets = [spreadsheet for spreadsheet in spreadsheets if is_pet.pet_file(spreadsheet)]
+                spread_sheet_values = {}
+
+                for pet_spreadsheet in pet_spreadsheets:
+                    spread_sheet_values.update(
+                        helper_functions.single_spreadsheet_reader(
+                            pet_spreadsheet,
+                            dicom_metadata=self.dicom_headers[next(iter(self.dicom_headers))],
+                            **self.additional_arguments))
+
             if not self.spreadsheet_metadata.get('nifti_json', None):
                 self.spreadsheet_metadata['nifti_json'] = {}
             self.spreadsheet_metadata['nifti_json'].update(spread_sheet_values)
 
         self.file_format = file_format
         # we may want to include additional information to the sidecar, tsv, or json files generated after conversion
         # this variable stores the mapping between output files and a single dicom header used to generate those files
@@ -474,15 +497,15 @@
                 if check.returncode == 0:
                     return dcm2niix_path
             else:
                 logger.error(f"Unable to locate dcm2niix executable at {dcm2niix_path.__str__()}")
                 dcm2niix_path = None
         else:
             logger.error(f"Config file not found at {pypet2bids_config}, .pet2bidsconfig file must exist and "
-                          f"have variable DCM2NIIX_PATH set to installed path of installed dcm2niix.")
+                         f"have variable DCM2NIIX_PATH set to installed path of installed dcm2niix.")
         return dcm2niix_path
 
     def check_for_dcm2niix(self):
         """
         Just checks for dcm2niix using the system shell, returns 0 if dcm2niix is present.
 
         :return: status code of the command dcm2niix -h
@@ -524,15 +547,14 @@
                         self.subject_id = dicom_header.PatientID
 
                     dicom_headers[dicom_path.name] = dicom_header
                     n += 1
 
                 except pydicom.errors.InvalidDicomError:
                     pass
-                
 
         return dicom_headers
 
     def run_dcm2niix(self):
         """
         This runs dcm2niix and uses the other methods within this class to supplement the sidecar json's produced as
         dcm2niix output.
@@ -723,15 +745,15 @@
                     else:
                         run = ''
 
                     if self.full_file_path_given:
                         new_path = self.destination_path.with_suffix(suffix)
                     else:
                         new_path = self.destination_path / Path(self.subject_id + session_id + task + trc + rec +
-                                                                     run + '_pet' + suffix)
+                                                                run + '_pet' + suffix)
 
                     try:
                         new_path.parent.mkdir(parents=True, exist_ok=True)
                     except FileExistsError:
                         pass
 
                 elif not self.subject_id:
@@ -951,15 +973,15 @@
         numeric_check = [helper_functions.is_numeric(str(SpecificRadioactivity)),
                          helper_functions.is_numeric(str(InjectedMass))]
         if False in numeric_check:
             data_out['InjectedRadioactivity'] = 'n/a'
             data_out['InjectedRadioactivityUnits'] = 'n/a'
         else:
             tmp = ((InjectedMass / (10 ** 6)) * SpecificRadioactivity) / (
-                        10 ** 6)  # ((ug / 10 ^ 6) / Bq / g)/10 ^ 6 = MBq
+                    10 ** 6)  # ((ug / 10 ^ 6) / Bq / g)/10 ^ 6 = MBq
             if InjectedRadioactivity:
                 if InjectedRadioactivity != tmp:
                     print(colored("WARNING inferred InjectedRadioactivity in MBq doesn't match SpecificRadioactivity "
                                   "and InjectedMass, could be a unit issue", "yellow"))
                 data_out['InjectedRadioactivity'] = InjectedRadioactivity
                 data_out['InjectedRadioactivityUnits'] = kwargs.get('InjectedRadioactivityUnits', 'n/a')
             else:
@@ -1062,15 +1084,15 @@
         check_code_value = ""
         check_code_meaning = ""
 
         if code_value in verified_nucleotides.keys():
             check_code_value = code_value
         else:
             logger.warning(f"Radionuclide Code {code_value} does not match any known codes in dcm2bids.json\n"
-                          f"will attempt to infer from code meaning {code_meaning}")
+                           f"will attempt to infer from code meaning {code_meaning}")
 
         if code_meaning in verified_nucleotides.values():
             radionuclide = re.sub(r'\^', "", code_meaning)
             check_code_meaning = code_meaning
         else:
             logger.warning(f"Radionuclide Meaning {code_meaning} not in known values in dcm2bids json")
             if code_value in verified_nucleotides.keys():
@@ -1107,28 +1129,28 @@
     :param -t, --translation-script-path: path to script used to extract information from metadata spreadsheet
     :param -d, --destination-path: path to place outputfiles post conversion from dicom to nifti + json
     :return: arguments collected from argument parser
     """
     parser = argparse.ArgumentParser(formatter_class=argparse.RawDescriptionHelpFormatter, epilog=epilog)
     parser.add_argument('folder', nargs='?', type=str,
                         help="Folder path containing imaging data")
-    parser.add_argument('--metadata-path', '-m', type=str, default=None,
+    parser.add_argument('--metadata-path', '-m', type=str, default=None, const='', nargs='?',
                         help="Path to metadata file for scan")
     parser.add_argument('--translation-script-path', '-t', default=None,
                         help="Path to a script written to extract and transform metadata from a spreadsheet to BIDS" +
                              " compliant text files (tsv and json)")
     parser.add_argument('--destination-path', '-d', type=str, default=None,
                         help="Destination path to send converted imaging and metadata files to. If subject id and "
                              "session id is included in the path files created by dcm2niix4pet will be named as such. "
                              "e.g. sub-NDAR123/ses-ABCD/pet will yield fields named sub-NDAR123_ses-ABCD_*. If " +
                              "omitted defaults to using the path supplied to folder path. If destination path " +
                              "doesn't exist an attempt to create it will be made.", required=False)
     parser.add_argument('--kwargs', '-k', nargs='*', action=helper_functions.ParseKwargs, default={},
                         help="Include additional values in the nifti sidecar json or override values extracted from "
-                             "the supplied nifti. e.g. including `--kwargs TimeZero='12:12:12'` would override the "
+                             "the supplied nifti. e.g. including `--kwargs TimeZero=\"12:12:12\"` would override the "
                              "calculated TimeZero. Any number of additional arguments can be supplied after --kwargs "
                              "e.g. `--kwargs BidsVariable1=1 BidsVariable2=2` etc etc."
                              "Note: the value portion of the argument (right side of the equal's sign) should always"
                              "be surrounded by double quotes BidsVarQuoted=\"[0, 1 , 3]\"")
     parser.add_argument('--silent', '-s', type=bool, default=False, help="Display missing metadata warnings and errors"
                                                                          "to stdout/stderr")
     parser.add_argument('--show-examples', '-E', '--HELP', '-H', help="Shows example usage of this cli.",
```

### Comparing `pypet2bids-1.1.2/pypet2bids/dicom_convert.py` & `pypet2bids-1.2.2/pypet2bids/dicom_convert.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/ecat.py` & `pypet2bids-1.2.2/pypet2bids/ecat.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/ecat2nii.py` & `pypet2bids-1.2.2/pypet2bids/ecat2nii.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/ecat_cli.py` & `pypet2bids-1.2.2/pypet2bids/ecat_cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,18 +75,20 @@
         Output header and subheader info as JSON to stdout, overrides all other options""")
     parser.add_argument("--nifti", "-n", metavar="file_name", help="Name of nifti output file", required=False,
                         default=None)
     parser.add_argument("--subheader", '-s', help="Display subheaders", action="store_true", default=False)
     parser.add_argument("--sidecar", action="store_true", help="Output a bids formatted sidecar for pairing with"
                                                                "a nifti.")
     parser.add_argument('--kwargs', '-k', nargs='*', action=helper_functions.ParseKwargs, default={},
-                        help="Include additional values int the nifti sidecar json or override values extracted from "
-                             "the supplied nifti. e.g. including `--kwargs TimeZero='12:12:12'` would override the "
+                        help="Include additional values in the nifti sidecar json or override values extracted from "
+                             "the supplied nifti. e.g. including `--kwargs TimeZero=\"12:12:12\"` would override the "
                              "calculated TimeZero. Any number of additional arguments can be supplied after --kwargs "
-                             "e.g. `--kwargs BidsVariable1=1 BidsVariable2=2` etc etc.")
+                             "e.g. `--kwargs BidsVariable1=1 BidsVariable2=2` etc etc."
+                             "Note: the value portion of the argument (right side of the equal's sign) should always"
+                             "be surrounded by double quotes BidsVarQuoted=\"[0, 1 , 3]\"")
     parser.add_argument('--scannerparams', nargs='*',
                         help="Loads saved scanner params from a configuration file following "
                              "--scanner-params/-s if this option is used without an argument "
                              "this cli will look for any scanner parameters file in the "
                              "directory with the name *parameters.txt from which this cli is "
                              "called.")
     parser.add_argument("--directory_table", '-t', help="Collect table/array of ECAT frame byte location map",
```

### Comparing `pypet2bids-1.1.2/pypet2bids/ecat_headers.json` & `pypet2bids-1.2.2/pypet2bids/ecat_headers.json`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/golden_ecat.py` & `pypet2bids-1.2.2/pypet2bids/golden_ecat.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/helper_functions.py` & `pypet2bids-1.2.2/pypet2bids/helper_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,23 @@
     elif len(simplified_series_object) == 1:
         simplified_series_object = simplified_series_object[0]
     else:
         raise f"Invalid Series: {series}"
     return simplified_series_object
 
 
+def collect_spreadsheets(folder_path: pathlib.Path):
+    spreadsheet_files = []
+    all_files = [folder_path / pathlib.Path(file) for file in os.listdir(folder_path) if os.path.isfile(os.path.join(folder_path, file))]
+    for file in all_files:
+        if file.suffix == '.xlsx' or file.suffix == '.csv' or file.suffix == '.xls' or file.suffix == '.tsv':
+            spreadsheet_files.append(file)
+    return spreadsheet_files
+
+
 def single_spreadsheet_reader(
         path_to_spreadsheet: Union[str, pathlib.Path],
         pet2bids_metadata_json: Union[str, pathlib.Path] = pet_metadata_json,
         dicom_metadata={},
         **kwargs) -> dict:
 
     metadata = {}
```

### Comparing `pypet2bids-1.1.2/pypet2bids/is_pet.py` & `pypet2bids-1.2.2/pypet2bids/is_pet.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/metadata/PET_Radionuclide.mkd` & `pypet2bids-1.2.2/pypet2bids/metadata/PET_Radionuclide.mkd`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/metadata/PET_metadata.json` & `pypet2bids-1.2.2/pypet2bids/metadata/PET_metadata.json`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/metadata/PET_reconstruction_methods.json` & `pypet2bids-1.2.2/pypet2bids/metadata/PET_reconstruction_methods.json`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/metadata/definitions.json` & `pypet2bids-1.2.2/pypet2bids/metadata/definitions.json`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/metadata/dicom2bids.json` & `pypet2bids-1.2.2/pypet2bids/metadata/dicom2bids.json`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/metadata_spreadsheet_example_reader.py` & `pypet2bids-1.2.2/pypet2bids/metadata_spreadsheet_example_reader.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/multiple_spreadsheets.py` & `pypet2bids-1.2.2/pypet2bids/multiple_spreadsheets.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/pyproject.toml` & `pypet2bids-1.2.2/pypet2bids/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypet2bids"
-version = "1.1.2"
+version = "1.2.2"
 description = "A python implementation of an ECAT to BIDS converter."
 authors = ["anthony galassi <28850131+bendhouseart@users.noreply.github.com>"]
 license = "MIT"
 include = [
     'pypet2bids/metadata/blood_metadata.json',
     'pypet2bids/metadata/definitions.json',
     'pypet2bids/metadata/dicom2bids.json',
```

### Comparing `pypet2bids-1.1.2/pypet2bids/read_ecat.py` & `pypet2bids-1.2.2/pypet2bids/read_ecat.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/sidecar.py` & `pypet2bids-1.2.2/pypet2bids/sidecar.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pypet2bids/single_spreadsheet.py` & `pypet2bids-1.2.2/pypet2bids/single_spreadsheet.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     import helper_functions
 except ModuleNotFoundError:
     import pypet2bids.helper_functions as helper_functions
 
 #from pypet2bids.helper_functions import single_spreadsheet_reader, \
 #    collect_bids_part, open_meta_data, load_pet_bids_requirements_json, ParseKwargs
 
-
 def read_single_subject_spreadsheets(
         general_metadata_spreadsheet: pathlib.Path,
         **kwargs) -> dict:
     """
     Reads in spreadsheet as formatted in PET2BIDS/spreadsheet_conversion/single_subject_sheet,
     extra arguments are supplied in key pair form via kwargs as is convention.
```

### Comparing `pypet2bids-1.1.2/pypet2bids/write_ecat.py` & `pypet2bids-1.2.2/pypet2bids/write_ecat.py`

 * *Files identical despite different names*

### Comparing `pypet2bids-1.1.2/pyproject.toml` & `pypet2bids-1.2.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypet2bids"
-version = "1.1.2"
+version = "1.2.2"
 description = "A python implementation of an ECAT to BIDS converter."
 authors = ["anthony galassi <28850131+bendhouseart@users.noreply.github.com>"]
 license = "MIT"
 include = [
     'pypet2bids/metadata/blood_metadata.json',
     'pypet2bids/metadata/definitions.json',
     'pypet2bids/metadata/dicom2bids.json',
```

### Comparing `pypet2bids-1.1.2/setup.py` & `pypet2bids-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
                      'ecatpet2bids = pypet2bids.ecat_cli:main',
                      'ispet = pypet2bids.is_pet:main',
                      'pet2bids-spreadsheet-template = '
                      'pypet2bids.helper_functions:write_out_module']}
 
 setup_kwargs = {
     'name': 'pypet2bids',
-    'version': '1.1.2',
+    'version': '1.2.2',
     'description': 'A python implementation of an ECAT to BIDS converter.',
     'long_description': 'None',
     'author': 'anthony galassi',
     'author_email': '28850131+bendhouseart@users.noreply.github.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `pypet2bids-1.1.2/PKG-INFO` & `pypet2bids-1.2.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypet2bids
-Version: 1.1.2
+Version: 1.2.2
 Summary: A python implementation of an ECAT to BIDS converter.
 License: MIT
 Author: anthony galassi
 Author-email: 28850131+bendhouseart@users.noreply.github.com
 Requires-Python: >=3.8,<=3.11.1
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

