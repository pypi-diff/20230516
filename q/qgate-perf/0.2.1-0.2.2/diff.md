# Comparing `tmp/qgate_perf-0.2.1-py3-none-any.whl.zip` & `tmp/qgate_perf-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 16379 bytes, number of entries: 16
+Zip file size: 16532 bytes, number of entries: 16
 -rw-rw-rw-  2.0 fat       40 b- defN 23-Apr-29 09:53 qgate_perf/__init__.py
 -rw-rw-rw-  2.0 fat      428 b- defN 23-May-06 06:01 qgate_perf/bundle_helper.py
 -rw-rw-rw-  2.0 fat     5714 b- defN 23-May-06 17:21 qgate_perf/executor_helper.py
 -rw-rw-rw-  2.0 fat     1053 b- defN 23-May-04 18:36 qgate_perf/file_format.py
--rw-rw-rw-  2.0 fat    11516 b- defN 23-May-06 12:24 qgate_perf/parallel_executor.py
+-rw-rw-rw-  2.0 fat    11741 b- defN 23-May-16 18:07 qgate_perf/parallel_executor.py
 -rw-rw-rw-  2.0 fat     5431 b- defN 23-May-06 11:59 qgate_perf/parallel_probe.py
 -rw-rw-rw-  2.0 fat      384 b- defN 23-May-06 12:01 qgate_perf/run_return.py
 -rw-rw-rw-  2.0 fat     1705 b- defN 23-May-06 07:10 qgate_perf/run_setup.py
--rw-rw-rw-  2.0 fat      215 b- defN 23-May-06 19:21 qgate_perf/version.py
+-rw-rw-rw-  2.0 fat      215 b- defN 23-May-15 18:16 qgate_perf/version.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-May-05 17:45 tests/__init__.py
--rw-rw-rw-  2.0 fat     3339 b- defN 23-May-06 11:56 tests/test_run.py
--rw-rw-rw-  2.0 fat    11558 b- defN 23-May-06 19:21 qgate_perf-0.2.1.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     6938 b- defN 23-May-06 19:21 qgate_perf-0.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-06 19:21 qgate_perf-0.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       17 b- defN 23-May-06 19:21 qgate_perf-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1286 b- defN 23-May-06 19:21 qgate_perf-0.2.1.dist-info/RECORD
-16 files, 49716 bytes uncompressed, 14265 bytes compressed:  71.3%
+-rw-rw-rw-  2.0 fat     4550 b- defN 23-May-16 18:10 tests/test_run.py
+-rw-rw-rw-  2.0 fat    11558 b- defN 23-May-16 18:11 qgate_perf-0.2.2.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     6964 b- defN 23-May-16 18:11 qgate_perf-0.2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-16 18:11 qgate_perf-0.2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       17 b- defN 23-May-16 18:11 qgate_perf-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1286 b- defN 23-May-16 18:11 qgate_perf-0.2.2.dist-info/RECORD
+16 files, 51178 bytes uncompressed, 14418 bytes compressed:  71.8%
```

## zipnote {}

```diff
@@ -27,23 +27,23 @@
 
 Filename: tests/__init__.py
 Comment: 
 
 Filename: tests/test_run.py
 Comment: 
 
-Filename: qgate_perf-0.2.1.dist-info/LICENSE
+Filename: qgate_perf-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: qgate_perf-0.2.1.dist-info/METADATA
+Filename: qgate_perf-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: qgate_perf-0.2.1.dist-info/WHEEL
+Filename: qgate_perf-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: qgate_perf-0.2.1.dist-info/top_level.txt
+Filename: qgate_perf-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: qgate_perf-0.2.1.dist-info/RECORD
+Filename: qgate_perf-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qgate_perf/parallel_executor.py

```diff
@@ -250,35 +250,39 @@
 
         except Exception as e:
             self._print(file, str(e) if e is not None else '!! Noname exception !!')
         finally:
             if file is not None:
                 file.close()
 
-    def one_shot(self):
-        """ Run test, only one shot (execution) of test function """
+    def one_run(self, parameters=None):
+        """ Run test, only one shot (execution, in new process) of test function """
 
         # setup minimalistic values
-        setup = RunSetup(duration_second=0, start_delay=0, parameters=None)
+        setup = RunSetup(duration_second=0, start_delay=0, parameters=parameters)
 
         # run
         self.run(processes=1,
                  threads=1,
                  run_setup=setup)
 
-    def test_call(self, run_setup: RunSetup=None):
-        """ Test call without parallel execution"""
+    def test_run(self, run_setup: RunSetup=None):
+        """ Test call in current process/thread (without ability to define parallel execution)."""
 
         # init
         key="test-no-parallel"
         dictionary={key: ""}
+        run_return = RunReturn(key, dictionary)
+
+        if not run_setup:
+            run_setup = RunSetup(duration_second=0, start_delay=0)
         run_setup.set_start_time()
 
         # test call
-        self._func(key, dictionary, run_setup)
+        self._func(run_return, run_setup)
 
         # show output
         ret=dictionary[key]
         if ret:
             print(ret.ToString())
 
     #TODO: create dir, if not exist
```

## qgate_perf/version.py

```diff
@@ -1,5 +1,5 @@
 # Store the version here so:
 # 1) we don't load dependencies by storing it in __init__.py
 # 2) we can import it in setup.py for the same reason
 # 3) we can import it into your module module
-__version__ = '0.2.1'
+__version__ = '0.2.2'
```

## tests/test_run.py

```diff
@@ -38,21 +38,52 @@
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def test_one_shot(self):
+    def test_one_run(self):
         generator = ParallelExecutor(prf_GIL_impact,
                                      label="GIL_impact",
                                      detail_output=True,
                                      output_file="../output/test_gil_impact_test.txt")
 
-        generator.one_shot()
+        generator.one_run()
+
+    def test_one_run_param(self):
+        generator = ParallelExecutor(prf_GIL_impact,
+                                     label="GIL_impact",
+                                     detail_output=True,
+                                     output_file="../output/test_gil_impact_test.txt")
+
+        setting={"aa":10,
+               "name": "Adam"}
+
+        generator.one_run(parameters=setting)
+
+    def test_testrun(self):
+        generator = ParallelExecutor(prf_GIL_impact,
+                                     label="GIL_impact",
+                                     detail_output=True,
+                                     output_file="../output/test_gil_impact_test.txt")
+
+        generator.test_run()
+
+    def test_testrun_setup(self):
+        generator = ParallelExecutor(prf_GIL_impact,
+                                     label="GIL_impact",
+                                     detail_output=True,
+                                     output_file="../output/test_gil_impact_test.txt")
+
+        setting = {"aa": 10,
+                   "name": "Adam"}
+
+        setup=RunSetup(duration_second=0, start_delay=0,parameters=setting)
+        generator.test_run(run_setup=setup)
 
     def test_run(self):
         generator = ParallelExecutor(prf_GIL_impact,
                                      label="GIL_impact",
                                      detail_output=True,
                                      output_file="../output/test_gil_impact_test.txt")
```

## Comparing `qgate_perf-0.2.1.dist-info/LICENSE` & `qgate_perf-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `qgate_perf-0.2.1.dist-info/METADATA` & `qgate_perf-0.2.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: qgate-perf
-Version: 0.2.1
+Version: 0.2.2
 Summary: Performance test generator, part of Quality Gate
 Home-page: https://github.com/george0st/qgate-perf/
 Download-URL: https://pypi.org/project/qgate_perf/
 Author: Jiri Steuer
 Author-email: steuer.jiri@gmail.com
 License: MIT
 Keywords: PerformanceTest,Performance,QualityGate
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy (<=1.24.3)
 
 [![PyPI version fury.io](https://badge.fury.io/py/qgate-perf.svg)](https://pypi.python.org/pypi/qgate-perf/)
 # QGate-Perf
 
-Performance test generator part of Quality Gate solution. Key benefits:
- - **easy performance testing*** your python code (key parts - init, start, stop, return)
+Performance test generator, part of Quality Gate solution. Key benefits:
+ - **easy performance testing** your python code (key parts - init, start, stop, return)
  - **measure only specific part** of your code 
- - scalability **without limits** (e.g. from 1 to 10k executor)
- - scalability **in level of processes and threads** (easy avoid of python GIL)
- - **sequences for execution and data bunlk**
+ - scalability **without limits** (e.g. from 1 to 1k executors)
+ - scalability **in level of processes and threads** (easy way, how to avoid GIL in python)
+ - **sequences for execution and data bulk**
  - relation to graph generator
 
 ## Usage
 
 ```lang-python
 from qgate_perf.parallel_executor import ParallelExecutor
 from qgate_perf.parallel_probe import ParallelProbe
@@ -59,17 +59,19 @@
 
 # Execution setting
 generator = ParallelExecutor(prf_GIL_impact,
                              label="GIL_impact",
                              detail_output=True,
                              output_file="prf_gil_impact_01.txt")
 
+setup=RunSetup(duration_second=20,start_delay=0)
+
 generator.run_bulk_executor(bulk_list=[[1, 1]],
                             executor_list=[[16, 1, '1x thread'], [8, 2, '2x threads'],[4, 4,'4x threads']],
-                            run_setup=RunSetup(duration_second=20,start_delay=0))
+                            run_setup=setup)
 ```
 
 ## Outputs in text file 
 ```
 ############### 2023-05-05 06:30:36.194849 ###############
 {"type": "headr", "label": "GIL_impact", "bulk": [1, 1], "available_cpu": 12, "now": "2023-05-05 06:30:36.194849"}
   {"type": "core", "plan_executors": 4, "plan_executors_detail": [4, 1], "real_executors": 4, "group": "1x thread", "total_calls": 7590439, "avrg_time": 1.4127372338382197e-06, "std_deviation": 3.699171006877347e-05, "total_call_per_sec": 2831382.8673804617, "endexec": "2023-05-05 06:30:44.544829"}
```

