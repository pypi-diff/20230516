# Comparing `tmp/modelfree-protein15n-0.0.1.tar.gz` & `tmp/modelfree-protein15n-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelfree-protein15n-0.0.1.tar", last modified: Mon May 15 19:54:22 2023, max compression
+gzip compressed data, was "modelfree-protein15n-0.0.2.tar", last modified: Tue May 16 15:00:32 2023, max compression
```

## Comparing `modelfree-protein15n-0.0.1.tar` & `modelfree-protein15n-0.0.2.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-15 19:54:22.970019 modelfree-protein15n-0.0.1/
--rwxrwxrwx   0 vschnapka  (1000) vschnapka  (1000)     1066 2023-05-15 19:11:49.000000 modelfree-protein15n-0.0.1/LICENSE
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       15 2023-05-11 20:55:09.000000 modelfree-protein15n-0.0.1/MANIFEST.in
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3612 2023-05-15 19:54:22.970019 modelfree-protein15n-0.0.1/PKG-INFO
--rwxrwxrwx   0 vschnapka  (1000) vschnapka  (1000)     2647 2023-05-15 19:50:51.000000 modelfree-protein15n-0.0.1/README.md
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-15 19:54:22.946693 modelfree-protein15n-0.0.1/modelfree_protein15n.egg-info/
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3612 2023-05-15 19:54:22.000000 modelfree-protein15n-0.0.1/modelfree_protein15n.egg-info/PKG-INFO
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      573 2023-05-15 19:54:22.000000 modelfree-protein15n-0.0.1/modelfree_protein15n.egg-info/SOURCES.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        1 2023-05-15 19:54:22.000000 modelfree-protein15n-0.0.1/modelfree_protein15n.egg-info/dependency_links.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       50 2023-05-15 19:54:22.000000 modelfree-protein15n-0.0.1/modelfree_protein15n.egg-info/entry_points.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       40 2023-05-15 19:54:22.000000 modelfree-protein15n-0.0.1/modelfree_protein15n.egg-info/requires.txt
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        8 2023-05-15 19:54:22.000000 modelfree-protein15n-0.0.1/modelfree_protein15n.egg-info/top_level.txt
-drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-15 19:54:22.970019 modelfree-protein15n-0.0.1/modfree/
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-11 00:43:37.000000 modelfree-protein15n-0.0.1/modfree/__init__.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       71 2023-05-11 15:55:03.000000 modelfree-protein15n-0.0.1/modfree/__main__.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1736 2023-05-11 15:53:38.000000 modelfree-protein15n-0.0.1/modfree/analysis.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      719 2023-05-12 18:30:51.000000 modelfree-protein15n-0.0.1/modfree/constants_functions.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     8708 2023-05-11 00:51:38.000000 modelfree-protein15n-0.0.1/modfree/data_format.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5331 2023-05-11 15:54:43.000000 modelfree-protein15n-0.0.1/modfree/generator.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2327 2023-05-11 00:52:50.000000 modelfree-protein15n-0.0.1/modfree/inputs.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)    14304 2023-05-11 15:54:44.000000 modelfree-protein15n-0.0.1/modfree/mf_standard.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5842 2023-05-11 20:19:46.000000 modelfree-protein15n-0.0.1/modfree/modfree.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3667 2023-05-11 15:54:46.000000 modelfree-protein15n-0.0.1/modfree/outputs.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2481 2023-05-11 15:54:47.000000 modelfree-protein15n-0.0.1/modfree/parser.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5079 2023-05-11 15:54:48.000000 modelfree-protein15n-0.0.1/modfree/ploter.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2912 2023-05-11 15:54:41.000000 modelfree-protein15n-0.0.1/modfree/run_fit.py
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       38 2023-05-15 19:54:22.979878 modelfree-protein15n-0.0.1/setup.cfg
--rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1075 2023-05-15 19:46:18.000000 modelfree-protein15n-0.0.1/setup.py
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-16 15:00:32.112038 modelfree-protein15n-0.0.2/
+-rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     1066 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/LICENSE
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       15 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/MANIFEST.in
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3586 2023-05-16 15:00:32.111029 modelfree-protein15n-0.0.2/PKG-INFO
+-rwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)     2621 2023-05-15 21:35:59.000000 modelfree-protein15n-0.0.2/README.md
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-16 15:00:32.081463 modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3586 2023-05-16 15:00:31.000000 modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/PKG-INFO
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      573 2023-05-16 15:00:31.000000 modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/SOURCES.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        1 2023-05-16 15:00:31.000000 modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/dependency_links.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       50 2023-05-16 15:00:31.000000 modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/entry_points.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       40 2023-05-16 15:00:31.000000 modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/requires.txt
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        8 2023-05-16 15:00:31.000000 modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/top_level.txt
+drwxr-xr-x   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-16 15:00:32.108854 modelfree-protein15n-0.0.2/modfree/
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)        0 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/__init__.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       71 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/__main__.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1736 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/analysis.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)      719 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/constants_functions.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     8708 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/data_format.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     6461 2023-05-16 14:24:26.000000 modelfree-protein15n-0.0.2/modfree/generator.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2327 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/inputs.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)    14130 2023-05-16 14:28:18.000000 modelfree-protein15n-0.0.2/modfree/mf_standard.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5842 2023-05-16 14:21:36.000000 modelfree-protein15n-0.0.2/modfree/modfree.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     3667 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/outputs.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2481 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/parser.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     5079 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/ploter.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     2912 2023-05-15 21:32:37.000000 modelfree-protein15n-0.0.2/modfree/run_fit.py
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)       38 2023-05-16 15:00:32.112741 modelfree-protein15n-0.0.2/setup.cfg
+-rw-r--r--   0 vschnapka  (1000) vschnapka  (1000)     1075 2023-05-16 14:16:51.000000 modelfree-protein15n-0.0.2/setup.py
```

### Comparing `modelfree-protein15n-0.0.1/LICENSE` & `modelfree-protein15n-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.1/PKG-INFO` & `modelfree-protein15n-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.1
 Name: modelfree-protein15n
-Version: 0.0.1
+Version: 0.0.2
 Summary: Model free analysis of protein backbone amide 15N spin relaxation rates.
 Home-page: https://github.com/VSchnapka/modelfree-protein15n.git
 Author: Vincent Schnapka
 Author-email: vincentschnapka@gmail.com
 License: UNKNOWN
 Description: # modelfree-protein15n
         Simple flexible model free analysis framework for protein backbone amide 15N NMR spin relaxation rates
         
-        The tool is flexible enough to allow spin relaxation data fitting with a chosen number of dynamic modes and the fixing of given variables.
+        This tools allows spin relaxation data fitting with a chosen number of dynamic modes. any variable can be fixed.
         Typically, one can perform 1, 2, and 3 dynamic mode MF analysis and see which model is most relevant for the data.
         IMPACT analysis is also possible.
         
         ## Relevant litterature
         
         Lipari & Szabo, Journal of the American Chemical Society (1982);
         Halle, The Journal of chemical physics (2009);
```

### Comparing `modelfree-protein15n-0.0.1/README.md` & `modelfree-protein15n-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # modelfree-protein15n
 Simple flexible model free analysis framework for protein backbone amide 15N NMR spin relaxation rates
 
-The tool is flexible enough to allow spin relaxation data fitting with a chosen number of dynamic modes and the fixing of given variables.
+This tools allows spin relaxation data fitting with a chosen number of dynamic modes. any variable can be fixed.
 Typically, one can perform 1, 2, and 3 dynamic mode MF analysis and see which model is most relevant for the data.
 IMPACT analysis is also possible.
 
 ## Relevant litterature
 
 Lipari & Szabo, Journal of the American Chemical Society (1982);
 Halle, The Journal of chemical physics (2009);
```

### Comparing `modelfree-protein15n-0.0.1/modelfree_protein15n.egg-info/PKG-INFO` & `modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 1.1
 Name: modelfree-protein15n
-Version: 0.0.1
+Version: 0.0.2
 Summary: Model free analysis of protein backbone amide 15N spin relaxation rates.
 Home-page: https://github.com/VSchnapka/modelfree-protein15n.git
 Author: Vincent Schnapka
 Author-email: vincentschnapka@gmail.com
 License: UNKNOWN
 Description: # modelfree-protein15n
         Simple flexible model free analysis framework for protein backbone amide 15N NMR spin relaxation rates
         
-        The tool is flexible enough to allow spin relaxation data fitting with a chosen number of dynamic modes and the fixing of given variables.
+        This tools allows spin relaxation data fitting with a chosen number of dynamic modes. any variable can be fixed.
         Typically, one can perform 1, 2, and 3 dynamic mode MF analysis and see which model is most relevant for the data.
         IMPACT analysis is also possible.
         
         ## Relevant litterature
         
         Lipari & Szabo, Journal of the American Chemical Society (1982);
         Halle, The Journal of chemical physics (2009);
```

### Comparing `modelfree-protein15n-0.0.1/modelfree_protein15n.egg-info/SOURCES.txt` & `modelfree-protein15n-0.0.2/modelfree_protein15n.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.1/modfree/analysis.py` & `modelfree-protein15n-0.0.2/modfree/analysis.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.1/modfree/constants_functions.py` & `modelfree-protein15n-0.0.2/modfree/constants_functions.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.1/modfree/data_format.py` & `modelfree-protein15n-0.0.2/modfree/data_format.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.1/modfree/generator.py` & `modelfree-protein15n-0.0.2/modfree/generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,14 +24,40 @@
         idx, dat = 0, 1000
         while (dat > 1-amp1[i] or dat < 0) and idx < 10000:
             dat = rd.gauss(output[i-1], 0.1)
         output.append(dat)
     return np.array(output)
 
 
+def random_amps(length, nb, sigma=0.1):
+    outputs = [rd.uniform(0, 1) for i in range(nb)]
+    outputs = [[el/np.sum(outputs)] for el in outputs]
+    for j in range(1, length):
+        dats = [-1000 for el in outputs]
+        for i, el in enumerate(outputs):
+            while dats[i] < 0:
+                dats[i] = rd.gauss(outputs[i][j-1], sigma)
+        dats = [el/np.sum(dats) for el in dats]
+        for i, el in enumerate(outputs):
+            outputs[i].append(dats[i])
+    return outputs
+
+
+def random_taus(length, nb, sigma_scale=0.1):
+    timescales = np.logspace(-11, -7.8, nb)
+    outputs = [[rd.uniform(el-sigma_scale*el, el+sigma_scale*el)] for el in timescales]
+    for j in range(1, length):
+        dats = [-1000 for el in outputs]
+        for i, el in enumerate(outputs):
+            while dats[i] < 0 or dats[i] > 50*sigma_scale*timescales[i] or dats[i] < 0.35*sigma_scale*timescales[i]:
+                dats[i] = rd.gauss(outputs[i][j-1], sigma_scale*timescales[i])
+            outputs[i].append(dats[i])
+    return outputs
+
+
 def random_tau_50ps(length):
     output = [rd.gauss(50e-12, 5e-12)]
     for i in range(1, length):
         idx, dat = 0, 1000
         while (dat > 100e-12 or dat < 10e-12) and idx < 10000:
             dat = rd.gauss(50e-12, 5e-12)
         output.append(dat)
@@ -93,14 +119,17 @@
         f.write(f"mf_minimization_iterations = 3\n")
         f.write(f"monte_carlo_iterations = 50\n")
         f.write(f"monte_carlo_minimization_iterations = 3\n")
     return None
 
 
 def generate(N, output_dir, fields=(400, 600, 800, 1000, 1200), rates=('R1', 'R2', 'nOe', 'etaXY'), modes=2, noise_proportion=0.01):
+    if type(modes) is not int:
+        print("the number of dynamic modes must be an int")
+        modes = int(modes)
     RES = np.arange(1, N+1)
     print("Parameter generation...")
     if modes == 1:
         amps = [1]
         taus = [random_tau_100ps(N)]
     elif modes == 2:
         a1 = random_amp1(N)
@@ -108,16 +137,16 @@
         taus = [random_tau_100ps(N), random_tumb_ns(N)]
     elif modes == 3:
         a1 = random_amp1(N)
         a2 = random_amp2(N, a1)
         amps = [a1, a2, 1-a1-a2]
         taus = [random_tau_50ps(N), random_tau_100ps(N), random_tau_ns(N)]
     else:
-        print("so far, only random data from 1, 2 or 3 dynamic modes can be generated")
-        return None
+        amps = random_amps(N, modes)
+        taus = random_taus(N, modes)
     if not os.path.isdir(output_dir):
         os.mkdir(output_dir)
     RATES, ERROR = dict(), dict()
     print("Data calculation...")
     for i, r in enumerate(RES):
         params = give_params([el[i] for el in amps], [el[i] for el in taus])
         if noise_proportion == 0:
```

### Comparing `modelfree-protein15n-0.0.1/modfree/inputs.py` & `modelfree-protein15n-0.0.2/modfree/inputs.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.1/modfree/mf_standard.py` & `modelfree-protein15n-0.0.2/modfree/mf_standard.py`

 * *Files 2% similar despite different names*

```diff
@@ -128,22 +128,18 @@
         return params
 
     amps = []
     if 'Rex' in fix.keys():
         params.add('Rex', value=fix['Rex'], min=0, max=50, vary=False)
     else:
         params.add('Rex', value=0, min=0, max=50, vary=exchange)
+    amps = [rd.uniform(0, 1) for i in range(modes)]
+    amps = [el/np.sum(amps) for el in amps]
     for i in range(modes):
-        term = sum(amps) if amps else 0
-        if i == modes-1:
-            #params.add('amp'+str(i+1), expr='1'+minus_amps(len(amps)), min=0, max=1, vary=vary_amps) # makes a mess
-            pass
-        else:
-            amps.append((1-term)*rd.uniform(0, 0.6))
-            params.add('amp'+str(i+1), value=amps[i], min=0, max=1, vary=vary_amps)
+        params.add('amp'+str(i+1), value=amps[i], min=0, max=1, vary=vary_amps)
         if 'tau'+str(i+1) in fix.keys():
             params.add('tau'+str(i+1), value=fix['tau'+str(i+1)], min=1e-12, max=5e-7, vary=False)
         else:
             params.add('tau'+str(i+1), value=(10**i)*rd.uniform(1, 9)*1e-11, min=1e-12, max=5e-7, vary=vary_taus)
     return params
```

### Comparing `modelfree-protein15n-0.0.1/modfree/modfree.py` & `modelfree-protein15n-0.0.2/modfree/modfree.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import modfree.inputs as inputs
 import modfree.outputs as outputs
 import modfree.run_fit as run_fit
 import modfree.ploter as ploter
 import modfree.generator as generator
 
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 
 
 console = Console()
 
 
 header = "\n".join(
 [
```

### Comparing `modelfree-protein15n-0.0.1/modfree/outputs.py` & `modelfree-protein15n-0.0.2/modfree/outputs.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.1/modfree/parser.py` & `modelfree-protein15n-0.0.2/modfree/parser.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.1/modfree/ploter.py` & `modelfree-protein15n-0.0.2/modfree/ploter.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.1/modfree/run_fit.py` & `modelfree-protein15n-0.0.2/modfree/run_fit.py`

 * *Files identical despite different names*

### Comparing `modelfree-protein15n-0.0.1/setup.py` & `modelfree-protein15n-0.0.2/setup.py`

 * *Files identical despite different names*

