# Comparing `tmp/finite_difference-0.0.2.tar.gz` & `tmp/finite_difference-0.0.3.tar.gz`

## Comparing `finite_difference-0.0.2.tar` & `finite_difference-0.0.3.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 finite_difference-0.0.2/.gitattributes
--rw-r--r--   0        0        0    42768 2020-02-02 00:00:00.000000 finite_difference-0.0.2/src/finite_difference/FD.py
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 finite_difference-0.0.2/src/finite_difference/__init__.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 finite_difference-0.0.2/src/finite_difference/progress.txt
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 finite_difference-0.0.2/LICENSE
--rw-r--r--   0        0        0     2811 2020-02-02 00:00:00.000000 finite_difference-0.0.2/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 finite_difference-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3286 2020-02-02 00:00:00.000000 finite_difference-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 finite_difference-0.0.3/.gitattributes
+-rw-r--r--   0        0        0    42769 2020-02-02 00:00:00.000000 finite_difference-0.0.3/src/finite_difference/FD.py
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 finite_difference-0.0.3/src/finite_difference/__init__.py
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 finite_difference-0.0.3/src/finite_difference/progress.txt
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 finite_difference-0.0.3/src/finite_difference/test.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 finite_difference-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 finite_difference-0.0.3/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 finite_difference-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3288 2020-02-02 00:00:00.000000 finite_difference-0.0.3/PKG-INFO
```

### Comparing `finite_difference-0.0.2/src/finite_difference/FD.py` & `finite_difference-0.0.3/src/finite_difference/FD.py`

 * *Files 0% similar despite different names*

```diff
@@ -1048,15 +1048,15 @@
         if periodic:
             # for edge and periodic, it's just gonna be one less length, so can just roll now :) no removing and/or copying required
 
             # for the periodic case, number edges=number of cells
             derivative = np.zeros(f.data.shape)
 
             for i in range(len(shifts)):
-                derivative += weights[i] * np.roll(f.data, shifts[i], axis=axis_n)
+                derivative += weights[i] * np.roll(f.data, -shifts[i], axis=axis_n)
 
         # not periodic case:
         else:
 
             # shape only changes if it's not periodic
             fprime_shape = list(f.data.shape)
             fprime_shape[axis_n] += shape_shift
```

### Comparing `finite_difference-0.0.2/src/finite_difference/progress.txt` & `finite_difference-0.0.3/src/finite_difference/progress.txt`

 * *Files identical despite different names*

### Comparing `finite_difference-0.0.2/LICENSE` & `finite_difference-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `finite_difference-0.0.2/README.md` & `finite_difference-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 T = fd.Field(m, "Temperature", n_time_ders = 1)
 ```
 
 3. Create stencils for numerical approximations of spatial derivatives.
 
 ```python
 
-diff_2 = fd.Stencil([-1,0,1],der_order=2)
+diff_2 = fd.Stencil([-1,0,1], der_order = 2)
 ```
 
 
 4. Apply boundary conditions and initial conditions.
 
 ```python
 
@@ -58,17 +58,17 @@
 
 5. Run the simulation in a loop, updating the fields each iteration.
 
 ```python
 
 k = 2 # thermal conductivity
 
-m.check_IC() # not required, but recommended: check's if all necessary initial conditions have been set up
+m.check_IC() # not required, but recommended: checks if all necessary initial conditions have been set up
 
-while not m.finished: # checks if it his reached the final timestep
+while not m.finished: # checks if it has reached the final timestep
 
     # implements the equations: dT/dt = k * d^2T/dx^2
     Tp = k*diff_2.der(T.prev)
     T.dot.assign_update(Tp)
     T.time_integrate_update()
 
     m.increment_time() # increment the time step
```

### Comparing `finite_difference-0.0.2/pyproject.toml` & `finite_difference-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 [project]
 name = "finite_difference"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Ephraim Bryski", email="ebryski1@gmail.com"},
 ]
 description = "Library for setting up finite difference problems"
 readme = "README.md"
 requires-python = ">=3"
 classifiers = [
```

### Comparing `finite_difference-0.0.2/PKG-INFO` & `finite_difference-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finite_difference
-Version: 0.0.2
+Version: 0.0.3
 Summary: Library for setting up finite difference problems
 Project-URL: Homepage, https://github.com/Ephraim-Bryski/Finite-Difference
 Project-URL: Bug Tracker, https://github.com/Ephraim-Bryski/Finite-Difference/issues
 Author-email: Ephraim Bryski <ebryski1@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -53,15 +53,15 @@
 T = fd.Field(m, "Temperature", n_time_ders = 1)
 ```
 
 3. Create stencils for numerical approximations of spatial derivatives.
 
 ```python
 
-diff_2 = fd.Stencil([-1,0,1],der_order=2)
+diff_2 = fd.Stencil([-1,0,1], der_order = 2)
 ```
 
 
 4. Apply boundary conditions and initial conditions.
 
 ```python
 
@@ -72,17 +72,17 @@
 
 5. Run the simulation in a loop, updating the fields each iteration.
 
 ```python
 
 k = 2 # thermal conductivity
 
-m.check_IC() # not required, but recommended: check's if all necessary initial conditions have been set up
+m.check_IC() # not required, but recommended: checks if all necessary initial conditions have been set up
 
-while not m.finished: # checks if it his reached the final timestep
+while not m.finished: # checks if it has reached the final timestep
 
     # implements the equations: dT/dt = k * d^2T/dx^2
     Tp = k*diff_2.der(T.prev)
     T.dot.assign_update(Tp)
     T.time_integrate_update()
 
     m.increment_time() # increment the time step
```

