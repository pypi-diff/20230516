# Comparing `tmp/qoqo_qiskit-0.1.1.tar.gz` & `tmp/qoqo_qiskit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qoqo_qiskit-0.1.1.tar", last modified: Mon May  8 13:41:04 2023, max compression
+gzip compressed data, was "qoqo_qiskit-0.1.2.tar", last modified: Tue May 16 09:10:56 2023, max compression
```

## Comparing `qoqo_qiskit-0.1.1.tar` & `qoqo_qiskit-0.1.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:41:04.973906 qoqo_qiskit-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-05-08 13:41:04.973906 qoqo_qiskit-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:41:04.969906 qoqo_qiskit-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-08 13:41:04.973906 qoqo_qiskit-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:41:04.969906 qoqo_qiskit-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:41:04.969906 qoqo_qiskit-0.1.1/src/qoqo_qiskit/
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/src/qoqo_qiskit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:41:04.969906 qoqo_qiskit-0.1.1/src/qoqo_qiskit/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/src/qoqo_qiskit/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11992 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/src/qoqo_qiskit/backend/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:41:04.969906 qoqo_qiskit-0.1.1/src/qoqo_qiskit/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/src/qoqo_qiskit/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4401 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/src/qoqo_qiskit/interface/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:41:04.969906 qoqo_qiskit-0.1.1/src/qoqo_qiskit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14012 2023-05-08 13:41:04.000000 qoqo_qiskit-0.1.1/src/qoqo_qiskit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-08 13:41:04.000000 qoqo_qiskit-0.1.1/src/qoqo_qiskit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-08 13:41:04.000000 qoqo_qiskit-0.1.1/src/qoqo_qiskit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-08 13:41:04.000000 qoqo_qiskit-0.1.1/src/qoqo_qiskit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-08 13:41:04.000000 qoqo_qiskit-0.1.1/src/qoqo_qiskit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:41:04.969906 qoqo_qiskit-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:41:04.969906 qoqo_qiskit-0.1.1/tests/backend/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/tests/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/tests/backend/test_backend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-08 13:41:04.973906 qoqo_qiskit-0.1.1/tests/interface/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/tests/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-08 13:40:48.000000 qoqo_qiskit-0.1.1/tests/interface/test_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:10:56.108547 qoqo_qiskit-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-05-16 09:10:56.108547 qoqo_qiskit-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:10:56.104547 qoqo_qiskit-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5837 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 09:10:56.108547 qoqo_qiskit-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:10:56.104547 qoqo_qiskit-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:10:56.104547 qoqo_qiskit-0.1.2/src/qoqo_qiskit/
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/src/qoqo_qiskit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:10:56.104547 qoqo_qiskit-0.1.2/src/qoqo_qiskit/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/src/qoqo_qiskit/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12060 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/src/qoqo_qiskit/backend/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:10:56.104547 qoqo_qiskit-0.1.2/src/qoqo_qiskit/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/src/qoqo_qiskit/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/src/qoqo_qiskit/interface/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:10:56.104547 qoqo_qiskit-0.1.2/src/qoqo_qiskit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14013 2023-05-16 09:10:56.000000 qoqo_qiskit-0.1.2/src/qoqo_qiskit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-16 09:10:56.000000 qoqo_qiskit-0.1.2/src/qoqo_qiskit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 09:10:56.000000 qoqo_qiskit-0.1.2/src/qoqo_qiskit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-16 09:10:56.000000 qoqo_qiskit-0.1.2/src/qoqo_qiskit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-16 09:10:56.000000 qoqo_qiskit-0.1.2/src/qoqo_qiskit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:10:56.104547 qoqo_qiskit-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:10:56.104547 qoqo_qiskit-0.1.2/tests/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/tests/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10506 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/tests/backend/test_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 09:10:56.104547 qoqo_qiskit-0.1.2/tests/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/tests/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4395 2023-05-16 09:10:29.000000 qoqo_qiskit-0.1.2/tests/interface/test_interface.py
```

### Comparing `qoqo_qiskit-0.1.1/LICENSE` & `qoqo_qiskit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.1/PKG-INFO` & `qoqo_qiskit-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo_qiskit
-Version: 0.1.1
+Version: 0.1.2
 Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 Maintainer-email: Matteo Lodi <matteo.lodi@quantumsimulations.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,8 +224,8 @@
 qoqo_qiskit provides an interface to Qiskit's package.
 Qiskit is under the Apache-2.0 license ( see https://github.com/Qiskit/qiskit/blob/master/LICENSE.txt ). qoqo_qiskit itself is also provided under the Apache-2.0 license.
 
 __Testing__
 
 This software is still in the beta stage. Functions and documentation are not yet complete and breaking changes can occur.
 
-If you find unexpected behaviour please open a github issue. You can also run the pytests in qoqo_myqlm/tests/ locally.
+If you find unexpected behaviour please open a github issue. You can also run the pytests in qoqo_qiskit/tests/ locally.
```

### Comparing `qoqo_qiskit-0.1.1/README.md` & `qoqo_qiskit-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 qoqo_qiskit provides an interface to Qiskit's package.
 Qiskit is under the Apache-2.0 license ( see https://github.com/Qiskit/qiskit/blob/master/LICENSE.txt ). qoqo_qiskit itself is also provided under the Apache-2.0 license.
 
 __Testing__
 
 This software is still in the beta stage. Functions and documentation are not yet complete and breaking changes can occur.
 
-If you find unexpected behaviour please open a github issue. You can also run the pytests in qoqo_myqlm/tests/ locally.
+If you find unexpected behaviour please open a github issue. You can also run the pytests in qoqo_qiskit/tests/ locally.
```

### Comparing `qoqo_qiskit-0.1.1/docs/Makefile` & `qoqo_qiskit-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.1/docs/conf.py` & `qoqo_qiskit-0.1.2/docs/conf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 #
 """Configuration of sphinx documentation module."""
 import tomli
 
-main_version = tomli.load(open("../qoqo_qiskit/pyproject.toml", "rb"))["project"]["version"]
+main_version = tomli.load(open("../pyproject.toml", "rb"))["project"]["version"]
 
 # -- General configuration ------------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 #
 # needs_sphinx = '1.0'
```

### Comparing `qoqo_qiskit-0.1.1/pyproject.toml` & `qoqo_qiskit-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qoqo_qiskit"
-version = "0.1.1"
+version = "0.1.2"
 license = {file="LICENSE"}
 authors = [
     {name="HQS Quantum Simulation GmbH", email="info@quantumsimulations.de"}
 ]
 maintainers = [
     {name="Matteo Lodi", email="matteo.lodi@quantumsimulations.de"}
 ]
```

### Comparing `qoqo_qiskit-0.1.1/src/qoqo_qiskit/__init__.py` & `qoqo_qiskit-0.1.2/src/qoqo_qiskit/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.1/src/qoqo_qiskit/backend/__init__.py` & `qoqo_qiskit-0.1.2/src/qoqo_qiskit/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.1/src/qoqo_qiskit/backend/backend.py` & `qoqo_qiskit-0.1.2/src/qoqo_qiskit/backend/backend.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,25 +78,29 @@
         internal_complex_register_dict: Dict[str, List[complex]] = dict()
 
         output_bit_register_dict: Dict[str, List[List[bool]]] = dict()
         output_float_register_dict: Dict[str, List[List[float]]] = dict()
         output_complex_register_dict: Dict[str, List[List[complex]]] = dict()
 
         for bit_def in circuit.filter_by_tag("DefinitionBit"):
-            internal_bit_register_dict[bit_def.name()] = [False for _ in range(bit_def.length())]
+            internal_bit_register_dict[bit_def.name()] = [
+                False for _ in range(bit_def.length())
+            ]
             clas_regs_sizes[bit_def.name()] = bit_def.length()
             if bit_def.is_output():
                 output_bit_register_dict[bit_def.name()] = list()
 
         for float_def in circuit.filter_by_tag("DefinitionFloat"):
             internal_float_register_dict[float_def.name()] = [
                 0.0 for _ in range(float_def.length())
             ]
             if float_def.is_output():
-                output_float_register_dict[float_def.name()] = cast(List[List[float]], list())
+                output_float_register_dict[float_def.name()] = cast(
+                    List[List[float]], list()
+                )
 
         for complex_def in circuit.filter_by_tag("DefinitionComplex"):
             internal_complex_register_dict[complex_def.name()] = [
                 complex(0.0) for _ in range(complex_def.length())
             ]
             if complex_def.is_output():
                 output_complex_register_dict[complex_def.name()] = cast(
```

### Comparing `qoqo_qiskit-0.1.1/src/qoqo_qiskit/interface/__init__.py` & `qoqo_qiskit-0.1.2/src/qoqo_qiskit/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.1/src/qoqo_qiskit/interface/interface.py` & `qoqo_qiskit-0.1.2/src/qoqo_qiskit/interface/interface.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,19 +27,25 @@
     Args:
         circuit (Circuit): the qoqo Circuit to port.
         qubit_register_name (Optional[str]): the name of the qubit register.
 
     Returns:
         Tuple[QuantumCircuit, Dict[str, int]]: the equivalent QuantumCircuit and the dict
                                             containing info for Qiskit's backend.
+
+    Raises:
+        ValueError: the circuit contains a symbolic PragmaLoop operation.
     """
     # Populating dict output. Currently handling:
     #   - PragmaSetStateVector (continues further down)
+    #   - PragmaGetStateVector
+    #   - PragmaGetDensityMatrix
     #   - PragmaSetNumberOfMeasurement
     #   - PragmaRepeatedMeasurement
+    #   - PragmaLoop
     #   - MeasureQubit
     filtered_circuit = Circuit()
     circuit_info: Dict[str, Any] = {}
     circuit_info["MeasurementInfo"] = {}
     circuit_info["SimulationInfo"] = {}
     circuit_info["SimulationInfo"]["PragmaGetStateVector"] = False
     circuit_info["SimulationInfo"]["PragmaGetDensityMatrix"] = False
@@ -67,24 +73,32 @@
             circuit_info["SimulationInfo"]["PragmaSetNumberOfMeasurements"].append(
                 (op.readout(), op.number_measurements())
             )
         elif "PragmaGetStateVector" in op.tags():
             circuit_info["SimulationInfo"]["PragmaGetStateVector"] = True
         elif "PragmaGetDensityMatrix" in op.tags():
             circuit_info["SimulationInfo"]["PragmaGetDensityMatrix"] = True
+        elif "PragmaLoop" in op.tags():
+            if op.repetitions().is_float:
+                for _ in range(int(op.repetitions().float())):
+                    filtered_circuit += op.circuit()
+            else:
+                raise ValueError("A symbolic PragmaLoop operation is not supported.")
         else:
             filtered_circuit += op
 
     # qoqo_qasm call
     qasm_backend = QasmBackend(qubit_register_name=qubit_register_name)
     input_qasm_str = qasm_backend.circuit_to_qasm_str(filtered_circuit)
 
-    # Handling PragmaSetStateVector + QASM -> Qiskit transformation
+    # QASM -> Qiskit transformation
     return_circuit = QuantumCircuit()
     from_qasm_circuit = QuantumCircuit.from_qasm_str(input_qasm_str)
+
+    # Handling PragmaSetStateVector
     if len(initial_statevector) != 0:
         qregs = []
         for qreg in from_qasm_circuit.qregs:
             qregs.append(QuantumRegister(qreg.size, qreg.name))
         cregs = []
         for creg in from_qasm_circuit.cregs:
             cregs.append(ClassicalRegister(creg.size, creg.name))
```

### Comparing `qoqo_qiskit-0.1.1/src/qoqo_qiskit.egg-info/PKG-INFO` & `qoqo_qiskit-0.1.2/src/qoqo_qiskit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qoqo-qiskit
-Version: 0.1.1
+Version: 0.1.2
 Author-email: HQS Quantum Simulation GmbH <info@quantumsimulations.de>
 Maintainer-email: Matteo Lodi <matteo.lodi@quantumsimulations.de>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -224,8 +224,8 @@
 qoqo_qiskit provides an interface to Qiskit's package.
 Qiskit is under the Apache-2.0 license ( see https://github.com/Qiskit/qiskit/blob/master/LICENSE.txt ). qoqo_qiskit itself is also provided under the Apache-2.0 license.
 
 __Testing__
 
 This software is still in the beta stage. Functions and documentation are not yet complete and breaking changes can occur.
 
-If you find unexpected behaviour please open a github issue. You can also run the pytests in qoqo_myqlm/tests/ locally.
+If you find unexpected behaviour please open a github issue. You can also run the pytests in qoqo_qiskit/tests/ locally.
```

### Comparing `qoqo_qiskit-0.1.1/src/qoqo_qiskit.egg-info/SOURCES.txt` & `qoqo_qiskit-0.1.2/src/qoqo_qiskit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.1/tests/__init__.py` & `qoqo_qiskit-0.1.2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.1/tests/backend/__init__.py` & `qoqo_qiskit-0.1.2/tests/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.1/tests/backend/test_backend.py` & `qoqo_qiskit-0.1.2/tests/backend/test_backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     ClassicalRegister,
     PauliZProduct,
     PauliZProductInput,
 )
 
 from qiskit_aer import AerSimulator
 
-from qoqo_qiskit.backend import QoqoQiskitBackend
+from qoqo_qiskit.backend import QoqoQiskitBackend  # type:ignore
 
 from typing import List, Any
 
 
 def test_constructor():
     simulator = AerSimulator()
     try:
@@ -231,15 +231,17 @@
     for op in operations:
         involved_qubits.update(op.involved_qubits())
         circuit += op
 
     circuit += ops.DefinitionBit("ri", len(involved_qubits), True)
     circuit += ops.PragmaRepeatedMeasurement("ri", 10)
 
-    input = PauliZProductInput(number_qubits=len(involved_qubits), use_flipped_measurement=True)
+    input = PauliZProductInput(
+        number_qubits=len(involved_qubits), use_flipped_measurement=True
+    )
 
     measurement = PauliZProduct(constant_circuit=None, circuits=[circuit], input=input)
 
     try:
         _ = backend.run_measurement(measurement=measurement)
     except:
         assert False
```

### Comparing `qoqo_qiskit-0.1.1/tests/interface/__init__.py` & `qoqo_qiskit-0.1.2/tests/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_qiskit-0.1.1/tests/interface/test_interface.py` & `qoqo_qiskit-0.1.2/tests/interface/test_interface.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,19 +9,23 @@
 # is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express
 # or implied. See the License for the specific language governing permissions and limitations under
 # the License.
 """Test file for interface.py."""
 
 import pytest
 import sys
+
 from qoqo import Circuit
 from qoqo import operations as ops
+
 from qiskit import QuantumCircuit, QuantumRegister, ClassicalRegister
 
-from qoqo_qiskit.interface import to_qiskit_circuit
+from qoqo_qiskit.interface import to_qiskit_circuit  # type:ignore
+
+from typing import Union
 
 
 def test_basic_circuit():
     circuit = Circuit()
     circuit += ops.Hadamard(0)
     circuit += ops.PauliX(1)
 
@@ -110,14 +114,40 @@
 
     out_circ, sim_dict = to_qiskit_circuit(circuit)
 
     assert out_circ == qc
     assert (0, "crg", 0) in sim_dict["MeasurementInfo"]["MeasureQubit"]
 
 
+@pytest.mark.parametrize("repetitions", [0, 2, 4, "test"])
+def test_pragma_loop(repetitions: Union[int, str]):
+    inner_circuit = Circuit()
+    inner_circuit += ops.PauliX(1)
+    inner_circuit += ops.PauliY(2)
+
+    circuit = Circuit()
+    circuit += ops.Hadamard(0)
+    circuit += ops.PragmaLoop(repetitions=repetitions, circuit=inner_circuit)
+    circuit += ops.Hadamard(3)
+
+    qc = QuantumCircuit(4)
+    qc.h(0)
+    if type(repetitions) != str:
+        for _ in range(repetitions):
+            qc.x(1)
+            qc.y(2)
+    qc.h(3)
+
+    try:
+        out_circ, _ = to_qiskit_circuit(circuit)
+        assert out_circ == qc
+    except ValueError as e:
+        assert e.args == ("A symbolic PragmaLoop operation is not supported.",)
+
+
 def test_simulation_info():
     circuit = Circuit()
     circuit += ops.Hadamard(0)
     circuit += ops.CNOT(0, 1)
     circuit += ops.DefinitionBit("ro", 2, True)
     circuit += ops.PragmaGetStateVector("ro", None)
     circuit += ops.PragmaGetDensityMatrix("ro", None)
```

