# Comparing `tmp/ldimbenchmark-0.1.9.tar.gz` & `tmp/ldimbenchmark-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ldimbenchmark-0.1.9.tar", max compression
+gzip compressed data, was "ldimbenchmark-0.2.0.tar", max compression
```

## Comparing `ldimbenchmark-0.1.9.tar` & `ldimbenchmark-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,39 @@
--rw-r--r--   0        0        0     2184 2022-12-08 09:44:58.002439 ldimbenchmark-0.1.9/README.md
--rw-r--r--   0        0        0     2449 2022-12-07 17:55:45.382773 ldimbenchmark-0.1.9/ldimbenchmark/__init__.py
--rw-r--r--   0        0        0    17746 2022-12-08 20:04:16.994222 ldimbenchmark-0.1.9/ldimbenchmark/benchmark.py
--rw-r--r--   0        0        0     4687 2022-12-08 17:13:49.593178 ldimbenchmark-0.1.9/ldimbenchmark/benchmark_complexity.py
--rw-r--r--   0        0        0     5709 2022-12-08 23:04:46.102023 ldimbenchmark-0.1.9/ldimbenchmark/benchmark_evaluation.py
--rw-r--r--   0        0        0     4654 2022-12-09 10:26:29.264538 ldimbenchmark-0.1.9/ldimbenchmark/classes.py
--rw-r--r--   0        0        0      104 2022-12-07 12:43:26.938979 ldimbenchmark-0.1.9/ldimbenchmark/constants.py
--rw-r--r--   0        0        0      163 2022-12-08 10:05:07.374298 ldimbenchmark-0.1.9/ldimbenchmark/datasets/__init__.py
--rw-r--r--   0        0        0     5517 2022-12-08 14:45:21.102206 ldimbenchmark-0.1.9/ldimbenchmark/datasets/analysis.py
--rw-r--r--   0        0        0    11144 2022-12-08 15:08:17.197924 ldimbenchmark-0.1.9/ldimbenchmark/datasets/classes.py
--rw-r--r--   0        0        0     5420 2022-12-08 14:41:09.835054 ldimbenchmark-0.1.9/ldimbenchmark/datasets/derivation.py
--rw-r--r--   0        0        0     2028 2022-12-08 15:31:59.645549 ldimbenchmark-0.1.9/ldimbenchmark/datasets/library.py
--rw-r--r--   0        0        0     5773 2022-12-08 11:46:48.213455 ldimbenchmark-0.1.9/ldimbenchmark/datasets/loaders/load_battledim.py
--rw-r--r--   0        0        0      312 2022-12-08 10:40:30.033936 ldimbenchmark-0.1.9/ldimbenchmark/datasets/loaders/load_dataset_base.py
--rw-r--r--   0        0        0     9269 2022-12-08 14:33:34.460442 ldimbenchmark-0.1.9/ldimbenchmark/generator/__init__.py
--rw-r--r--   0        0        0    11471 2022-12-08 16:58:59.249498 ldimbenchmark-0.1.9/ldimbenchmark/generator/dataset_generator.py
--rw-r--r--   0        0        0     6332 2022-12-07 15:22:03.260874 ldimbenchmark-0.1.9/ldimbenchmark/generator/poulakis_network.py
--rw-r--r--   0        0        0      588 2022-12-08 14:32:20.044668 ldimbenchmark-0.1.9/ldimbenchmark/generator/test_poulakis_network.py
--rw-r--r--   0        0        0       44 2022-12-08 21:38:17.813674 ldimbenchmark-0.1.9/ldimbenchmark/methods/__init__.py
--rw-r--r--   0        0        0    12187 2022-12-06 15:23:38.164295 ldimbenchmark-0.1.9/ldimbenchmark/methods/lila.py
--rw-r--r--   0        0        0     6687 2022-12-08 22:56:03.765644 ldimbenchmark-0.1.9/ldimbenchmark/methods/mnf.py
--rw-r--r--   0        0        0      849 2022-12-09 10:31:00.054343 ldimbenchmark-0.1.9/ldimbenchmark/methods/null.py
--rw-r--r--   0        0        0      868 2022-12-09 10:31:42.506619 ldimbenchmark-0.1.9/pyproject.toml
--rw-r--r--   0        0        0     3204 1970-01-01 00:00:00.000000 ldimbenchmark-0.1.9/setup.py
--rw-r--r--   0        0        0     2955 1970-01-01 00:00:00.000000 ldimbenchmark-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0     3330 2023-05-16 20:22:12.027560 ldimbenchmark-0.2.0/README.md
+-rw-r--r--   0        0        0     2359 2023-05-16 20:24:38.143954 ldimbenchmark-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      158 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/__init__.py
+-rw-r--r--   0        0        0       60 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/__init__.py
+-rw-r--r--   0        0        0    40101 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/benchmark.py
+-rw-r--r--   0        0        0     6456 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/runners/BaseMethodRunner.py
+-rw-r--r--   0        0        0     8655 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/runners/DockerMethodRunner.py
+-rw-r--r--   0        0        0     3457 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/runners/FileMethodRunner.py
+-rw-r--r--   0        0        0     7812 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/runners/LocalMethodRunner.py
+-rw-r--r--   0        0        0      195 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark/runners/__init__.py
+-rw-r--r--   0        0        0     5117 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark_complexity.py
+-rw-r--r--   0        0        0     6578 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark_evaluation.py
+-rw-r--r--   0        0        0    10115 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/classes.py
+-rw-r--r--   0        0        0     3928 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/cli.py
+-rw-r--r--   0        0        0      176 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/constants.py
+-rw-r--r--   0        0        0      211 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/__init__.py
+-rw-r--r--   0        0        0    10884 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/analysis.py
+-rw-r--r--   0        0        0    17897 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/classes.py
+-rw-r--r--   0        0        0    11765 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/derivation.py
+-rw-r--r--   0        0        0     1285 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/derivation_show.py
+-rw-r--r--   0        0        0     2087 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/library.py
+-rw-r--r--   0        0        0        0 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/loaders/__init__.py
+-rw-r--r--   0        0        0     9939 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/loaders/load_battledim.py
+-rw-r--r--   0        0        0      880 2023-05-16 20:22:12.051561 ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/loaders/load_dataset_base.py
+-rw-r--r--   0        0        0     1288 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/evaluation_metrics/__init__.py
+-rw-r--r--   0        0        0     9680 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/generator/__init__.py
+-rw-r--r--   0        0        0    12993 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/generator/dataset_generator.py
+-rw-r--r--   0        0        0     6332 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/generator/poulakis_network.py
+-rw-r--r--   0        0        0      158 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/__init__.py
+-rw-r--r--   0        0        0    13338 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/dualmethod.py
+-rw-r--r--   0        0        0    18958 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/lila.py
+-rw-r--r--   0        0        0    10445 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/mnf.py
+-rw-r--r--   0        0        0     1171 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/null.py
+-rw-r--r--   0        0        0     2033 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/random.py
+-rw-r--r--   0        0        0        0 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/utils/__init__.py
+-rw-r--r--   0        0        0     5309 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/methods/utils/cusum.py
+-rw-r--r--   0        0        0     8229 2023-05-16 20:22:12.055561 ldimbenchmark-0.2.0/src/ldimbenchmark/utilities.py
+-rw-r--r--   0        0        0     4964 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.0/setup.py
+-rw-r--r--   0        0        0     4517 1970-01-01 00:00:00.000000 ldimbenchmark-0.2.0/PKG-INFO
```

### Comparing `ldimbenchmark-0.1.9/ldimbenchmark/benchmark_complexity.py` & `ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark_complexity.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,44 @@
+from concurrent.futures import ProcessPoolExecutor, ThreadPoolExecutor, as_completed
 import importlib
 import os
 import time
 from datetime import datetime
 from glob import glob
 import logging
+
+import enlighten
 from ldimbenchmark.constants import LDIM_BENCHMARK_CACHE_DIR
 from ldimbenchmark.datasets import Dataset
 from ldimbenchmark.generator import (
     generateDatasetsForTimespan,
     generateDatasetsForJunctions,
 )
 from ldimbenchmark.classes import LDIMMethodBase
 import numpy as np
 import pandas as pd
 import wntr
 import yaml
 import big_o
-from multiprocessing import Pool, cpu_count
-from tqdm import tqdm
 import matplotlib as mpl
+from typing import List
 
 
 def loadDataset_local(dataset_path):
-    dataset = Dataset(dataset_path).loadDataset().loadBenchmarkData()
+    dataset = Dataset(dataset_path).loadData().loadBenchmarkData()
     number = int(os.path.basename(os.path.normpath(dataset_path)).split("-")[-1])
     return (
         number,
         dataset.getTrainingBenchmarkData(),
         dataset.getEvaluationBenchmarkData(),
     )
 
 
 def run_benchmark_complexity(
-    methods: list[LDIMMethodBase],
+    methods: List[LDIMMethodBase],
     cache_dir=os.path.join(LDIM_BENCHMARK_CACHE_DIR, "datagen"),
     out_folder="out/complexity",
     style=None,
     additionalOutput=False,
 ):
     """
     Run the benchmark for the given methods and datasets.
@@ -45,64 +47,67 @@
 
     if not os.path.exists(out_folder):
         os.mkdir(out_folder)
     logging.info("Complexity Analysis:")
     logging.info(" > Generating Datasets")
     if style == "time":
         datasets_dir = os.path.join(cache_dir, "synthetic-days")
-        generateDatasetsForTimespan(1, 61, datasets_dir)
+        generateDatasetsForTimespan(1, 91, datasets_dir)
     if style == "junctions":
         datasets_dir = os.path.join(cache_dir, "synthetic-junctions")
         generateDatasetsForJunctions(4, 59, datasets_dir)
 
     dataset_dirs = glob(datasets_dir + "/*/")
 
+    manager = enlighten.get_manager()
+    bar_loading_data = manager.counter(
+        total=len(dataset_dirs), desc="Loading data", unit="datasets"
+    )
+    bar_loading_data.update(incr=0)
+
     logging.info(" > Loading Data")
     datasets = {}
-    with Pool(processes=cpu_count() - 1) as p:
-        max_ = len(dataset_dirs)
-        with tqdm(total=max_) as pbar:
-            for (datasetid, training, evaluation) in p.imap_unordered(
-                loadDataset_local, dataset_dirs
-            ):
-                datasets[datasetid] = {}
-                datasets[datasetid]["training"] = training
-                datasets[datasetid]["evaluation"] = evaluation
-                pbar.update()
-    # for dataset in dataset_dirs:
-    #     (datasetid, training, evaluation) = loadDataset_local(dataset)
-    #     datasets[datasetid] = {}
-    #     datasets[datasetid]["training"] = training
-    #     datasets[datasetid]["evaluation"] = evaluation
+    try:
+        with ThreadPoolExecutor(max_workers=os.cpu_count()) as executor:
+            # submit all tasks and get future objects
+            futures = [
+                executor.submit(loadDataset_local, dataset_dir)
+                for dataset_dir in dataset_dirs
+            ]
+            # process results from tasks in order of task completion
+            for future in as_completed(futures):
+                dataset_id, training, evaluation = future.result()
+                datasets[dataset_id] = {}
+                datasets[dataset_id]["training"] = training
+                datasets[dataset_id]["evaluation"] = evaluation
+                bar_loading_data.update()
+    except KeyboardInterrupt:
+        manager.stop()
+        executor._processes.clear()
+        os.kill(os.getpid(), 9)
+    bar_loading_data.close()
 
     results = {}
     result_measures = []
 
-    # self.experiments.append(
-    #                 LocalMethodRunner(
-    #                     method,
-    #                     dataset,
-    #                     self.hyperparameters,
-    #                     resultsFolder=self.runner_results_dir,
-    #                 )
-    #             )
-
-    logging.info(" > Starting Complexity analyis")
+    bar_running_analysis = manager.counter(
+        total=len(methods), desc="Running Analysis", unit="methods"
+    )
+    logging.info(" > Starting Complexity analysis")
     for method in methods:
-
         logging.info(f" - {method.name}")
 
         if additionalOutput:
             method.init_with_benchmark_params(
                 os.path.join(out_folder, "additional_output_path"), {}
             )
 
         def runAlgorithmWithNetwork(n):
-            method.train(datasets[n]["training"])
-            method.detect(datasets[n]["evaluation"])
+            method.prepare(datasets[n]["training"])
+            method.detect_offline(datasets[n]["evaluation"])
 
         # Run Big-O
         best, others = big_o.big_o(
             runAlgorithmWithNetwork,
             big_o.datagen.n_,
             min_n=4,
             max_n=len(dataset_dirs),
@@ -114,15 +119,22 @@
 
         measures = pd.DataFrame({"times": others["times"]}, index=others["measures"])
         result_measures.append(measures.rename(columns={"times": method.name}))
         measures.to_csv(os.path.join(out_folder, "measures_raw.csv"))
         pd.DataFrame(list(others.items())[1:8]).to_csv(
             os.path.join(out_folder, "big_o.csv"), header=False, index=False
         )
+        bar_running_analysis.update()
+        # Cooldown for 10 seconds
+        time.sleep(10)
+
+    bar_running_analysis.close()
+    manager.stop()
 
+    logging.info(f"Exporting results to {out_folder}")
     results = pd.DataFrame(
         {
             "Leakage Detection Method": results.keys(),
             "Time Complexity": results.values(),
         }
     )
     results.to_csv(os.path.join(out_folder, "results.csv"), index=False)
@@ -133,7 +145,8 @@
     result_measures = pd.concat(result_measures, axis=1)
     result_measures.to_csv(os.path.join(out_folder, "measures.csv"))
     mpl.rcParams.update(mpl.rcParamsDefault)
     plot = (result_measures / result_measures.max()).plot()
     plot.set_title(f"Complexity Analysis: {style}")
     fig = plot.get_figure()
     fig.savefig(os.path.join(out_folder, "measures.png"))
+    return results
```

### Comparing `ldimbenchmark-0.1.9/ldimbenchmark/benchmark_evaluation.py` & `ldimbenchmark-0.2.0/src/ldimbenchmark/benchmark_evaluation.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,18 +29,24 @@
     existing_leak_not_detected = 0
     time_to_detection = ""
     wrong_pipe_detected = 0
 
     # Make sure dates are the same
 
     expected_leaks = expected_leaks.astype(
-        {"leak_time_start": "datetime64[ns]", "leak_time_end": "datetime64[ns]"}
+        {
+            "leak_time_start": "datetime64[ns, UTC]",
+            "leak_time_end": "datetime64[ns, UTC]",
+        }
     )
     detected_leaks = detected_leaks.astype(
-        {"leak_time_start": "datetime64[ns]", "leak_time_end": "datetime64[ns]"}
+        {
+            "leak_time_start": "datetime64[ns, UTC]",
+            "leak_time_end": "datetime64[ns, UTC]",
+        }
     )
 
     # Match detected Leaks with existing Leaks
     expected_leaks_times = expected_leaks
     expected_leaks_times["type"] = "expected"
     detected_leaks_times = detected_leaks
     detected_leaks_times["type"] = "detected"
@@ -61,81 +67,103 @@
 
     matched_list = []
     # TODO: Make sure that the table index (int) is used and not the pipe_id
     for index, leak in list_of_all.iterrows():
         if list_of_all["used"][index] == 1:
             continue
         source_array_index = list_of_all["index"][index]
-        source_array_index = list_of_all["index"][index]
 
         if leak["type"] == "expected":
             # If the type is expected try to find the closest leak from the detected array
             timespan_to_other_leaks = dist_mat.iloc[:, source_array_index]
             # print(timespan_to_other_leaks)
             # If all detected leaks ar before the expected Leak there is None to match it to.
             if all(np.isnat(i.to_numpy()) for i in timespan_to_other_leaks):
-                matched_list.append((expected_leaks.loc[source_array_index], None))
+                matched_list.append(
+                    (expected_leaks.loc[source_array_index].to_dict(), None)
+                )
                 continue
 
             min_x = timespan_to_other_leaks.idxmin(skipna=True)
             ref = list_of_all[list_of_all["type"] == "detected"]
             ref = ref[ref["index"] == min_x]
             index_new = ref.index
 
-            if dist_mat.iloc[min_x, :].idxmin(skipna=True) == source_array_index:
+            if dist_mat.iloc[min_x, :].idxmin(skipna=True) == source_array_index and (
+                # Leak also has to be within the expected leak time
+                expected_leaks.loc[source_array_index].leak_time_end
+                >= detected_leaks.loc[min_x].leak_time_start
+            ):
                 # if (ref["used"].values[0] == 0):
                 list_of_all.loc[index_new, "used"] = 1
                 # list_of_all.iloc[index_new]["used"] = 1
                 matched_list.append(
-                    (expected_leaks.loc[source_array_index], detected_leaks.loc[min_x])
+                    (
+                        expected_leaks.loc[source_array_index].to_dict(),
+                        detected_leaks.loc[min_x].to_dict(),
+                    )
                 )
             else:
-                matched_list.append((expected_leaks.loc[source_array_index], None))
+                matched_list.append(
+                    (expected_leaks.loc[source_array_index].to_dict(), None)
+                )
             # print(ref)
         else:
-            matched_list.append((None, detected_leaks.loc[source_array_index]))
+            matched_list.append(
+                (None, detected_leaks.loc[source_array_index].to_dict())
+            )
 
         # print(list_of_all)
         # for detected_leak, expected_leak in matched_list:
         #     print(detected_leak.pipe_id,
         #           expected_leak.pipe_id if expected_leak != None else None)
 
         # matched_list.append((expected_leaks[expected_index], leak))
     # for detected_leak, expected_leak in matched_list:
     #     print(detected_leak.pipe_id if detected_leak != None else None,
     #           expected_leak.pipe_id if expected_leak != None else None)
 
     # print("###########")
     # for detected_leak, expected_leak in itertools.zip_longest(sorted_detected_leaks, sorted_expected_leaks):
 
+    time_to_detection = []
     for expected_leak, detected_leak in matched_list:
         if detected_leak is None:
             existing_leak_not_detected += 1
             continue
         if expected_leak is None:
             non_existing_leak_detected += 1
             continue
         # print(detected_leak.pipe_id, expected_leak.pipe_id)
         if (
-            detected_leak.leak_time_start >= expected_leak.leak_time_start
-            and detected_leak.leak_time_end <= expected_leak.leak_time_end
+            detected_leak["leak_time_start"] >= expected_leak["leak_time_start"]
+            and detected_leak["leak_time_end"] <= expected_leak["leak_time_end"]
         ):
             right_leak_detected += 1
             # Calculate TimeSpan Between Detections
-            time_to_detection = (
-                detected_leak.leak_time_start - expected_leak.leak_time_start
-            ).total_seconds()
-            if expected_leak.leak_pipe_id == detected_leak.leak_pipe_id:
+            time_to_detection.append(
+                (
+                    detected_leak["leak_time_start"] - expected_leak["leak_time_start"]
+                ).total_seconds()
+            )
+            if expected_leak["leak_pipe_id"] == detected_leak["leak_pipe_id"]:
                 pass
             else:
                 wrong_pipe_detected += 1
         else:
             existing_leak_not_detected += 1
-    return {
-        "true_positives": right_leak_detected,
-        "false_positives": non_existing_leak_detected,
-        "true_negatives": None,  # Not applicable, we dont have information about non-leaks
-        "false_negatives": existing_leak_not_detected,
-        "time_to_detection": time_to_detection,
-        "wrong_pipe": wrong_pipe_detected,
-        "score": 0,
-    }
+
+        # TODO Refactor and only give back the matched list
+        # TODO make another function which takes a list of evaluators and executes them to get an evaluation table
+    return (
+        {
+            "true_positives": right_leak_detected,
+            "false_positives": non_existing_leak_detected,
+            "true_negatives": None,  # Not applicable, we dont have information about non-leaks
+            "false_negatives": existing_leak_not_detected,
+            "time_to_detection": None
+            if len(time_to_detection) == 0
+            else np.sum(time_to_detection),
+            "wrong_pipe": wrong_pipe_detected,
+        },
+        matched_list,
+    )
```

### Comparing `ldimbenchmark-0.1.9/ldimbenchmark/datasets/library.py` & `ldimbenchmark-0.2.0/src/ldimbenchmark/datasets/library.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from enum import Enum
 import tempfile
+from typing import Union, List
 from ldimbenchmark.datasets.loaders.load_battledim import BattledimDatasetLoader
 
 import os
 from ldimbenchmark.datasets.classes import Dataset
 import numpy as np
-
+import logging
 import shutil
 
 
 class DATASETS(Enum):
     """
     Enum of available datasets
     """
@@ -22,16 +23,16 @@
     Library of datasets
     """
 
     def __init__(self, download_path: str):
         self.path = download_path
 
     def download(
-        self, dataset_name: str | list[str] | DATASETS | list[DATASETS], force=False
-    ) -> list[Dataset]:
+        self, dataset_name: Union[str, List[str], DATASETS, List[DATASETS]], force=False
+    ) -> List[Dataset]:
         """
         Downloads a dataset from the internet
 
         :param dataset_name: Name of the dataset to download
         :param force: Force download even if dataset is already downloaded
         """
         # TODO: Try to import download module for "dataset_name" and execute it.
@@ -41,20 +42,20 @@
             dataset_name = [DATASETS[dataset_name.upper()]]
         if isinstance(dataset_name, DATASETS):
             dataset_name = [dataset_name]
 
         datasets = []
 
         for dataset in dataset_name:
-            print("Downloading dataset: " + dataset.value)
+            logging.info("Loading dataset: " + dataset.value)
             tempdir = tempfile.TemporaryDirectory()
             tempdir_path = tempdir.name
             dataset_download_path = os.path.join(self.path, dataset.value)
             if os.path.exists(dataset_download_path) and not force:
-                print("Dataset already downloaded")
+                logging.info("Dataset already downloaded")
                 datasets.append(Dataset(dataset_download_path))
                 continue
             shutil.rmtree(dataset_download_path, ignore_errors=True)
             if dataset == DATASETS.BATTLEDIM:
                 BattledimDatasetLoader.download_dataset(tempdir_path)
                 BattledimDatasetLoader.prepare_dataset(
                     tempdir_path, dataset_download_path
```

### Comparing `ldimbenchmark-0.1.9/ldimbenchmark/generator/__init__.py` & `ldimbenchmark-0.2.0/src/ldimbenchmark/generator/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,21 @@
+from concurrent.futures import ProcessPoolExecutor, as_completed
 from ldimbenchmark.constants import LDIM_BENCHMARK_CACHE_DIR
 from ldimbenchmark.generator.dataset_generator import (
     DatasetGenerator,
-    DatasetGeneratorConfig,
 )
 from ldimbenchmark.generator.poulakis_network import generatePoulakisNetwork
 import wntr
 import matplotlib.pyplot as plt
 import os
 import yaml
-from math import sqrt
-from multiprocessing import Pool, cpu_count
-from tqdm import tqdm
 import numpy as np
-import math
-from datetime import datetime
-from itertools import repeat
+
 
 import logging
-from argparse import ArgumentParser
-from functools import partial
 
 
 # TODO: Move to main __init__.py
 # parser = ArgumentParser()
 # parser.add_argument(
 #     "-o",
 #     "--outputFolder",
@@ -111,15 +104,15 @@
 #     fig.savefig(f"out/network_poulakis-{size}.png")
 
 
 def generateDatasetForJunctionNumber(
     junctions: int, out_dir: str = LDIM_BENCHMARK_CACHE_DIR
 ):
     if os.path.exists(out_dir):
-        # print(f"Skipping {junctions} as it already exists")
+        logging.info(f"Skipping {out_dir} as it already exists")
         return
     os.makedirs(out_dir, exist_ok=True)
 
     wn = generatePoulakisNetwork(network_size=0, max_junctions=junctions)
 
     fig, ax = plt.subplots(1, 1, figsize=(12, 10))
     ax = wntr.graphics.plot_network(
@@ -160,15 +153,15 @@
     generator = DatasetGenerator(wn, config)
     generator.generate()
     generator.write_generated_data(out_dir, f"synthetic-j-{junctions}")
 
 
 def generateDatasetForTimeSpanDays(days: int, out_dir: str):
     if os.path.exists(out_dir):
-        # print(f"Skipping {out_dir} as it already exists")
+        logging.info(f"Skipping {out_dir} as it already exists")
         return
     os.makedirs(out_dir, exist_ok=True)
     wn = generatePoulakisNetwork()
 
     startDate = np.datetime64("2022-01-01 00:00")
     endDate = startDate + np.timedelta64(days, "D")
     yaml_example = """
@@ -226,40 +219,52 @@
             junctions,
             [
                 os.path.join(out_dir, f"synthetic-j-{junction}")
                 for junction in junctions
             ],
         )
 
-        with Pool(processes=cpu_count() - 1) as p:
-            jobs = [
-                p.apply_async(func=generateDatasetForJunctionNumber, args=arguments)
-                for arguments in arguments_list
-            ]
-            for job in tqdm(jobs):
-                job.get()  # wait for job to complete
+        try:
+            with ProcessPoolExecutor(max_workers=os.cpu_count()) as executor:
+                # submit all tasks and get future objects
+                futures = [
+                    executor.submit(generateDatasetForJunctionNumber, junction, num)
+                    for junction, num in arguments_list
+                ]
+                # process results from tasks in order of task completion
+                for future in as_completed(futures):
+                    future.result()
+        except KeyboardInterrupt:
+            executor._processes.clear()
+            os.kill(os.getpid(), 9)
 
 
 def generateDatasetsForTimespan(
     days_low: int, days_high: int, out_dir: str = LDIM_BENCHMARK_CACHE_DIR
 ):
     parallel = True
     if parallel == True:
         days = range(days_low, days_high)
         arguments_list = zip(
             days, [os.path.join(out_dir, f"synthetic-days-{day}") for day in days]
         )
 
-        with Pool(processes=cpu_count() - 1) as p:
-            jobs = [
-                p.apply_async(func=generateDatasetForTimeSpanDays, args=arguments)
-                for arguments in arguments_list
-            ]
-            for job in tqdm(jobs):
-                job.get()  # wait for job to complete
+        try:
+            with ProcessPoolExecutor(max_workers=os.cpu_count()) as executor:
+                # submit all tasks and get future objects
+                futures = [
+                    executor.submit(generateDatasetForTimeSpanDays, day, num)
+                    for day, num in arguments_list
+                ]
+                # process results from tasks in order of task completion
+                for future in as_completed(futures):
+                    future.result()
+        except KeyboardInterrupt:
+            executor._processes.clear()
+            os.kill(os.getpid(), 9)
 
 
 # if args.variations == "junctions":
 #     generateDatasetsForJunctions(4, 59)
 
 # for pipes in range(3, 57):
 #     wn = generatePoulakisNetwork(8, max_pipes=pipes)
```

### Comparing `ldimbenchmark-0.1.9/ldimbenchmark/generator/dataset_generator.py` & `ldimbenchmark-0.2.0/src/ldimbenchmark/generator/dataset_generator.py`

 * *Files 13% similar despite different names*

```diff
@@ -192,22 +192,27 @@
         return self.time_stamps, self.results, self.leak_dataframe, wn_with_leaks
 
     def write_generated_data(self, results_folder, model_name="synthetic_dataset"):
         if self.results == None:
             print("Run the 'dataset_generator()' Function before. No results to write.")
             return
 
-        # TODO: Use Dataset.exportTo() function
         # Create CSV files
         decimal_size = 4
 
         training_evaluation_split = (
             self.simulation_start_time
             + (self.leakages[0].startTime - self.simulation_start_time) / 2
         )
+        # TODO: Fix start and end times to be exclusive, should be (instead of same day for training and evaluation)
+        #     start: 2019-01-01 00:00
+        #     end: 2019-12-31 23:55
+        #   training:
+        #     start: 2018-01-01 00:00
+        #     end: 2019-12-31 23:55
         dataset_info = f"""
         name: {model_name}
         inp_file: model.inp
         dataset:
           training:
             start: '{str(self.simulation_start_time)}'
             end: '{str(training_evaluation_split)}'
@@ -240,54 +245,80 @@
         )
 
         # Create xlsx file with Measurements
         total_pressures = pd.DataFrame(index=self.time_stamps)
         total_demands = pd.DataFrame(index=self.time_stamps)
         total_flows = pd.DataFrame(index=self.time_stamps)
         total_levels = pd.DataFrame(index=self.time_stamps)
+
+        for folders in ["pressures", "demands", "flows", "levels"]:
+            os.makedirs(os.path.join(results_folder, folders), exist_ok=True)
+
         for node_id, values in self.results.node["demand"].items():
             if (
                 node_id in self.pressure_sensors
                 and self.wn.get_node(node_id).node_type == "Junction"
             ):
                 pres = self.results.node["pressure"][node_id].values[
                     : len(self.time_stamps)
                 ]
+                pd.DataFrame(pres, index=self.time_stamps).round(decimal_size).to_csv(
+                    os.path.join(results_folder, "pressures", f"{node_id}.csv"),
+                    index_label="Timestamp",
+                    header=[node_id],
+                )
                 # pres = pres[:len(self.time_stamp)]
                 total_pressures[node_id] = pres
 
             if node_id in self.amrs:
                 dem = self.results.node["demand"][node_id].values[
                     : len(self.time_stamps)
                 ]
+                pd.DataFrame(dem, index=self.time_stamps).round(decimal_size).to_csv(
+                    os.path.join(results_folder, "demands", f"{node_id}.csv"),
+                    index_label="Timestamp",
+                    header=[node_id],
+                )
                 # dem = dem[:len(self.time_stamp)]
                 # dem = [elem * 3600 * 1000 for elem in dem] #CMH / L/s
                 total_demands[node_id] = dem
 
             if node_id in self.level_sensors:
                 level_pres = self.results.node["pressure"][node_id].values[
                     : len(self.time_stamps)
                 ]
+                pd.DataFrame(level_pres, index=self.time_stamps).round(
+                    decimal_size
+                ).to_csv(
+                    os.path.join(results_folder, "levels", f"{node_id}.csv"),
+                    index_label="Timestamp",
+                    header=[node_id],
+                )
                 # level_pres = level_pres[:len(self.time_stamp)]
                 # level_pres = [round(elem, decimal_size) for elem in level_pres]
                 total_levels[node_id] = level_pres
 
         for link_id, values in self.results.link["flowrate"].items():
             if link_id in self.flow_sensors:
                 flows = self.results.link["flowrate"][link_id].values[
                     : len(self.time_stamps)
                 ]
+                pd.DataFrame(flows, index=self.time_stamps).round(decimal_size).to_csv(
+                    os.path.join(results_folder, "flows", f"{link_id}.csv"),
+                    index_label="Timestamp",
+                    header=[link_id],
+                )
                 total_flows[link_id] = flows
 
         # Pressures (m), Demands (m^3/s), Flows (m^3/s), Levels (m)
-        total_pressures.round(decimal_size).to_csv(
-            os.path.join(results_folder, "pressures.csv"), index_label="Timestamp"
-        )
-        total_demands.round(decimal_size).to_csv(
-            os.path.join(results_folder, "demands.csv"), index_label="Timestamp"
-        )
-        total_flows.round(decimal_size).to_csv(
-            os.path.join(results_folder, "flows.csv"), index_label="Timestamp"
-        )
-        total_levels.round(decimal_size).to_csv(
-            os.path.join(results_folder, "levels.csv"), index_label="Timestamp"
-        )
+        # total_pressures.round(decimal_size).to_csv(
+        #     os.path.join(results_folder, "pressures.csv"), index_label="Timestamp"
+        # )
+        # total_demands.round(decimal_size).to_csv(
+        #     os.path.join(results_folder, "demands.csv"), index_label="Timestamp"
+        # )
+        # total_flows.round(decimal_size).to_csv(
+        #     os.path.join(results_folder, "flows.csv"), index_label="Timestamp"
+        # )
+        # total_levels.round(decimal_size).to_csv(
+        #     os.path.join(results_folder, "levels.csv"), index_label="Timestamp"
+        # )
```

### Comparing `ldimbenchmark-0.1.9/ldimbenchmark/generator/poulakis_network.py` & `ldimbenchmark-0.2.0/src/ldimbenchmark/generator/poulakis_network.py`

 * *Files identical despite different names*

### Comparing `ldimbenchmark-0.1.9/ldimbenchmark/methods/null.py` & `ldimbenchmark-0.2.0/src/ldimbenchmark/methods/null.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 from ldimbenchmark import LDIMMethodBase, BenchmarkData, BenchmarkLeakageResult
-from ldimbenchmark.classes import MethodMetadata
+from ldimbenchmark.classes import MethodMetadata, MethodMetadataDataNeeded
+from typing import List, Union
 
 
 class NullLeakagedDetectionMethod(LDIMMethodBase):
     """
     Null Algorithm
     """
 
     def __init__(self):
         super().__init__(
             name="Null",
             version="1.0",
             metadata=MethodMetadata(
-                data_needed=["pressures", "demands", "flows", "levels"],
+                data_needed=MethodMetadataDataNeeded(
+                    pressures="ignored",
+                    flows="ignored",
+                    levels="ignored",
+                    model="ignored",
+                    demands="ignored",
+                    structure="ignored",
+                ),
                 hyperparameters=[],
             )
             # hyperparameters={"est_length": "3 days", "C_threshold": 3, "delta": 4},
         )
 
     def train(self, train_data: BenchmarkData) -> None:
         return
 
-    def detect(self, evaluation_data: BenchmarkData) -> list[BenchmarkLeakageResult]:
+    def detect_offline(
+        self, evaluation_data: BenchmarkData
+    ) -> List[BenchmarkLeakageResult]:
         return []
 
-    def detect_datapoint(self, evaluation_data) -> BenchmarkLeakageResult:
+    def detect_online(self, evaluation_data) -> Union[BenchmarkLeakageResult, None]:
         return None
```

### Comparing `ldimbenchmark-0.1.9/setup.py` & `ldimbenchmark-0.2.0/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,140 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+[![ldimbenchmark version](https://badgen.net/pypi/v/ldimbenchmark/)](https://pypi.org/project/ldimbenchmark)
+[![Documentation badge](https://img.shields.io/badge/Documentation-here!-GREEN.svg)](https://tumt2022.github.io/LDIMBench/)
 
-packages = \
-['ldimbenchmark',
- 'ldimbenchmark.datasets',
- 'ldimbenchmark.datasets.loaders',
- 'ldimbenchmark.generator',
- 'ldimbenchmark.methods']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['big-o>=0.10.2,<0.11.0',
- 'docker>=6.0.1,<7.0.0',
- 'pydantic>=1.10.2,<2.0.0',
- 'pyyaml>=6.0,<7.0',
- 'scikit-learn>=1.1.3,<2.0.0',
- 'tabulate>=0.9.0,<0.10.0',
- 'tqdm>=4.64.1,<5.0.0',
- 'wntr>=0.5.0,<0.6.0']
-
-setup_kwargs = {
-    'name': 'ldimbenchmark',
-    'version': '0.1.9',
-    'description': '',
-    'long_description': '# LDIMBenchmark\n\nLeakage Detection and Isolation Methods Benchmark\n\n## Usage\n\n### Installation\n\n```bash\npip install ldimbenchmark\n```\n\n### Python\n\n```python\nfrom ldimbenchmark.datasets import DatasetLibrary, DATASETS\nfrom ldimbenchmark import (\n    LDIMBenchmark,\n    BenchmarkData,\n    BenchmarkLeakageResult,\n)\nfrom ldimbenchmark.classes import LDIMMethodBase\n\n\nclass YourCustomLDIMMethod(LDIMMethodBase):\n    def __init__(self):\n        super().__init__(\n            name="YourCustomLDIMMethod",\n            version="0.1.0"\n        )\n\n    def train(self, data: BenchmarkData):\n        pass\n\n    def detect(self, data: BenchmarkData) -> list[BenchmarkLeakageResult]:\n        return [\n            {\n                "leak_start": "2020-01-01",\n                "leak_end": "2020-01-02",\n                "leak_area": 0.2,\n                "pipe_id": "test",\n            }\n        ]\n\n    def detect_datapoint(self, evaluation_data) -> BenchmarkLeakageResult:\n        return {}\n\n\ndatasets = DatasetLibrary("datasets").download(DATASETS.BATTLEDIM)\n\nlocal_methods = [YourCustomLDIMMethod()]\n\nhyperparameters = {}\n\nbenchmark = LDIMBenchmark(\n    hyperparameters, datasets, results_dir="./benchmark-results"\n)\nbenchmark.add_local_methods(local_methods)\n\nbenchmark.run_benchmark()\n\nbenchmark.evaluate()\n```\n\n### CLI\n\n```bash\n# TODO (not yet working)\nldimbenchmark --help\n```\n\n## Roadmap\n\n- v1: Just Leakage Detection\n- v2: Provides Benchmark of Isolation Methods\n\nhttps://mathspp.com/blog/how-to-create-a-python-package-in-2022\n\n## Development\n\nhttps://python-poetry.org/docs/basic-usage/\n\n```bash\n# Use Environment\npoetry config virtualenvs.in-project true\npoetry shell\npoetry install --without ci # --with ci\n\n\n# Test\npoetry build\ncp -r dist tests/dist\ncd tests\ndocker build . -t testmethod\npytest -s -o log_cli=true\n\n# Test-Publish\npoetry config repositories.testpypi https://test.pypi.org/legacy/\npoetry config http-basic.testpypi __token__ pypi-your-api-token-here\npoetry build\npoetry publish -r testpypi\n\n# Real Publish\npoetry config pypi-token.pypi pypi-your-token-here\n```\n\n### Documentation\n\nhttps://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/\n\n```\nmkdocs serve\n```\n',
-    'author': 'DanielHabenicht',
-    'author_email': 'daniel-habenicht@outlook.de',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<4.0',
-}
+# LDIMBenchmark
 
+Leakage Detection and Isolation Methods Benchmark
 
-setup(**setup_kwargs)
+> Instead of collecting all the different dataset to benchmark different methods on. We wanted to create a Benchmarking Tool which makes it easy to reproduce the results of the different methods locally on your own dataset.
+
+It provides a close to real-world conditions environment and forces researchers to provide a reproducible method implementation, which is supposed to run automated on any input dataset, thus hindering custom solutions which work well in one specific case.
+
+## Usage
+
+### Installation
+
+```bash
+pip install ldimbenchmark
+```
+
+### Python
+
+```python
+from ldimbenchmark.datasets import DatasetLibrary, DATASETS
+from ldimbenchmark import (
+    LDIMBenchmark,
+    BenchmarkData,
+    BenchmarkLeakageResult,
+)
+from ldimbenchmark.classes import LDIMMethodBase
+from typing import List
+
+class YourCustomLDIMMethod(LDIMMethodBase):
+    def __init__(self):
+        super().__init__(
+            name="YourCustomLDIMMethod",
+            version="0.1.0"
+        )
+
+    def train(self, data: BenchmarkData):
+        pass
+
+    def detect(self, data: BenchmarkData) -> List[BenchmarkLeakageResult]:
+        return [
+            {
+                "leak_start": "2020-01-01",
+                "leak_end": "2020-01-02",
+                "leak_area": 0.2,
+                "pipe_id": "test",
+            }
+        ]
+
+    def detect_datapoint(self, evaluation_data) -> BenchmarkLeakageResult:
+        return {}
+
+
+datasets = DatasetLibrary("datasets").download(DATASETS.BATTLEDIM)
+
+local_methods = [YourCustomLDIMMethod()]
+
+hyperparameters = {}
+
+benchmark = LDIMBenchmark(
+    hyperparameters, datasets, results_dir="./benchmark-results"
+)
+benchmark.add_local_methods(local_methods)
+
+benchmark.run_benchmark()
+
+benchmark.evaluate()
+```
+
+### CLI
+
+```bash
+ldimbenchmark --help
+```
+
+## Roadmap
+
+- v1: Just Leakage Detection
+- v2: Provides Benchmark of Isolation Methods
+
+https://mathspp.com/blog/how-to-create-a-python-package-in-2022
+
+## Development
+
+https://python-poetry.org/docs/basic-usage/
+
+```bash
+# python 3.10
+# Use Environment
+poetry config virtualenvs.in-project true
+poetry shell
+poetry install --without ci # --with ci
+
+
+# Test
+poetry build
+cp -r dist tests/dist
+cd tests
+docker build . -t testmethod
+pytest -s -o log_cli=true
+pytest tests/test_derivation.py -k 'test_mything'
+pytest --testmon
+pytest --snapshot-update
+
+# Pytest watch
+ptw
+ptw -- --testmon
+
+# Watch a file during development
+npm install -g nodemon
+nodemon -L experiments/auto_hyperparameter.py
+
+# Test-Publish
+poetry config repositories.testpypi https://test.pypi.org/legacy/
+poetry config http-basic.testpypi __token__ pypi-your-api-token-here
+poetry build
+poetry publish -r testpypi
+
+# Real Publish
+poetry config pypi-token.pypi pypi-your-token-here
+```
+
+### Documentation
+
+https://squidfunk.github.io/mkdocs-material/
+https://click.palletsprojects.com/en/8.1.x/
+
+```
+mkdocs serve
+```
+
+# TODO
+
+LDIMBenchmark:
+Data Cleansing before working with them
+
+- per sensor type, e.g. waterflow (cut of at 0)
+- removing datapoints which are clearly a malfunction
```

