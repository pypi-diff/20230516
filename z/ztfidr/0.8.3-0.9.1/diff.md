# Comparing `tmp/ztfidr-0.8.3.tar.gz` & `tmp/ztfidr-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ztfidr-0.8.3.tar", last modified: Tue May  2 12:32:41 2023, max compression
+gzip compressed data, was "ztfidr-0.9.1.tar", last modified: Tue May 16 08:43:34 2023, max compression
```

## Comparing `ztfidr-0.8.3.tar` & `ztfidr-0.9.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 12:32:41.540930 ztfidr-0.8.3/
--rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.8.3/LICENSE
--rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-05-02 12:32:41.540800 ztfidr-0.8.3/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.8.3/README.md
--rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-02 12:32:41.540967 ztfidr-0.8.3/setup.cfg
--rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-05-02 12:32:23.000000 ztfidr-0.8.3/setup.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 12:32:41.540179 ztfidr-0.8.3/ztfidr/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2023-05-02 12:32:20.000000 ztfidr-0.8.3/ztfidr/__init__.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    14128 2023-05-02 12:32:11.000000 ztfidr-0.8.3/ztfidr/io.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    22044 2023-03-20 14:23:14.000000 ztfidr-0.8.3/ztfidr/lightcurve.py
--rw-r--r--   0 rigault   (2358) staff       (20)    18659 2022-11-06 15:43:33.000000 ztfidr-0.8.3/ztfidr/linefitter.py
--rw-r--r--   0 rigault   (2358) staff       (20)     3215 2023-05-02 07:49:21.000000 ztfidr-0.8.3/ztfidr/plotting.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.8.3/ztfidr/salt2.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    31042 2023-04-27 13:54:23.000000 ztfidr-0.8.3/ztfidr/sample.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.8.3/ztfidr/script.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)      950 2022-05-18 13:01:28.000000 ztfidr-0.8.3/ztfidr/snid.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    20341 2022-11-15 12:56:31.000000 ztfidr-0.8.3/ztfidr/spectroscopy.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.8.3/ztfidr/target.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)    23339 2023-05-02 10:02:49.000000 ztfidr-0.8.3/ztfidr/typing.py
--rwxrwxrwx   0 rigault   (2358) staff       (20)     4034 2023-03-24 07:32:25.000000 ztfidr-0.8.3/ztfidr/utils.py
-drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-02 12:32:41.540638 ztfidr-0.8.3/ztfidr.egg-info/
--rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-05-02 12:32:41.000000 ztfidr-0.8.3/ztfidr.egg-info/PKG-INFO
--rwxrwxrwx   0 rigault   (2358) staff       (20)      377 2023-05-02 12:32:41.000000 ztfidr-0.8.3/ztfidr.egg-info/SOURCES.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-02 12:32:41.000000 ztfidr-0.8.3/ztfidr.egg-info/dependency_links.txt
--rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-02 12:32:41.000000 ztfidr-0.8.3/ztfidr.egg-info/top_level.txt
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-16 08:43:34.907080 ztfidr-0.9.1/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    11357 2022-04-07 08:06:46.000000 ztfidr-0.9.1/LICENSE
+-rw-r--r--   0 rigault   (2358) staff       (20)      234 2023-05-16 08:43:34.906956 ztfidr-0.9.1/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     2186 2022-04-30 12:26:28.000000 ztfidr-0.9.1/README.md
+-rw-r--r--   0 rigault   (2358) staff       (20)       38 2023-05-16 08:43:34.907120 ztfidr-0.9.1/setup.cfg
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      609 2023-05-16 08:43:18.000000 ztfidr-0.9.1/setup.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-16 08:43:34.906237 ztfidr-0.9.1/ztfidr/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      127 2023-05-16 08:43:13.000000 ztfidr-0.9.1/ztfidr/__init__.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    14600 2023-05-16 08:41:57.000000 ztfidr-0.9.1/ztfidr/io.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    22044 2023-03-20 14:23:14.000000 ztfidr-0.9.1/ztfidr/lightcurve.py
+-rw-r--r--   0 rigault   (2358) staff       (20)    18659 2022-11-06 15:43:33.000000 ztfidr-0.9.1/ztfidr/linefitter.py
+-rw-r--r--   0 rigault   (2358) staff       (20)     3223 2023-05-07 16:40:33.000000 ztfidr-0.9.1/ztfidr/plotting.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1893 2022-04-07 08:06:50.000000 ztfidr-0.9.1/ztfidr/salt2.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    31049 2023-05-15 15:49:11.000000 ztfidr-0.9.1/ztfidr/sample.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      629 2022-05-02 15:53:23.000000 ztfidr-0.9.1/ztfidr/script.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     1170 2023-05-15 11:47:44.000000 ztfidr-0.9.1/ztfidr/snid.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    21063 2023-05-15 15:36:52.000000 ztfidr-0.9.1/ztfidr/spectroscopy.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    10043 2022-11-19 14:22:02.000000 ztfidr-0.9.1/ztfidr/target.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)    23521 2023-05-08 11:49:03.000000 ztfidr-0.9.1/ztfidr/typing.py
+-rwxrwxrwx   0 rigault   (2358) staff       (20)     4034 2023-03-24 07:32:25.000000 ztfidr-0.9.1/ztfidr/utils.py
+drwxr-xr-x   0 rigault   (2358) staff       (20)        0 2023-05-16 08:43:34.906812 ztfidr-0.9.1/ztfidr.egg-info/
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      234 2023-05-16 08:43:34.000000 ztfidr-0.9.1/ztfidr.egg-info/PKG-INFO
+-rwxrwxrwx   0 rigault   (2358) staff       (20)      377 2023-05-16 08:43:34.000000 ztfidr-0.9.1/ztfidr.egg-info/SOURCES.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        1 2023-05-16 08:43:34.000000 ztfidr-0.9.1/ztfidr.egg-info/dependency_links.txt
+-rwxrwxrwx   0 rigault   (2358) staff       (20)        7 2023-05-16 08:43:34.000000 ztfidr-0.9.1/ztfidr.egg-info/top_level.txt
```

### Comparing `ztfidr-0.8.3/LICENSE` & `ztfidr-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.3/README.md` & `ztfidr-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.3/setup.py` & `ztfidr-0.9.1/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 """
 from distutils.core import setup
 from setuptools import setup, find_packages
 
 
 packages = find_packages()
 
-VERSION = '0.8.3'
+VERSION = '0.9.1'
         
 setup(name='ztfidr',
       version=VERSION,
       description='Tools for ZTF Ia *Internal*DataReleases',
       author='Mickael Rigault',
       author_email='m.rigault@ipnl.in2p3.fr',
       url='https://github.com/MickaelRigault/ztfdr',
```

### Comparing `ztfidr-0.8.3/ztfidr/io.py` & `ztfidr-0.9.1/ztfidr/io.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,27 +15,31 @@
 #                    #
 # ================== #
 def get_targets_data():
     """ """
     redshifts = get_redshif_data()[["redshift","redshift_err", "source"]]
     salt2params = get_salt2params()
     coords = get_coords_data()
-#    
+    
     # merging
     data_ = pandas.merge(redshifts,salt2params, left_index=True, right_index=True,
                      suffixes=("","_salt"), how="outer")
     data_ = pandas.merge(data_, coords, left_index=True, right_index=True,
                          how="outer")
+    
     # force limit to target to use
     target_list = get_targetlist()
     data_ = data_.loc[target_list["ztfname"]]
 
     # adding classification
     typing = get_target_typing()
     data_ = data_.join(typing["classification"], how="left")
+
+
+    
     return data_
 
 def get_localhost_data(local_nkpc=2, which="mag"):
     """ """
     hostlocal = get_host_local(nkpc=2, which="mag")
     hostcoords = get_host_coords()
     dlr = get_host_mags().xs("global", axis=1)["host_dlr"]
@@ -62,28 +66,40 @@
                             "ztfdr2_targetlist.csv")
     if not load:
         return filepath
     
     return pandas.read_csv(filepath, **kwargs)
 
 def get_target_typing(load=True, index_col=0, sep=" ",
-                          clean=True, **kwargs):
+                        clean=True, generic_typing=True,
+                          **kwargs):
     """ """
     filepath = os.path.join(IDR_PATH, "tables/.dataset_creation/sample_def",
                             "ztfdr2_typing.csv")
     if not load:
         return filepath
     
     data = pandas.read_csv(filepath, index_col=index_col, sep=sep, **kwargs)
     if clean:
         data["typing"] = data["typing"].str.replace("[","", regex=False).str.replace("]","", regex=False).str.replace("'","") # clean
         data["typing"] = data["typing"].str.replace("sn ia", "snia").str.replace("not ia", "notia")
         data["typing"] = data["typing"].str.split(" ")
         
         data["ntypings"] = data["ntypings"].str.replace("[","", regex=False).str.replace("]","", regex=False).str.split(" ")
+
+    if generic_typing:
+        TYPING = {'sn ia': 'snia',
+                  'ia-norm': 'snia-norm',
+                  'ia(-norm)': 'snia-norm',
+                  'ia-91t':'snia-pec-91t',
+                  'ia-91bg':'snia-pec-91bg',
+                  'ia-other':'snia-pec'}
+
+        data["classification"] = data["classification"].apply(TYPING.get)
+        
     return data
 
 # Master List
 def get_masterlist(load=True, **kwargs):
     """ """
     filepath = os.path.join(IDR_PATH, "tables",
                             ".dataset_creation/sample_def/ztfdr2_masterlist.csv")
@@ -218,47 +234,47 @@
 #                    #
 #   HOST             #
 #                    #
 # ================== #
 def get_host_coords(load=True, **kwargs):
     """ """
     filepath = os.path.join(IDR_PATH, "tables",
-                            ".dataset_creation/host_prop/host_photometry/ztfdr2_hostcoords.csv")
+                            ".dataset_creation/host_prop/host_photometry/global/archive/ztfdr2_hostcoords.csv")
     if not load:
         return filepath
     
     return pandas.read_csv(filepath, **{**dict(sep=" "),**kwargs}).set_index("ztfname")
 
 def get_host_local(nkpc=2, which="mag", load=True, **kwargs):
     """ """
     filepath = os.path.join(IDR_PATH, "tables",
-                            f".dataset_creation/host_prop/host_photometry/ztfdr2_local{nkpc}kpc_{which}.csv")
+                            f".dataset_creation/host_prop/host_photometry/local/archive/ztfdr2_local{nkpc}kpc_{which}.csv")
     if not load:
         return filepath
     if not os.path.isfile(filepath):
         raise IOError(f"no such file {filepath}")
 
     return pandas.read_csv(filepath, index_col=0, **kwargs)
 
 def get_host_sedfit(nkpc=2, load=True, **kwargs):
     """ """
     filepath = os.path.join(IDR_PATH, "tables",
-                            f".dataset_creation/host_prop/host_properties/ztfdr2_local{nkpc}kpc_sedfit.csv")
+                            f".dataset_creation/host_prop/host_properties/local/archive/ztfdr2_local{nkpc}kpc_sedfit.csv")
     if not load:
         return filepath
     if not os.path.isfile(filepath):
         raise IOError(f"no such file {filepath}")
 
     return pandas.read_csv(filepath, index_col=0, **kwargs)
     
 
 def get_host_mags(load=True, index_col=0, raw=False, **kwargs):
     """ """
     filepath = os.path.join(IDR_PATH, "tables",
-                            ".dataset_creation/host_prop/host_photometry/ztfdr2_hostmags.csv")
+                            ".dataset_creation/host_prop/host_photometry/global/archive/ztfdr2_hostmags.csv")
     if not load:
         return filepath
 
     host_alldata = pandas.read_csv(filepath, index_col=index_col, **kwargs)
     if raw:
         return host_alldata
```

### Comparing `ztfidr-0.8.3/ztfidr/lightcurve.py` & `ztfidr-0.9.1/ztfidr/lightcurve.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.3/ztfidr/linefitter.py` & `ztfidr-0.9.1/ztfidr/linefitter.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.3/ztfidr/plotting.py` & `ztfidr-0.9.1/ztfidr/plotting.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,10 +77,10 @@
 
     ax.text(rest+30,-2, f'{rest}', fontsize="large",
             color="k", va="center", ha="left")
 
     clearwhich = ["bottom","right","top",] # "bottom"
     [ax.spines[which].set_visible(False) for which in clearwhich]
     ax.set_xticks([])
-    ax.set_yticks([1,0,-1,-2], ["SN Ia\nnorm","SN Ia","SN Ia\npeculiar", "Unclear"])
+    ax.set_yticks([1,0,-1,-2], ["SN Ia\nnorm","SN Ia","SN Ia\npeculiar", "Unclear\nnon-ia"])
 
     return fig
```

### Comparing `ztfidr-0.8.3/ztfidr/salt2.py` & `ztfidr-0.9.1/ztfidr/salt2.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.3/ztfidr/sample.py` & `ztfidr-0.9.1/ztfidr/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,38 +8,33 @@
 def get_sample(**kwargs):
     """ Short to to Sample.load() """
     return Sample.load(**kwargs)
 
 
 class Sample():
 
-    NON_IA_CLASSIFICATIONS = ["nonia","ib/c","unclear","confusing"]
     
     def __init__(self, data=None):
         """ """
         self.set_data(data)
     
     @classmethod
-    def load(cls, redshift_range=None, target_list=None, has_spectra=True,
-                 rm_nonia=False):
+    def load(cls, redshift_range=None, target_list=None, has_spectra=True):
         """ Load a Sample instance building it from io.get_targets_data() """
         data = io.get_targets_data()
         
         if redshift_range is not None:
             data = data[data["redshift"].between(*redshift_range)]
 
         if target_list is not None:
             data = data.loc[target_list]
 
         if has_spectra:
             specfile = io.get_spectra_datafile(data=data)
             data = data[data.index.isin(specfile["ztfname"])]
-
-        if rm_nonia:
-            data = data[~data["classification"].isin(cls.NON_IA_CLASSIFICATIONS)]
             
         return cls(data=data)
 
     # ------- #
     # LOADER  #
     # ------- #
     def load_hostdata(self):
@@ -282,36 +277,43 @@
         # Additional Query
         if query:
             data = data.query(query)
             
         return data
 
     def get_ianorm(self, incl_snia=False):
-        """ get the list targets that are ia-norm or ia(-norm) (or sn ia if incl_snia=True)
+        """ get the list targets that are ia-norm (or sn ia if incl_snia=True)
         
         Returns
         -------
         array
             list of targetname (data.index)
-        """
-        classifications = ["ia-norm","ia(-norm)"]
+        """        
+        classifications = ["snia-norm"]
         if incl_snia:
-            classifications += ["sn ia"]
+            classifications += ["snia"]
             
         return np.asarray(self.data[self.data["classification"].isin(classifications)].index)
     
     # Target | High level
     def get_target(self, name):
         """ """
         from . import target
         lightcurve = self.get_target_lightcurve(name)
         spectra = self.get_target_spectra(name, as_spectra=False)
         meta = self.data.loc[name]
         return target.Target(lightcurve, spectra, meta=meta)
 
+    def get_target_typing(self, name=None):
+        """ """
+        if name is None:
+            return self.data["classification"].copy()
+        
+        return self.data.loc[np.atleast_1d(name)]["classification"].copy()
+    
     # LightCurve
     def get_target_lightcurve(self, name, **kwargs):
         """ Get the {name} LightCurve object """
         from . import lightcurve
         return lightcurve.LightCurve.from_name(name)
 
     # Spectrum
```

### Comparing `ztfidr-0.8.3/ztfidr/script.py` & `ztfidr-0.9.1/ztfidr/script.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.3/ztfidr/spectroscopy.py` & `ztfidr-0.9.1/ztfidr/spectroscopy.py`

 * *Files 3% similar despite different names*

```diff
@@ -265,21 +265,37 @@
         
         phase = obsdate.mjd-t0
         if z is not None:
             phase /=(1+z)
             
         return phase
 
-    def get_redshift(self):
+    def get_redshift(self, typing=None, verbose=False, **kwargs):
         """ """
         if self.snidresult is None:
             warnings.warn("snidres is not defined (None)")
             return [np.nan, np.nan]
 
-        return self.snidresult.get_redshift()
+        SNIDPARSE_TYPING = {"snia": "Ia",
+                            "snia-norm": "Ia-norm",
+                            "snia-pec-91t": "Ia-91T",
+                            "snia-pec-91bg": "Ia-91bg",
+                            "snia-pec": "Ia!norm",
+                            }
+        if typing is not None:
+            snid_typing = SNIDPARSE_TYPING.get(typing,None)
+            if snid_typing is None:
+                warnings.warn(f"Could not parse input {typing} typing")
+            elif verbose:
+                print(f"using snid_typing:{snid_typing} as input typing:{typing}")
+                
+        else:
+            snid_typing = None
+
+        return self.snidresult.get_redshift(typing=snid_typing, **kwargs)
 
     # --------- #
     #  FITTER   #
     # --------- #
     def fit_hanii(self, redshift=None, **kwargs):
         """ """
         if not hasattr(self,"_linefitter"):
```

### Comparing `ztfidr-0.8.3/ztfidr/target.py` & `ztfidr-0.9.1/ztfidr/target.py`

 * *Files identical despite different names*

### Comparing `ztfidr-0.8.3/ztfidr/typing.py` & `ztfidr-0.9.1/ztfidr/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -325,52 +325,52 @@
 
     def get_typing(self, **kwargs):
         """ """
         if "classification" not in self.data:
             self.load_classification(**kwargs)
             
         data = self.get_classification_df()
-        classification = self.data.groupby("target_name").first()["classification"]
+        classification = self.data.groupby("target_name").first()[["classification","class_origin"]]
         data = data.join(classification)
         return data
     
     def store_typing(self, **kwargs):
         """ """
         data = self.get_typing(**kwargs)
         return data.to_csv( io.get_target_typing(False), sep=" ")
 
     def load_classification(self, **kwargs):
         """ """
         classifications = self.get_classification(**kwargs)
         self._data = self.data.join(classifications, on="target_name", how="outer")
         
-    def get_classification(self, min_review=2,
+    def get_classification(self,  min_review=2,
                                   min_autotyping=3,
                                   min_generic_typing=3,
                                 # Master keys
                                   min_review_master=1,
                                   min_autotyping_master=2,
-                                  min_generic_typing_master=3):
+                                  min_generic_typing_master=3,
+                               # arbiter
+                                 incl_arbiter=True):
         """ """
         # All auto | default
         auto_data = self._get_classification(prefix="auto_",
                                                  min_review=min_review, min_autotyping=min_autotyping,
                                                  min_generic_typing=min_generic_typing)
 
         # Masters
         master = self.get_masterclassification(incl_unclear=False) # do not consider unclear's input
         master_data = master._get_classification(prefix="master_",
                                                       min_review=min_review_master, min_autotyping=min_autotyping_master,
                                                       min_generic_typing=min_generic_typing_master)
         # do not consider master's None or confusing. Only final classification
 
         # Arbiter
-        arbiter_data = Reports.get_arbiters(prefix="arbiter_").groupby("target_name").last()[["arbiter_classification"]] # [[ to get a dataframe
-        # - force in data list
-        arbiter_data = arbiter_data.loc[ arbiter_data.index.isin(self.target_list) ]
+        
 
         #
         # Now let's join
         #
         # - Default
         cdata = pandas.DataFrame(auto_data["auto_classification"].values, index=auto_data.index, columns=["classification"])
         cdata["class_origin"] = "auto"
@@ -381,17 +381,22 @@
         master_data = master_data[~master_data["master_classification"].isin(["None","confusing", np.NaN])]
         
         cdata.loc[master_data.index, "classification"] = master_data["master_classification"]
         cdata.loc[master_data.index, "class_origin"] = "master"
         cdata = cdata.join(master_data)
         
         # - add arbiter
-        cdata.loc[arbiter_data.index, "classification"] = arbiter_data["arbiter_classification"]
-        cdata.loc[arbiter_data.index, "class_origin"] = "arbiter"
-        cdata = cdata.join(arbiter_data)
+        if incl_arbiter:
+            arbiter_data = Reports.get_arbiters(prefix="arbiter_").groupby("target_name").last()[["arbiter_classification"]] # [[ to get a dataframe
+            # - force in data list
+            arbiter_data = arbiter_data.loc[ arbiter_data.index.isin(self.target_list) ]
+            
+            cdata.loc[arbiter_data.index, "classification"] = arbiter_data["arbiter_classification"]
+            cdata.loc[arbiter_data.index, "class_origin"] = "arbiter"
+            cdata = cdata.join(arbiter_data)
 
         return cdata
         
         
     def _get_classification(self, prefix="", reindex=True, **kwargs):
         # Normal
         class_df = self.get_classification_df()
```

### Comparing `ztfidr-0.8.3/ztfidr/utils.py` & `ztfidr-0.9.1/ztfidr/utils.py`

 * *Files identical despite different names*

