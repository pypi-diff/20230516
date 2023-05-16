# Comparing `tmp/cirqqrack-0.5.1.tar.gz` & `tmp/cirqqrack-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirqqrack-0.5.1.tar", last modified: Fri Jan 27 20:17:51 2023, max compression
+gzip compressed data, was "cirqqrack-0.6.0.tar", last modified: Tue May 16 15:15:54 2023, max compression
```

## Comparing `cirqqrack-0.5.1.tar` & `cirqqrack-0.6.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-01-27 20:17:51.712945 cirqqrack-0.5.1/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2022-05-18 13:39:24.000000 cirqqrack-0.5.1/LICENSE
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1619 2023-01-27 20:17:51.711945 cirqqrack-0.5.1/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      637 2022-05-18 13:39:24.000000 cirqqrack-0.5.1/README.md
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-01-27 20:17:51.711945 cirqqrack-0.5.1/cirqqrack.egg-info/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1619 2023-01-27 20:17:51.000000 cirqqrack-0.5.1/cirqqrack.egg-info/PKG-INFO
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      232 2023-01-27 20:17:51.000000 cirqqrack-0.5.1/cirqqrack.egg-info/SOURCES.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-01-27 20:17:51.000000 cirqqrack-0.5.1/cirqqrack.egg-info/dependency_links.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       15 2023-01-27 20:17:51.000000 cirqqrack-0.5.1/cirqqrack.egg-info/requires.txt
--rw-rw-r--   0 iamu      (1000) iamu      (1000)        6 2023-01-27 20:17:51.000000 cirqqrack-0.5.1/cirqqrack.egg-info/top_level.txt
-drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-01-27 20:17:51.711945 cirqqrack-0.5.1/qrack/
--rw-rw-r--   0 iamu      (1000) iamu      (1000)      549 2022-05-18 13:39:24.000000 cirqqrack-0.5.1/qrack/__init__.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)    15336 2023-01-27 19:28:41.000000 cirqqrack-0.5.1/qrack/qasm_simulator.py
--rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-01-27 20:17:51.712945 cirqqrack-0.5.1/setup.cfg
--rw-rw-r--   0 iamu      (1000) iamu      (1000)     1517 2023-01-27 19:49:46.000000 cirqqrack-0.5.1/setup.py
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-16 15:15:53.998763 cirqqrack-0.6.0/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    11357 2022-05-18 13:39:24.000000 cirqqrack-0.6.0/LICENSE
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1619 2023-05-16 15:15:53.998763 cirqqrack-0.6.0/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      637 2022-05-18 13:39:24.000000 cirqqrack-0.6.0/README.md
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-16 15:15:53.998763 cirqqrack-0.6.0/cirqqrack.egg-info/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1619 2023-05-16 15:15:53.000000 cirqqrack-0.6.0/cirqqrack.egg-info/PKG-INFO
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      232 2023-05-16 15:15:53.000000 cirqqrack-0.6.0/cirqqrack.egg-info/SOURCES.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        1 2023-05-16 15:15:53.000000 cirqqrack-0.6.0/cirqqrack.egg-info/dependency_links.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       15 2023-05-16 15:15:53.000000 cirqqrack-0.6.0/cirqqrack.egg-info/requires.txt
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)        6 2023-05-16 15:15:53.000000 cirqqrack-0.6.0/cirqqrack.egg-info/top_level.txt
+drwxrwxr-x   0 iamu      (1000) iamu      (1000)        0 2023-05-16 15:15:53.998763 cirqqrack-0.6.0/qrack/
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)      549 2022-05-18 13:39:24.000000 cirqqrack-0.6.0/qrack/__init__.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)    16446 2023-05-16 15:11:23.000000 cirqqrack-0.6.0/qrack/qasm_simulator.py
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)       38 2023-05-16 15:15:53.998763 cirqqrack-0.6.0/setup.cfg
+-rw-rw-r--   0 iamu      (1000) iamu      (1000)     1517 2023-05-16 13:27:57.000000 cirqqrack-0.6.0/setup.py
```

### Comparing `cirqqrack-0.5.1/LICENSE` & `cirqqrack-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cirqqrack-0.5.1/PKG-INFO` & `cirqqrack-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirqqrack
-Version: 0.5.1
+Version: 0.6.0
 Summary: Cirq Qrack Plugin - Qrack High-Performance GPU simulation for Cirq
 Home-page: https://github.com/vm6502q/cirq-qrack
 Author: Daniel Strano
 Author-email: stranoj@gmail.com
 License: Apache 2.0
 Keywords: cirq qrack simulator quantum addon backend
 Classifier: Environment :: Console
```

### Comparing `cirqqrack-0.5.1/README.md` & `cirqqrack-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `cirqqrack-0.5.1/cirqqrack.egg-info/PKG-INFO` & `cirqqrack-0.6.0/cirqqrack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cirqqrack
-Version: 0.5.1
+Version: 0.6.0
 Summary: Cirq Qrack Plugin - Qrack High-Performance GPU simulation for Cirq
 Home-page: https://github.com/vm6502q/cirq-qrack
 Author: Daniel Strano
 Author-email: stranoj@gmail.com
 License: Apache 2.0
 Keywords: cirq qrack simulator quantum addon backend
 Classifier: Environment :: Console
```

### Comparing `cirqqrack-0.5.1/qrack/__init__.py` & `cirqqrack-0.6.0/qrack/__init__.py`

 * *Files identical despite different names*

### Comparing `cirqqrack-0.5.1/qrack/qasm_simulator.py` & `cirqqrack-0.6.0/qrack/qasm_simulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 
 # pylint: disable=invalid-name
 
 
 import numpy as np
 import scipy as sp
 import collections
-from typing import Dict
+from typing import (
+    Dict,
+    Iterator
+)
 from pyqrack import QrackSimulator, Pauli
 
 import cirq
 from cirq import circuits, ops, protocols, study
 from cirq.sim import SimulatesSamples
 from cirq.sim.simulator import check_all_resolved, split_into_matching_protocol_then_general
 
@@ -100,14 +103,48 @@
         self._configuration = configuration or self.DEFAULT_CONFIGURATION
         self._number_of_qubits = None
         self._memory = collections.defaultdict(list)
         self._results = {}
         self._shots = {}
         self._local_random = np.random.RandomState()
 
+    def run_sweep_iter(
+        self, program: 'cirq.AbstractCircuit', params: 'cirq.Sweepable', repetitions: int = 1
+    ) -> Iterator['cirq.Result']:
+        """Runs the supplied Circuit, mimicking quantum hardware.
+
+        In contrast to run, this allows for sweeping over different parameter
+        values.
+
+        Args:
+            program: The circuit to simulate.
+            params: Parameters to run with the program.
+            repetitions: The number of repetitions to simulate.
+
+        Returns:
+            Result list for this run; one for each possible parameter
+            resolver.
+
+        Raises:
+            ValueError: If the circuit has no measurements.
+        """
+        if not program.has_measurements():
+            raise ValueError("Circuit has no measurements to sample.")
+
+        for param_resolver in study.to_resolvers(params):
+            records = {}
+            if repetitions == 0:
+                for _, op, _ in program.findall_operations_with_gate_type(ops.MeasurementGate):
+                    records[protocols.measurement_key_name(op)] = np.empty([0, 1, 1])
+            else:
+                measurements = self._run(
+                    circuit=program, param_resolver=param_resolver, repetitions=repetitions
+                )
+            yield study.ResultDict(params=param_resolver, measurements=measurements)
+
     def _run(
         self, circuit: circuits.Circuit, param_resolver: study.ParamResolver, repetitions: int
     ) -> Dict[str, np.ndarray]:
         """Run a simulation, mimicking quantum hardware."""
         param_resolver = param_resolver or study.ParamResolver({})
         resolved_circuit = protocols.resolve_parameters(circuit, param_resolver)
         check_all_resolved(resolved_circuit)
@@ -154,43 +191,36 @@
                 qb_index = 0
                 for op in general_ops:
                     key = protocols.measurement_key_name(op.gate)
                     value = []
                     for _ in op.qubits:
                         value.append(sample[qb_index])
                         qb_index = qb_index + 1
-                    self._memory[key].append(np.asarray([value]))
-
-            __memory = {}
-            for key, value in self._memory.items():
-                __memory[key] = np.asarray(value)
-            self._memory = __memory
+                    self._memory[key] += [value]
 
             return self._memory
 
         self._sample_measure = False
         preamble_sim = self._sim
 
         for shot in range(repetitions):
             self._sim = preamble_sim.clone()
             for moment in general_suffix:
                 operations = moment.operations
                 for op in operations:
                     indices = [num_qubits - 1 - qubit_map[qubit] for qubit in op.qubits]
                     key = protocols.measurement_key_name(op.gate)
-                    self._memory[key].append(np.asarray([self._add_qasm_measure(indices)]))
-
-        __memory = {}
-        for key, value in self._memory.items():
-            __memory[key] = np.asarray(value)
-        self._memory = __memory
+                    self._memory[key] = [self._add_qasm_measure(indices)]
 
         return self._memory
         
     def _try_gate(self, op: ops.GateOperation, indices: np.array):
+        if isinstance(op.gate, ops.IdentityGate):
+            return True
+
         # One qubit gate
         if isinstance(op.gate, ops.pauli_gates._PauliX):
             self._sim.x(indices[0])
         elif isinstance(op.gate, ops.pauli_gates._PauliY):
             self._sim.y(indices[0])
         elif isinstance(op.gate, ops.pauli_gates._PauliZ):
             self._sim.z(indices[0])
```

### Comparing `cirqqrack-0.5.1/setup.py` & `cirqqrack-0.6.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from distutils.core import setup
 
 requirements = [
     'pyqrack>=0.8.0'
 ]
 
 # Handle version.
-VERSION = "0.5.1"
+VERSION = "0.6.0"
 
 # Read long description from README.
 README_PATH = os.path.join(os.path.abspath(os.path.dirname(__file__)),
                            'README.md')
 with open(README_PATH) as readme_file:
     README = readme_file.read()
```

