# Comparing `tmp/qwak-sim-2023.1012a0.tar.gz` & `tmp/qwak-sim-2023.1013a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qwak-sim-2023.1012a0.tar", last modified: Thu Jan 12 20:38:58 2023, max compression
+gzip compressed data, was "qwak-sim-2023.1013a0.tar", last modified: Tue May 16 14:40:52 2023, max compression
```

## Comparing `qwak-sim-2023.1012a0.tar` & `qwak-sim-2023.1013a0.tar`

### file list

```diff
@@ -1,30 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-01-12 20:38:58.927173 qwak-sim-2023.1012a0/
--rw-rw-rw-   0        0        0    35823 2022-04-06 17:13:42.000000 qwak-sim-2023.1012a0/LICENSE
--rw-rw-rw-   0        0        0    44887 2023-01-12 20:38:58.927173 qwak-sim-2023.1012a0/PKG-INFO
--rw-rw-rw-   0        0        0     2997 2023-01-12 19:46:46.000000 qwak-sim-2023.1012a0/README.md
-drwxrwxrwx   0        0        0        0 2023-01-12 20:38:58.868984 qwak-sim-2023.1012a0/core/
-drwxrwxrwx   0        0        0        0 2023-01-12 20:38:58.897166 qwak-sim-2023.1012a0/core/qwak/
--rw-rw-rw-   0        0        0     3173 2023-01-12 18:57:54.000000 qwak-sim-2023.1012a0/core/qwak/Errors.py
--rw-rw-rw-   0        0        0    19164 2023-01-12 18:09:36.000000 qwak-sim-2023.1012a0/core/qwak/GraphicalQWAK.py
--rw-rw-rw-   0        0        0    15794 2023-01-12 18:57:55.000000 qwak-sim-2023.1012a0/core/qwak/Operator.py
--rw-rw-rw-   0        0        0     8684 2023-01-12 20:33:39.000000 qwak-sim-2023.1012a0/core/qwak/ProbabilityDistribution.py
--rw-rw-rw-   0        0        0     7929 2023-01-12 18:08:20.000000 qwak-sim-2023.1012a0/core/qwak/QuantumWalk.py
--rw-rw-rw-   0        0        0    10907 2023-01-12 18:57:56.000000 qwak-sim-2023.1012a0/core/qwak/State.py
--rw-rw-rw-   0        0        0     5868 2022-09-11 00:13:38.000000 qwak-sim-2023.1012a0/core/qwak/StochasticOperator.py
--rw-rw-rw-   0        0        0     1392 2022-09-11 00:13:38.000000 qwak-sim-2023.1012a0/core/qwak/StochasticProbabilityDistribution.py
--rw-rw-rw-   0        0        0     3282 2022-09-11 00:13:38.000000 qwak-sim-2023.1012a0/core/qwak/StochasticQuantumWalk.py
--rw-rw-rw-   0        0        0     5017 2022-09-11 00:13:38.000000 qwak-sim-2023.1012a0/core/qwak/StochasticQwak.py
--rw-rw-rw-   0        0        0      164 2023-01-12 20:38:29.000000 qwak-sim-2023.1012a0/core/qwak/__init__.py
--rw-rw-rw-   0        0        0    27682 2023-01-12 20:35:08.000000 qwak-sim-2023.1012a0/core/qwak/qwak.py
-drwxrwxrwx   0        0        0        0 2023-01-12 20:38:58.920172 qwak-sim-2023.1012a0/core/qwak_sim.egg-info/
--rw-rw-rw-   0        0        0    44887 2023-01-12 20:38:58.000000 qwak-sim-2023.1012a0/core/qwak_sim.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      642 2023-01-12 20:38:58.000000 qwak-sim-2023.1012a0/core/qwak_sim.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-12 20:38:58.000000 qwak-sim-2023.1012a0/core/qwak_sim.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       74 2023-01-12 20:38:58.000000 qwak-sim-2023.1012a0/core/qwak_sim.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-01-12 20:38:58.000000 qwak-sim-2023.1012a0/core/qwak_sim.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-01-12 20:38:58.925173 qwak-sim-2023.1012a0/core/utils/
--rw-rw-rw-   0        0        0     8767 2022-09-26 03:47:41.000000 qwak-sim-2023.1012a0/core/utils/PerfectStateTransfer.py
--rw-rw-rw-   0        0        0       33 2023-01-12 20:38:29.000000 qwak-sim-2023.1012a0/core/utils/__init__.py
--rw-rw-rw-   0        0        0     1081 2023-01-12 18:57:57.000000 qwak-sim-2023.1012a0/core/utils/jsonMethods.py
--rw-rw-rw-   0        0        0     1572 2023-01-12 20:38:29.000000 qwak-sim-2023.1012a0/pyproject.toml
--rw-rw-rw-   0        0        0      575 2023-01-12 20:38:58.935176 qwak-sim-2023.1012a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 14:40:52.384733 qwak-sim-2023.1013a0/
+-rw-rw-rw-   0        0        0    35823 2022-04-06 17:13:42.000000 qwak-sim-2023.1013a0/LICENSE
+-rw-rw-rw-   0        0        0    44887 2023-05-16 14:40:52.384733 qwak-sim-2023.1013a0/PKG-INFO
+-rw-rw-rw-   0        0        0     2997 2023-03-03 16:23:09.000000 qwak-sim-2023.1013a0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-16 14:40:52.332733 qwak-sim-2023.1013a0/core/
+drwxrwxrwx   0        0        0        0 2023-05-16 14:40:52.350733 qwak-sim-2023.1013a0/core/qwak/
+-rw-rw-rw-   0        0        0     3173 2023-01-12 18:57:54.000000 qwak-sim-2023.1013a0/core/qwak/Errors.py
+-rw-rw-rw-   0        0        0    19476 2023-01-12 21:11:43.000000 qwak-sim-2023.1013a0/core/qwak/GraphicalQWAK.py
+-rw-rw-rw-   0        0        0    18390 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/core/qwak/Operator.py
+-rw-rw-rw-   0        0        0     9100 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/core/qwak/ProbabilityDistribution.py
+-rw-rw-rw-   0        0        0     7927 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/core/qwak/QuantumWalk.py
+-rw-rw-rw-   0        0        0    10903 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/core/qwak/State.py
+-rw-rw-rw-   0        0        0     5868 2022-09-11 00:13:38.000000 qwak-sim-2023.1013a0/core/qwak/StochasticOperator.py
+-rw-rw-rw-   0        0        0     1392 2022-09-11 00:13:38.000000 qwak-sim-2023.1013a0/core/qwak/StochasticProbabilityDistribution.py
+-rw-rw-rw-   0        0        0     3282 2022-09-11 00:13:38.000000 qwak-sim-2023.1013a0/core/qwak/StochasticQuantumWalk.py
+-rw-rw-rw-   0        0        0     5017 2022-09-11 00:13:38.000000 qwak-sim-2023.1013a0/core/qwak/StochasticQwak.py
+-rw-rw-rw-   0        0        0      164 2023-05-16 14:39:40.000000 qwak-sim-2023.1013a0/core/qwak/__init__.py
+-rw-rw-rw-   0        0        0    31792 2023-05-16 02:17:11.000000 qwak-sim-2023.1013a0/core/qwak/qwak.py
+drwxrwxrwx   0        0        0        0 2023-05-16 14:40:52.372732 qwak-sim-2023.1013a0/core/qwak_sim.egg-info/
+-rw-rw-rw-   0        0        0    44887 2023-05-16 14:40:52.000000 qwak-sim-2023.1013a0/core/qwak_sim.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      800 2023-05-16 14:40:52.000000 qwak-sim-2023.1013a0/core/qwak_sim.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-16 14:40:52.000000 qwak-sim-2023.1013a0/core/qwak_sim.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       74 2023-05-16 14:40:52.000000 qwak-sim-2023.1013a0/core/qwak_sim.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-16 14:40:52.000000 qwak-sim-2023.1013a0/core/qwak_sim.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-16 14:40:52.377733 qwak-sim-2023.1013a0/core/utils/
+-rw-rw-rw-   0        0        0     8767 2022-09-26 03:47:41.000000 qwak-sim-2023.1013a0/core/utils/PerfectStateTransfer.py
+-rw-rw-rw-   0        0        0       33 2023-05-16 14:39:40.000000 qwak-sim-2023.1013a0/core/utils/__init__.py
+-rw-rw-rw-   0        0        0     1081 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/core/utils/jsonTools.py
+-rw-rw-rw-   0        0        0    16222 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/core/utils/plotTools.py
+-rw-rw-rw-   0        0        0     1572 2023-05-16 14:39:40.000000 qwak-sim-2023.1013a0/pyproject.toml
+-rw-rw-rw-   0        0        0      575 2023-05-16 14:40:52.386733 qwak-sim-2023.1013a0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-16 14:40:52.383217 qwak-sim-2023.1013a0/tests/
+-rw-rw-rw-   0        0        0    19690 2023-01-12 20:35:08.000000 qwak-sim-2023.1013a0/tests/test_GraphicalQwakCycle.py
+-rw-rw-rw-   0        0        0     9573 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/tests/test_QwakComplete.py
+-rw-rw-rw-   0        0        0     8030 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/tests/test_QwakCycle.py
+-rw-rw-rw-   0        0        0     9608 2023-05-04 16:33:03.000000 qwak-sim-2023.1013a0/tests/test_QwakPath.py
+-rw-rw-rw-   0        0        0     1960 2022-09-10 23:35:23.000000 qwak-sim-2023.1013a0/tests/test_StochasticQwak.py
```

### Comparing `qwak-sim-2023.1012a0/LICENSE` & `qwak-sim-2023.1013a0/LICENSE`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1012a0/PKG-INFO` & `qwak-sim-2023.1013a0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-sim
-Version: 2023.1012a0
+Version: 2023.1013a0
 Summary: Simulate Continuous-Time Quantum Walks
 Home-page: https://github.com/qwchagas/qwak
 Author: Jaime Santos
 Author-email: Jaime Santos <jaimepereirasantos123@gmail.com>, Bruno Chagas <na@na.na>, Rodrigo Chaves <na@na.na>, Lorenzo Buffoni <na@na.na>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `qwak-sim-2023.1012a0/README.md` & `qwak-sim-2023.1013a0/README.md`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1012a0/core/qwak/Errors.py` & `qwak-sim-2023.1013a0/core/qwak/Errors.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1012a0/core/qwak/GraphicalQWAK.py` & `qwak-sim-2023.1013a0/core/qwak/GraphicalQWAK.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,16 @@
         dynamicN: int,
         staticGraph: nx.Graph,
         dynamicGraph: nx.Graph,
         staticStateList: list,
         dynamicStateList: list,
         staticTime: float,
         dynamicTimeList: list,
+        staticGamma: float = None,
+        dynamicGamma: float = None,
         qwakId: str = 'undefinedUser',
     ) -> None:
         """_summary_
 
         Parameters
         ----------
         staticN : int
@@ -45,26 +47,32 @@
             _description_
         dynamicStateList : list
             _description_
         staticTime : float
             _description_
         dynamicTimeList : list
             _description_
+        staticGamma : float
+            _description_
+        dynamicGamma : float
+            _description_
         """
         self._staticN = staticN
         self._dynamicN = dynamicN
         self._staticGraph = staticGraph
         self._dynamicGraph = dynamicGraph
         self._staticStateList = staticStateList
         self._dynamicStateList = dynamicStateList
         self._staticTime = staticTime
         self._dynamicTime = dynamicTimeList
         self._dynamicTimeList = np.linspace(
             self._dynamicTime[0], self._dynamicTime[1], int(
                 self._dynamicTime[1]))
+        self._staticGamma = staticGamma
+        self._dynamicGamma = dynamicGamma
         self._staticQWAK = QWAK(self._staticGraph)
         # self._staticProbDist = self._staticQWAK.getProbDist()
         # self._dynamicQWAK = QWAK(self._dynamicGraph)
         # self._dynamicProbDistList = self._dynamicQWAK.getProbDistList()
         # self._dynamicAmpList = self._dynamicQWAK.getWalkList()
         self._qwakId = qwakId
 
@@ -182,15 +190,15 @@
         -------
         _type_
             _description_
         """
         try:
             # self._staticQWAK.resetWalk()
             self._staticQWAK.runWalk(
-                self._staticTime, self._staticStateList)
+                time=self._staticTime,gamma=self._staticGamma,initStateList=self._staticStateList)
             self._staticProbDist = self._staticQWAK.getProbDist()
             qwProbVec = self._staticProbDist.getProbVec().tolist()
             return [False, qwProbVec]
         except StateOutOfBounds as err:
             return [True, str(err)]
 
     def runMultipleWalks(self):
```

### Comparing `qwak-sim-2023.1012a0/core/qwak/Operator.py` & `qwak-sim-2023.1013a0/core/qwak/Operator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 from __future__ import annotations
 from typing import Union
 
 import networkx as nx
 import sympy as sp
-from scipy.linalg import inv
+from scipy.linalg import inv, expm
 from sympy.abc import pi
 import numpy as np
-from utils.jsonMethods import json_matrix_to_complex, complex_matrix_to_json
+from utils.jsonTools import json_matrix_to_complex, complex_matrix_to_json
 import json
 
 from qwak.Errors import MissingNodeInput
 from utils.PerfectStateTransfer import isStrCospec, checkRoots, swapNodes, getEigenVal
 
-
 class Operator:
     def __init__(
             self,
             graph: nx.Graph,
-            time: float = None,
+            gamma: float = 1,
+            time: float = 0,
             laplacian: bool = False,
-            markedSearch: list = None,
+            markedElements: list = [],
     ) -> None:
         """
         Class for the quantum walk operator.
 
         This object is initialized with a user inputted graph, which is then used to
         generate the dimension of the operator and the adjacency matrix, which is
         the central structure required to perform walks on regular graphs. Note that this
@@ -35,169 +35,138 @@
         decomposition. This was the chosen method since it is computationally cheaper than calculating
         the matrix exponent directly.
 
         Parameters
         ----------
         graph : nx.Graph
             Graph where the walk will be performed.
+        gamma : float
+            Needs Completion.
         time: float, optional
             Time for which to calculate the operator, by default None.
         laplacian : bool, optional
             Allows the user to choose whether to use the Laplacian or simple adjacency matrix, by default False.
-        markedSearch : list, optional
+        markedElements : list, optional
             List with marked elements for search, by default None.
         """
-        if time is not None:
-            self._time = time
-        else:
-            self._time = 0
-        if laplacian is not None:
-            self._laplacian = laplacian
-        else:
-            self._laplacian = False
-        if markedSearch is not None:
-            self._markedSearch = markedSearch
-        else:
-            self._markedSearch = None
+        self._time = time
+        self._gamma = gamma
+        self._laplacian = laplacian
+        self._markedElements = markedElements
         self._graph = graph
-        self._buildAdjacency(self._laplacian, self._markedSearch)
         self._n = len(graph)
         self._operator = np.zeros((self._n, self._n), dtype=complex)
-        self._isHermitian = np.allclose(
-            self._adjacencyMatrix,
-            self._adjacencyMatrix.conjugate().transpose())
-        self._buildEigenValues(self._isHermitian)
 
-    def to_json(self) -> str:
-        """
-            Converts the operator object to a JSON string.
+        self._hamiltonian = self._buildHamiltonian(self._graph,self._laplacian)
+        if self._markedElements:
+            self._hamiltonian = self._buildSearchHamiltonian(self._hamiltonian, self._markedElements)
 
-        Returns
-        -------
-        str
-            JSON string of the operator object.
-        """
-        return json.dumps({
-            'graph': nx.node_link_data(self._graph),
-            'time': self._time,
-            'laplacian': self._laplacian,
-            'markedSearch': self._markedSearch,
-            'adjacencyMatrix': complex_matrix_to_json(self._adjacencyMatrix),
-            'eigenvalues': self._eigenvalues.tolist(),
-            'eigenvectors': complex_matrix_to_json(self._eigenvectors),
-            'operator': complex_matrix_to_json(self._operator),
-        })
+        self._isHermitian = self._hermitianTest(self._hamiltonian)
+        self._eigenvalues, self._eigenvectors = self._buildEigenValues(self._hamiltonian)
 
-    @classmethod
-    def from_json(cls, json_var: Union([str, dict])) -> Operator:
-        """Converts a JSON string to an operator object.
-
-        Parameters
-        ----------
-        json_str : str
-            JSON string of the operator object.
-
-        Returns
-        -------
-        Operator
-            Operator object.
-        """
-        if isinstance(json_var, str):
-            data = json.loads(json_var)
-        elif isinstance(json_var, dict):
-            data = json_var
-        graph = nx.node_link_graph(data['graph'])
-        time = data['time']
-        laplacian = data['laplacian']
-        markedSearch = data['markedSearch']
-        adjacencyMatrix = np.array(
-            json_matrix_to_complex(
-                data['adjacencyMatrix']))
-        eigenvalues = np.array(data['eigenvalues'])
-
-        eigenvectors = np.array(
-            json_matrix_to_complex(
-                data['eigenvectors']))
-        operator = np.array(json_matrix_to_complex(data['operator']))
-
-        newOp = cls(graph, time, laplacian, markedSearch)
-        newOp._setAdjacencyMatrixOnly(adjacencyMatrix)
-        newOp._setEigenValues(eigenvalues)
-        newOp._setEigenVectors(eigenvectors)
-        newOp._setOperatorVec(operator)
-        return newOp
-
-    def buildDiagonalOperator(self, time: float = None) -> None:
+    def buildDiagonalOperator(self, time: float = 0) -> None:
         """Builds operator matrix from optional time and transition rate parameters, defined by user.
 
         The first step is to calculate the diagonal matrix that takes in time, transition rate and
         eigenvalues and convert it to a list of the diagonal entries.
 
         The entries are then multiplied
         by the eigenvectors, and the last step is to perform matrix multiplication with the complex
         conjugate of the eigenvectors.
 
         Parameters
         ----------
         time : float, optional
             Time for which to calculate the operator, by default 0.
+        gamma : float, optional
+            Needs completion.
+        round : int, optional
         """
-        if time is not None:
-            self._time = time
+        self._time = time
         diag = np.diag(
             np.exp(-1j * self._eigenvalues * self._time)).diagonal()
         self._operator = np.multiply(self._eigenvectors, diag)
         if self._isHermitian:
             self._operator = np.matmul(
-                self._operator,
-                self._eigenvectors.conjugate().transpose())
+                    self._operator, self._eigenvectors.conjugate().transpose())
         else:
             self._operator = np.matmul(
-                self._operator, inv(
+                    self._operator, inv(
                     self._eigenvectors))
 
-    def _buildAdjacency(
+    def buildExpmOperator(self, time: float = 0) -> None:
+        """Builds operator matrix from optional time and transition rate parameters, defined by user.
+
+        Uses the scipy function expm to calculate the matrix exponential of the adjacency matrix.
+
+        Parameters
+        ----------
+        time : float, optional
+            Time for which to calculate the operator, by default 0.
+        """
+        self._time = time
+        self._operator = expm(-1j * self._hamiltonian * self._time)
+
+    def _buildHamiltonian(
             self,
+            graph,
             laplacian: bool,
-            markedSearch: list) -> None:
-        """Builds the adjacency matrix of the graph, which is either the Laplacian or the simple matrix.
+                    ) -> np.ndarray:
+        """Builds the hamiltonian of the graph, which is either the Laplacian or the simple matrix.
 
         Parameters
         ----------
         laplacian : bool
             Allows the user to choose whether to use the Laplacian or simple adjacency matrix.
-        markedSearch : list
+        markedElements : list
             List of elements for the search.
         """
+        self._adjacency = nx.to_numpy_array(
+            graph, dtype=complex)
         if laplacian:
-            self._adjacencyMatrix = np.asarray(
-                nx.laplacian_matrix(
-                    self._graph).todense().astype(complex))
-        else:
-            self._adjacencyMatrix = nx.to_numpy_array(
-                self._graph, dtype=complex)
-        if markedSearch is not None:
-            for marked in markedSearch:
-                self._adjacencyMatrix[marked[0], marked[0]] += marked[1]
+            self._adjacency = self._adjacency - self._degreeDiagonalMatrix(graph)
+        return -self._adjacency * self._gamma
+
+    def _buildSearchHamiltonian(self,hamiltonian,markedElements):
+        for marked in markedElements:
+            hamiltonian[marked[0], marked[0]] += marked[1]
+        return hamiltonian
 
-    def _buildEigenValues(self, isHermitian: bool) -> None:
+    def _buildEigenValues(self, hamiltonian) -> None:
         """Builds the eigenvalues and eigenvectors of the adjacency matrix.
 
         Parameters
         ----------
         isHermitian : bool
             Checks if the adjacency matrix is Hermitian.
         """
-        if isHermitian:
-            self._eigenvalues, self._eigenvectors = np.linalg.eigh(
-                self._adjacencyMatrix
+
+        if self._isHermitian:
+            eigenvalues, eigenvectors = np.linalg.eigh(
+                hamiltonian
             )
         else:
-            self._eigenvalues, self._eigenvectors = np.linalg.eig(
-                self._adjacencyMatrix)
+            eigenvalues, eigenvectors  = np.linalg.eig(
+                hamiltonian )
+        return eigenvalues, eigenvectors
+
+    def _hermitianTest(self, hamiltonian) -> bool:
+        """Checks if the adjacency matrix is Hermitian.
+
+        Parameters
+        ----------
+        hamiltonian : np.ndarray
+            Adjacency matrix.
+
+        Returns
+        -------
+        bool
+            True if Hermitian, False otherwise.
+        """
+        return np.allclose(hamiltonian, hamiltonian.conj().T)
 
     def getEigenValues(self) -> list:
         """Returns the eigenvalues of the adjacency matrix.
 
         Returns
         -------
         list
@@ -211,33 +180,54 @@
         Parameters
         ----------
         eigenValues : list
             List of eigenvalues.
         """
         self._eigenvalues = eigenValues
 
+    def getEigenVectors(self) -> list:
+        """Returns the eigenvectors of the adjacency matrix.
+
+        Returns
+        -------
+        list
+            List of eigenvectors.
+        """
+        return self._eigenvectors
+
     def _setEigenVectors(self, eigenVectors: list) -> None:
         """Sets the eigenvectors of the adjacency matrix.
 
         Parameters
         ----------
         eigenVectors : list
             _description_
         """
         self._eigenvectors = eigenVectors
 
-    def getEigenVectors(self) -> list:
-        """Returns the eigenvectors of the adjacency matrix.
+    def getHamiltonian(self):
+        """Returns the hamiltonian of the graph, which is either the Laplacian or the simple matrix.
 
         Returns
         -------
-        list
-            List of eigenvectors.
+        np.ndarray
+            Hamiltonian of the graph.
         """
-        return self._eigenvectors
+        return self._hamiltonian
+
+    def setHamiltonian(self, hamiltonian):
+        """Sets the hamiltonian for the walk.
+
+        Parameters
+        ----------
+        hamiltonian : np.ndarray
+            Hamiltonian of the graph.
+        """
+        self._hamiltonian = hamiltonian
+        self._eigenvalues, self._eigenvectors = self._buildEigenValues(self._hamiltonian)
 
     def resetOperator(self) -> None:
         """Resets Operator object."""
         self._operator = np.zeros((self._n, self._n), dtype=complex)
 
     def setDim(self, newDim: int, graph: nx.Graph) -> None:
         """Sets the current Operator objects dimension to a user defined one.
@@ -248,18 +238,21 @@
             New dimension for the Operator object.
         graph : nx.Graph
             New graph for the Operator object.
         """
         self._n = newDim
         self._operator = np.zeros((self._n, self._n), dtype=complex)
         self._graph = graph
-        self._adjacencyMatrix = (
+        #TODO: We might need to make a laplacian check here.
+        self._hamiltonian = (
             nx.adjacency_matrix(self._graph).todense().astype(complex)
         )
-        self.setAdjacencyMatrix(self._adjacencyMatrix)
+        #TODO: This function and setAdjacencyMatrix need to be reworked.
+        self._adjacency = self._hamiltonian
+        self.setAdjacencyMatrix(self._hamiltonian)
 
     def getDim(self) -> int:
         """Gets the current graph dimension.
 
         Returns
         -------
         int
@@ -293,43 +286,46 @@
         them instead change the graph entirely.
 
         Parameters
         ----------
         adjacencyMatrix : np.ndarray
             New adjacency matrix.
         """
-        self._adjacencyMatrix = adjacencyMatrix.astype(complex)
-        self._n = len(self._adjacencyMatrix)
+        #TODO: Laplacian check here aswell.
+        #TODO: Inconsistentcy with adjaceny matrix.
+        self._hamiltonian = adjacencyMatrix.astype(complex)
+        self._adjacency = self._hamiltonian
+        self._n = len(self._hamiltonian)
         self.resetOperator()
-        self._buildEigenValues(self._isHermitian)
+        self._eigenvalues, self._eigenvectors = self._buildEigenValues(self._hamiltonian)
 
     def _setAdjacencyMatrixOnly(
             self, adjacencyMatrix: np.ndarray) -> None:
         """Sets the adjacency matrix of the operator to a user defined one.
         Might make more sense to not give the user control over this parameter, and make
         them instead change the graph entirely.
 
         Parameters
         ----------
         adjacencyMatrix : np.ndarray
             New adjacency matrix.
         """
-        self._adjacencyMatrix = adjacencyMatrix.astype(complex)
-        self._n = len(self._adjacencyMatrix)
+        self._hamiltonian = adjacencyMatrix.astype(complex)
+        self._n = len(self._hamiltonian)
         self.resetOperator()
 
     def getAdjacencyMatrix(self) -> np.ndarray:
         """Gets the current adjacency matrix of the Operator.
 
         Returns
         -------
         np.ndarray
             Adjacency matrix of the Operator.
         """
-        return self._adjacencyMatrix
+        return self._adjacency
 
     def _setOperatorVec(self, newOperator: np.ndarray) -> None:
         """Sets all the parameters of the current operator to user defined ones.
 
         Parameters
         ----------
         newOperator : Operator
@@ -379,15 +375,15 @@
         # TODO: Check if numpy is faster for eigenvecs and vals.
         try:
             nodeA = int(nodeA)
             nodeB = int(nodeB)
             if nodeA > nodeB:
                 nodeA, nodeB = swapNodes(nodeA, nodeB)
 
-            symAdj = sp.Matrix(self._adjacencyMatrix.tolist())
+            symAdj = sp.Matrix(self._hamiltonian.tolist())
             # Isto já foi calculado.
             eigenVec, D = symAdj.diagonalize()
             eigenVal = getEigenVal(D)
             isCospec = isStrCospec(symAdj, nodeA, nodeB)
             chRoots, g, delta = checkRoots(
                 symAdj, nodeA, eigenVec, eigenVal)
             if isCospec and chRoots:
@@ -395,14 +391,98 @@
             else:
                 result = -1
             return result
         except ValueError:
             raise MissingNodeInput(
                 f"A node number is missing: nodeA = {nodeA}; nodeB = {nodeB}")
 
+    def getMarkedElements(self) -> list:
+        """Returns the marked elements of the operator.
+
+        Returns
+        -------
+        list
+            List of marked elements.
+        """
+        return self._markedElements
+
+    def setMarkedElements(self, markedElements: list) -> None:
+        """Sets the marked elements of the operator.
+
+        Parameters
+        ----------
+        markedElements : list
+            List of marked elements.
+        """
+        self._markedElements = markedElements
+
+    def to_json(self) -> str:
+        """
+            Converts the operator object to a JSON string.
+
+        Returns
+        -------
+        str
+            JSON string of the operator object.
+        """
+        return json.dumps({
+            'graph': nx.node_link_data(self._graph),
+            'time': self._time,
+            'laplacian': self._laplacian,
+            'markedElements': self._markedElements,
+            'adjacencyMatrix': complex_matrix_to_json(self._hamiltonian),
+            'eigenvalues': self._eigenvalues.tolist(),
+            'eigenvectors': complex_matrix_to_json(self._eigenvectors),
+            'operator': complex_matrix_to_json(self._operator),
+        })
+
+    @classmethod
+    def from_json(cls, json_var: Union[str, dict]) -> Operator:
+        """Converts a JSON string to an operator object.
+
+        Parameters
+        ----------
+        json_var : str, dict
+            JSON string of the operator object.
+
+        Returns
+        -------
+        Operator
+            Operator object.
+        """
+        if isinstance(json_var, str):
+            data = json.loads(json_var)
+        elif isinstance(json_var, dict):
+            data = json_var
+        graph = nx.node_link_graph(data['graph'])
+        time = data['time']
+        laplacian = data['laplacian']
+        markedElements = data['markedElements']
+        adjacencyMatrix = np.array(
+            json_matrix_to_complex(
+                data['adjacencyMatrix']))
+        eigenvalues = np.array(data['eigenvalues'])
+
+        eigenvectors = np.array(
+            json_matrix_to_complex(
+                data['eigenvectors']))
+        operator = np.array(json_matrix_to_complex(data['operator']))
+
+        newOp = cls(graph, time, laplacian, markedElements)
+        newOp._setAdjacencyMatrixOnly(adjacencyMatrix)
+        newOp._setEigenValues(eigenvalues)
+        newOp._setEigenVectors(eigenvectors)
+        newOp._setOperatorVec(operator)
+        return newOp
+
+    @staticmethod
+    def _degreeDiagonalMatrix(G):
+        degrees = np.array(list(dict(G.degree()).values()))
+        return np.diag(degrees)
+
     def __mul__(self, other: np.ndarray) -> np.ndarray:
         """Left-side multiplication for the Operator class.
 
         Parameters
         ----------
         other : np.ndarray
             Another Numpy ndarray to multiply the operator by.
```

### Comparing `qwak-sim-2023.1012a0/core/qwak/ProbabilityDistribution.py` & `qwak-sim-2023.1013a0/core/qwak/ProbabilityDistribution.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 from typing import Union
 
 import numpy as np
 from qwak.State import State
 from qwak.Errors import MissingNodeInput
 import json
-from utils.jsonMethods import json_matrix_to_complex, complex_matrix_to_json
+from utils.jsonTools import json_matrix_to_complex, complex_matrix_to_json
 from functools import reduce
 
 
 class ProbabilityDistribution:
     def __init__(self, state: State) -> None:
         """The dimension of the probability vector will then be loaded from
         the state inputted by the user.
@@ -251,14 +251,28 @@
                 for i in range(int(fromNode), int(toNode) + 1):
                     survProb += self._probVec[i]
             return survProb
         except ValueError:
             raise MissingNodeInput(
                 f"A node number is missing: fromNode = {fromNode}; toNode={toNode}")
 
+    def searchNodeProbability(self, searchNode: int) -> float:
+        """Searches and gets the probability associated with a given node.
+
+        Parameters
+        ----------
+        searchNode : int
+            User inputted node for the search.
+
+        Returns
+        -------
+        float
+            Probability of the searched node.
+        """
+        return self._probVec.item(searchNode)
     def __str__(self) -> str:
         """String representation of the ProbabilityDistribution object.
 
         Returns
         -------
         str
             String of the ProbabilityDistribution object.
@@ -272,7 +286,9 @@
         -------
         str
             String of the ProbabilityDistribution object.
         """
         return f"N: {self._n}\n" \
                f"State:\n\t{self._stateVec}\n" \
                f"ProbDist:\n\t{self._probVec}"
+
+
```

### Comparing `qwak-sim-2023.1012a0/core/qwak/QuantumWalk.py` & `qwak-sim-2023.1013a0/core/qwak/QuantumWalk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 import warnings
 import numpy as np
 import json
-from utils.jsonMethods import json_matrix_to_complex, complex_matrix_to_json
+from utils.jsonTools import json_matrix_to_complex, complex_matrix_to_json
 
 from qwak.Operator import Operator
 from qwak.State import State
 
 
 warnings.filterwarnings("ignore")
```

### Comparing `qwak-sim-2023.1012a0/core/qwak/State.py` & `qwak-sim-2023.1013a0/core/qwak/State.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Union
 
 import numpy as np
 from scipy.linalg import inv
 import json
 
 from qwak.Errors import StateOutOfBounds, NonUnitaryState
-from utils.jsonMethods import json_matrix_to_complex, complex_matrix_to_json
+from utils.jsonTools import json_matrix_to_complex, complex_matrix_to_json
 
 
 class State:
     def __init__(self, n: int, nodeList: list = None,
                  customStateList: list = None) -> None:
         """Object is initialized with a mandatory user inputted dimension, an optional
         stateList parameter which will be used to create the amplitudes for each node in the state
@@ -57,15 +57,15 @@
             "custom_state_list": self._customStateList,
             "state_vec": complex_matrix_to_json(
                 self._stateVec.tolist()),
         }
         return json.dumps(state_dict)
 
     @classmethod
-    def from_json(cls, json_var: Union([str, dict])):
+    def from_json(cls, json_var: Union[str, dict]):
         """The from_json method is marked with the @classmethod decorator because it is a method that is called on the class itself,
         rather than on an instance of the class.
 
         This is necessary because it is used to create a new instance of the Operator class from a JSON string,
         and it does not require an instance of the Operator class to do so.
 
         Parameters
```

### Comparing `qwak-sim-2023.1012a0/core/qwak/StochasticOperator.py` & `qwak-sim-2023.1013a0/core/qwak/StochasticOperator.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1012a0/core/qwak/StochasticProbabilityDistribution.py` & `qwak-sim-2023.1013a0/core/qwak/StochasticProbabilityDistribution.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1012a0/core/qwak/StochasticQuantumWalk.py` & `qwak-sim-2023.1013a0/core/qwak/StochasticQuantumWalk.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1012a0/core/qwak/StochasticQwak.py` & `qwak-sim-2023.1013a0/core/qwak/StochasticQwak.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1012a0/core/qwak/qwak.py` & `qwak-sim-2023.1013a0/core/qwak/qwak.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,23 +19,24 @@
 from qwak.ProbabilityDistribution import (
     ProbabilityDistribution,
 )
 
 
 class QWAK:
     def __init__(
-        self,
-        graph: nx.Graph,
-        time: float = None,
-        timeList: list = None,
-        initStateList: list = None,
-        customStateList: list = None,
-        laplacian: bool = False,
-        markedSearch: list = None,
-        qwakId: str = 'userUndef',
+            self,
+            graph: nx.Graph,
+            time: float = 0,
+            timeList: list = None,
+            gamma: float = 1,
+            initStateList: list = None,
+            customStateList: list = None,
+            laplacian: bool = False,
+            markedElements: list = [],
+            qwakId: str = 'userUndef',
     ) -> None:
         """Data access class that combines all three components required to
         perform a continuous-time quantum walk, given by the multiplication of
         an operator (represented by the Operator class) by an initial state
         (State class).  This multiplication is achieved in the
         StaticQuantumwalk class, which returns a final state (State Class)
         representing the amplitudes of each state associated with a graph node.
@@ -60,140 +61,82 @@
         initStateList : list[int], optional
             List with chosen initial states for uniform superposition, by default None
         customStateList : list[(int,complex)], optional
             Custom init state, by default None.
         laplacian : bool, optional
             Allows the user to choose whether to use the
             Laplacian or simple adjacency matrix, by default False.
-        markedSearch : list, optional
+        markedElements : list, optional
             List with marked elements for search, by default None.
         qwakId : str, optional
             User-defined ID for the QWAK instance, by default 'userUndef'.
         """
         self._graph = graph
         self._n = len(self._graph)
         if timeList is not None:
-            self._timeList = np.array(timeList)
+            self._timeList = [x for x in timeList]
         else:
-            self._timeList = np.zeros(self._n)
+            self._timeList = [0]*self._n
         self._qwakId = qwakId
         self._operator = Operator(
             self._graph,
             time=time,
+            gamma=gamma,
             laplacian=laplacian,
-            markedSearch=markedSearch)
+            markedElements=markedElements)
         self._initState = State(
             self._n,
             nodeList=initStateList,
             customStateList=customStateList)
         self._quantumWalk = QuantumWalk(self._initState, self._operator)
-
         self._probDist = ProbabilityDistribution(
             self._quantumWalk.getFinalState())
-
         self._probDistList = []
 
-    def to_json(self, isDynamic=False) -> str:
-        """Returns a JSON representation of the QWAK instance
-
-        Parameters
-        ----------
-        isDynamic : bool, optional
-            If True, the JSON will contain the timeList, probDistList and
-            walkList attributes, by default False.
 
-        Returns
-        -------
-        str
-            JSON representation of the QWAK instance.
-        """
-        if isDynamic:
-            qwakJson = json.dumps({
-                'dim': self._n,
-                'graph': nx.node_link_data(self._graph),
-                'timeList': self._timeList.tolist(),
-                'initState': json.loads(self._initState.to_json()),
-                'operator': json.loads(self._operator.to_json()),
-                'quantumWalk': json.loads(self._quantumWalk.to_json()),
-                'probDistList': [probDist.to_json() for probDist in self._probDistList],
-                'qwakId': self._qwakId
-            })
-        else:
-            qwakJson = json.dumps({
-                'dim': self._n,
-                'graph': nx.node_link_data(self._graph),
-                'initState': json.loads(self._initState.to_json()),
-                'operator': json.loads(self._operator.to_json()),
-                'quantumWalk': json.loads(self._quantumWalk.to_json()),
-                'probDist': json.loads(self._probDist.to_json()),
-                'qwakId': self._qwakId
-            })
-        return qwakJson
-
-    @classmethod
-    def from_json(cls, json_var: str, isDynamic=False) -> QWAK:
-        """Returns a QWAK instance from a JSON representation.
+    def runWalk(
+            self,
+            time: float = 0,
+            initStateList: list = None,
+            customStateList: list = None) -> None:
+        """Builds class' attributes, runs the walk and calculates the amplitudes
+        and probability distributions with the given parameters. These can be
+        accessed with their respective get methods.
 
         Parameters
         ----------
-        json_var : str
-            JSON representation of the QWAK instance.
-        isDynamic : bool, optional
-            If True, the JSON will contain the timeList and probDistList attributes,
-            by default False.
-
-        Returns
-        -------
-        QWAK
-            QWAK instance from a JSON representation.
-        """
-        if isinstance(json_var, str):
-            data = json.loads(json_var)
-        elif isinstance(json_var, dict):
-            data = json_var
-        qwakId = data['qwakId']
-        graph = nx.node_link_graph(data['graph'])
-
-        initState = State.from_json(data['initState'])
-        operator = Operator.from_json(data['operator'])
-        quantumWalk = QuantumWalk.from_json(data['quantumWalk'])
-        if isDynamic:
-            timeList = data['timeList']
-            newQwak = cls(graph=graph, timeList=timeList, qwakId=qwakId)
-            probDistList = [ProbabilityDistribution.from_json(
-                probDist) for probDist in data['probDistList']]
-            newQwak.setProbDistList(probDistList)
-        else:
-            probDist = ProbabilityDistribution.from_json(
-                data['probDist'])
-            newQwak = cls(graph=graph, qwakId=qwakId)
-            newQwak.setProbDist(probDist)
-        newQwak.setInitState(initState)
-        newQwak.setOperator(operator)
-        newQwak.setWalk(quantumWalk)
-        return newQwak
-
-    def setQWAK(self, newQWAK: QWAK) -> None:
-        """Sets the QWAK instance's attributes to the ones of the given QWAK instance.
+        time : float, optional
+            Time for which to calculate the quantum walk, by default 0.
+        initStateList : list[int], optional
+            List with chosen initial states for uniform superposition, by default None.
+        customStateList : list[(int,complex)], optional
+            Custom init state, by default None.
 
-        Parameters
-        ----------
-        newQWAK : QWAK
-            QWAK instance to copy the attributes from.
+        Raises
+        ------
+        stOBErr
+            State out of bounds exception.
+        nUErr
+            State not unitary exception.
         """
-        self.setGraph(newQWAK.getGraph())
-        self.setDim(newQWAK.getDim(), graph=self._graph)
-        self.setInitState(newQWAK.getInitState())
-        self.setOperator(newQWAK.getOperator())
-        self.setWalk(newQWAK.getWalk())
-        self.setProbDist(newQWAK.getProbDist())
+        try:
+            self._initState.buildState(
+                nodeList=initStateList, customStateList=customStateList
+            )
+        except StateOutOfBounds as stOBErr:
+            raise stOBErr
+        except NonUnitaryState as nUErr:
+            raise nUErr
+        self._operator.buildDiagonalOperator(time=time)
+        self._quantumWalk.buildWalk(self._initState, self._operator)
+        self._probDist.buildProbDist(self._quantumWalk.getFinalState())
 
-    def runWalk(
+    def runExpmWalk(
             self,
-            time: float = None,
+            time: float = 0,
             initStateList: list = None,
             customStateList: list = None) -> None:
         """Builds class' attributes, runs the walk and calculates the amplitudes
         and probability distributions with the given parameters. These can be
         accessed with their respective get methods.
 
         Parameters
@@ -216,16 +159,15 @@
             self._initState.buildState(
                 nodeList=initStateList, customStateList=customStateList
             )
         except StateOutOfBounds as stOBErr:
             raise stOBErr
         except NonUnitaryState as nUErr:
             raise nUErr
-
-        self._operator.buildDiagonalOperator(time=time)
+        self._operator.buildExpmOperator(time=time)
         self._quantumWalk.buildWalk(self._initState, self._operator)
         self._probDist.buildProbDist(self._quantumWalk.getFinalState())
 
     def runMultipleWalks(
             self,
             timeList: list = None,
             initStateList: list = None,
@@ -255,14 +197,48 @@
         for time in self._timeList:
             self.runWalk(
                 time=time,
                 initStateList=initStateList,
                 customStateList=customStateList)
             self._probDistList.append(copy.deepcopy(self.getProbDist()))
 
+    def runMultipleExpmWalks(
+            self,
+            timeList: list = None,
+            initStateList: list = None,
+            customStateList: list = None) -> None:
+        """Runs the walk for multiple times and stores the probability distributions
+        in a list.
+
+        Parameters
+        ----------
+        timeList : list, optional
+            List of times for which to calculate the quantum walk, by default None.
+        initStateList : list, optional
+            List with chosen initial states for uniform superposition, by default None.
+        customStateList : list, optional
+            Custom init state, by default None.
+
+        Raises
+        ------
+        UndefinedTimeList
+            Raised when the timeList is None.
+        """
+        self._probDistList = []
+        if timeList is not None:
+            self._timeList = timeList
+        elif self._timeList is None:
+            raise UndefinedTimeList(f"TimeList is {self._timeList}.")
+        for time in self._timeList:
+            self.runExpmWalk(
+                time=time,
+                initStateList=initStateList,
+                customStateList=customStateList)
+            self._probDistList.append(copy.deepcopy(self.getProbDist()))
+
     def resetWalk(self) -> None:
         """Resets the components of a walk."""
         self._initState.resetState()
         self._operator.resetOperator()
         self._quantumWalk.resetWalk()
         self._probDist.resetProbDist()
         self._probDistList = []
@@ -394,15 +370,15 @@
         ----------
         newTimeList : list
             New time list.
         """
         timeList = np.linspace(
             newTimeList[0], newTimeList[1], int(
                 newTimeList[1]))
-        self._timeList = timeList
+        self._timeList = timeList.tolist()
 
     def getTime(self) -> float:
         """Gets the current walk time.
 
         Returns
         -------
         float
@@ -444,14 +420,34 @@
 
         Returns:
             np.ndarray:
                 Current adjacency matrix.
         """
         return self._operator.getAdjacencyMatrix()
 
+    def setHamiltonian(self, newHamiltonian: np.ndarray) -> None:
+        """Sets the current Hamiltonian to a user defined one.
+
+        Parameters
+        ----------
+        newHamiltonian : np.ndarray
+            New Hamiltonian.
+        """
+        self._operator.setHamiltonian(newHamiltonian)
+
+    def getHamiltonian(self) -> np.ndarray:
+        """Gets the current Hamiltonian.
+
+        Returns
+        -------
+        np.ndarray
+            Current Hamiltonian.
+        """
+        return self._operator.getHamiltonian()
+
     def setOperator(self, newOperator: Operator) -> None:
         """Sets the current walk operator a user defined one.
 
         Parameters
         ----------
         newOperator : Operator
             New operator object.
@@ -614,15 +610,15 @@
 
         Returns
         -------
         float
             Mean of the probability distribution.
         """
         return self._probDist.moment(1) if (
-            resultRounding is None) \
+                resultRounding is None) \
             else round(self._probDist.moment(1), resultRounding)
 
     def getMeanList(self, resultRounding: int = None) -> list:
         """Gets the mean of the probability distribution list.
 
         Parameters
         ----------
@@ -632,15 +628,15 @@
         Returns
         -------
         list
             List of means of the probability distributions.
         """
         return [
             probDist.moment(1) for probDist in self._probDistList] if (
-            resultRounding is None) \
+                resultRounding is None) \
             else [
             round(
                 probDist.moment(1),
                 resultRounding) for probDist in self._probDistList]
 
     def getSndMoment(self, resultRounding: int = None) -> float:
         """Gets the second moment of the probability distribution.
@@ -688,15 +684,15 @@
         Returns
         -------
         list
             List of standard deviations of the probability distributions.
         """
         return [
             probDist.stDev() for probDist in self._probDistList] if (
-            resultRounding is None) \
+                resultRounding is None) \
             else [
             round(
                 probDist.stDev(),
                 resultRounding) for probDist in self._probDistList]
 
     def getInversePartRatio(self, resultRounding: int = None) -> float:
         """Gets the inverse participation ratio of the probability distribution.
@@ -708,15 +704,15 @@
 
         Returns
         -------
         float
             Inverse participation ratio of the probability distribution.
         """
         return self._probDist.invPartRatio() if (
-            resultRounding is None) \
+                resultRounding is None) \
             else round(
             self._probDist.invPartRatio(), resultRounding)
 
     def getInversePartRatioList(
             self, resultRounding: int = None) -> list:
         """Gets the inverse participation ratio of the probability distribution list.
 
@@ -728,15 +724,15 @@
         Returns
         -------
         list
             List of inverse participation ratios of the probability distributions.
         """
         return [
             probDist.invPartRatio() for probDist in self._probDistList] if (
-            resultRounding is None) else [
+                resultRounding is None) else [
             round(
                 probDist.invPartRatio(),
                 resultRounding) for probDist in self._probDistList]
 
     def getSurvivalProb(
             self,
             fromNode,
@@ -763,15 +759,15 @@
         MissingNodeInput
             Missing input node error.
         """
         try:
             return self._probDist.survivalProb(
                 fromNode,
                 toNode) if (
-                resultRounding is None) else round(
+                    resultRounding is None) else round(
                 self._probDist.survivalProb(
                     fromNode,
                     toNode),
                 resultRounding)
         except MissingNodeInput as err:
             raise err
 
@@ -802,24 +798,24 @@
             Missing input node error.
         """
         try:
             return [
                 probDist.survivalProb(
                     fromNode,
                     toNode) for probDist in self._probDistList] if (
-                resultRounding is None) else [
+                    resultRounding is None) else [
                 round(
                     probDist.survivalProb(
                         fromNode,
                         toNode),
                     resultRounding) for probDist in self._probDistList]
         except MissingNodeInput as err:
             raise err
 
-    def checkPST(self, fromNode, toNode) -> Union([str, bool]):
+    def checkPST(self, fromNode, toNode) -> Union[str, bool]:
         """Checks if a structure allows for PST between certain nodes.
 
         Parameters
         ----------
         fromNode : _type_
             Starting node.
         toNode : _type_
@@ -844,8 +840,133 @@
         """Gets the transport efficiency of the quantum walk.
 
         Returns
         -------
         float
             Transport efficiency of the quantum walk.
         """
-        return self._quantumWalk.transportEfficiency()
+        return self._quantumWalk.transportEfficiency()
+
+    def getMarkedElements(self) -> list:
+        """Gets the marked elements of the quantum walk.
+
+        Returns
+        -------
+        list
+            Marked elements of the quantum walk.
+        """
+        return self._operator.getMarkedElements()
+
+    def setMarkedElements(self, markedElements: list) -> None:
+        """Sets the marked elements of the quantum walk.
+
+        Parameters
+        ----------
+        markedElements : list
+            Marked elements of the quantum walk.
+        """
+        self._operator.setMarkedElements(markedElements)
+
+    def getQWAK(self) :
+        """Gets the QWAK instance.
+
+        Returns
+        -------
+        QWAK
+            QWAK instance.
+        """
+        return self._qwak
+
+    def setQWAK(self, newQWAK: QWAK) -> None:
+        """Sets the QWAK instance's attributes to the ones of the given QWAK instance.
+
+        Parameters
+        ----------
+        newQWAK : QWAK
+            QWAK instance to copy the attributes from.
+        """
+        self.setGraph(newQWAK.getGraph())
+        self.setDim(newQWAK.getDim(), graph=self._graph)
+        self.setInitState(newQWAK.getInitState())
+        self.setOperator(newQWAK.getOperator())
+        self.setWalk(newQWAK.getWalk())
+        self.setProbDist(newQWAK.getProbDist())
+
+    def to_json(self, isDynamic=False) -> str:
+        """Returns a JSON representation of the QWAK instance
+
+        Parameters
+        ----------
+        isDynamic : bool, optional
+            If True, the JSON will contain the timeList, probDistList and
+            walkList attributes, by default False.
+
+        Returns
+        -------
+        str
+            JSON representation of the QWAK instance.
+        """
+        if isDynamic:
+            qwakJson = json.dumps({
+                'dim': self._n,
+                'graph': nx.node_link_data(self._graph),
+                'timeList': self._timeList,
+                'initState': json.loads(self._initState.to_json()),
+                'operator': json.loads(self._operator.to_json()),
+                'quantumWalk': json.loads(self._quantumWalk.to_json()),
+                'probDistList': [probDist.to_json() for probDist in self._probDistList],
+                'qwakId': self._qwakId
+            })
+        else:
+            qwakJson = json.dumps({
+                'dim': self._n,
+                'graph': nx.node_link_data(self._graph),
+                'initState': json.loads(self._initState.to_json()),
+                'operator': json.loads(self._operator.to_json()),
+                'quantumWalk': json.loads(self._quantumWalk.to_json()),
+                'probDist': json.loads(self._probDist.to_json()),
+                'qwakId': self._qwakId
+            })
+        return qwakJson
+
+    @classmethod
+    def from_json(cls, json_var: str, isDynamic=False) -> QWAK:
+        """Returns a QWAK instance from a JSON representation.
+
+        Parameters
+        ----------
+        json_var : str
+            JSON representation of the QWAK instance.
+        isDynamic : bool, optional
+            If True, the JSON will contain the timeList and probDistList attributes,
+            by default False.
+
+        Returns
+        -------
+        QWAK
+            QWAK instance from a JSON representation.
+        """
+        if isinstance(json_var, str):
+            data = json.loads(json_var)
+        elif isinstance(json_var, dict):
+            data = json_var
+        qwakId = data['qwakId']
+        graph = nx.node_link_graph(data['graph'])
+
+        initState = State.from_json(data['initState'])
+        operator = Operator.from_json(data['operator'])
+        quantumWalk = QuantumWalk.from_json(data['quantumWalk'])
+        if isDynamic:
+            timeList = data['timeList']
+            newQwak = cls(graph=graph, timeList=timeList, qwakId=qwakId)
+            probDistList = [ProbabilityDistribution.from_json(
+                probDist) for probDist in data['probDistList']]
+            newQwak.setProbDistList(probDistList)
+        else:
+            probDist = ProbabilityDistribution.from_json(
+                data['probDist'])
+            newQwak = cls(graph=graph, qwakId=qwakId)
+            newQwak.setProbDist(probDist)
+        newQwak.setInitState(initState)
+        newQwak.setOperator(operator)
+        newQwak.setWalk(quantumWalk)
+        return newQwak
```

### Comparing `qwak-sim-2023.1012a0/core/qwak_sim.egg-info/PKG-INFO` & `qwak-sim-2023.1013a0/core/qwak_sim.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qwak-sim
-Version: 2023.1012a0
+Version: 2023.1013a0
 Summary: Simulate Continuous-Time Quantum Walks
 Home-page: https://github.com/qwchagas/qwak
 Author: Jaime Santos
 Author-email: Jaime Santos <jaimepereirasantos123@gmail.com>, Bruno Chagas <na@na.na>, Rodrigo Chaves <na@na.na>, Lorenzo Buffoni <na@na.na>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
```

### Comparing `qwak-sim-2023.1012a0/core/qwak_sim.egg-info/SOURCES.txt` & `qwak-sim-2023.1013a0/core/qwak_sim.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -17,8 +17,14 @@
 core/qwak_sim.egg-info/PKG-INFO
 core/qwak_sim.egg-info/SOURCES.txt
 core/qwak_sim.egg-info/dependency_links.txt
 core/qwak_sim.egg-info/requires.txt
 core/qwak_sim.egg-info/top_level.txt
 core/utils/PerfectStateTransfer.py
 core/utils/__init__.py
-core/utils/jsonMethods.py
+core/utils/jsonTools.py
+core/utils/plotTools.py
+tests/test_GraphicalQwakCycle.py
+tests/test_QwakComplete.py
+tests/test_QwakCycle.py
+tests/test_QwakPath.py
+tests/test_StochasticQwak.py
```

### Comparing `qwak-sim-2023.1012a0/core/utils/PerfectStateTransfer.py` & `qwak-sim-2023.1013a0/core/utils/PerfectStateTransfer.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1012a0/core/utils/jsonMethods.py` & `qwak-sim-2023.1013a0/core/utils/jsonTools.py`

 * *Files identical despite different names*

### Comparing `qwak-sim-2023.1012a0/pyproject.toml` & `qwak-sim-2023.1013a0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     "setuptools>=54",
     "wheel",
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qwak-sim"
-version = "2023.1012-alpha"
+version = "2023.1013-alpha"
 description = "Simulate Continuous-Time Quantum Walks"
 readme = "README.md"
 authors = [{ name = "Jaime Santos", email = "jaimepereirasantos123@gmail.com" },
             { name = "Bruno Chagas", email = "na@na.na" },
             { name = "Rodrigo Chaves", email = "na@na.na" },
             { name = "Lorenzo Buffoni", email = "na@na.na" }]
 license = { file = "LICENSE" }
@@ -38,15 +38,15 @@
 
 [tool.setuptools.packages.find]
 where = ["core"]
 include = ["qwak","utils"]  # alternatively: `exclude = ["additional*"]`
 namespaces = false
 
 [tool.bumpver]
-current_version = "2023.1012-alpha"
+current_version = "2023.1013-alpha"
 version_pattern = "YYYY.BUILD[-TAG]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `qwak-sim-2023.1012a0/setup.cfg` & `qwak-sim-2023.1013a0/setup.cfg`

 * *Files identical despite different names*

