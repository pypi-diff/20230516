# Comparing `tmp/scipion-em-locscale-3.0.5.tar.gz` & `tmp/scipion-em-locscale-3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-locscale-3.0.5.tar", last modified: Fri Sep  2 13:48:43 2022, max compression
+gzip compressed data, was "scipion-em-locscale-3.1.tar", last modified: Tue May 16 10:42:30 2023, max compression
```

## Comparing `scipion-em-locscale-3.0.5.tar` & `scipion-em-locscale-3.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 13:48:43.592783 scipion-em-locscale-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/CHANGES.txt
--rw-r--r--   0 runner    (1001) docker     (121)    35146 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/LICENCE
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     4044 2022-09-02 13:48:43.592783 scipion-em-locscale-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2619 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 13:48:43.588783 scipion-em-locscale-3.0.5/locscale/
--rw-r--r--   0 runner    (1001) docker     (121)     3279 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/locscale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1817 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/locscale/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (121)     1219 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/locscale/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     3452 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/locscale/convert.py
--rw-r--r--   0 runner    (1001) docker     (121)   153665 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/locscale/locscale_logo.jpg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 13:48:43.588783 scipion-em-locscale-3.0.5/locscale/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)     1195 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/locscale/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8311 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/locscale/protocols/protocol_locscale.py
--rw-r--r--   0 runner    (1001) docker     (121)     3103 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/locscale/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 13:48:43.588783 scipion-em-locscale-3.0.5/locscale/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1204 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/locscale/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5175 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/locscale/tests/test_protocol_locscale.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-02 13:48:43.592783 scipion-em-locscale-3.0.5/scipion_em_locscale.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     4044 2022-09-02 13:48:43.000000 scipion-em-locscale-3.0.5/scipion_em_locscale.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      583 2022-09-02 13:48:43.000000 scipion-em-locscale-3.0.5/scipion_em_locscale.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-02 13:48:43.000000 scipion-em-locscale-3.0.5/scipion_em_locscale.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-09-02 13:48:43.000000 scipion-em-locscale-3.0.5/scipion_em_locscale.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2022-09-02 13:48:43.000000 scipion-em-locscale-3.0.5/scipion_em_locscale.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-09-02 13:48:43.000000 scipion-em-locscale-3.0.5/scipion_em_locscale.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-02 13:48:43.592783 scipion-em-locscale-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     8498 2022-09-02 13:46:35.000000 scipion-em-locscale-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:42:30.747167 scipion-em-locscale-3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35146 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-16 10:42:30.747167 scipion-em-locscale-3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2917 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:42:30.743167 scipion-em-locscale-3.1/locscale/
+-rw-r--r--   0 runner    (1001) docker     (123)     5192 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/locscale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2188 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/locscale/bibtex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/locscale/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/locscale/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153665 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/locscale/locscale_logo.jpg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:42:30.743167 scipion-em-locscale-3.1/locscale/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/locscale/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12254 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/locscale/protocols/protocol_locscale.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/locscale/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:42:30.747167 scipion-em-locscale-3.1/locscale/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/locscale/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4670 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/locscale/tests/test_protocol_locscale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 10:42:30.747167 scipion-em-locscale-3.1/scipion_em_locscale.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4341 2023-05-16 10:42:30.000000 scipion-em-locscale-3.1/scipion_em_locscale.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-16 10:42:30.000000 scipion-em-locscale-3.1/scipion_em_locscale.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 10:42:30.000000 scipion-em-locscale-3.1/scipion_em_locscale.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 10:42:30.000000 scipion-em-locscale-3.1/scipion_em_locscale.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-16 10:42:30.000000 scipion-em-locscale-3.1/scipion_em_locscale.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-16 10:42:30.000000 scipion-em-locscale-3.1/scipion_em_locscale.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 10:42:30.747167 scipion-em-locscale-3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8483 2023-05-16 10:40:38.000000 scipion-em-locscale-3.1/setup.py
```

### Comparing `scipion-em-locscale-3.0.5/LICENCE` & `scipion-em-locscale-3.1/LICENCE`

 * *Files identical despite different names*

### Comparing `scipion-em-locscale-3.0.5/locscale/bibtex.py` & `scipion-em-locscale-3.1/locscale/bibtex.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # *
 # * Authors:     David Maluenda (dmaluenda@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
-# * the Free Software Foundation; either version 2 of the License, or
+# * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
@@ -22,14 +22,25 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 """
+@article{Bharadwaj2022,
+author = "Bharadwaj, Alok and Jakobi, Arjen J.",
+title = "Electron scattering properties of biological macromolecules and their use for cryo-EM map sharpening",
+journal = "Faraday Discuss.",
+year = "2022",
+volume = "240",
+issue = "0",
+pages = "168-183",
+publisher = "The Royal Society of Chemistry",
+doi = "http://dx.doi.org/10.1039/D2FD00078D"
+}
 
 @article{Jakobi2017,
   Title                    = {Model-based local density sharpening of cryo-EM maps},
   Author                   = {Jakobi, Arjen J and Wilmanns, Matthias and Sachse, Carsten},
   Journal                  = {eLife},
   Year                     = {2017},
   Month                    = {October},
```

### Comparing `scipion-em-locscale-3.0.5/locscale/constants.py` & `scipion-em-locscale-3.1/locscale/tests/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,16 @@
-
 # **************************************************************************
 # *
 # * Authors:    Yunior C. Fonseca Reyna (cfonseca@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
-# * the Free Software Foundation; either version 2 of the License, or
+# * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
@@ -21,11 +20,8 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-LOCSCALE_HOME = 'LOCSCALE_HOME'
-
-# Supported versions
-V0_1 = '0.1'
+from .test_protocol_locscale import TestProtLocscale
```

### Comparing `scipion-em-locscale-3.0.5/locscale/locscale_logo.jpg` & `scipion-em-locscale-3.1/locscale/locscale_logo.jpg`

 * *Files identical despite different names*

### Comparing `scipion-em-locscale-3.0.5/locscale/protocols/__init__.py` & `scipion-em-locscale-3.1/locscale/protocols/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # *
 # * Authors:    Yunior C. Fonseca Reyna (cfonseca@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
-# * the Free Software Foundation; either version 2 of the License, or
+# * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
```

### Comparing `scipion-em-locscale-3.0.5/locscale/tests/__init__.py` & `scipion-em-locscale-3.1/locscale/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # *
 # * Authors:    Yunior C. Fonseca Reyna (cfonseca@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
-# * the Free Software Foundation; either version 2 of the License, or
+# * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
@@ -20,8 +20,20 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
-from .test_protocol_locscale import TestProtLocscale
+# Supported versions
+V2_1 = '2.1'
+VERSIONS = [V2_1]
+LOCSCALE_DEFAULT_VER_NUM = VERSIONS[-1]
+
+DEFAULT_ENV_NAME = f"locscale-{LOCSCALE_DEFAULT_VER_NUM}"
+DEFAULT_ACTIVATION_CMD = 'conda activate ' + DEFAULT_ENV_NAME
+LOCSCALE_ENV_ACTIVATION = 'LOCSCALE_ENV_ACTIVATION'
+
+# reference types
+REF_NONE = 0
+REF_PDB = 1
+REF_VOL = 2
```

### Comparing `scipion-em-locscale-3.0.5/locscale/tests/test_protocol_locscale.py` & `scipion-em-locscale-3.1/locscale/tests/test_protocol_locscale.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # ***************************************************************************
 # *
-# * Authors:     David Maluenda (dmaluenda@cnb.csic.es) (2018)
+# * Authors:     David Maluenda (dmaluenda@cnb.csic.es)
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
-# * the Free Software Foundation; either version 2 of the License, or
+# * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
@@ -18,107 +18,87 @@
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # ***************************************************************************
 
 from pyworkflow.tests import BaseTest, setupTestProject, DataSet
-from pwem.protocols import ProtImportVolumes, ProtImportMask
+from pwem.protocols import ProtImportVolumes, ProtImportPdb
 from pyworkflow.utils import magentaStr
 
 from ..protocols import ProtLocScale
 
 
 class TestProtLocscale(BaseTest):
     @classmethod
+    def runImportVolumes(cls, samplingRate, vol, half1, half2):
+        """ Run Import volumes protocol. """
+        cls.protImport = cls.newProtocol(ProtImportVolumes,
+                                         filesPath=vol,
+                                         samplingRate=samplingRate,
+                                         setHalfMaps=True,
+                                         half1map=half1,
+                                         half2map=half2)
+        cls.launchProtocol(cls.protImport)
+        return cls.protImport
+
+    @classmethod
     def setUpClass(cls):
         setupTestProject(cls)
-        cls.dataSet = DataSet.getDataSet('xmipp_tutorial')
-
-        # Imports
-        print(magentaStr("\n==> Importing data - Input data"))
-        new = cls.proj.newProtocol  # short notation
-        launch = cls.proj.launchProtocol
-
-        # Volumes
-        print(magentaStr("\nImporting Volumes:"))
-        pImpVolume = new(ProtImportVolumes, samplingRate=1,
-                         filesPath=cls.dataSet.getFile('vol2'))
-        launch(pImpVolume, wait=True)
-        #   volume.vol
-        cls.inputVol = pImpVolume.outputVolume
-        pImpVolume2 = new(ProtImportVolumes, samplingRate=1,
-                          filesPath=cls.dataSet.getFile('vol1'))
-        launch(pImpVolume2, wait=True)
-        cls.inputVol2 = pImpVolume2.outputVolume
-
-        # References
-        print(magentaStr("\nImporting References:"))
-        pImpRef = new(ProtImportVolumes, samplingRate=1,
-                      filesPath=cls.dataSet.getFile('vol3'))
-        launch(pImpRef, wait=True)
-        #   reference.vol
-        cls.inputRef = pImpRef.outputVolume
-        pImpRef2 = new(ProtImportVolumes, samplingRate=1,
-                       filesPath=cls.dataSet.getFile('vol1'))
-        launch(pImpRef2, wait=True)
-        cls.inputRef2 = pImpRef2.outputVolume
-
-        # Masks
-        print(magentaStr("\nImporting Mask:"))
-        pImpMask = new(ProtImportMask,
-                       maskPath=cls.dataSet.getFile('mask3d'),
-                       samplingRate=1)
-        launch(pImpMask, wait=True)
-        cls.mask = pImpMask.outputMask
+        cls.ds = DataSet.getDataSet('model_building_tutorial')
+        cls.half1 = cls.ds.getFile('volumes/emd_3488_Noisy_half1.vol')
+        cls.half2 = cls.ds.getFile('volumes/emd_3488_Noisy_half2.vol')
+        cls.map = cls.ds.getFile('volumes/emd_3488.map')
+        cls.model = cls.ds.getFile('PDBx_mmCIF/5ni1.pdb')
+
+        print(magentaStr("\n==> Importing data - volume:"))
+        cls.protImportMap = cls.runImportVolumes(1.05,
+                                                 cls.map,
+                                                 cls.half1,
+                                                 cls.half2)
+
+        print(magentaStr("\n==> Importing data - pdb:"))
+        cls.protImportModel = cls.newProtocol(ProtImportPdb,
+                                              inputPdbData=1,
+                                              pdbFile=cls.model)
+        cls.launchProtocol(cls.protImportModel)
 
     def testLocscale(self):
-        """ Check that an output was generated and the condition is valid.
-            In addition, returns the size of the set.
-        """
-        print(magentaStr("\n==> Testing locscale:"))
-
-        def launchTest(label, vol, ref, mask=None, mpi=3):
-            print(magentaStr("\nTest %s:" % label))
-            pLocScale = self.proj.newProtocol(ProtLocScale,
-                                              objLabel='locscale - ' + label,
-                                              inputVolume=vol,
-                                              refObj=ref,
-                                              patchSize=16,
-                                              binaryMask=mask,
-                                              numberOfMpi=mpi)
-            self.proj.launchProtocol(pLocScale, wait=True)
+        def launchTest(label, vol, volRef=None, pdbRef=None, useNN=False):
+            print(magentaStr(f"\n==> Testing locscale ({label}):"))
+            pLocScale = self.newProtocol(ProtLocScale,
+                                         objLabel='locscale - ' + label,
+                                         inputVolume=vol)
+            if useNN:
+                pLocScale.useNNpredict.set(True)
+            else:
+                if volRef is not None:
+                    pLocScale.refType.set(2)
+                    pLocScale.refObj.set(volRef)
+                elif pdbRef is not None:
+                    pLocScale.refType.set(1)
+                    pLocScale.refPdb.set(pdbRef)
+                else:
+                    pLocScale.refType.set(0)
+
+            self.launchProtocol(pLocScale, wait=True)
 
             self.assertIsNotNone(pLocScale.outputVolume,
-                                 "outputVolume is None for %s test." % label)
+                                 "outputVolume is None for %s test" % label)
 
-            self.assertEqual(self.inputVol.getDim(),
+            self.assertEqual(vol.getDim(),
                              pLocScale.outputVolume.getDim(),
-                             "outputVolume has diferent size than inputVol "
+                             "outputVolume has a different size than inputVol "
                              "for %s test" % label)
 
-            self.assertEqual(self.inputVol.getSamplingRate(),
+            self.assertEqual(vol.getSamplingRate(),
                              pLocScale.outputVolume.getSamplingRate(),
-                             "outputVolume has diferent sampling rate than "
+                             "outputVolume has a different sampling rate than "
                              "inputVol for %s test" % label)
 
-        # default test
-        launchTest('with MPI + noMask', vol=self.inputVol, ref=self.inputRef)
+        inputVol = self.protImportMap.outputVolume
+        pdbRef = self.protImportModel.outputPdb
 
-        # with mask test
-        launchTest('with MPI + Mask', vol=self.inputVol, ref=self.inputRef,
-                   mask=self.mask)
-
-        # with mask test
-        launchTest('with Mask + noMPI', vol=self.inputVol, ref=self.inputRef,
-                   mask=self.mask, mpi=1)
-
-        # without MPI
-        launchTest('noMask + noMPI', vol=self.inputVol, ref=self.inputRef,
-                   mpi=1)
-
-        # convert input volume
-        launchTest('convert inputVol', vol=self.inputVol2, ref=self.inputRef)
-
-        # convert reference volume
-        launchTest('convert reference', vol=self.inputVol, ref=self.inputRef2,
-                   mask=self.mask)
+        #launchTest('noRef', vol=inputVol)
+        #launchTest('volRef', vol=inputVol, volRef=volRef)  # TODO: test reference volume case
+        launchTest('pdbRef', vol=inputVol, pdbRef=pdbRef)
+        launchTest('EMmerNet', vol=inputVol, useNN=True)
```

### Comparing `scipion-em-locscale-3.0.5/scipion_em_locscale.egg-info/SOURCES.txt` & `scipion-em-locscale-3.1/scipion_em_locscale.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `scipion-em-locscale-3.0.5/setup.py` & `scipion-em-locscale-3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # *
 # * Authors:    Yunior C. Fonseca Reyna (cfonseca@cnb.csic.es)
 # *
 # * Unidad de  Bioinformatica of Centro Nacional de Biotecnologia , CSIC
 # *
 # * This program is free software; you can redistribute it and/or modify
 # * it under the terms of the GNU General Public License as published by
-# * the Free Software Foundation; either version 2 of the License, or
+# * the Free Software Foundation; either version 3 of the License, or
 # * (at your option) any later version.
 # *
 # * This program is distributed in the hope that it will be useful,
 # * but WITHOUT ANY WARRANTY; without even the implied warranty of
 # * MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # * GNU General Public License for more details.
 # *
@@ -102,25 +102,25 @@
     # For a list of valid classifiers, see
     # https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[  # Optional
         # How mature is this project? Common values are
         #   3 - Alpha
         #   4 - Beta
         #   5 - Production/Stable
-        'Development Status :: 5 - Production/Stable',
+        'Development Status :: 4 - Beta',
 
         # Indicate who your project is intended for
         #   'Intended Audience :: Users',
 
         # Pick your license as you wish
         'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
 
         # Specify the Python versions you support here. In particular, ensure
         # that you indicate whether you support Python 2, Python 3 or both.
-        'Programming Language :: Python :: 3.5'
+        'Programming Language :: Python :: 3'
     ],
 
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a string of words separated by whitespace, not a list.
     keywords='scipion electron-microscopy cryo-em structural-biology image-processing scipion-3.0',  # Optional
```

