# Comparing `tmp/richvalues-3.1.1.tar.gz` & `tmp/richvalues-3.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "richvalues-3.1.1.tar", last modified: Mon Apr 24 09:09:37 2023, max compression
+gzip compressed data, was "richvalues-3.1.2.tar", last modified: Tue May 16 20:15:35 2023, max compression
```

## Comparing `richvalues-3.1.1.tar` & `richvalues-3.1.2.tar`

### file list

```diff
@@ -1,15 +1,14 @@
-drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2023-04-24 09:09:37.776116 richvalues-3.1.1/
--rw-rw-r--   0 andresmegias   (501) staff       (20)     1532 2023-04-20 22:48:48.000000 richvalues-3.1.1/LICENSE
--rw-r--r--   0 andresmegias   (501) staff       (20)     1319 2023-04-24 09:09:37.775865 richvalues-3.1.1/PKG-INFO
--rw-rw-r--   0 andresmegias   (501) staff       (20)      848 2023-04-24 07:29:24.000000 richvalues-3.1.1/README.md
--rw-rw-r--   0 andresmegias   (501) staff       (20)      671 2023-04-24 09:09:00.000000 richvalues-3.1.1/pyproject.toml
-drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2023-04-24 09:09:37.773193 richvalues-3.1.1/richvalues/
--rw-rw-r--   0 andresmegias   (501) staff       (20)   155180 2023-04-24 09:08:47.000000 richvalues-3.1.1/richvalues/__init__.py
-drwxr-xr-x   0 andresmegias   (501) staff       (20)        0 2023-04-24 09:09:37.775371 richvalues-3.1.1/richvalues.egg-info/
--rw-r--r--   0 andresmegias   (501) staff       (20)     1319 2023-04-24 09:09:37.000000 richvalues-3.1.1/richvalues.egg-info/PKG-INFO
--rw-r--r--   0 andresmegias   (501) staff       (20)      233 2023-04-24 09:09:37.000000 richvalues-3.1.1/richvalues.egg-info/SOURCES.txt
--rw-r--r--   0 andresmegias   (501) staff       (20)        1 2023-04-24 09:09:37.000000 richvalues-3.1.1/richvalues.egg-info/dependency_links.txt
--rw-r--r--   0 andresmegias   (501) staff       (20)       30 2023-04-24 09:09:37.000000 richvalues-3.1.1/richvalues.egg-info/requires.txt
--rw-r--r--   0 andresmegias   (501) staff       (20)       11 2023-04-24 09:09:37.000000 richvalues-3.1.1/richvalues.egg-info/top_level.txt
--rw-r--r--   0 andresmegias   (501) staff       (20)       38 2023-04-24 09:09:37.776203 richvalues-3.1.1/setup.cfg
--rw-rw-r--   0 andresmegias   (501) staff       (20)      748 2023-04-24 09:09:25.000000 richvalues-3.1.1/setup.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-05-16 20:15:34.998761 richvalues-3.1.2/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1391 2023-05-16 20:15:34.998761 richvalues-3.1.2/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      812 2023-04-12 00:09:14.000000 richvalues-3.1.2/README.md
+-rw-rw-r--   0 andres    (1000) andres    (1000)      688 2023-05-16 20:13:51.000000 richvalues-3.1.2/pyproject.toml
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-05-16 20:15:34.998761 richvalues-3.1.2/richvalues/
+-rw-rw-r--   0 andres    (1000) andres    (1000)   155615 2023-05-16 20:12:42.000000 richvalues-3.1.2/richvalues/__init__.py
+drwxrwxr-x   0 andres    (1000) andres    (1000)        0 2023-05-16 20:15:34.998761 richvalues-3.1.2/richvalues.egg-info/
+-rw-rw-r--   0 andres    (1000) andres    (1000)     1391 2023-05-16 20:15:34.000000 richvalues-3.1.2/richvalues.egg-info/PKG-INFO
+-rw-rw-r--   0 andres    (1000) andres    (1000)      225 2023-05-16 20:15:34.000000 richvalues-3.1.2/richvalues.egg-info/SOURCES.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)        1 2023-05-16 20:15:34.000000 richvalues-3.1.2/richvalues.egg-info/dependency_links.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       30 2023-05-16 20:15:34.000000 richvalues-3.1.2/richvalues.egg-info/requires.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       11 2023-05-16 20:15:34.000000 richvalues-3.1.2/richvalues.egg-info/top_level.txt
+-rw-rw-r--   0 andres    (1000) andres    (1000)       38 2023-05-16 20:15:34.998761 richvalues-3.1.2/setup.cfg
+-rw-rw-r--   0 andres    (1000) andres    (1000)      869 2023-05-16 20:14:48.000000 richvalues-3.1.2/setup.py
```

### Comparing `richvalues-3.1.1/README.md` & `richvalues-3.1.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,5 +1,3 @@
-RichValues is a Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. 
+RichValues is a Python 3 library for working with numeric values with uncertainties, upper/lower limits and finite intervals, which may be called _rich values_. With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values.
 
-With it, one can import rich values written in plain text documents in an easily readable format, operate with them propagating the uncertainties automatically, and export them in the same formatting style as the import. It also allows to easily plot rich values and to make fits to any function, taking into account the uncertainties and the upper/limits or finite intervals. Moreover, correlations between variables are taken into account when performing calculations with rich values. 
-
-The libraries NumPy, Pandas, SciPy and Matplotlib are required by RichValues. An user guide and some examples are available in the GitHub repository: https://github.com/andresmegias/richvalues/.
+The libraries NumPy, Pandas, SciPy and Matplotlib are required. An user guide is available on the GitHub repository: https://github.com/andresmegias/richvalues/.
```

### Comparing `richvalues-3.1.1/pyproject.toml` & `richvalues-3.1.2/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "richvalues"
-version = "3.1.1"
+version = "3.1.2"
 description = "Python library for working with uncertainties and upper/lower limits"
 license = {file="LICENSE"}
 authors = [{name="Andrés Megías Toledano"}]
 readme = "README.md"
 dependencies = ["numpy", "pandas", "scipy", "matplotlib"]
-classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: BSD License",
-    "Operating System :: OS Independent"]
-
+classifiers = ["Programming Language :: Python :: 3",
+               "License :: OSI Approved :: BSD License",
+               "Operating System :: OS Independent"]
 [project.urls]
 homepage = "https://github.com/andresmegias/richvalues/"
-documentation = "https://github.com/andresmegias/richvalues/blob/main/userguide.pdf"
+documentation = "https://github.com/andresmegias/richvalues/blob/main/userguide.pdf"
```

### Comparing `richvalues-3.1.1/richvalues/__init__.py` & `richvalues-3.1.2/richvalues/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
 HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
 STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING
 IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE
 POSSIBILITY OF SUCH DAMAGE.
 """
 
-__version__ = '3.1.1'
+__version__ = '3.1.2'
 __author__ = 'Andrés Megías Toledano'
 
 import copy
 import math
 import inspect
 import itertools
 import numpy as np
@@ -412,28 +412,37 @@
             is_range = False
         
         global variable_count
         expression = 'x{}'.format(variable_count)
         variable_count += 1
                 
         self.main = main
-        self.unc = unc
+        self._unc = unc
         self.is_lolim = is_lolim
         self.is_uplim = is_uplim
         self.is_range = is_range
         self.domain = domain
         self.num_sf = defaultparams['number of significant figures']
         self.min_exp = defaultparams['minimum exponent for scientific notation']
         self.extra_sf_lim = defaultparams['limit for extra significant figure']
         self.vars = [expression]
         self.expression = expression
         
         global variable_dict
         variable_dict[expression] = self
-          
+ 
+    @property
+    def unc(self): return self._unc
+    @unc.setter
+    def unc(self, x):
+        if not hasattr(x, '__iter__'):
+            x = [x, x]
+        x = list(x)
+        self._unc = x
+         
     @property
     def is_lim(self):
         """Upper/lower limit"""
         islim = self.is_lolim or self.is_uplim
         return islim
     @property
     def is_interv(self):
@@ -2186,15 +2195,18 @@
             domain = [x1, x2]
             text = text.split('[')[0][:-1]
         else:
             domain = [-np.inf, np.inf]
         if not '--' in text:
             if text.startswith('+'):
                 text = text[1:]
-            if ' e' in text:
+            if 'e' in text:
+                text = text.replace('e+', 'e')
+                if not ' e' in text:
+                    text = text.replace('e', ' e')
                 min_exp = abs(int(text.split('e')[1]))
             else:
                 min_exp = np.inf
                 text = '{} e0'.format(text)
             min_exp = min(min_exp, defaultparams['minimum exponent for '
                                                  + 'scientific notation'])
             single_value = True
@@ -2370,15 +2382,15 @@
     new_array = RichArray(mains, uncs, are_lolims, are_uplims, are_ranges,
                           domains)
     min_exp = round(np.mean(min_exps))
     extra_sf_lim = min(extra_sf_lims)
     new_array.set_params({'min_exp': min_exp, 'extra_sf_lim': extra_sf_lim})
     return new_array
 
-def rich_dataframe(df, domains=None, use_default_extra_sf_lim=False):
+def rich_dataframe(df, domains=None, use_default_extra_sf_lim=False, **kwargs):
     """
     Convert the values of the input dataframe of text strings to rich values.
 
     Parameters
     ----------
     df : dataframe (str)
         Input dataframe which contains text strings formatted as rich values.
@@ -2389,43 +2401,46 @@
         input dataframe is already a rich value, its original domain will be
         preserved; if not, the default domain will be used, that is,
         [-np.inf, np.inf].
     use_default_extra_sf_lim : bool, optional
         If True, the default limit for extra significant figure will be used
         instead of inferring it from the input text. This will reduce the
         computation time a little bit.
+    **kwargs : keyword arguments, optional
+        Keyword arguments for the DataFrame class.
 
     Returns
     -------
     new_df : dataframe
         Resulting dataframe of rich values.
     """
-    df = pd.DataFrame(df)
+    df = pd.DataFrame(df, **kwargs)
     if type(domains) is not dict:
         domains = {col: domains for col in df}
     new_df = copy.copy(df)
     for i,row in new_df.iterrows():
         for col in new_df:
             is_rich_value = (True if type(new_df.at[i,col]) is RichValue
                              else False)
             domain = domains[col] if col in domains else None
             if is_rich_value:
                 x = new_df.at[i,col]
                 if domain is not None:
                     x.domain = domain
             else:
-                is_number = True
+                is_number = False
                 text = str(new_df.at[i,col])
-                for char in text.replace(' e', ''):
-                    if char.isalpha():
-                        is_number = False
+                for char in text.replace('e', ''):
+                    if char.isnumeric():
+                        is_number = True
                         break
                 if is_number:
-                    x = rich_value(new_df.at[i,col], domain,
-                                   use_default_extra_sf_lim)
+                    if domain is None:
+                        domain = defaultparams['domain']
+                    x = rich_value(text, domain, use_default_extra_sf_lim)
             if is_rich_value or is_number:
                 new_df.at[i,col] = x
     new_df = RichDataFrame(new_df)
     return new_df
 
 def bounded_gaussian(x, m=0., s=1., a=np.inf):
     """
@@ -3597,15 +3612,14 @@
             for j in range(num_params):
                 samples[j] += [params_i[j]]
             if num_disp_points > 0:
                 ys_cond = function(xs[cond], *params_i)
                 dispersions += [(np.sum((ys[cond] - ys_cond)**2)
                                 / (num_disp_points - 1))**0.5]
             losses += [result.fun]
-            guess = params_i
         else:
             num_fails += 1
         if ((i+1) % (num_samples//4)) == 0:
             print('  {} %'.format(100*(i+1)//num_samples))
     if num_fails > 0.9*num_samples:
         raise Exception('The fit failed more than 90 % of the time.')
     params_fit = [evaluate_distr(samples[i]) for i in range(num_params)]
@@ -3684,15 +3698,14 @@
             for j in range(num_params):
                 samples[j] += [params_i[j]]
             if num_disp_points > 0:
                 ys_cond = function(*params_i)
                 dispersions += [(np.sum((ys[cond] - ys_cond)**2)
                                 / (num_disp_points - 1))**0.5]
             losses += [result.fun]
-            guess = params_i
         else:
             num_fails += 1
         if ((i+1) % (num_samples//4)) == 0:
             print('  {} %'.format(100*(i+1)//num_samples))
     if num_fails > 0.9*num_samples:
         raise Exception('The fit failed more than 90 % of the time.')
     params_fit = [evaluate_distr(samples[i]) for i in range(num_params)]
@@ -3816,8 +3829,8 @@
 function = function_with_rich_values
 array_function = function_with_rich_arrays
 distribution = distr_with_rich_values
 evaluate_distribution = evaluate_distr
 center_and_uncertainties = center_and_uncs
 is_not_a_number = is_nan = isnan
 is_infinite = is_inf = isinf
-is_finite = is_finite = isfinite
+is_finite = is_finite = isfinite
```

### Comparing `richvalues-3.1.1/setup.py` & `richvalues-3.1.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import setuptools
 
 with open('README.md', 'r') as file:
     long_description = file.read()
 
 setuptools.setup(
     name = 'richvalues',
-    version = '3.1.1',
+    version = '3.1.2',
     license = 'BSD-3-Clause',
     author = 'Andrés Megías Toledano',
     description = 'Python library for working with uncertainties and upper/lower limits',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     packages = setuptools.find_packages('.'),
     url = 'https://github.com/andresmegias/richvalues/',
     install_requires = ['numpy', 'pandas', 'scipy', 'matplotlib'],
-    classifiers = [
-        'Programming Language :: Python :: 3',
-        'License :: OSI Approved :: BSD License',
-        'Operating System :: OS Independent']
+    classifiers = ['Programming Language :: Python :: 3',
+                   'License :: OSI Approved :: BSD License',
+                   'Operating System :: OS Independent'],
+    project_urls = {"Documentation": "https://github.com/andresmegias/richvalues/blob/main/userguide.pdf"}
 )
```

