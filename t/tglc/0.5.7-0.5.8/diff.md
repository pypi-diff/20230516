# Comparing `tmp/tglc-0.5.7.tar.gz` & `tmp/tglc-0.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tglc-0.5.7.tar", last modified: Wed Mar  8 05:07:15 2023, max compression
+gzip compressed data, was "tglc-0.5.8.tar", last modified: Mon May 15 23:40:54 2023, max compression
```

## Comparing `tglc-0.5.7.tar` & `tglc-0.5.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2023-03-08 05:07:15.570889 tglc-0.5.7/
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     1063 2022-09-16 07:04:15.000000 tglc-0.5.7/LICENSE
--rw-rw-r--   0 tehan     (1000) tehan     (1000)       35 2022-09-16 07:04:15.000000 tglc-0.5.7/MANIFEST.in
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     4700 2023-03-08 05:07:15.570889 tglc-0.5.7/PKG-INFO
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     4277 2023-03-08 05:07:09.000000 tglc-0.5.7/README.rst
--rw-rw-r--   0 tehan     (1000) tehan     (1000)       38 2023-03-08 05:07:15.570889 tglc-0.5.7/setup.cfg
--rw-rw-r--   0 tehan     (1000) tehan     (1000)      925 2023-03-08 05:05:52.000000 tglc-0.5.7/setup.py
-drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2023-03-08 05:07:15.570889 tglc-0.5.7/tglc/
--rw-rw-r--   0 tehan     (1000) tehan     (1000)      115 2023-03-08 05:05:52.000000 tglc-0.5.7/tglc/__init__.py
-drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2023-03-08 05:07:15.570889 tglc-0.5.7/tglc/background_mask/
--rw-rw-r--   0 tehan     (1000) tehan     (1000)        0 2022-09-16 07:04:15.000000 tglc-0.5.7/tglc/background_mask/__init__.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)   267840 2022-09-16 07:04:15.000000 tglc-0.5.7/tglc/background_mask/median_mask.fits
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    22304 2023-03-08 05:05:02.000000 tglc-0.5.7/tglc/effective_psf.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    15273 2023-01-31 18:35:34.000000 tglc-0.5.7/tglc/ffi.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    11279 2023-03-06 19:16:16.000000 tglc-0.5.7/tglc/ffi_cut.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)   136246 2023-02-12 08:25:40.000000 tglc-0.5.7/tglc/lc_plot.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     4324 2023-02-19 01:37:19.000000 tglc-0.5.7/tglc/mast.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    16072 2023-03-08 05:05:02.000000 tglc-0.5.7/tglc/quick_lc.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     3008 2022-12-05 19:54:14.000000 tglc-0.5.7/tglc/run.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     2789 2022-09-26 21:46:44.000000 tglc-0.5.7/tglc/source_output.py
--rw-rw-r--   0 tehan     (1000) tehan     (1000)    19011 2023-03-08 05:05:02.000000 tglc-0.5.7/tglc/target_lightcurve.py
-drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2023-03-08 05:07:15.570889 tglc-0.5.7/tglc.egg-info/
--rw-rw-r--   0 tehan     (1000) tehan     (1000)     4700 2023-03-08 05:07:15.000000 tglc-0.5.7/tglc.egg-info/PKG-INFO
--rw-rw-r--   0 tehan     (1000) tehan     (1000)      422 2023-03-08 05:07:15.000000 tglc-0.5.7/tglc.egg-info/SOURCES.txt
--rw-rw-r--   0 tehan     (1000) tehan     (1000)        1 2023-03-08 05:07:15.000000 tglc-0.5.7/tglc.egg-info/dependency_links.txt
--rw-rw-r--   0 tehan     (1000) tehan     (1000)       96 2023-03-08 05:07:15.000000 tglc-0.5.7/tglc.egg-info/requires.txt
--rw-rw-r--   0 tehan     (1000) tehan     (1000)        5 2023-03-08 05:07:15.000000 tglc-0.5.7/tglc.egg-info/top_level.txt
+drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2023-05-15 23:40:54.723476 tglc-0.5.8/
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     1063 2022-09-16 07:04:15.000000 tglc-0.5.8/LICENSE
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)       35 2022-09-16 07:04:15.000000 tglc-0.5.8/MANIFEST.in
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     5313 2023-05-15 23:40:54.723476 tglc-0.5.8/PKG-INFO
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     4890 2023-05-15 23:39:45.000000 tglc-0.5.8/README.rst
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)       38 2023-05-15 23:40:54.723476 tglc-0.5.8/setup.cfg
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)      925 2023-05-15 23:40:30.000000 tglc-0.5.8/setup.py
+drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2023-05-15 23:40:54.723476 tglc-0.5.8/tglc/
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)      115 2023-05-15 23:40:46.000000 tglc-0.5.8/tglc/__init__.py
+drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2023-05-15 23:40:54.723476 tglc-0.5.8/tglc/background_mask/
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)        0 2022-09-16 07:04:15.000000 tglc-0.5.8/tglc/background_mask/__init__.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)   267840 2022-09-16 07:04:15.000000 tglc-0.5.8/tglc/background_mask/median_mask.fits
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    22524 2023-05-10 19:08:34.000000 tglc-0.5.8/tglc/effective_psf.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    15306 2023-04-05 01:10:48.000000 tglc-0.5.8/tglc/ffi.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    11630 2023-05-12 17:16:48.000000 tglc-0.5.8/tglc/ffi_cut.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)   136246 2023-02-12 08:25:40.000000 tglc-0.5.8/tglc/lc_plot.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     4331 2023-03-18 21:06:07.000000 tglc-0.5.8/tglc/mast.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    20381 2023-05-15 23:39:22.000000 tglc-0.5.8/tglc/quick_lc.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     3008 2022-12-05 19:54:14.000000 tglc-0.5.8/tglc/run.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     2789 2022-09-26 21:46:44.000000 tglc-0.5.8/tglc/source_output.py
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)    19167 2023-05-14 20:19:13.000000 tglc-0.5.8/tglc/target_lightcurve.py
+drwxrwxr-x   0 tehan     (1000) tehan     (1000)        0 2023-05-15 23:40:54.723476 tglc-0.5.8/tglc.egg-info/
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)     5313 2023-05-15 23:40:54.000000 tglc-0.5.8/tglc.egg-info/PKG-INFO
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)      422 2023-05-15 23:40:54.000000 tglc-0.5.8/tglc.egg-info/SOURCES.txt
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)        1 2023-05-15 23:40:54.000000 tglc-0.5.8/tglc.egg-info/dependency_links.txt
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)       96 2023-05-15 23:40:54.000000 tglc-0.5.8/tglc.egg-info/requires.txt
+-rw-rw-r--   0 tehan     (1000) tehan     (1000)        5 2023-05-15 23:40:54.000000 tglc-0.5.8/tglc.egg-info/top_level.txt
```

### Comparing `tglc-0.5.7/LICENSE` & `tglc-0.5.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tglc-0.5.7/PKG-INFO` & `tglc-0.5.8/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tglc
-Version: 0.5.7
+Version: 0.5.8
 Summary: TESS-Gaia Light Curve
 Home-page: https://github.com/TeHanHunter/TESS_Gaia_Light_Curve
 Author: Te Han
 Author-email: tehanhunter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,17 +20,17 @@
 
 ==================================
 Usage
 ==================================
 There are four fluxes in each FITS file: aperture flux, PSF flux, calibrated aperture flux, and calibrated PSF flux.
 If you are uncertain which to use:
 
-* Calibrated aperture flux is the most robust in transit depth. Use this if you are doing transit science.
-* Calibrated psf flux is better in deblending targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior.
-* The aperture flux and PSF flux are not detrended or normalized. Use this if you are doing stellar variability science. Or, if the detrending is not optimal (default detrending has a window length of 1 day), start with the aperture flux or PSF flux and detrend carefully!
+* Calibrated psf flux is better in **deblending** targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior. It also gives the more accurate **transit depth** in most cases, especially when fitting with an optimized prior.
+* Calibrated aperture flux usually has slightly **higher SNR**. The transit depth (or variation amplitude), however, can be imperfect since the normalization depends on the PSF fitting which is imperfect. This imperfection can be minimized by using a bigger aperture than the default aperture (3*3). One need to use the tglc package and set tglc_lc(save_aper=True) to access the 5*5 aperture. In the presence of a bright but "constant" contamination (several magnitudes brighter), the calibrated aperture flux is better in removing the constant contamination. 
+* The aperture flux and PSF flux are not detrended or normalized. Use this if you are doing stellar variability science with long baseline. Or, if the detrending is not optimal (default detrending has a window length of 1 day; see Known Problems below), start with the aperture flux or PSF flux and detrend carefully!
 * **If you are uncertain, start with calibrated aperture flux!**
 
 The `tutorial <tutorial/TGLC_tutorial.ipynb>`_ shows the syntaxes and differences among these light curves in several examples.
 
 ==================================
 Data Access
 ==================================
@@ -56,13 +56,14 @@
 for the latest tglc release. After installation, follow the `tutorial <tutorial/TGLC_tutorial.ipynb>`_ to fit light curves. If there is a problem, please leave a comment in the Issues section to help us improve. Thank you!
 
 
 ==================================
 Known Problems
 ==================================
 There are several imperfections we noticed in the MAST TGLC light curves and tglc package:
-* If the star is very dim (~< 15 Tmag) near a variable source, it can make the aperture and/or PSF light curve negative for some cadences. This is a very rare scenario, but could be important. The detrending algorithm could malfunction and result in bad cal_aper_flux and/or cal_psf_flux. This is now fixed for tglc package, but this problem remains for the primary mission light curves published on MAST. Please detrend again if necessary. We will also correct for the extended mission light curves on MAST.
+
+* If the star is very dim (~< 15 Tmag) near a variable source, it can make the aperture and/or PSF light curve negative for some cadences. The detrending algorithm could malfunction and result in bad cal_aper_flux and/or cal_psf_flux. This is now fixed for tglc package, but this problem remains for the primary mission light curves published on MAST. Please detrend again if necessary.The extended mission light curves on MAST will not be affected. This is a very rare scenario, but could be important.
 
 ==================================
 Reference
 ==================================
 If you find the TGLC light curves or the tglc package useful in your research, please cite `our paper <https://iopscience.iop.org/article/10.3847/1538-3881/acaaa7>`_ published on the Astronomical Journal.
```

### Comparing `tglc-0.5.7/README.rst` & `tglc-0.5.8/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 
 ==================================
 Usage
 ==================================
 There are four fluxes in each FITS file: aperture flux, PSF flux, calibrated aperture flux, and calibrated PSF flux.
 If you are uncertain which to use:
 
-* Calibrated aperture flux is the most robust in transit depth. Use this if you are doing transit science.
-* Calibrated psf flux is better in deblending targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior.
-* The aperture flux and PSF flux are not detrended or normalized. Use this if you are doing stellar variability science. Or, if the detrending is not optimal (default detrending has a window length of 1 day), start with the aperture flux or PSF flux and detrend carefully!
+* Calibrated psf flux is better in **deblending** targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior. It also gives the more accurate **transit depth** in most cases, especially when fitting with an optimized prior.
+* Calibrated aperture flux usually has slightly **higher SNR**. The transit depth (or variation amplitude), however, can be imperfect since the normalization depends on the PSF fitting which is imperfect. This imperfection can be minimized by using a bigger aperture than the default aperture (3*3). One need to use the tglc package and set tglc_lc(save_aper=True) to access the 5*5 aperture. In the presence of a bright but "constant" contamination (several magnitudes brighter), the calibrated aperture flux is better in removing the constant contamination. 
+* The aperture flux and PSF flux are not detrended or normalized. Use this if you are doing stellar variability science with long baseline. Or, if the detrending is not optimal (default detrending has a window length of 1 day; see Known Problems below), start with the aperture flux or PSF flux and detrend carefully!
 * **If you are uncertain, start with calibrated aperture flux!**
 
 The `tutorial <tutorial/TGLC_tutorial.ipynb>`_ shows the syntaxes and differences among these light curves in several examples.
 
 ==================================
 Data Access
 ==================================
@@ -42,13 +42,14 @@
 for the latest tglc release. After installation, follow the `tutorial <tutorial/TGLC_tutorial.ipynb>`_ to fit light curves. If there is a problem, please leave a comment in the Issues section to help us improve. Thank you!
 
 
 ==================================
 Known Problems
 ==================================
 There are several imperfections we noticed in the MAST TGLC light curves and tglc package:
-* If the star is very dim (~< 15 Tmag) near a variable source, it can make the aperture and/or PSF light curve negative for some cadences. This is a very rare scenario, but could be important. The detrending algorithm could malfunction and result in bad cal_aper_flux and/or cal_psf_flux. This is now fixed for tglc package, but this problem remains for the primary mission light curves published on MAST. Please detrend again if necessary. We will also correct for the extended mission light curves on MAST.
+
+* If the star is very dim (~< 15 Tmag) near a variable source, it can make the aperture and/or PSF light curve negative for some cadences. The detrending algorithm could malfunction and result in bad cal_aper_flux and/or cal_psf_flux. This is now fixed for tglc package, but this problem remains for the primary mission light curves published on MAST. Please detrend again if necessary.The extended mission light curves on MAST will not be affected. This is a very rare scenario, but could be important.
 
 ==================================
 Reference
 ==================================
 If you find the TGLC light curves or the tglc package useful in your research, please cite `our paper <https://iopscience.iop.org/article/10.3847/1538-3881/acaaa7>`_ published on the Astronomical Journal.
```

### Comparing `tglc-0.5.7/setup.py` & `tglc-0.5.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 sys.path.insert(0, "tglc")
 with open("README.rst", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setuptools.setup(
     name="tglc",
-    version='0.5.7',
+    version='0.5.8',
     author="Te Han",
     author_email="tehanhunter@gmail.com",
     description="TESS-Gaia Light Curve",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/TeHanHunter/TESS_Gaia_Light_Curve",
     classifiers=[
```

### Comparing `tglc-0.5.7/tglc/background_mask/median_mask.fits` & `tglc-0.5.8/tglc/background_mask/median_mask.fits`

 * *Files identical despite different names*

### Comparing `tglc-0.5.7/tglc/effective_psf.py` & `tglc-0.5.8/tglc/effective_psf.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,15 @@
         star_pos = np.where(star_info_num[0] == index[i])[0]
         A_[star_info_num[1][star_pos]] = star_info_num[2][star_pos]
         A_cut[i] = A[index[i], :] - A_
     aperture = np.zeros((len(source.time), len(index)))
     for j in range(len(source.time)):
         aperture[j] = np.array(source.flux[j][down:up, left:right]).flatten() - np.dot(A_cut, e_psf[j])
     aperture = aperture.reshape((len(source.time), up - down, right - left))
+    # np.save(f'_residual_{source.sector}.npy', aperture)
 
     # psf_lc
     over_size = psf_size * factor + 1
     if near_edge:  # TODO: near_edge
         psf_lc = np.zeros(len(source.time))
         psf_lc[:] = np.NaN
         e_psf_1d = np.nanmedian(e_psf[:, :over_size ** 2], axis=0).reshape(over_size, over_size)
@@ -255,14 +256,16 @@
         else:
             aper_flat = aperture[j, :, :].flatten()
             A_[:, 0] = psf_sim[j, :, :].flatten() / epsf_sum
             a = np.delete(A_, edge_pixel[outliers], 0)
             aper_flat = np.delete(aper_flat, edge_pixel[outliers])
             psf_lc[j] = np.linalg.lstsq(a, aper_flat)[0][0]
     portion = np.nansum(psf_shape[:, 4:7, 4:7]) / np.nansum(psf_shape)
+    # print(np.nansum(psf_shape[:, 5, 5]) / np.nansum(psf_shape))
+    # np.save(f'toi-5344_psf_{source.sector}.npy', psf_shape)
     return aperture, psf_lc, y - down, x - left, portion
 
 
 def fit_lc_float_field(A, source, star_info=None, x=np.array([]), y=np.array([]), star_num=0, factor=2, psf_size=11,
                        e_psf=None, near_edge=False, prior=0.001):
     """
     Produce matrix for least_square fitting without a certain target
@@ -423,20 +426,22 @@
     :param star_num: int, required,
     star index
     :param near_edge: boolean, required
     whether the star is 2 pixels or closer to the edge of a CCD
     :return: local background, modified aperture light curve, modified PSF light curve
     '''
     bar = 15000 * 10 ** ((source.gaia['tess_mag'][star_num] - 10) / -2.5)
+    # print(bar)
     # med_epsf = np.nanmedian(e_psf[:, :23 ** 2].reshape(len(source.time), 23, 23), axis=0)
     # centroid_to_aper_ratio = 4/9 * np.sum(med_epsf[10:13, 10:13]) / np.sum(med_epsf)
     # centroid_to_aper_ratio = np.nanmedian(ratio)
     # flux_bar = aperture_bar * centroid_to_aper_ratio
     # lightcurve = lightcurve + (flux_bar - np.nanmedian(lightcurve[q]))
     aperture_bar = bar * portion
+    # print(bar)
     local_bg = np.nanmedian(aper_lc[q]) - aperture_bar
     if np.isnan(local_bg):
         local_bg = 0
     aper_lc = aper_lc - local_bg
     psf_bar = bar
     local_bg = np.nanmedian(psf_lc[q]) - psf_bar
     if np.isnan(local_bg):
```

### Comparing `tglc-0.5.7/tglc/ffi.py` & `tglc-0.5.8/tglc/ffi.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,22 +58,22 @@
             atype = "str"
         if atype == "boolean":
             atype = "bool"
         data_table[col] = np.array([x.get(col, None) for x in json_obj['data']], dtype=atype)
     return data_table
 
 
-def tic_advanced_search_position_rows(ra=1., dec=1., radius=0.5):
+def tic_advanced_search_position_rows(ra=1., dec=1., radius=0.5, limit_mag=16):
     request = {"service": "Mast.Catalogs.Filtered.Tic.Position.Rows",
                "format": "json",
                "params": {
                    "columns": 'ID, GAIA',
                    "filters": [
                        {"paramName": "Tmag",
-                        "values": [{"min": -10., "max": 16.5}]}],
+                        "values": [{"min": -10., "max": (limit_mag + 0.5)}]}],
                    "ra": ra,
                    "dec": dec,
                    "radius": radius
                }}
 
     headers, out_string = mast_query(request)
     out_data = json.loads(out_string)
@@ -85,15 +85,15 @@
             SELECT dr2_source_id, dr3_source_id
             FROM gaiadr3.dr2_neighbourhood
             WHERE dr2_source_id IN {gaia_ids}
             """
     gaia_array = np.array(catalogdata_tic['GAIA'])
     gaia_array = gaia_array[gaia_array != 'None']
     # np.save('gaia_array.npy', gaia_array)
-    segment = len(gaia_array) // 10000
+    segment = (len(gaia_array) - 1) // 10000
     gaia_tuple = tuple(gaia_array[:10000])
     results = Gaia.launch_job_async(query.format(gaia_ids=gaia_tuple)).get_results()
     # np.save('result.npy', np.array(results))
     for i in range(segment):
         gaia_array_cut = gaia_array[((i+1)*10000):((i+2)*10000)]
         gaia_tuple_cut = tuple(gaia_array_cut)
         results = vstack([results, Gaia.launch_job_async(query.format(gaia_ids=gaia_tuple_cut)).get_results()])
```

### Comparing `tglc-0.5.7/tglc/ffi_cut.py` & `tglc-0.5.8/tglc/ffi_cut.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 os.environ['TF_CPP_MIN_LOG_LEVEL'] = '2'
 
 Gaia.ROW_LIMIT = -1
 Gaia.MAIN_GAIA_TABLE = "gaiadr3.gaia_source"
 
 
 class Source_cut(object):
-    def __init__(self, name, size=50, sector=None, cadence=None):
+    def __init__(self, name, size=50, sector=None, cadence=None, limit_mag=None):
         """
         Source_cut object that includes all data from TESS and Gaia DR3
         :param name: str, required
         Target identifier (e.g. "NGC 7654" or "M31"),
         or coordinate in the format of ra dec (e.g. '351.40691 61.646657')
         :param size: int, optional
         The side length in pixel  of TESScut image
@@ -58,26 +58,29 @@
         coord = SkyCoord(ra=ra, dec=dec, unit=(u.degree, u.degree), frame='icrs')
         radius = u.Quantity((self.size + 6) * 21 * 0.707 / 3600, u.deg)
         print(f'Target Gaia: {target[0]["designation"]}')
         catalogdata = Gaia.cone_search_async(coord, radius,
                                              columns=['DESIGNATION', 'phot_g_mean_mag', 'phot_bp_mean_mag',
                                                       'phot_rp_mean_mag', 'ra', 'dec', 'pmra', 'pmdec']).get_results()
         print(f'Found {len(catalogdata)} Gaia DR3 objects.')
-        catalogdata_tic = tic_advanced_search_position_rows(ra=ra, dec=dec, radius=(self.size + 2) * 21 * 0.707 / 3600)
+        catalogdata_tic = tic_advanced_search_position_rows(ra=ra, dec=dec, radius=(self.size + 2) * 21 * 0.707 / 3600, limit_mag=limit_mag)
         print(f'Found {len(catalogdata_tic)} TIC objects.')
         self.tic = convert_gaia_id(catalogdata_tic)
         sector_table = Tesscut.get_sectors(coordinates=coord)
         if len(sector_table) == 0:
             warnings.warn('TESS has not observed this position yet :(')
         print(sector_table)
         if sector is None:
             hdulist = Tesscut.get_cutouts(coordinates=coord, size=self.size)
-        elif sector is True:
+        elif sector == 'first':
             hdulist = Tesscut.get_cutouts(coordinates=coord, size=self.size, sector=sector_table['sector'][0])
             sector = sector_table['sector'][0]
+        elif sector == 'last':
+            hdulist = Tesscut.get_cutouts(coordinates=coord, size=self.size, sector=sector_table['sector'][-1])
+            sector = sector_table['sector'][-1]
         else:
             hdulist = Tesscut.get_cutouts(coordinates=coord, size=self.size, sector=sector)
         self.catalogdata = catalogdata
         self.sector_table = sector_table
         self.camera = int(sector_table[0]['camera'])
         self.ccd = int(sector_table[0]['ccd'])
         self.hdulist = hdulist
@@ -230,37 +233,39 @@
         t[f'sector_{self.sector}_x'] = star_x
         t[f'sector_{self.sector}_y'] = star_y
         gaia_targets = t  # TODO: sorting not sorting all columns
         gaia_targets.sort('tess_mag')
         self.gaia = gaia_targets
 
 
-def ffi_cut(target='', local_directory='', size=90, sector=None):
+def ffi_cut(target='', local_directory='', size=90, sector=None, limit_mag=None):
     """
     Function to generate Source_cut objects
     :param target: string, required
     target name
     :param local_directory: string, required
     output directory
     :param size: int, required
     FFI cut side length
     :param sector: int, required
     TESS sector number
     :return: tglc.ffi_cut.Source_cut
     """
     if sector is None:
         source_name = f'source_{target}'
-    elif sector is True:
+    elif sector == 'first':
         source_name = f'source_{target}_earliest_sector'
+    elif sector == 'last':
+        source_name = f'source_{target}_last_sector'
     else:
         source_name = f'source_{target}_sector_{sector}'
     source_exists = exists(f'{local_directory}source/{source_name}.pkl')
     if source_exists and os.path.getsize(f'{local_directory}source/{source_name}.pkl') > 0:
         with open(f'{local_directory}source/{source_name}.pkl', 'rb') as input_:
             source = pickle.load(input_)
         print(source.sector_table)
         print('Loaded ffi_cut from directory. ')
     else:
         with open(f'{local_directory}source/{source_name}.pkl', 'wb') as output:
-            source = Source_cut(target, size=size, sector=sector)
+            source = Source_cut(target, size=size, sector=sector, limit_mag=limit_mag)
             pickle.dump(source, output, pickle.HIGHEST_PROTOCOL)
     return source
```

### Comparing `tglc-0.5.7/tglc/lc_plot.py` & `tglc-0.5.8/tglc/lc_plot.py`

 * *Files identical despite different names*

### Comparing `tglc-0.5.7/tglc/mast.py` & `tglc-0.5.8/tglc/mast.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,20 +34,20 @@
     time.sleep(i)
     cam = 1 + i // 4
     ccd = 1 + i % 4
     zip_file = f'/home/tehan/data/mast/sector{sector:04d}/sector_{sector}_cam_{cam}_ccd_{ccd}'
     original_file = f'/home/tehan/data/sector{sector:04d}/lc/{cam}-{ccd}/'
     files = glob(f'{original_file}*.fits')
     if do_zip:
-        num_zips = int(len(files) // lc_num_per_zip + 1)
-        for i in range(num_zips):
-            with zipfile.ZipFile(f'{zip_file}_{i:02d}.zip', 'w') as zipMe:
-                for file in files[int(i * lc_num_per_zip):int((i + 1) * lc_num_per_zip)]:
-                    zipMe.write(file, compress_type=zipfile.ZIP_DEFLATED)
-        # shutil.make_archive(zip_file, 'zip', original_file)
+        # num_zips = int(len(files) // lc_num_per_zip + 1)
+        # for i in range(num_zips):
+            # with zipfile.ZipFile(f'{zip_file}_{i:02d}.zip', 'w') as zipMe:
+            #     for file in files[int(i * lc_num_per_zip):int((i + 1) * lc_num_per_zip)]:
+            #         zipMe.write(file, compress_type=zipfile.ZIP_DEFLATED)
+        shutil.make_archive(zip_file, 'zip', original_file)
         return
     else:
         ftps = ftplib.FTP_TLS('archive.stsci.edu')
         ftps.login('tehanhunter@gmail.com', getpass.getpass())
         ftps.prot_p()
         ftps.cwd('pub/hlsp/tglc/')
         print(f"Sector {sector}")
@@ -104,12 +104,13 @@
         os.makedirs(f'/home/tehan/data/cosmos/dominic_EB/sector{i:04d}/', exist_ok=True)
         with Pool(16) as p:
             p.map(partial(search_stars, sector=i, star_list=prsa_ebs), range(16))
     return
 
 
 if __name__ == '__main__':
-    # sector = 1
-    # filter_no_tic(sector=sector)
-    # hlsp_transfer(sector=sector, do_zip=True)
+    sector = 1
+    filter_no_tic(sector=sector)
+    hlsp_transfer(sector=sector, do_zip=True)
     # hlsp_transfer(sector=sector, do_zip=False)
-    star_spliter(server=1)  # star_list='/home/tehan/Documents/tglc/dominic_EB/eb_cat.txt'
+    # star_spliter(server=1)
+    # star_list='/home/tehan/Documents/tglc/dominic_EB/eb_cat.txt'
```

### Comparing `tglc-0.5.7/tglc/quick_lc.py` & `tglc-0.5.8/tglc/quick_lc.py`

 * *Files 22% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import numpy as np
 
 controller = ThreadpoolController()
 
 
 @controller.wrap(limits=1, user_api='blas')
 def tglc_lc(target='TIC 264468702', local_directory='', size=90, save_aper=True, limit_mag=16, get_all_lc=False,
-            first_sector_only=False, sector=None, prior=None):
+            first_sector_only=False, last_sector_only=False, sector=None, prior=None):
     '''
     Generate light curve for a single target.
 
     :param target: target identifier
     :type target: str, required
     :param local_directory: output directory
     :type local_directory: str, required
@@ -33,16 +33,19 @@
     :type size: int, optional
     '''
     os.makedirs(local_directory + f'logs/', exist_ok=True)
     os.makedirs(local_directory + f'lc/', exist_ok=True)
     os.makedirs(local_directory + f'epsf/', exist_ok=True)
     os.makedirs(local_directory + f'source/', exist_ok=True)
     if first_sector_only:
-        sector = True
-    source = ffi_cut(target=target, size=size, local_directory=local_directory, sector=sector)  # sector
+        sector = 'first'
+    elif last_sector_only:
+        sector = 'last'
+    source = ffi_cut(target=target, size=size, local_directory=local_directory, sector=sector,
+                     limit_mag=limit_mag)  # sector
     if get_all_lc:
         name = None
     else:
         catalogdata = Catalogs.query_object(str(target), radius=0.02, catalog="TIC")
         if target[0:3] == 'TIC':
             name = int(target[4:])
         else:
@@ -50,22 +53,28 @@
             print("Since the provided target is not TIC ID, the resulted light curve with get_all_lc=False can not be "
                   "guaranteed to be the target's light curve. Please check the TIC ID of the output file before using "
                   "the light curve or try use TIC ID as the target in the format of 'TIC 12345678'.")
     if type(sector) == int:
         source.select_sector(sector=sector)
         epsf(source, factor=2, sector=source.sector, target=target, local_directory=local_directory,
              name=name, limit_mag=limit_mag, save_aper=save_aper, prior=prior)
+    elif first_sector_only:
+        source.select_sector(sector=source.sector_table['sector'][0])
+        epsf(source, factor=2, sector=source.sector, target=target, local_directory=local_directory,
+             name=name, limit_mag=limit_mag, save_aper=save_aper, prior=prior)
+    elif last_sector_only:
+        source.select_sector(sector=source.sector_table['sector'][-1])
+        epsf(source, factor=2, sector=source.sector, target=target, local_directory=local_directory,
+             name=name, limit_mag=limit_mag, save_aper=save_aper, prior=prior)
     else:
         for j in range(len(source.sector_table)):
             # try:
             source.select_sector(sector=source.sector_table['sector'][j])
             epsf(source, factor=2, sector=source.sector, target=target, local_directory=local_directory,
                  name=name, limit_mag=limit_mag, save_aper=save_aper, prior=prior)
-            if first_sector_only:
-                break
 
 
 def search_stars(i, sector=1, tics=None, local_directory=None):
     cam = 1 + i // 4
     ccd = 1 + i % 4
     files = glob(f'/home/tehan/data/sector{sector:04d}/lc/{cam}-{ccd}/hlsp_*.fits')
     for j in trange(len(files)):
@@ -82,115 +91,185 @@
                  tics=None, local_directory=None):
     for i in range(server, 27, 2):
         with Pool(16) as p:
             p.map(partial(search_stars, sector=i, tics=tics, local_directory=local_directory), range(16))
     return
 
 
-def plot_lc(local_directory=None):
+def plot_lc(local_directory=None, type='cal_aper_flux'):
     files = glob(f'{local_directory}*.fits')
     os.makedirs(f'{local_directory}plots/', exist_ok=True)
     for i in range(len(files)):
         with fits.open(files[i], mode='denywrite') as hdul:
             q = [a and b for a, b in zip(list(hdul[1].data['TESS_flags'] == 0), list(hdul[1].data['TGLC_flags'] == 0))]
             plt.figure(constrained_layout=False, figsize=(8, 4))
-            plt.plot(hdul[1].data['time'], hdul[1].data['cal_aper_flux'], '.', c='silver', label='cal_aper')
-            plt.plot(hdul[1].data['time'][q], hdul[1].data['cal_aper_flux'][q], '.k', label='cal_aper_flagged')
+            plt.plot(hdul[1].data['time'], hdul[1].data[type], '.', c='silver', label=type)
+            plt.plot(hdul[1].data['time'][q], hdul[1].data[type][q], '.k', label=f'{type}_flagged')
             # plt.xlim(2845, 2855)
+            plt.ylim(0.5, 1.5)
+            plt.title(f'TIC_{hdul[0].header["TICID"]}_sector_{hdul[0].header["SECTOR"]:04d}_{type}')
+            plt.legend()
+            # plt.show()
+            plt.savefig(
+                f'{local_directory}plots/TIC_{hdul[0].header["TICID"]}_sector_{hdul[0].header["SECTOR"]:04d}.png',
+                dpi=300)
+            plt.close()
+
+
+def plot_aperture(local_directory=None, type='cal_aper_flux'):
+    files = glob(f'{local_directory}*.fits')
+    os.makedirs(f'{local_directory}plots/', exist_ok=True)
+    portion = [0.9361215204370542, 0.9320709087810205]
+    data = np.empty((3, 0))
+
+    for i in range(len(files)):
+        with fits.open(files[i], mode='denywrite') as hdul:
+            print(files[i], portion[i])
+            q = [a and b for a, b in zip(list(hdul[1].data['TESS_flags'] == 0), list(hdul[1].data['TGLC_flags'] == 0))]
+            plt.figure(constrained_layout=False, figsize=(8, 4))
+            plt.plot(hdul[1].data['time'] % 3.79262026, hdul[1].data[type], '.', c='silver', label=type)
+            plt.plot(hdul[1].data['time'][q] % 3.79262026, hdul[1].data[type][q], '.k', label=f'{type}_flagged')
+            aperture_bar = 709.5512462444653 * portion[i]
+            aper_lc = np.nansum(hdul[0].data, axis=(1, 2))
+            local_bg = np.nanmedian(aper_lc) - aperture_bar
+            aper_lc = (aper_lc - local_bg) / portion[i]
+            cal_aper_lc = aper_lc / np.nanmedian(aper_lc)
+            cal_aper_lc[np.where(cal_aper_lc > 100)] = np.nan
+            _, trend = flatten(hdul[1].data['time'], cal_aper_lc - np.nanmin(cal_aper_lc) + 1000,
+                               window_length=1, method='biweight', return_trend=True)
+            cal_aper_lc = (cal_aper_lc - np.nanmin(cal_aper_lc) + 1000 - trend) / np.nanmedian(cal_aper_lc) + 1
+            non_outliers = np.where(cal_aper_lc[q] > 0.6)[0]
+            plt.plot(hdul[1].data['time'][q][non_outliers] % 3.79262026, cal_aper_lc[q][non_outliers], '.r',
+                     label=f'5_5_pixel_flagged')
+            plt.xlim(0.5, 1.0)
+            plt.ylim(0.95, 1.1)
             plt.title(f'TIC_{hdul[0].header["TICID"]}_sector_{hdul[0].header["SECTOR"]:04d}')
             plt.legend()
             # plt.show()
             plt.savefig(
                 f'{local_directory}plots/TIC_{hdul[0].header["TICID"]}_sector_{hdul[0].header["SECTOR"]:04d}.png',
                 dpi=300)
+            time = hdul[1].data['time'][q][non_outliers]
+            flux = cal_aper_lc[q][non_outliers]
+            f_err = 1.4826 * np.nanmedian(np.abs(flux - np.nanmedian(flux)))
+            not_nan = np.invert(np.isnan(flux))
+            data_ = np.array([time[not_nan],
+                              flux[not_nan],
+                              np.array([f_err] * len(time[not_nan]))
+                              ])
+            data = np.append(data, data_, axis=1)
+    np.savetxt(f'{local_directory}TESS_TOI-5344_5_5_aper.csv', data, delimiter=',')
 
 
-def plot_pf_lc(local_directory=None, period=None):
+def plot_pf_lc(local_directory=None, period=None, type='cal_aper_flux'):
     files = glob(f'{local_directory}*.fits')
     os.makedirs(f'{local_directory}plots/', exist_ok=True)
     fig = plt.figure(figsize=(13, 5))
     for j in range(len(files)):
         not_plotted_num = 0
         with fits.open(files[j], mode='denywrite') as hdul:
             q = [a and b for a, b in
                  zip(list(hdul[1].data['TESS_flags'] == 0), list(hdul[1].data['TGLC_flags'] == 0))]
             if len(hdul[1].data['cal_aper_flux']) == len(hdul[1].data['time']):
                 if hdul[0].header["SECTOR"] <= 26:
                     t = hdul[1].data['time'][q]
-                    f = hdul[1].data['cal_psf_flux'][q]
-                else:
+                    f = hdul[1].data[type][q]
+                elif hdul[0].header["SECTOR"] <= 55:
                     t = np.mean(hdul[1].data['time'][q][:len(hdul[1].data['time'][q]) // 3 * 3].reshape(-1, 3), axis=1)
                     f = np.mean(
-                        hdul[1].data['cal_aper_flux'][q][:len(hdul[1].data['cal_aper_flux'][q]) // 3 * 3].reshape(-1,
-                                                                                                                  3),
-                        axis=1)
-                plt.plot(hdul[1].data['time'] % period / period, hdul[1].data['cal_aper_flux'], '.', c=f'C{j}', ms=2)
-                plt.errorbar(t % period / period, f, hdul[1].header['CAPE_ERR'], c=f'C{j}', ls='', elinewidth=0,
+                        hdul[1].data[type][q][:len(hdul[1].data[type][q]) // 3 * 3].reshape(-1, 3), axis=1)
+                else:
+                    t = np.mean(hdul[1].data['time'][q][:len(hdul[1].data['time'][q]) // 9 * 9].reshape(-1, 9), axis=1)
+                    f = np.mean(
+                        hdul[1].data[type][q][:len(hdul[1].data[type][q]) // 9 * 9].reshape(-1, 9), axis=1)
+                plt.plot(hdul[1].data['time'] % period / period, hdul[1].data[type], '.', c='silver', ms=2)
+                plt.errorbar(t % period / period, f, hdul[1].header['CAPE_ERR'], c=f'C{j}', ls='', elinewidth=1,
                              marker='.', ms=2, zorder=2, label=f'Sector {hdul[0].header["sector"]}')
-                #
             else:
                 not_plotted_num += 1
-            title = f'TIC_{hdul[0].header["TICID"]} with {len(files) - not_plotted_num} sector(s) of data'
+            title = f'TIC_{hdul[0].header["TICID"]} with {len(files) - not_plotted_num} sector(s) of data, {type}'
     # PDCSAP_files = glob('/home/tehan/Documents/GEMS/TIC 172370679/PDCSAP/*.txt')
     # for i in range(len(files)):
     #     PDCSAP = ascii.read(PDCSAP_files[i])
     #     t = np.mean(PDCSAP['col1'][:len(PDCSAP['col1']) // 15 * 15].reshape(-1, 15), axis=1)
     #     f = np.mean(PDCSAP['col2'][:len(PDCSAP['col2']) // 15 * 15].reshape(-1, 15), axis=1)
     #     ferr = np.mean(PDCSAP['col3'][:len(PDCSAP['col3']) // 15 * 15].reshape(-1, 15), axis=1)
     #     plt.errorbar((t - 2457000) % period / period, f, ferr, c='C0', ls='', elinewidth=0, marker='.', ms=2, zorder=1)
     # plt.ylim(0.94, 1.025)
     # plt.xlim(0.84, 0.86)
     plt.legend()
     plt.title(title)
-    plt.xlabel('Phase (days)')
+    plt.xlim(0.16, 0.26)
+    plt.ylim(0.9, 1.1)
+    plt.xlabel('Phase')
     plt.ylabel('Normalized flux')
     plt.savefig(f'{local_directory}/plots/{title}.png', dpi=300)
     plt.close(fig)
 
 
 def plot_contamination(local_directory=None, gaia_dr3=None):
     files = glob(f'{local_directory}lc/*.fits')
+    os.makedirs(f'{local_directory}lc/plots/', exist_ok=True)
     for i in range(len(files)):
         with open(glob(f'{local_directory}source/*.pkl')[0], 'rb') as input_:
             with fits.open(files[i], mode='denywrite') as hdul:
                 sector = hdul[0].header['SECTOR']
                 source = pickle.load(input_)
                 source.select_sector(sector=sector)
                 star_num = np.where(source.gaia['DESIGNATION'] == f'Gaia DR3 {gaia_dr3}')
                 # print(source.gaia[891])
                 # print(source.gaia[140])
                 nearby_stars = np.argsort(
-                    (source.gaia[f'sector_{sector}_x'][:1000] - source.gaia[star_num][f'sector_{sector}_x']) ** 2 +
-                    (source.gaia[f'sector_{sector}_y'][:1000] - source.gaia[star_num][f'sector_{sector}_y']) ** 2)[1:10]
+                    (source.gaia[f'sector_{sector}_x'][:500] - source.gaia[star_num][f'sector_{sector}_x']) ** 2 +
+                    (source.gaia[f'sector_{sector}_y'][:500] - source.gaia[star_num][f'sector_{sector}_y']) ** 2)[0:5]
                 # print(f'sector = {source.sector}')
                 star_x = source.gaia[star_num][f'sector_{sector}_x'][0]
                 star_y = source.gaia[star_num][f'sector_{sector}_y'][0]
                 max_flux = np.max(
                     np.median(source.flux[:, round(star_y) - 2:round(star_y) + 3, round(star_x) - 2:round(star_x) + 3],
                               axis=0))
                 fig = plt.figure(constrained_layout=False, figsize=(15, 7))
                 gs = fig.add_gridspec(5, 10)
                 gs.update(wspace=0.5, hspace=0.5)
                 ax0 = fig.add_subplot(gs[:5, :5])
                 ax0.imshow(source.flux[0], cmap='RdBu', vmin=-max_flux, vmax=max_flux, origin='lower')
 
-                ax0.scatter(source.gaia[f'sector_{sector}_x'][:1000], source.gaia[f'sector_{sector}_y'][:1000], s=50,
+                ax0.scatter(source.gaia[f'sector_{sector}_x'][:500], source.gaia[f'sector_{sector}_y'][:500], s=50,
                             c='r', label='background stars')
                 ax0.scatter(source.gaia[f'sector_{sector}_x'][nearby_stars],
                             source.gaia[f'sector_{sector}_y'][nearby_stars], s=50,
                             c='r', label='background stars')
                 for l in range(len(nearby_stars)):
                     index = np.where(
                         source.tic['dr3_source_id'] == int(source.gaia['DESIGNATION'][nearby_stars[l]].split(' ')[-1]))
+                    gaia_targets = source.gaia
+                    median_time = np.median(source.time)
+                    interval = (median_time - 388.5) / 365.25 + 3000
+                    ra = gaia_targets['ra'][nearby_stars[l]]
+                    dec = gaia_targets['dec'][nearby_stars[l]]
+                    if not np.isnan(gaia_targets['pmra'][nearby_stars[l]]):
+                        ra += gaia_targets['pmra'][nearby_stars[l]] * np.cos(np.deg2rad(dec)) * interval / 1000 / 3600
+                    if not np.isnan(gaia_targets['pmdec'][nearby_stars[l]]):
+                        dec += gaia_targets['pmdec'][nearby_stars[l]] * interval / 1000 / 3600
+                    pixel = source.wcs.all_world2pix(np.array([ra, dec]).reshape((1, 2)), 0)
+                    x_gaia = pixel[0][0]
+                    y_gaia = pixel[0][1]
+                    ax0.arrow(source.gaia[f'sector_{sector}_x'][nearby_stars[l]],
+                              source.gaia[f'sector_{sector}_y'][nearby_stars[l]],
+                              x_gaia - source.gaia[f'sector_{sector}_x'][nearby_stars[l]],
+                              y_gaia - source.gaia[f'sector_{sector}_y'][nearby_stars[l]],
+                              width=0.02, color='r', edgecolor=None, head_width=0.1)
                     try:
                         ax0.text(source.gaia[f'sector_{sector}_x'][nearby_stars[l]] - 0.1,
-                                    source.gaia[f'sector_{sector}_y'][nearby_stars[l]] + 0.2,
-                                    f'TIC {int(source.tic["TIC"][index])}', rotation=90)
+                                 source.gaia[f'sector_{sector}_y'][nearby_stars[l]] + 0.3,
+                                 f'TIC {int(source.tic["TIC"][index])}', rotation=90)
                     except TypeError:
-                        pass
+                        ax0.text(source.gaia[f'sector_{sector}_x'][nearby_stars[l]] - 0.1,
+                                 source.gaia[f'sector_{sector}_y'][nearby_stars[l]] + 0.2,
+                                 f'{source.gaia[f"DESIGNATION"][nearby_stars[l]]}', rotation=90)
                 ax0.scatter(star_x, star_y, s=300, c='r', marker='*', label='target star')
 
                 # ax0.legend()
                 ax0.set_xlim(round(star_x) - 5.5, round(star_x) + 5.5)
                 ax0.set_ylim(round(star_y) - 5.5, round(star_y) + 5.5)
                 ax0.set_title(f'TIC_{hdul[0].header["TICID"]}_sector_{hdul[0].header["SECTOR"]:04d}')
                 ax0.vlines(round(star_x) - 2.5, round(star_y) - 2.5, round(star_y) + 2.5, colors='k')
@@ -210,76 +289,67 @@
                 t_, y_, x_ = np.shape(hdul[0].data)
                 max_flux = np.max(
                     np.median(source.flux[:, int(star_y) - 2:int(star_y) + 3, int(star_x) - 2:int(star_x) + 3], axis=0))
                 for j in range(y_):
                     for k in range(x_):
                         ax_ = fig.add_subplot(gs[(4 - j), (5 + k)])
                         ax_.patch.set_facecolor('C0')
-                        ax_.patch.set_alpha(min(1, max(0, 3 * np.median(hdul[0].data[:, j, k]) / max_flux)))
+                        ax_.patch.set_alpha(min(1, max(0, 5 * np.nanmedian(hdul[0].data[:, j, k]) / max_flux)))
                         q = [a and b for a, b in
                              zip(list(hdul[1].data['TESS_flags'] == 0), list(hdul[1].data['TGLC_flags'] == 0))]
 
                         _, trend = flatten(hdul[1].data['time'][q],
-                                           hdul[0].data[:, j, k][q] - np.min(hdul[0].data[:, j, k][q]) + 1000,
+                                           hdul[0].data[:, j, k][q] - np.nanmin(hdul[0].data[:, j, k][q]) + 1000,
                                            window_length=1, method='biweight', return_trend=True)
-                        cal_aper = (hdul[0].data[:, j, k][q] - np.min(
-                            hdul[0].data[:, j, k][q]) + 1000 - trend) / np.median(
+                        cal_aper = (hdul[0].data[:, j, k][q] - np.nanmin(
+                            hdul[0].data[:, j, k][q]) + 1000 - trend) / np.nanmedian(
                             hdul[0].data[:, j, k][q]) + 1
                         ax_.plot(hdul[1].data['time'][q], cal_aper, '.k', ms=1, label='center pixel')
+                        ax_.set_ylim(0.95, 1.05)
                 plt.savefig(f'{local_directory}lc/plots/contamination_sector_{hdul[0].header["SECTOR"]:04d}.pdf',
                             dpi=300)
                 plt.show()
 
 
-def choose_prior(local_directory=None, priors=np.logspace(-5, 0, 100)):
-    mad = np.zeros((5, 100))
+def choose_prior(tics, local_directory=None, priors=np.logspace(-5, 0, 100)):
+    mad = np.zeros((2, 100))
     for i in trange(len(priors)):
-        get_tglc_lc(tics=tics, method='query', server=1, directory=local_directory, prior=priors[i])
-        with fits.open(
-                '/home/tehan/data/cosmos/GEMS/TIC 172370679/lc/hlsp_tglc_tess_ffi_gaiaid-2073530190996615424-s0014-cam1-ccd1_tess_v1_llc.fits',
-                mode='denywrite') as hdul:
-            mad[0, i] = np.median(abs(hdul[1].data['cal_psf_flux'] - np.median(hdul[1].data['cal_psf_flux'])))
-        with fits.open(
-                '/home/tehan/data/cosmos/GEMS/TIC 172370679/lc/hlsp_tglc_tess_ffi_gaiaid-2073530190996615424-s0015-cam1-ccd2_tess_v1_llc.fits',
-                mode='denywrite') as hdul:
-            mad[1, i] = np.median(abs(hdul[1].data['cal_psf_flux'] - np.median(hdul[1].data['cal_psf_flux'])))
-        with fits.open(
-                '/home/tehan/data/cosmos/GEMS/TIC 172370679/lc/hlsp_tglc_tess_ffi_gaiaid-2073530190996615424-s0041-cam1-ccd1_tess_v1_llc.fits',
-                mode='denywrite') as hdul:
-            mad[2, i] = np.median(abs(hdul[1].data['cal_psf_flux'] - np.median(hdul[1].data['cal_psf_flux'])))
-        with fits.open(
-                '/home/tehan/data/cosmos/GEMS/TIC 172370679/lc/hlsp_tglc_tess_ffi_gaiaid-2073530190996615424-s0054-cam3-ccd2_tess_v1_llc.fits',
-                mode='denywrite') as hdul:
-            mad[3, i] = np.median(abs(hdul[1].data['cal_psf_flux'] - np.median(hdul[1].data['cal_psf_flux'])))
-        with fits.open(
-                '/home/tehan/data/cosmos/GEMS/TIC 172370679/lc/hlsp_tglc_tess_ffi_gaiaid-2073530190996615424-s0055-cam3-ccd1_tess_v1_llc.fits',
-                mode='denywrite') as hdul:
-            mad[4, i] = np.median(abs(hdul[1].data['cal_psf_flux'] - np.median(hdul[1].data['cal_psf_flux'])))
-    np.save('/home/tehan/data/cosmos/GEMS/TIC 172370679/mad.npy', mad)
+        resid = get_tglc_lc(tics=tics, method='query', server=1, directory=local_directory, prior=priors[i])
+        print(resid)
+        mad[:, i] = resid
+        # with fits.open(
+        #         '/home/tehan/data/cosmos/GEMS/TIC 16005254/lc/hlsp_tglc_tess_ffi_gaiaid-52359538285081728-s0043-cam3-ccd3_tess_v1_llc.fits',
+        #         mode='denywrite') as hdul:
+        #     mad[0, i] = np.nanmedian(abs(hdul[1].data['cal_psf_flux'] - np.nanmedian(hdul[1].data['cal_psf_flux'])))
+        # with fits.open(
+        #         '/home/tehan/data/cosmos/GEMS/TIC 16005254/lc/hlsp_tglc_tess_ffi_gaiaid-52359538285081728-s0044-cam1-ccd1_tess_v1_llc.fits',
+        #         mode='denywrite') as hdul:
+        #     mad[1, i] = np.nanmedian(abs(hdul[1].data['cal_psf_flux'] - np.nanmedian(hdul[1].data['cal_psf_flux'])))
+    np.save('/home/tehan/Documents/GEMS/TIC 16005254/mad.npy', mad)
     # plt.plot(priors, mad)
     # plt.xscale('log')
     # plt.title(f'best prior = {priors[np.argmin(mad)]:04d}')
     # plt.show()
 
 
 def get_tglc_lc(tics=None, method='query', server=1, directory=None, prior=None):
     if method == 'query':
         for i in range(len(tics)):
             target = f'TIC {tics[i]}'
             local_directory = f'{directory}{target}/'
             os.makedirs(local_directory, exist_ok=True)
-            tglc_lc(target=target, local_directory=local_directory, size=90, save_aper=True, limit_mag=16,
-                    get_all_lc=False, first_sector_only=False, sector=None, prior=prior)
+            tglc_lc(target=target, local_directory=local_directory, size=90, save_aper=False, limit_mag=16,
+                    get_all_lc=False, first_sector_only=False, last_sector_only=True, sector=None, prior=prior)
     if method == 'search':
         star_spliter(server=server, tics=tics, local_directory=directory)
 
 
 if __name__ == '__main__':
-    tics = [119585136]
+    tics = [11893637]
     directory = f'/home/tehan/data/cosmos/GEMS/'
     os.makedirs(directory, exist_ok=True)
     get_tglc_lc(tics=tics, method='query', server=1, directory=directory)
-    # plot_contamination(local_directory=f'{directory}TIC 27858644/', gaia_dr3=2091177593123254016)
-    # plot_contamination(local_directory=f'{directory}TIC 172370679/', gaia_dr3=2073530190996615424)
-    # plot_lc(local_directory=f'{directory}TIC 135272255/lc/')
-    # plot_pf_lc(local_directory=f'{directory}TIC 27858644/lc/', period=384)
-    # choose_prior(local_directory=directory)
+    plot_lc(local_directory=f'{directory}TIC {tics[0]}/lc/', type='cal_aper_flux')
+    # plot_aperture(local_directory=f'{directory}TIC {tics[0]}/lc/', type='cal_aper_flux')
+    # plot_contamination(local_directory=f'{directory}TIC {tics[0]}/', gaia_dr3=52359538285081728)
+    # plot_pf_lc(local_directory=f'{directory}TIC {tics[0]}/lc/', period=3.7926244)
+    # choose_prior(tics, local_directory=directory)
```

### Comparing `tglc-0.5.7/tglc/run.py` & `tglc-0.5.8/tglc/run.py`

 * *Files identical despite different names*

### Comparing `tglc-0.5.7/tglc/source_output.py` & `tglc-0.5.8/tglc/source_output.py`

 * *Files identical despite different names*

### Comparing `tglc-0.5.7/tglc/target_lightcurve.py` & `tglc-0.5.8/tglc/target_lightcurve.py`

 * *Files 2% similar despite different names*

```diff
@@ -274,17 +274,19 @@
     end = num_stars
     if name is not None:
         try:
             start = int(np.where(source.gaia['DESIGNATION'] == 'Gaia DR3 ' +
                                  str(source.tic['dr3_source_id'][np.where(source.tic['TIC'] == name)][0]))[0][0])
             end = start + 1
         except IndexError:
-            print(f'Target not found in the requested sector (Sector {sector}). It is possible that this target does '
-                  f'not have a Gaia ID. ')
-            return
+            print(f'Target not found in the requested sector (Sector {sector}). This can be caused by a lack of Gaia '
+                  f'ID or an incomplete TESS to Gaia crossmatch table. Please check whether the output light curve Gaia'
+                  f' DR3 ID agrees with your target.')
+            start = 0
+            end = 1
     for i in trange(start, end, desc='Fitting lc', disable=no_progress_bar):
         if x_left <= x_round[i] < source.size - x_right and y_left <= y_round[i] < source.size - y_right:
             if type(source) == Source:
                 x_left = 1.5
                 x_right = 2.5
                 y_left = 1.5
                 y_right = 2.5
```

### Comparing `tglc-0.5.7/tglc.egg-info/PKG-INFO` & `tglc-0.5.8/tglc.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tglc
-Version: 0.5.7
+Version: 0.5.8
 Summary: TESS-Gaia Light Curve
 Home-page: https://github.com/TeHanHunter/TESS_Gaia_Light_Curve
 Author: Te Han
 Author-email: tehanhunter@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -20,17 +20,17 @@
 
 ==================================
 Usage
 ==================================
 There are four fluxes in each FITS file: aperture flux, PSF flux, calibrated aperture flux, and calibrated PSF flux.
 If you are uncertain which to use:
 
-* Calibrated aperture flux is the most robust in transit depth. Use this if you are doing transit science.
-* Calibrated psf flux is better in deblending targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior.
-* The aperture flux and PSF flux are not detrended or normalized. Use this if you are doing stellar variability science. Or, if the detrending is not optimal (default detrending has a window length of 1 day), start with the aperture flux or PSF flux and detrend carefully!
+* Calibrated psf flux is better in **deblending** targets. Use this if you need to deblend a target near a variable source. The best deblending can be achieved with tglc package by setting a non-zero prior. It also gives the more accurate **transit depth** in most cases, especially when fitting with an optimized prior.
+* Calibrated aperture flux usually has slightly **higher SNR**. The transit depth (or variation amplitude), however, can be imperfect since the normalization depends on the PSF fitting which is imperfect. This imperfection can be minimized by using a bigger aperture than the default aperture (3*3). One need to use the tglc package and set tglc_lc(save_aper=True) to access the 5*5 aperture. In the presence of a bright but "constant" contamination (several magnitudes brighter), the calibrated aperture flux is better in removing the constant contamination. 
+* The aperture flux and PSF flux are not detrended or normalized. Use this if you are doing stellar variability science with long baseline. Or, if the detrending is not optimal (default detrending has a window length of 1 day; see Known Problems below), start with the aperture flux or PSF flux and detrend carefully!
 * **If you are uncertain, start with calibrated aperture flux!**
 
 The `tutorial <tutorial/TGLC_tutorial.ipynb>`_ shows the syntaxes and differences among these light curves in several examples.
 
 ==================================
 Data Access
 ==================================
@@ -56,13 +56,14 @@
 for the latest tglc release. After installation, follow the `tutorial <tutorial/TGLC_tutorial.ipynb>`_ to fit light curves. If there is a problem, please leave a comment in the Issues section to help us improve. Thank you!
 
 
 ==================================
 Known Problems
 ==================================
 There are several imperfections we noticed in the MAST TGLC light curves and tglc package:
-* If the star is very dim (~< 15 Tmag) near a variable source, it can make the aperture and/or PSF light curve negative for some cadences. This is a very rare scenario, but could be important. The detrending algorithm could malfunction and result in bad cal_aper_flux and/or cal_psf_flux. This is now fixed for tglc package, but this problem remains for the primary mission light curves published on MAST. Please detrend again if necessary. We will also correct for the extended mission light curves on MAST.
+
+* If the star is very dim (~< 15 Tmag) near a variable source, it can make the aperture and/or PSF light curve negative for some cadences. The detrending algorithm could malfunction and result in bad cal_aper_flux and/or cal_psf_flux. This is now fixed for tglc package, but this problem remains for the primary mission light curves published on MAST. Please detrend again if necessary.The extended mission light curves on MAST will not be affected. This is a very rare scenario, but could be important.
 
 ==================================
 Reference
 ==================================
 If you find the TGLC light curves or the tglc package useful in your research, please cite `our paper <https://iopscience.iop.org/article/10.3847/1538-3881/acaaa7>`_ published on the Astronomical Journal.
```

