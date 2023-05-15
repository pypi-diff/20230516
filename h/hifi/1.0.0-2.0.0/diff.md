# Comparing `tmp/hifi-1.0.0-py3.9.egg` & `tmp/hifi-2.0.0-py3.9.egg`

## zipinfo {}

```diff
@@ -1,9 +1,10 @@
-Zip file size: 4944 bytes, number of entries: 7
--rw-r--r--  2.0 unx     5145 b- defN 23-May-15 18:10 EGG-INFO/PKG-INFO
--rw-r--r--  2.0 unx      190 b- defN 23-May-15 18:10 EGG-INFO/SOURCES.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-15 18:10 EGG-INFO/dependency_links.txt
--rw-r--r--  2.0 unx     1162 b- defN 23-May-15 18:10 EGG-INFO/requires.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-15 18:10 EGG-INFO/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-15 18:10 EGG-INFO/zip-safe
--rwxr-xr-x  2.0 unx     3192 b- defN 23-May-15 18:10 EGG-INFO/scripts/hifi
-7 files, 9692 bytes uncompressed, 4096 bytes compressed:  57.7%
+Zip file size: 5885 bytes, number of entries: 8
+-rw-r--r--  2.0 unx     5145 b- defN 23-May-15 18:24 EGG-INFO/PKG-INFO
+-rw-r--r--  2.0 unx      207 b- defN 23-May-15 18:24 EGG-INFO/SOURCES.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-15 18:24 EGG-INFO/dependency_links.txt
+-rw-r--r--  2.0 unx     1519 b- defN 23-May-15 18:24 EGG-INFO/requires.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-15 18:24 EGG-INFO/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-15 18:24 EGG-INFO/zip-safe
+-rwxr-xr-x  2.0 unx     3192 b- defN 23-May-15 18:24 EGG-INFO/scripts/hifi
+-rwxr-xr-x  2.0 unx     1543 b- defN 23-May-15 18:24 EGG-INFO/scripts/visbeats
+8 files, 11609 bytes uncompressed, 4911 bytes compressed:  57.7%
```

## zipnote «TEMP»/diffoscope_etsbee7s_/tmpdbkub_9z_.zip

```diff
@@ -15,8 +15,11 @@
 
 Filename: EGG-INFO/zip-safe
 Comment: 
 
 Filename: EGG-INFO/scripts/hifi
 Comment: 
 
+Filename: EGG-INFO/scripts/visbeats
+Comment: 
+
 Zip file comment:
```

## EGG-INFO/PKG-INFO

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hifi
-Version: 1.0.0
+Version: 2.0.0
 Summary: Command-line tool to find nearest store.
 Home-page: https://github.com/austinbrown34/hifi
 Author: Austin Brown
 Author-email: austinbrown34@gmail.com
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

## EGG-INFO/SOURCES.txt

```diff
@@ -3,8 +3,9 @@
 README.md
 setup.py
 hifi.egg-info/PKG-INFO
 hifi.egg-info/SOURCES.txt
 hifi.egg-info/dependency_links.txt
 hifi.egg-info/requires.txt
 hifi.egg-info/top_level.txt
-scripts/hifi
+scripts/hifi
+scripts/visbeats
```

## EGG-INFO/requires.txt

```diff
@@ -1,64 +1,86 @@
-aubio==0.4.9
+appdirs==1.4.4
+argcomplete==3.0.8
+audioread==3.0.0
 awscli==1.27.41
-beautifulsoup4==4.7.1
-bleach==6.0.0
-boto3==1.26.41
-botocore==1.29.41
-certifi==2019.3.9
-chardet==3.0.4
+beautifulsoup4==4.12.2
+blinker==1.6.2
+boto3
+botocore
+bs4==0.0.1
+certifi==2023.5.7
+cffi==1.15.1
+cfn-flip==1.3.0
 charset-normalizer==3.1.0
-click==8.0.3
-colorama==0.4.4
-coverage==7.2.5
-decorator==4.3.0
-docutils==0.14
-exceptiongroup==1.1.1
-Flask==2.0.2
-future==0.16.0
-geocoder==1.38.1
-idna==2.8
+click==8.1.3
+contourpy==1.0.7
+cycler==0.11.0
+decorator==4.4.2
+durationpy==0.5
+Flask==2.3.2
+Flask-Uploads==0.2.1
+fonttools==4.39.3
+future==0.18.3
+hjson==3.1.0
+idna==3.4
+imageio==2.28.1
+imageio-ffmpeg==0.4.8
 importlib-metadata==6.6.0
-iniconfig==2.0.0
-itsdangerous==2.0.1
-jaraco.classes==3.2.3
-Jinja2==3.0.2
-jmespath==0.9.4
-keyring==23.13.1
-markdown-it-py==2.2.0
-MarkupSafe==2.0.1
-mdurl==0.1.2
-mido==1.2.9
-more-itertools==9.1.0
-nose2==0.7.4
-numpy==1.24.3
+importlib-resources==5.12.0
+itsdangerous==2.1.2
+Jinja2==3.1.2
+jmespath==1.0.1
+joblib==1.2.0
+kappa==0.7.0
+kiwisolver==1.4.4
+lazy_loader==0.2
+librosa==0.10.0.post2
+llvmlite==0.40.0
+MarkupSafe==2.1.2
+matplotlib==3.7.1
+mido==1.2.10
+moviepy==1.0.3
+msgpack==1.0.5
+networkx==3.1
+numba==0.57.0
+opencv-python==4.7.0.72
 packaging==23.1
-pkginfo==1.9.6
-pluggy==1.0.0
+Pillow==9.5.0
+placebo==0.10.0
+pooch==1.6.0
+proglog==0.1.10
 pyasn1==0.4.8
 PyAudio==0.2.13
-pydub==0.23.1
-Pygments==2.15.1
-pytest==7.3.1
-python-dateutil==2.8.0
+pycparser==2.21
+pyparsing==3.0.9
+python-dateutil==2.8.2
 python-magic==0.4.27
-pytube==15.0.0
-PyYAML==5.4.1
-ratelim==0.1.6
-readme-renderer==37.3
+python-slugify==8.0.1
+PyWavelets==1.4.1
+PyYAML
 requests==2.30.0
-requests-toolbelt==1.0.0
-rfc3986==2.0.0
-rich==13.3.5
+resampy==0.4.2
 rsa==4.7.2
 s3transfer==0.6.1
-six==1.12.0
-soupsieve==1.9
+scikit-image==0.20.0
+scikit-learn==1.2.2
+scipy==1.9.1
+setuptools-scm==7.1.0
+six==1.16.0
+soundfile==0.12.1
+soupsieve==2.4.1
+soxr==0.3.5
+termcolor==2.3.0
+text-unidecode==1.3
+threadpoolctl==3.1.0
+tifffile==2023.4.12
+toml==0.10.2
 tomli==2.0.1
-twine==4.0.2
-typing-extensions==3.10.0.2
+tqdm==4.65.0
+troposphere==4.3.2
+typing_extensions==4.5.0
+uipath==0.0.1
 urllib3==1.26.15
-webencodings==0.5.1
-Werkzeug==2.0.2
+Werkzeug==2.3.4
+wsgi-request-logger==0.4.6
 youtube-dl@ git+https://github.com/ytdl-org/youtube-dl.git@211cbfd5d46025a8e4d8f9f3d424aaada4698974
-youtube-dlc==2020.11.11.post3
-zipp==3.6.0
+zipp==3.15.0
```

