# Comparing `tmp/twirl-0.3.0.tar.gz` & `tmp/twirl-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twirl-0.3.0.tar", max compression
+gzip compressed data, was "twirl-0.3.1.tar", max compression
```

## Comparing `twirl-0.3.0.tar` & `twirl-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4932 2023-05-15 14:23:33.892014 twirl-0.3.0/README.md
--rw-r--r--   0        0        0     3077 2023-05-15 14:23:33.900014 twirl-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4126 2023-05-15 14:23:33.900014 twirl-0.3.0/twirl/__init__.py
--rw-r--r--   0        0        0     3535 2023-05-15 14:23:33.900014 twirl-0.3.0/twirl/geometry.py
--rw-r--r--   0        0        0     3520 2023-05-15 14:23:33.904014 twirl-0.3.0/twirl/match.py
--rw-r--r--   0        0        0     2145 2023-05-15 14:23:33.904014 twirl-0.3.0/twirl/quads.py
--rw-r--r--   0        0        0     2174 2023-05-15 14:23:33.904014 twirl-0.3.0/twirl/triangles.py
--rw-r--r--   0        0        0     5896 1970-01-01 00:00:00.000000 twirl-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     4918 2023-05-16 16:44:56.831245 twirl-0.3.1/README.md
+-rw-r--r--   0        0        0     3076 2023-05-16 16:44:56.839245 twirl-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4126 2023-05-16 16:44:56.839245 twirl-0.3.1/twirl/__init__.py
+-rw-r--r--   0        0        0     3535 2023-05-16 16:44:56.839245 twirl-0.3.1/twirl/geometry.py
+-rw-r--r--   0        0        0     3520 2023-05-16 16:44:56.839245 twirl-0.3.1/twirl/match.py
+-rw-r--r--   0        0        0     2145 2023-05-16 16:44:56.839245 twirl-0.3.1/twirl/quads.py
+-rw-r--r--   0        0        0     2174 2023-05-16 16:44:56.839245 twirl-0.3.1/twirl/triangles.py
+-rw-r--r--   0        0        0     5981 1970-01-01 00:00:00.000000 twirl-0.3.1/PKG-INFO
```

### Comparing `twirl-0.3.0/README.md` & `twirl-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 twirl compute a WCS following these steps:
 
 1. detection of stars in the image if not provided
 2. catalog query using image known center
 3. asterisms building and matching
 4. image recombination and wcs fit using astropy.wcs
 
-Astersims are of 3 or 4 points. 4 points asterisms are built following Lang et al. 2009 while 3 points asterims are based on a novel  algorithm (paper in preparation).
+Astersisms are made of 3 or 4 points. 4 points asterisms are built following Lang et al. 2009 while 3 points asterims are based on an original algorithm.
 
 ---
 
 ## Installation
 
 twirl can be installed using pip:
```

#### html2text {}

```diff
@@ -4,55 +4,54 @@
                   [github] [license] [paper] [documentation]
 twirl is an astrometric plate solving package for Python. It is suited for
 cases where the Right Ascension and Declination (RA, dec) coordinates of the
 image center and the field of view is known, computing a World Coordinate
 System (WCS) based on GAIA reference stars. twirl compute a WCS following these
 steps: 1. detection of stars in the image if not provided 2. catalog query
 using image known center 3. asterisms building and matching 4. image
-recombination and wcs fit using astropy.wcs Astersims are of 3 or 4 points. 4
-points asterisms are built following Lang et al. 2009 while 3 points asterims
-are based on a novel algorithm (paper in preparation). --- ## Installation
-twirl can be installed using pip: ```shell pip install twirl ``` or using
-poetry: ```shell poetry add twirl ``` --- ## Example Usage twirl is designed to
-be complementary to the astropy package. It is used to compute a WCS from a set
-of stars detected in an image. As a prerequisite, star detection and plate
-solving is suited for when the image center and field of view are known. In
-this case, the image center and field of view can be provided as a SkyCoord
-object and a Quantity object respectively. Use any specified header that has
-been stored on the FITS primary HDU to obtain the center equatorial coordinate
-and field of view, for this example we will assum "RA" and "DEC" are the
-keywords for the center equatorial coordinate. ### Setup ```python import numpy
-as np from astropy.io import fits from astropy import units as u from
-astropy.coordinates import SkyCoord # Open some FITS image: hdul = fits.open
-("...") # ra, dec in degrees ra, dec = header["RA"], header["DEC"] # Provide
-the center as a SkyCoord object: center = SkyCoord(ra, dec, unit=["deg",
-"deg"]) center = [center.ra.value, center.dec.value] # Utilise the image shape
-and pixel size in arcseconds " to obtain the field of view in degrees: shape =
-data.shape # Pixel size in arcseconds: pixel = 0.66 * u.arcsec # Field of view
-in degrees: fov = np.max(shape)*pixel.to(u.deg).value ``` From here, we can
-pass the data, the center equatorial coordinate and the field-of-view to twirl
-to compute the World Coordinate System (WCS): ### Twirl Usage ```python import
-twirl # Find some starts in the image: stars = twirl.find_peaks(data)[0:15] #
-Compute the World Coordinate System: wcs = twirl.compute_wcs(stars, center,
-fov) ``` A more complete example is provided in [docs/notebooks](https://
-github.com/lgrcia/twirl/tree/master/docs/notebooks) --- ## Development ###
-Project Requirements - [Python](https://www.python.org/) 3.11.* - [Poetry]
-(https://python-poetry.org/) for Python package and environment management. ###
-Installing Dependencies The twirl project manages Python package dependencies
-using [Poetry](https://python-poetry.org/). You'll need to follow the
-instructions for installation there. Then you can start a shell session with
-the new environment with: ```console $ poetry shell ``` **N.B.** For
-development with vscode you will need to run the following command: ```console
-$ poetry config virtualenvs.in-project true ``` This will installed the poetry
-`.venv` in the root of the project and allow vscode to setup the environment
-correctly for development. To start development, install all of the
-dependencies as: ```console $ poetry install ``` **N.B.** _Ensure that any
-dependency changes are committed to source control, so everyone has a
-consistenct package dependecy list._ --- ## Acknowledgements This package has
-made use of the algorithm from Lang, D. et al. (2010). _Astrometry.net: Blind
-Astrometric Calibration of Arbitrary Astronomical Images_. The Astronomical
-Journal, 139(5), pp.1782â1800. [doi:10.1088/0004-6256/139/5/1782](https://
-iopscience.iop.org/article/10.1088/0004-6256/139/5/1782). implemented in
-Garcia, L. J. et al. (2022). prose: a Python framework for modular astronomical
-images processing. MNRAS, vol. 509, no. 4, pp. 4817â4828, 2022. [doi:10.1093/
-mnras/stab3113](https://academic.oup.com/mnras/article-abstract/509/4/4817/
-6414007).
+recombination and wcs fit using astropy.wcs Astersisms are made of 3 or 4
+points. 4 points asterisms are built following Lang et al. 2009 while 3 points
+asterims are based on an original algorithm. --- ## Installation twirl can be
+installed using pip: ```shell pip install twirl ``` or using poetry: ```shell
+poetry add twirl ``` --- ## Example Usage twirl is designed to be complementary
+to the astropy package. It is used to compute a WCS from a set of stars
+detected in an image. As a prerequisite, star detection and plate solving is
+suited for when the image center and field of view are known. In this case, the
+image center and field of view can be provided as a SkyCoord object and a
+Quantity object respectively. Use any specified header that has been stored on
+the FITS primary HDU to obtain the center equatorial coordinate and field of
+view, for this example we will assum "RA" and "DEC" are the keywords for the
+center equatorial coordinate. ### Setup ```python import numpy as np from
+astropy.io import fits from astropy import units as u from astropy.coordinates
+import SkyCoord # Open some FITS image: hdul = fits.open("...") # ra, dec in
+degrees ra, dec = header["RA"], header["DEC"] # Provide the center as a
+SkyCoord object: center = SkyCoord(ra, dec, unit=["deg", "deg"]) center =
+[center.ra.value, center.dec.value] # Utilise the image shape and pixel size in
+arcseconds " to obtain the field of view in degrees: shape = data.shape # Pixel
+size in arcseconds: pixel = 0.66 * u.arcsec # Field of view in degrees: fov =
+np.max(shape)*pixel.to(u.deg).value ``` From here, we can pass the data, the
+center equatorial coordinate and the field-of-view to twirl to compute the
+World Coordinate System (WCS): ### Twirl Usage ```python import twirl # Find
+some starts in the image: stars = twirl.find_peaks(data)[0:15] # Compute the
+World Coordinate System: wcs = twirl.compute_wcs(stars, center, fov) ``` A more
+complete example is provided in [docs/notebooks](https://github.com/lgrcia/
+twirl/tree/master/docs/notebooks) --- ## Development ### Project Requirements -
+[Python](https://www.python.org/) 3.11.* - [Poetry](https://python-poetry.org/
+) for Python package and environment management. ### Installing Dependencies
+The twirl project manages Python package dependencies using [Poetry](https://
+python-poetry.org/). You'll need to follow the instructions for installation
+there. Then you can start a shell session with the new environment with:
+```console $ poetry shell ``` **N.B.** For development with vscode you will
+need to run the following command: ```console $ poetry config virtualenvs.in-
+project true ``` This will installed the poetry `.venv` in the root of the
+project and allow vscode to setup the environment correctly for development. To
+start development, install all of the dependencies as: ```console $ poetry
+install ``` **N.B.** _Ensure that any dependency changes are committed to
+source control, so everyone has a consistenct package dependecy list._ --- ##
+Acknowledgements This package has made use of the algorithm from Lang, D. et
+al. (2010). _Astrometry.net: Blind Astrometric Calibration of Arbitrary
+Astronomical Images_. The Astronomical Journal, 139(5), pp.1782â1800. [doi:
+10.1088/0004-6256/139/5/1782](https://iopscience.iop.org/article/10.1088/0004-
+6256/139/5/1782). implemented in Garcia, L. J. et al. (2022). prose: a Python
+framework for modular astronomical images processing. MNRAS, vol. 509, no. 4,
+pp. 4817â4828, 2022. [doi:10.1093/mnras/stab3113](https://academic.oup.com/
+mnras/article-abstract/509/4/4817/6414007).
```

### Comparing `twirl-0.3.0/pyproject.toml` & `twirl-0.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twirl"
-version = "0.3.0"
+version = "0.3.1"
 description = "Astrometric plate solving in Python"
 authors = [
   "Lionel J. Garcia <lionel_garcia@live.fr>"
 ]
 maintainers = [
   "Lionel J. Garcia <lionel_garcia@live.fr>",
   "Michael J. Roberts <michael@observerly.com>"
@@ -12,15 +12,15 @@
 license = "MIT"
 readme = "README.md"
 homepage = "https://twirl.readthedocs.io"
 repository = "https://github.com/lgrcia/twirl"
 keywords = ["astronomy", "astrometry", "plate-solving"]
 
 [tool.poetry.dependencies]
-python = "^3.10"
+python = "^3.8"
 astropy = "^5.1.1"
 astroquery = "^0.4.6"
 matplotlib = "^3.6.2"
 numpy = "^1.23.5"
 requests = "^2.28.1"
 scikit-image = "^0.20.0"
 scipy = "^1.9.3"
```

### Comparing `twirl-0.3.0/twirl/__init__.py` & `twirl-0.3.1/twirl/__init__.py`

 * *Files identical despite different names*

### Comparing `twirl-0.3.0/twirl/geometry.py` & `twirl-0.3.1/twirl/geometry.py`

 * *Files identical despite different names*

### Comparing `twirl-0.3.0/twirl/match.py` & `twirl-0.3.1/twirl/match.py`

 * *Files identical despite different names*

### Comparing `twirl-0.3.0/twirl/quads.py` & `twirl-0.3.1/twirl/quads.py`

 * *Files identical despite different names*

### Comparing `twirl-0.3.0/twirl/triangles.py` & `twirl-0.3.1/twirl/triangles.py`

 * *Files identical despite different names*

### Comparing `twirl-0.3.0/PKG-INFO` & `twirl-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 Metadata-Version: 2.1
 Name: twirl
-Version: 0.3.0
+Version: 0.3.1
 Summary: Astrometric plate solving in Python
 Home-page: https://twirl.readthedocs.io
 License: MIT
 Keywords: astronomy,astrometry,plate-solving
 Author: Lionel J. Garcia
 Author-email: lionel_garcia@live.fr
 Maintainer: Lionel J. Garcia
 Maintainer-email: lionel_garcia@live.fr
-Requires-Python: >=3.10,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: astropy (>=5.1.1,<6.0.0)
 Requires-Dist: astroquery (>=0.4.6,<0.5.0)
 Requires-Dist: matplotlib (>=3.6.2,<4.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
@@ -55,15 +57,15 @@
 twirl compute a WCS following these steps:
 
 1. detection of stars in the image if not provided
 2. catalog query using image known center
 3. asterisms building and matching
 4. image recombination and wcs fit using astropy.wcs
 
-Astersims are of 3 or 4 points. 4 points asterisms are built following Lang et al. 2009 while 3 points asterims are based on a novel  algorithm (paper in preparation).
+Astersisms are made of 3 or 4 points. 4 points asterisms are built following Lang et al. 2009 while 3 points asterims are based on an original algorithm.
 
 ---
 
 ## Installation
 
 twirl can be installed using pip:
```

#### html2text {}

```diff
@@ -1,70 +1,71 @@
-Metadata-Version: 2.1 Name: twirl Version: 0.3.0 Summary: Astrometric plate
+Metadata-Version: 2.1 Name: twirl Version: 0.3.1 Summary: Astrometric plate
 solving in Python Home-page: https://twirl.readthedocs.io License: MIT
 Keywords: astronomy,astrometry,plate-solving Author: Lionel J. Garcia Author-
 email: lionel_garcia@live.fr Maintainer: Lionel J. Garcia Maintainer-email:
-lionel_garcia@live.fr Requires-Python: >=3.10,<4.0 Classifier: License :: OSI
+lionel_garcia@live.fr Requires-Python: >=3.8,<4.0 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
-Language :: Python :: 3.11 Provides-Extra: docs Requires-Dist: astropy
-(>=5.1.1,<6.0.0) Requires-Dist: astroquery (>=0.4.6,<0.5.0) Requires-Dist:
-matplotlib (>=3.6.2,<4.0.0) Requires-Dist: numpy (>=1.23.5,<2.0.0) Requires-
-Dist: requests (>=2.28.1,<3.0.0) Requires-Dist: scikit-image (>=0.20.0,<0.21.0)
-Requires-Dist: scipy (>=1.9.3,<2.0.0) Project-URL: Repository, https://
-github.com/lgrcia/twirl Description-Content-Type: text/markdown # twirl
+Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
+Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11 Provides-Extra: docs
+Requires-Dist: astropy (>=5.1.1,<6.0.0) Requires-Dist: astroquery
+(>=0.4.6,<0.5.0) Requires-Dist: matplotlib (>=3.6.2,<4.0.0) Requires-Dist:
+numpy (>=1.23.5,<2.0.0) Requires-Dist: requests (>=2.28.1,<3.0.0) Requires-
+Dist: scikit-image (>=0.20.0,<0.21.0) Requires-Dist: scipy (>=1.9.3,<2.0.0)
+Project-URL: Repository, https://github.com/lgrcia/twirl Description-Content-
+Type: text/markdown # twirl
       [https://github.com/lgrcia/twirl/blob/main/docs/_static/twirl.png]
                  Python package for astrometric plate solving
                   [github] [license] [paper] [documentation]
 twirl is an astrometric plate solving package for Python. It is suited for
 cases where the Right Ascension and Declination (RA, dec) coordinates of the
 image center and the field of view is known, computing a World Coordinate
 System (WCS) based on GAIA reference stars. twirl compute a WCS following these
 steps: 1. detection of stars in the image if not provided 2. catalog query
 using image known center 3. asterisms building and matching 4. image
-recombination and wcs fit using astropy.wcs Astersims are of 3 or 4 points. 4
-points asterisms are built following Lang et al. 2009 while 3 points asterims
-are based on a novel algorithm (paper in preparation). --- ## Installation
-twirl can be installed using pip: ```shell pip install twirl ``` or using
-poetry: ```shell poetry add twirl ``` --- ## Example Usage twirl is designed to
-be complementary to the astropy package. It is used to compute a WCS from a set
-of stars detected in an image. As a prerequisite, star detection and plate
-solving is suited for when the image center and field of view are known. In
-this case, the image center and field of view can be provided as a SkyCoord
-object and a Quantity object respectively. Use any specified header that has
-been stored on the FITS primary HDU to obtain the center equatorial coordinate
-and field of view, for this example we will assum "RA" and "DEC" are the
-keywords for the center equatorial coordinate. ### Setup ```python import numpy
-as np from astropy.io import fits from astropy import units as u from
-astropy.coordinates import SkyCoord # Open some FITS image: hdul = fits.open
-("...") # ra, dec in degrees ra, dec = header["RA"], header["DEC"] # Provide
-the center as a SkyCoord object: center = SkyCoord(ra, dec, unit=["deg",
-"deg"]) center = [center.ra.value, center.dec.value] # Utilise the image shape
-and pixel size in arcseconds " to obtain the field of view in degrees: shape =
-data.shape # Pixel size in arcseconds: pixel = 0.66 * u.arcsec # Field of view
-in degrees: fov = np.max(shape)*pixel.to(u.deg).value ``` From here, we can
-pass the data, the center equatorial coordinate and the field-of-view to twirl
-to compute the World Coordinate System (WCS): ### Twirl Usage ```python import
-twirl # Find some starts in the image: stars = twirl.find_peaks(data)[0:15] #
-Compute the World Coordinate System: wcs = twirl.compute_wcs(stars, center,
-fov) ``` A more complete example is provided in [docs/notebooks](https://
-github.com/lgrcia/twirl/tree/master/docs/notebooks) --- ## Development ###
-Project Requirements - [Python](https://www.python.org/) 3.11.* - [Poetry]
-(https://python-poetry.org/) for Python package and environment management. ###
-Installing Dependencies The twirl project manages Python package dependencies
-using [Poetry](https://python-poetry.org/). You'll need to follow the
-instructions for installation there. Then you can start a shell session with
-the new environment with: ```console $ poetry shell ``` **N.B.** For
-development with vscode you will need to run the following command: ```console
-$ poetry config virtualenvs.in-project true ``` This will installed the poetry
-`.venv` in the root of the project and allow vscode to setup the environment
-correctly for development. To start development, install all of the
-dependencies as: ```console $ poetry install ``` **N.B.** _Ensure that any
-dependency changes are committed to source control, so everyone has a
-consistenct package dependecy list._ --- ## Acknowledgements This package has
-made use of the algorithm from Lang, D. et al. (2010). _Astrometry.net: Blind
-Astrometric Calibration of Arbitrary Astronomical Images_. The Astronomical
-Journal, 139(5), pp.1782â1800. [doi:10.1088/0004-6256/139/5/1782](https://
-iopscience.iop.org/article/10.1088/0004-6256/139/5/1782). implemented in
-Garcia, L. J. et al. (2022). prose: a Python framework for modular astronomical
-images processing. MNRAS, vol. 509, no. 4, pp. 4817â4828, 2022. [doi:10.1093/
-mnras/stab3113](https://academic.oup.com/mnras/article-abstract/509/4/4817/
-6414007).
+recombination and wcs fit using astropy.wcs Astersisms are made of 3 or 4
+points. 4 points asterisms are built following Lang et al. 2009 while 3 points
+asterims are based on an original algorithm. --- ## Installation twirl can be
+installed using pip: ```shell pip install twirl ``` or using poetry: ```shell
+poetry add twirl ``` --- ## Example Usage twirl is designed to be complementary
+to the astropy package. It is used to compute a WCS from a set of stars
+detected in an image. As a prerequisite, star detection and plate solving is
+suited for when the image center and field of view are known. In this case, the
+image center and field of view can be provided as a SkyCoord object and a
+Quantity object respectively. Use any specified header that has been stored on
+the FITS primary HDU to obtain the center equatorial coordinate and field of
+view, for this example we will assum "RA" and "DEC" are the keywords for the
+center equatorial coordinate. ### Setup ```python import numpy as np from
+astropy.io import fits from astropy import units as u from astropy.coordinates
+import SkyCoord # Open some FITS image: hdul = fits.open("...") # ra, dec in
+degrees ra, dec = header["RA"], header["DEC"] # Provide the center as a
+SkyCoord object: center = SkyCoord(ra, dec, unit=["deg", "deg"]) center =
+[center.ra.value, center.dec.value] # Utilise the image shape and pixel size in
+arcseconds " to obtain the field of view in degrees: shape = data.shape # Pixel
+size in arcseconds: pixel = 0.66 * u.arcsec # Field of view in degrees: fov =
+np.max(shape)*pixel.to(u.deg).value ``` From here, we can pass the data, the
+center equatorial coordinate and the field-of-view to twirl to compute the
+World Coordinate System (WCS): ### Twirl Usage ```python import twirl # Find
+some starts in the image: stars = twirl.find_peaks(data)[0:15] # Compute the
+World Coordinate System: wcs = twirl.compute_wcs(stars, center, fov) ``` A more
+complete example is provided in [docs/notebooks](https://github.com/lgrcia/
+twirl/tree/master/docs/notebooks) --- ## Development ### Project Requirements -
+[Python](https://www.python.org/) 3.11.* - [Poetry](https://python-poetry.org/
+) for Python package and environment management. ### Installing Dependencies
+The twirl project manages Python package dependencies using [Poetry](https://
+python-poetry.org/). You'll need to follow the instructions for installation
+there. Then you can start a shell session with the new environment with:
+```console $ poetry shell ``` **N.B.** For development with vscode you will
+need to run the following command: ```console $ poetry config virtualenvs.in-
+project true ``` This will installed the poetry `.venv` in the root of the
+project and allow vscode to setup the environment correctly for development. To
+start development, install all of the dependencies as: ```console $ poetry
+install ``` **N.B.** _Ensure that any dependency changes are committed to
+source control, so everyone has a consistenct package dependecy list._ --- ##
+Acknowledgements This package has made use of the algorithm from Lang, D. et
+al. (2010). _Astrometry.net: Blind Astrometric Calibration of Arbitrary
+Astronomical Images_. The Astronomical Journal, 139(5), pp.1782â1800. [doi:
+10.1088/0004-6256/139/5/1782](https://iopscience.iop.org/article/10.1088/0004-
+6256/139/5/1782). implemented in Garcia, L. J. et al. (2022). prose: a Python
+framework for modular astronomical images processing. MNRAS, vol. 509, no. 4,
+pp. 4817â4828, 2022. [doi:10.1093/mnras/stab3113](https://academic.oup.com/
+mnras/article-abstract/509/4/4817/6414007).
```

