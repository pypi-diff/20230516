# Comparing `tmp/scipion-em-novactf-3.0.5.tar.gz` & `tmp/scipion-em-novactf-3.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scipion-em-novactf-3.0.5.tar", last modified: Tue Jul  6 15:04:37 2021, max compression
+gzip compressed data, was "scipion-em-novactf-3.1.1.tar", last modified: Tue May 16 08:01:21 2023, max compression
```

## Comparing `scipion-em-novactf-3.0.5.tar` & `scipion-em-novactf-3.1.1.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-06 15:04:37.160475 scipion-em-novactf-3.0.5/
--rw-r--r--   0 runner    (1001) docker     (121)    35147 2021-07-06 14:58:57.000000 scipion-em-novactf-3.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       43 2021-07-06 14:58:57.000000 scipion-em-novactf-3.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      962 2021-07-06 15:04:37.160475 scipion-em-novactf-3.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      441 2021-07-06 14:58:57.000000 scipion-em-novactf-3.0.5/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-06 15:04:37.160475 scipion-em-novactf-3.0.5/novactf/
--rw-r--r--   0 runner    (1001) docker     (121)     3632 2021-07-06 14:58:57.000000 scipion-em-novactf-3.0.5/novactf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3319 2021-07-06 14:58:57.000000 scipion-em-novactf-3.0.5/novactf/bibtex.py
--rw-r--r--   0 runner    (1001) docker     (121)     1251 2021-07-06 14:58:57.000000 scipion-em-novactf-3.0.5/novactf/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-06 15:04:37.160475 scipion-em-novactf-3.0.5/novactf/protocols/
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2021-07-06 14:58:57.000000 scipion-em-novactf-3.0.5/novactf/protocols/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13281 2021-07-06 14:58:57.000000 scipion-em-novactf-3.0.5/novactf/protocols/protocol_tomoDefocus.py
--rw-r--r--   0 runner    (1001) docker     (121)    16653 2021-07-06 14:58:57.000000 scipion-em-novactf-3.0.5/novactf/protocols/protocol_tomoReconstruction.py
--rw-r--r--   0 runner    (1001) docker     (121)      978 2021-07-06 14:58:57.000000 scipion-em-novactf-3.0.5/novactf/protocols.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-06 15:04:37.160475 scipion-em-novactf-3.0.5/novactf/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     1304 2021-07-06 14:58:57.000000 scipion-em-novactf-3.0.5/novactf/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9666 2021-07-06 14:58:57.000000 scipion-em-novactf-3.0.5/novactf/tests/test_protocols_novactf.py
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-07-06 14:58:57.000000 scipion-em-novactf-3.0.5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-06 15:04:37.160475 scipion-em-novactf-3.0.5/scipion_em_novactf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      962 2021-07-06 15:04:37.000000 scipion-em-novactf-3.0.5/scipion_em_novactf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      579 2021-07-06 15:04:37.000000 scipion-em-novactf-3.0.5/scipion_em_novactf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-06 15:04:37.000000 scipion-em-novactf-3.0.5/scipion_em_novactf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       39 2021-07-06 15:04:37.000000 scipion-em-novactf-3.0.5/scipion_em_novactf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-07-06 15:04:37.000000 scipion-em-novactf-3.0.5/scipion_em_novactf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2021-07-06 15:04:37.000000 scipion-em-novactf-3.0.5/scipion_em_novactf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-06 15:04:37.160475 scipion-em-novactf-3.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6924 2021-07-06 14:58:57.000000 scipion-em-novactf-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:21.474419 scipion-em-novactf-3.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-16 07:59:18.000000 scipion-em-novactf-3.1.1/CHANGES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    35147 2023-05-16 07:59:18.000000 scipion-em-novactf-3.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-05-16 07:59:18.000000 scipion-em-novactf-3.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-16 08:01:21.474419 scipion-em-novactf-3.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-05-16 07:59:18.000000 scipion-em-novactf-3.1.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:21.474419 scipion-em-novactf-3.1.1/novactf/
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-05-16 07:59:18.000000 scipion-em-novactf-3.1.1/novactf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-16 07:59:18.000000 scipion-em-novactf-3.1.1/novactf/bibtex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:21.474419 scipion-em-novactf-3.1.1/novactf/protocols/
+-rw-r--r--   0 runner    (1001) docker     (123)     1278 2023-05-16 07:59:18.000000 scipion-em-novactf-3.1.1/novactf/protocols/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11132 2023-05-16 07:59:18.000000 scipion-em-novactf-3.1.1/novactf/protocols/protocol_tomoDefocus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21657 2023-05-16 07:59:18.000000 scipion-em-novactf-3.1.1/novactf/protocols/protocol_tomoReconstruction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-16 07:59:18.000000 scipion-em-novactf-3.1.1/novactf/protocols.conf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:21.474419 scipion-em-novactf-3.1.1/novactf/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-16 07:59:18.000000 scipion-em-novactf-3.1.1/novactf/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6252 2023-05-16 07:59:18.000000 scipion-em-novactf-3.1.1/novactf/tests/test_protocols_novactf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:01:21.474419 scipion-em-novactf-3.1.1/scipion_em_novactf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-16 08:01:21.000000 scipion-em-novactf-3.1.1/scipion_em_novactf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-16 08:01:21.000000 scipion-em-novactf-3.1.1/scipion_em_novactf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:01:21.000000 scipion-em-novactf-3.1.1/scipion_em_novactf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 08:01:21.000000 scipion-em-novactf-3.1.1/scipion_em_novactf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-16 08:01:21.000000 scipion-em-novactf-3.1.1/scipion_em_novactf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-16 08:01:21.000000 scipion-em-novactf-3.1.1/scipion_em_novactf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:01:21.474419 scipion-em-novactf-3.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-16 07:59:18.000000 scipion-em-novactf-3.1.1/setup.py
```

### Comparing `scipion-em-novactf-3.0.5/LICENSE` & `scipion-em-novactf-3.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `scipion-em-novactf-3.0.5/novactf/__init__.py` & `scipion-em-novactf-3.1.1/novactf/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# **************************************************************************
+# *****************************************************************************
 # *
 # * Authors:     Federico P. de Isidro Gomez (fp.deisidro@cnb.csic.es) [1]
 # *
 # * [1] Centro Nacional de Biotecnologia, CSIC, Spain
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
@@ -18,27 +18,27 @@
 # * along with this program; if not, write to the Free Software
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
-# **************************************************************************
+# *****************************************************************************
 
 import pwem
 
-from .constants import NOVACTF_HOME
 
-__version__ = '3.0.5'
-_logo = ""
+__version__ = '3.1.1'
 _references = ["Turonova2017"]
+NOVACTF_HOME = 'NOVACTF_HOME'
 
 
 class Plugin(pwem.Plugin):
     _homeVar = NOVACTF_HOME
+    _url = "https://github.com/scipion-em/scipion-em-novactf"
 
     @classmethod
     def _defineVariables(cls):
         cls._defineEmVar(NOVACTF_HOME, 'novactf-master')
 
     @classmethod
     def getEnviron(cls):
@@ -81,11 +81,11 @@
                        version=version,
                        tar='void.tgz',
                        neededProgs=cls.getDependencies(),
                        commands=[(installationCmd, NOVACTF_INSTALLED)],
                        default=True)
 
     @classmethod
-    def runNovactf(cls, protocol, program, args, cwd=None):
+    def runNovactf(cls, protocol, program, args, **kwargs):
         """ Run NovaCTF command from a given protocol. """
         fullProgram = '%s/%s/%s' % (cls.getVar(NOVACTF_HOME), "novaCTF-master", program)
-        protocol.runJob(fullProgram, args, env=cls.getEnviron(), cwd=cwd)
+        protocol.runJob(fullProgram, args, env=cls.getEnviron(), **kwargs)
```

### Comparing `scipion-em-novactf-3.0.5/novactf/constants.py` & `scipion-em-novactf-3.1.1/novactf/tests/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# **************************************************************************
+# *****************************************************************************
 # *
 # * Authors:     Federico P. de Isidro Gomez (fp.deisidro@cnb.csic.es) [1]
 # *
 # * [1] Centro Nacional de Biotecnologia, CSIC, Spain
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
@@ -18,13 +18,15 @@
 # * along with this program; if not, write to the Free Software
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
-# **************************************************************************
+# *****************************************************************************
 
+from pyworkflow.tests import DataSet
 
-# ----------------- Constants values --------------------------------------
-
-NOVACTF_HOME = 'NOVACTF_HOME'
+DataSet(name='novaCtfTestData',
+        folder='novaCtfTestData',
+        files={
+            'tsCtf': 'tomo1_bin4.mrc'})
```

### Comparing `scipion-em-novactf-3.0.5/novactf/protocols/__init__.py` & `scipion-em-novactf-3.1.1/novactf/protocols/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# **************************************************************************
+# *****************************************************************************
 # *
 # * Authors:     Federico P. de Isidro Gomez (fp.deisidro@cnb.csic.es) [1]
 # *
 # * [1] Centro Nacional de Biotecnologia, CSIC, Spain
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
@@ -18,11 +18,11 @@
 # * along with this program; if not, write to the Free Software
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
-# **************************************************************************
+# *****************************************************************************
 
 from .protocol_tomoDefocus import ProtNovaCtfTomoDefocus
 from .protocol_tomoReconstruction import ProtNovaCtfTomoReconstruction
```

### Comparing `scipion-em-novactf-3.0.5/novactf/protocols/protocol_tomoDefocus.py` & `scipion-em-novactf-3.1.1/novactf/protocols/protocol_tomoDefocus.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# **************************************************************************
+# *****************************************************************************
 # *
 # * Authors:     Federico P. de Isidro Gomez (fp.deisidro@cnb.csic.es) [1]
 # *
 # * [1] Centro Nacional de Biotecnologia, CSIC, Spain
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
@@ -18,301 +18,246 @@
 # * along with this program; if not, write to the Free Software
 # * Foundation, Inc., 59 Temple Place, Suite 330, Boston, MA
 # * 02111-1307  USA
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
-# **************************************************************************
+# *****************************************************************************
 
 import os
+from glob import glob
+
 from pyworkflow import BETA
 import pyworkflow.protocol.params as params
 from pyworkflow.project import Manager
 import pyworkflow.utils.path as path
 from pyworkflow.protocol.constants import STEPS_PARALLEL
 from pyworkflow.object import Integer, List
+from pwem.emlib.image import ImageHandler
 from pwem.protocols import EMProtocol
 from tomo.protocols import ProtTomoBase
-from pwem.emlib.image import ImageHandler
-from novactf import Plugin
+
 from imod import utils as imodUtils
+from .. import Plugin
 
 
 class ProtNovaCtfTomoDefocus(EMProtocol, ProtTomoBase):
     """
-    Defocus estimation of each tilt-image procedure based on the novaCTF procedure.
+    Compute defocus array for each tilt-image with novaCTF.
 
     More info:
             https://github.com/turonova/novaCTF
     """
 
-    _label = 'tomo ctf defocus'
+    _label = 'compute defocus array'
     _devStatus = BETA
 
     def __init__(self, **args):
         EMProtocol.__init__(self, **args)
         ProtTomoBase.__init__(self)
         self.stepsExecutionMode = STEPS_PARALLEL
-        self.numberOfIntermediateStacks = List([])
 
     # -------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
         form.addSection('Input')
 
         form.addParam('inputSetOfTiltSeries',
                       params.PointerParam,
                       pointerClass='SetOfTiltSeries',
-                      label='Input set of tilt-Series')
+                      label='Input set of tilt-series')
 
         form.addParam('inputSetOfCtfTomoSeries',
                       params.PointerParam,
-                      label="input tilt-series CTF estimation",
+                      label="Input tilt-series CTF estimation",
                       pointerClass='SetOfCTFTomoSeries',
-                      help='Select the CTF estimation from the set of tilt-series.')
+                      help='Select the CTF estimation for the input tilt-series.')
 
         form.addParam('tomoThickness',
                       params.FloatParam,
-                      default=100,
+                      default=400,
                       label='Tomogram thickness (voxels)',
-                      important=True,
                       display=params.EnumParam.DISPLAY_HLIST,
-                      help='Size in voxels of the tomogram in the z axis (beam direction).')
+                      help='Size of the tomogram in voxels in the Z direction.')
 
         form.addParam('tomoShift',
                       params.FloatParam,
                       default=0,
                       label='Tomogram shift (voxels)',
-                      important=True,
                       display=params.EnumParam.DISPLAY_HLIST,
-                      help='Shift in voxels of the tomogram in the z axis (beam direction).')
+                      help='Shift of the tomogram in voxels in the Z direction. '
+                           'The shift should be set to zero even if for '
+                           'reconstruction we want to shift the tomogram in z! '
+                           'We assume the defocus to be estimated at the center '
+                           'of mass which should correspond to the shifted '
+                           'tomogram and thus here the shift should be zero.')
 
         form.addParam('defocusStep',
                       params.IntParam,
                       default=15,
                       label='Defocus step (nm)',
-                      important=True,
                       display=params.EnumParam.DISPLAY_HLIST,
-                      help='Minimum defocus difference used for reconstruction in nanometers.')
+                      help='The space between min and max in Z is sliced '
+                           'by defocus step. 15 nm is default step size. '
+                           'See Fig. 2 in Turonova et al., 2017 for optimal number.')
 
         form.addParam('correctionType',
                       params.EnumParam,
                       choices=['Phase flip', 'Multiplication'],
                       default=0,
                       label='Correction type',
-                      important=True,
                       display=params.EnumParam.DISPLAY_HLIST,
-                      help='Correction type to be applied for reconstruction')
+                      help='CTF correction type to be applied for the tilt-series.')
 
         form.addParam('correctAstigmatism',
                       params.EnumParam,
-                      choices=['Yes', 'No'],
-                      default=0,
+                      choices=['No', 'Yes'],
+                      default=1,
                       label='Correct astigmatism',
-                      important=True,
                       display=params.EnumParam.DISPLAY_HLIST,
-                      help='Correct for astigmatism in reconstruction')
-
-        self.defineFilterParameters(form)
-
-        form.addParallelSection(threads=8, mpi=1)
+                      help='Correct for astigmatism in reconstruction.')
 
-    @staticmethod
-    def defineFilterParameters(form):
-        groupRadialFrequencies = form.addGroup('Radial filtering',
-                                               help='This entry controls low-pass filtering with the radial weighting '
-                                                    'function.  The radial weighting function is linear away from the '
-                                                    'origin out to the distance in reciprocal space specified by the '
-                                                    'first value, followed by a Gaussian fall-off determined by the '
-                                                    'second value.')
-        groupRadialFrequencies.addParam('radialFirstParameter',
-                                        params.FloatParam,
-                                        default=0.3,
-                                        label='First parameter',
-                                        help='Linear region value')
-        groupRadialFrequencies.addParam('radialSecondParameter',
-                                        params.FloatParam,
-                                        default=0.05,
-                                        label='Second parameter',
-                                        help='Gaussian fall-off parameter')
+        form.addParallelSection(threads=2, mpi=1)
 
-    # -------------------------- INSERT steps functions ---------------------
+    # -------------------------- INSERT steps functions -----------------------
     def _insertAllSteps(self):
-
-        for ts in self.inputSetOfTiltSeries.get():
-            self._insertFunctionStep(self.convertInputStep,
-                                     ts.getObjId())
-
-            self._insertFunctionStep(self.computeDefocusStep,
-                                     ts.getObjId())
-
-            self._insertFunctionStep(self.getNumberOfIntermediateStacksStep,
-                                     ts.getObjId())
-
+        self.numberOfIntermediateStacks = List([])
+        for ts in self.getInputTs():
+            self._insertFunctionStep(self.convertInputStep, ts.getObjId())
+            self._insertFunctionStep(self.computeDefocusStep, ts.getObjId())
         self._insertFunctionStep(self.triggerReconstructionProtocolStep)
 
-    # --------------------------- STEPS functions ----------------------------
+    # --------------------------- STEPS functions -----------------------------
     def convertInputStep(self, tsObjId):
-        ts = self.inputSetOfTiltSeries.get()[tsObjId]
+        ts = self.getInputTs()[tsObjId]
         tsId = ts.getTsId()
 
-        ctfTomoSeries = self.getCtfTomoSeriesFromTsId(self.inputSetOfCtfTomoSeries.get(), tsId)
+        ctfTomoSeries = self.getCtfTomoSeriesFromTsId(tsId)
 
         tmpPrefix = self._getTmpPath(tsId)
         extraPrefix = self._getExtraPath(tsId)
 
         path.makePath(tmpPrefix)
         path.makePath(extraPrefix)
 
         firstItem = ts.getFirstItem()
 
-        """Generate angle file"""
-        angleFilePath = os.path.join(tmpPrefix, firstItem.parseFileName(extension=".tlt"))
+        # Generate angle file
+        angleFilePath = os.path.join(tmpPrefix,
+                                     firstItem.parseFileName(extension=".tlt"))
         ts.generateTltFile(angleFilePath)
 
-        """Generate defocus file"""
-        defocusFilePath = os.path.join(extraPrefix, firstItem.parseFileName(extension=".defocus"))
+        # Generate defocus file
+        defocusFilePath = os.path.join(extraPrefix,
+                                       firstItem.parseFileName(extension=".defocus"))
         imodUtils.generateDefocusIMODFileFromObject(ctfTomoSeries, defocusFilePath)
 
     def computeDefocusStep(self, tsObjId):
-        ts = self.inputSetOfTiltSeries.get()[tsObjId]
+        ts = self.getInputTs()[tsObjId]
         tsId = ts.getTsId()
 
         tmpPrefix = self._getTmpPath(ts.getTsId())
         extraPrefix = self._getExtraPath(tsId)
 
         firstItem = ts.getFirstItem()
 
         ih = ImageHandler()
-        xDim, yDim, _, _ = ih.getDimensions(firstItem.getFileName()+":mrc")
+        xDim, yDim, _, _ = ih.getDimensions(firstItem.getFileName() + ":mrc")
 
-        defocusFilePath = os.path.join(extraPrefix, firstItem.parseFileName(extension=".defocus"))
+        defocusFilePath = os.path.join(extraPrefix,
+                                       firstItem.parseFileName(extension=".defocus"))
+
+        if self.tomoShift.get() > 0.01:
+            defocusShift = self.tomoThickness.get() / 2 + self.tomoShift.get()
+            with open(defocusFilePath.replace(".defocus", ".def_shift"), "w") as fn:
+                fn.write(f"{defocusShift}")
 
         paramsDefocus = {
             'Algorithm': "defocus",
-            'InputProjections': firstItem.getLocation()[1],
+            'InputProjections': firstItem.getFileName(),
             'FullImage': str(xDim) + "," + str(yDim),
             'Thickness': self.tomoThickness.get(),
             'TiltFile': os.path.join(tmpPrefix, firstItem.parseFileName(extension=".tlt")),
-            'Shift': "0.0," + str(self.tomoShift.get()),
-            'CorrectionType': self.getCorrectionType(),
+            'CorrectionType': "phaseflip" if self.correctionType.get() == 0 else "multiplication",
             'DefocusFileFormat': "imod",
             'CorrectAstigmatism': self.correctAstigmatism.get(),
             'DefocusFile': defocusFilePath,
-            'PixelSize': self.inputSetOfTiltSeries.get().getSamplingRate() / 10,
-            'DefocusStep': self.defocusStep.get()
+            'PixelSize': self.getInputTs().getSamplingRate() / 10,
+            'DefocusStep': self.defocusStep.get(),
+            'DefocusShiftFile': defocusFilePath.replace(".defocus", ".def_shift")
         }
 
         argsDefocus = "-Algorithm %(Algorithm)s " \
                       "-InputProjections %(InputProjections)s " \
                       "-FULLIMAGE %(FullImage)s " \
                       "-THICKNESS %(Thickness)d " \
                       "-TILTFILE %(TiltFile)s " \
-                      "-SHIFT %(Shift)s " \
+                      "-SHIFT 0.0,0.0 " \
                       "-CorrectionType %(CorrectionType)s " \
                       "-DefocusFileFormat %(DefocusFileFormat)s " \
                       "-CorrectAstigmatism %(CorrectAstigmatism)d " \
                       "-DefocusFile %(DefocusFile)s " \
                       "-PixelSize %(PixelSize)s " \
-                      "-DefocusStep %(DefocusStep)d"
-
-        Plugin.runNovactf(self, 'novaCTF', argsDefocus % paramsDefocus)
-
-    def getNumberOfIntermediateStacksStep(self, tsObjId):
-        ts = self.inputSetOfTiltSeries.get()[tsObjId]
+                      "-DefocusStep %(DefocusStep)d "
 
-        extraPrefix = self._getExtraPath(ts.getTsId())
+        if self.tomoShift.get() > 0.01:
+            argsDefocus += "-DefocusShiftFile %(DefocusShiftFile)s "
 
-        defocusFilePath = os.path.join(extraPrefix,
-                                       ts.getFirstItem().parseFileName(extension=".defocus_"))
-        numberOfIntermediateStacks = 0
+        Plugin.runNovactf(self, 'novaCTF', argsDefocus % paramsDefocus)
 
-        counter = 0
-        while os.path.exists(defocusFilePath + str(counter)):
-            numberOfIntermediateStacks += 1
-            counter += 1
+        files = glob(defocusFilePath.replace(".defocus", ".defocus_*"))
+        self.numberOfIntermediateStacks.append(Integer(len(files)))
 
-        self.numberOfIntermediateStacks.append(Integer(numberOfIntermediateStacks))
+        self._store()
 
     def triggerReconstructionProtocolStep(self):
         # Local import to avoid looping
-        from novactf.protocols import ProtNovaCtfTomoReconstruction
+        from . import ProtNovaCtfTomoReconstruction
 
         manager = Manager()
         project = manager.loadProject(self.getProject().getName())
 
-        protTomoReconstruction = ProtNovaCtfTomoReconstruction()
-        protTomoReconstruction.setObjLabel('novactf - tomo ctf reconstruction')
+        applyAlignment = self.getInputTs().getFirstItem().getFirstItem().hasTransform()
+        protTomoReconstruction = ProtNovaCtfTomoReconstruction(applyAlignment=applyAlignment)
         protTomoReconstruction.protTomoCtfDefocus.set(self)
-        protTomoReconstruction.radialFirstParameter.set(self.radialFirstParameter.get())
-        protTomoReconstruction.radialSecondParameter.set(self.radialSecondParameter.get())
         protTomoReconstruction.numberOfThreads.set(self.numberOfThreads.get())
         protTomoReconstruction.numberOfMpi.set(self.numberOfMpi.get())
 
         project.scheduleProtocol(protTomoReconstruction)
 
-        self._store()
-
-    # --------------------------- UTILS functions ----------------------------
-    def getCtfTomoSeriesFromTsId(self, setOfCtfTomoSeries, tsId):
-        for ctfTomoSeries in self.inputSetOfCtfTomoSeries.get():
-            if tsId == ctfTomoSeries.getTsId():
-                return ctfTomoSeries
-
-    def getCorrectionType(self):
-        if self.correctionType.get() == 0:
-            correctionType = "phaseflip"
-        elif self.correctionType.get() == 1:
-            correctionType = "multiplication"
-
-        return correctionType
-
-    # --------------------------- INFO functions ----------------------------
+    # --------------------------- INFO functions ------------------------------
     def _validate(self):
         validateMsgs = []
 
-        if self.inputSetOfTiltSeries.get().getSize() != self.inputSetOfCtfTomoSeries.get().getSize():
-            validateMsgs.append("Input set of tilt-series and input set of CTF tomo estimations must contain the "
-                                "same number of elements.")
+        if self.getInputTs().getSize() != self.inputSetOfCtfTomoSeries.get().getSize():
+            validateMsgs.append("Input set of tilt-series and input set of CTFs "
+                                " must contain the same number of items.")
+
+        ctf = self.inputSetOfCtfTomoSeries.get().getFirstItem()
+        if hasattr(ctf, "_IMODDefocusFileFlag"):
+            defFlag = ctf.getIMODDefocusFileFlag()
+            if defFlag in [0, 4] and self.correctAstigmatism.get() == 1:
+                validateMsgs.append("CTF estimation does not have astigmatism values.")
 
         return validateMsgs
 
     def _summary(self):
         summary = []
 
-        counter = 0
-
-        for ts in self.inputSetOfTiltSeries.get():
-            tsId = ts.getTsId()
-            if os.path.exists(os.path.join(self._getExtraPath(tsId), tsId + ".defocus_0")):
-                counter += 1
-
-        if counter != 0:
-            summary.append("Input Tilt-Series: %d.\n"
-                           "Tilt-series defocus processed: %d.\n"
-                           "Defocus files generated for each tilt-series: %d.\n"
-                           % (self.inputSetOfTiltSeries.get().getSize(),
-                              counter,
-                              self.numberOfIntermediateStacks[0]))
+        if len(self.numberOfIntermediateStacks):
+            summary.append(f"Input tilt-series: {self.getInputTs().getSize()}\n"
+                           f"Defocus files generated for each tilt-series: "
+                           f"{self.numberOfIntermediateStacks[0]}\n\n"
+                           "Use this protocol as input for novaCTF - 3D CTF "
+                           "correction and reconstruction.")
         else:
-            summary.append("Output not ready yet.")
+            summary.append("Outputs are not ready yet.")
         return summary
 
-    def _methods(self):
-        methods = []
+    # --------------------------- UTILS functions -----------------------------
+    def getInputTs(self):
+        return self.inputSetOfTiltSeries.get()
 
-        counter = 0
-
-        for ts in self.inputSetOfTiltSeries.get():
-            tsId = ts.getTsId()
-            if os.path.exists(os.path.join(self._getExtraPath(tsId), tsId + ".defocus_0")):
-                counter += 1
-
-        if counter != 0:
-            methods.append("%d defocus files have been generated for each of the %d tilt-series using the defocus "
-                           "algorithm from novaCTF.\n"
-                           % (self.numberOfIntermediateStacks[0],
-                              counter))
-        else:
-            methods.append("Output not ready yet.")
-
-        return methods
+    def getCtfTomoSeriesFromTsId(self, tsId):
+        for ctfTomoSeries in self.inputSetOfCtfTomoSeries.get():
+            if tsId == ctfTomoSeries.getTsId():
+                return ctfTomoSeries
```

### Comparing `scipion-em-novactf-3.0.5/novactf/protocols/protocol_tomoReconstruction.py` & `scipion-em-novactf-3.1.1/novactf/protocols/protocol_tomoReconstruction.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # *
 # * Authors:     Federico P. de Isidro Gomez (fp.deisidro@cnb.csic.es) [1]
 # *
 # * [1] Centro Nacional de Biotecnologia, CSIC, Spain
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
@@ -22,362 +22,472 @@
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 import os
 
-from pwem.objects import Transform
 from pyworkflow import BETA
-from pyworkflow.exceptions import PyworkflowException
 from pyworkflow.object import Set
 import pyworkflow.protocol.params as params
 import pyworkflow.utils.path as path
 from pyworkflow.protocol.constants import STEPS_PARALLEL
 from pwem.protocols import EMProtocol
 from tomo.protocols import ProtTomoBase
-from tomo.objects import Tomogram, TomoAcquisition
-from novactf import Plugin
-from novactf.protocols import ProtNovaCtfTomoDefocus
+from tomo.objects import Tomogram
+
 from imod import Plugin as imodPlugin
-from pwem.emlib.image import ImageHandler
+import imod.utils as imodUtils
+
+from .. import Plugin
 
 
 class ProtNovaCtfTomoReconstruction(EMProtocol, ProtTomoBase):
     """
-    Tomogram reconstruction with ctf correction procedure based on the novaCTF procedure.
+    Tomogram reconstruction with 3D CTF correction by novaCTF.
 
     More info:
             https://github.com/turonova/novaCTF
     """
 
-    _label = 'tomo ctf reconstruction'
+    _label = '3D CTF correction and reconstruction'
     _devStatus = BETA
 
     def __init__(self, **args):
         EMProtocol.__init__(self, **args)
         ProtTomoBase.__init__(self)
         self.stepsExecutionMode = STEPS_PARALLEL
 
     # -------------------------- DEFINE param functions -----------------------
     def _defineParams(self, form):
         form.addSection('Input')
 
         form.addParam('protTomoCtfDefocus',
                       params.PointerParam,
-                      label="NovaCtf defocus estimation run",
-                      pointerClass='ProtNovaCtfTomoDefocus',
-                      help='Select the previous NovaCtf defocus estimation run.')
+                      label="NovaCTF compute defocus run",
+                      pointerClass='ProtNovaCtfTomoDefocus')
 
-        ProtNovaCtfTomoDefocus.defineFilterParameters(form)
+        form.addParam('applyAlignment', params.BooleanParam,
+                      default=True,
+                      label="Apply tilt-series alignment?")
+
+        form.addSection("Erase gold beads")
+        form.addParam('doEraseGold', params.BooleanParam,
+                      default=False, label='Erase gold beads',
+                      help='Remove the gold beads from the tilt-series.')
+
+        form.addParam('inputSetOfLandmarkModels',
+                      params.PointerParam,
+                      allowsNull=True,
+                      condition='doEraseGold',
+                      pointerClass='SetOfLandmarkModels',
+                      label='Input set of fiducial models',
+                      help='Set of fid. models with no gaps after alignment')
+
+        form.addParam('goldDiam', params.IntParam,
+                      condition='doEraseGold',
+                      default=18,
+                      label='Bead diameter (px)',
+                      help="For circle objects, this entry "
+                           "specifies a radius to use for points "
+                           "without an individual point size "
+                           "instead of the object's default sphere "
+                           "radius. This entry is floating point "
+                           "and can be used to overcome the "
+                           "limitations of having an integer "
+                           "default sphere radius. If there are "
+                           "multiple circle objects, enter one "
+                           "value to apply to all objects or a "
+                           "value for each object.")
+
+        form.addSection("Filtering")
+        group = form.addGroup('Radial filtering',
+                              help='This entry controls low-pass filtering with the radial weighting '
+                                   'function. The radial weighting function is linear away from the '
+                                   'origin out to the distance in reciprocal space specified by the '
+                                   'first value, followed by a Gaussian fall-off determined by the '
+                                   'second value.')
+        group.addParam('radialFirstParameter',
+                       params.FloatParam,
+                       default=0.3,
+                       label='Linear region')
+        group.addParam('radialSecondParameter',
+                       params.FloatParam,
+                       default=0.05,
+                       label='Gaussian fall-off')
 
         form.addParallelSection(threads=4, mpi=1)
 
     # -------------------------- INSERT steps functions ---------------------
     def _insertAllSteps(self):
-
         allCreateOutputId = []
+        nstacks = self.protTomoCtfDefocus.get().numberOfIntermediateStacks
 
-        for index, ts in enumerate(self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get()):
+        for index, ts in enumerate(self.getInputTs()):
             convertInputId = self._insertFunctionStep(self.convertInputStep,
-                                                      ts.getObjId(),
-                                                      prerequisites=[])
+                                                      ts.getObjId())
 
             intermediateStacksId = []
 
-            for counter in range(0, self.protTomoCtfDefocus.get().numberOfIntermediateStacks[index].get()):
+            for counter in range(nstacks[index].get()):
                 ctfId = self._insertFunctionStep(self.processIntermediateStacksStep,
                                                  ts.getObjId(),
                                                  counter,
                                                  prerequisites=[convertInputId])
                 intermediateStacksId.append(ctfId)
 
             reconstructionId = self._insertFunctionStep(self.computeReconstructionStep,
-                                                        ts.getObjId(),
+                                                        ts.getObjId(), nstacks[index].get(),
                                                         prerequisites=intermediateStacksId)
 
             createOutputId = self._insertFunctionStep(self.createOutputStep,
                                                       ts.getObjId(),
                                                       prerequisites=[reconstructionId])
             allCreateOutputId.append(createOutputId)
 
         self._insertFunctionStep(self.closeOutputSetsStep,
                                  prerequisites=allCreateOutputId)
 
     # --------------------------- STEPS functions ----------------------------
     def convertInputStep(self, tsObjId):
         with self._lock:
-            ts = self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get()[tsObjId]
-            ti = ts.getFirstItem()
+            ts = self.getInputTs()[tsObjId]
+            firstItem = ts.getFirstItem()
 
         tsId = ts.getTsId()
         extraPrefix = self._getExtraPath(tsId)
         tmpPrefix = self._getTmpPath(tsId)
         path.makePath(tmpPrefix)
         path.makePath(extraPrefix)
 
-        """Apply the transformation form the input tilt-series"""
-        outputTsFileName = os.path.join(tmpPrefix, ti.parseFileName(extension=".st"))
-
-        with self._lock:
-            ts.applyTransform(outputTsFileName)
-            """Generate angle file"""
-            outputTltFileName = os.path.join(tmpPrefix, ti.parseFileName(extension=".tlt"))
-            ts.generateTltFile(outputTltFileName)
+        outputTsFileName = os.path.join(tmpPrefix,
+                                        firstItem.parseFileName(extension=".mrc"))
+        self.info("Tilt series %s linked." % tsId)
+        path.createLink(firstItem.getFileName(), outputTsFileName)
+
+        # Generate angle file
+        outputTltFileName = os.path.join(tmpPrefix,
+                                         firstItem.parseFileName(extension=".tlt"))
+        ts.generateTltFile(outputTltFileName)
+
+        if firstItem.hasTransform():
+            # Generate transformation matrices file
+            outputTmFileName = os.path.join(tmpPrefix,
+                                            firstItem.parseFileName(extension=".xf"))
+            imodUtils.formatTransformFile(ts, outputTmFileName)
 
     def processIntermediateStacksStep(self, tsObjId, counter):
+
         with self._lock:
-            ts = self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get()[tsObjId]
-            ti = ts.getFirstItem()
+            ts = self.getInputTs()[tsObjId]
+            firstItem = ts.getFirstItem()
 
         tsId = ts.getTsId()
         tmpPrefix = self._getTmpPath(tsId)
         extraPrefixPreviousProt = self.protTomoCtfDefocus.get()._getExtraPath(tsId)
 
-        defocusFilePath = os.path.join(extraPrefixPreviousProt, ti.parseFileName(extension=".defocus_"))
-        tltFilePath = os.path.join(tmpPrefix, ti.parseFileName(extension=".tlt"))
-        outputFilePath = os.path.join(tmpPrefix, ti.parseFileName(extension=".st_"))
+        defocusFilePath = os.path.join(extraPrefixPreviousProt,
+                                       firstItem.parseFileName(extension=".defocus_"))
+        tltFilePath = os.path.join(tmpPrefix, firstItem.parseFileName(extension=".tlt"))
+        outputFilePath = os.path.join(tmpPrefix, firstItem.parseFileName(extension=".mrc_"))
 
         # CTF correction step
         paramsCtfCorrection = {
             'Algorithm': "ctfCorrection",
-            'InputProjections': os.path.join(tmpPrefix, ti.parseFileName(extension=".st")),
+            'InputProjections': os.path.join(tmpPrefix,
+                                             firstItem.parseFileName(extension=".mrc")),
             'OutputFile': outputFilePath + str(counter),
             'DefocusFile': defocusFilePath + str(counter),
             'TiltFile': tltFilePath,
             'CorrectionType': self.getCorrectionType(),
             'DefocusFileFormat': "imod",
             'CorrectAstigmatism': self.protTomoCtfDefocus.get().correctAstigmatism.get(),
-            'PixelSize': self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get().getSamplingRate() / 10,
+            'PixelSize': self.getInputTs().getSamplingRate() / 10,
             'AmplitudeContrast':
-                self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get().getAcquisition().getAmplitudeContrast(),
+                self.getInputTs().getAcquisition().getAmplitudeContrast(),
             'SphericalAberration':
-                self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get().getAcquisition().getSphericalAberration(),
-            'Voltage': self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get().getAcquisition().getVoltage()
+                self.getInputTs().getAcquisition().getSphericalAberration(),
+            'Voltage': self.getInputTs().getAcquisition().getVoltage()
         }
 
         argsCtfCorrection = "-Algorithm %(Algorithm)s " \
                             "-InputProjections %(InputProjections)s " \
                             "-OutputFile %(OutputFile)s " \
                             "-DefocusFile %(DefocusFile)s " \
                             "-TILTFILE %(TiltFile)s " \
                             "-CorrectionType %(CorrectionType)s " \
                             "-DefocusFileFormat %(DefocusFileFormat)s " \
                             "-CorrectAstigmatism %(CorrectAstigmatism)s " \
                             "-PixelSize %(PixelSize)f " \
                             "-AmplitudeContrast %(AmplitudeContrast)f " \
                             "-Cs %(SphericalAberration)f " \
-                            "-Volt %(Voltage)d"
+                            "-Volt %(Voltage)d "
 
         Plugin.runNovactf(self, 'novaCTF', argsCtfCorrection % paramsCtfCorrection)
+        currentFn = outputFilePath + str(counter)
+
+        # Alignment step
+        if self.applyAlignment and firstItem.hasTransform():
+            paramsAlignment = {
+                'input': currentFn,
+                'output': os.path.join(tmpPrefix,
+                                       firstItem.parseFileName(suffix="_ali",
+                                                               extension=".mrc_")) + str(counter),
+                'xform': os.path.join(tmpPrefix,
+                                      firstItem.parseFileName(extension=".xf"))
+            }
+
+            argsAlignment = "-input %(input)s " \
+                            "-output %(output)s " \
+                            "-xform %(xform)s -AdjustOrigin -NearestNeighbor -taper 1,1 "
+
+            rotationAngle = ts.getAcquisition().getTiltAxisAngle()
+
+            # Check if rotation angle is greater than 45º.
+            # If so, swap x and y dimensions to adapt output image
+            # sizes to the final sample disposition.
+            if 45 < abs(rotationAngle) < 135:
+                paramsAlignment.update({
+                    'size': "%d,%d" % (firstItem.getYDim(), firstItem.getXDim())
+                })
+
+                argsAlignment += "-size %(size)s "
+
+            imodPlugin.runImod(self, 'newstack', argsAlignment % paramsAlignment)
+            currentFn = os.path.join(tmpPrefix,
+                                     firstItem.parseFileName(suffix="_ali",
+                                                             extension=".mrc_")) + str(counter)
+
+        # Erase gold step  # TODO: fixme
+        if self.doEraseGold:
+            lm = self.inputSetOfLandmarkModels.get().getLandmarkModelFromTsId(tsId=tsId)
+
+            # apply alignment to fid. model
+            imodPlugin.runImod(self, 'xfmodel',
+                               f'-XformsToApply {outputTmFileName}'
+                               f' {lm.getModelName()} '
+                               f'{os.path.join(tmpPrefix, firstItem.parseFileName(suffix="_erase", extension=".fid"))}')
+
+            paramsCcderaser = {
+                'inputFile': currentFn,
+                'outputFile': os.path.join(tmpPrefix,
+                                           firstItem.parseFileName(suffix="_erase",
+                                                                   extension=".mrc_" + str(counter))),
+                'modelFile': os.path.join(tmpPrefix,
+                                          firstItem.parseFileName(suffix="_erase", extension=".fid")),
+                'betterRadius': self.goldDiam.get() / 2,
+                'polynomialOrder': 0,
+                'circleObjects': "/"
+            }
+
+            argsCcderaser = "-InputFile %(inputFile)s " \
+                            "-OutputFile %(outputFile)s " \
+                            "-ModelFile %(modelFile)s " \
+                            "-BetterRadius %(betterRadius)f " \
+                            "-PolynomialOrder %(polynomialOrder)d " \
+                            "-CircleObjects %(circleObjects)s " \
+                            "-MergePatches 1 " \
+                            "-ExcludeAdjacent " \
+                            "-SkipTurnedOffPoints 1 " \
+                            "-ExpandCircleIterations 3 "
+
+            imodPlugin.runImod(self, 'ccderaser', argsCcderaser % paramsCcderaser)
+            currentFn = os.path.join(tmpPrefix,
+                                     firstItem.parseFileName(suffix="_erase",
+                                                             extension=".mrc_" + str(counter)))
 
-        # Flipping step
+        # Flipping step (XYZ to XZY)
         paramsClip = {
-            'inputFilePath': os.path.join(tmpPrefix, ti.parseFileName(extension=".st_" + str(counter))),
-            'outputFilePath': os.path.join(tmpPrefix, ti.parseFileName(suffix="_flip",
-                                                                                      extension=".st_" + str(counter))),
+            'inputFilePath': currentFn,
+            'outputFilePath': os.path.join(tmpPrefix,
+                                           firstItem.parseFileName(suffix="_flip",
+                                                                   extension=".mrc_" + str(counter))),
         }
 
         argsClip = "flipyz " \
                    "%(inputFilePath)s " \
-                   "%(outputFilePath)s"
+                   "%(outputFilePath)s "
 
         imodPlugin.runImod(self, 'clip', argsClip % paramsClip)
+        currentFn = os.path.join(tmpPrefix,
+                                 firstItem.parseFileName(suffix="_flip",
+                                                         extension=".mrc_" + str(counter)))
 
         # Filtering step
-        flippedFilePath = os.path.join(tmpPrefix,
-                                       ti.parseFileName(suffix="_flip", extension=".st_"))
         outputFilePath = os.path.join(tmpPrefix,
-                                      ti.parseFileName(suffix="_flip_filter", extension=".st_"))
-        tltFilePath = os.path.join(tmpPrefix, ti.parseFileName(extension=".tlt"))
+                                      firstItem.parseFileName(suffix="_filter", extension=".mrc_"))
 
         paramsFilterProjections = {
             'Algorithm': "filterProjections",
-            'InputProjections': flippedFilePath + str(counter),
+            'InputProjections': currentFn,
             'OutputFile': outputFilePath + str(counter),
             'TiltFile': tltFilePath,
             'StackOrientation': "xz",
             'Radial': str(self.radialFirstParameter.get()) + "," + str(self.radialSecondParameter.get())
         }
 
         argsFilterProjections = "-Algorithm %(Algorithm)s " \
                                 "-InputProjections %(InputProjections)s " \
                                 "-OutputFile %(OutputFile)s " \
                                 "-TILTFILE %(TiltFile)s " \
                                 "-StackOrientation %(StackOrientation)s " \
-                                "-RADIAL %(Radial)s"
+                                "-RADIAL %(Radial)s "
 
         Plugin.runNovactf(self, 'novaCTF', argsFilterProjections % paramsFilterProjections)
 
-    def computeReconstructionStep(self, tsObjId):
-        ts = self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get()[tsObjId]
+    def computeReconstructionStep(self, tsObjId, nstacks):
+        with self._lock:
+            ts = self.getInputTs()[tsObjId]
+            firstItem = ts.getFirstItem()
+
         tsId = ts.getTsId()
+
         extraPrefix = self._getExtraPath(tsId)
         tmpPrefix = self._getTmpPath(tsId)
 
-        firstItem = ts.getFirstItem()
-
-        outputFileNameFlip = firstItem.parseFileName(suffix="_flip", extension=".mrc")
-        outputFileName = firstItem.parseFileName(extension=".mrc")
-
-        print("*** otuput file name")
-        print(outputFileNameFlip)
-        outputFilePathFlipped = os.path.join(tmpPrefix, outputFileNameFlip)
-        print(outputFilePathFlipped)
-
-        tltFilePath = os.path.join(tmpPrefix, firstItem.parseFileName(extension=".tlt"))
-
-        ih = ImageHandler()
-        xDim, yDim, _, _ = ih.getDimensions(firstItem.getFileName()+":mrc")
+        outputFilePath = os.path.join(tmpPrefix,
+                                      firstItem.parseFileName(suffix="_rec", extension=".mrc"))
+        tltFilePath = os.path.join(tmpPrefix,
+                                   firstItem.parseFileName(extension=".tlt"))
 
         params3dctf = {
             'Algorithm': "3dctf",
-            'InputProjections': os.path.join(tmpPrefix, firstItem.parseFileName(suffix="_flip_filter",
-                                                                                        extension=".st")),
-            'OutputFile': outputFilePathFlipped,
+            'InputProjections': os.path.join(tmpPrefix, firstItem.parseFileName(suffix="_filter",
+                                                                                extension=".mrc")),
+            'OutputFile': outputFilePath,
+            'FullImage': "%d,%d" % (firstItem.getXDim(), firstItem.getYDim()),
             'TiltFile': tltFilePath,
             'Thickness': self.protTomoCtfDefocus.get().tomoThickness.get(),
-            'FullImage': str(xDim) + "," + str(yDim),
             'Shift': "0.0," + str(self.protTomoCtfDefocus.get().tomoShift.get()),
-            'PixelSize': self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get().getSamplingRate() / 10,
-            'DefocusStep': self.protTomoCtfDefocus.get().defocusStep.get()
+            'PixelSize': self.getInputTs().getSamplingRate() / 10,
+            'NumberOfStacks': nstacks
         }
 
         args3dctf = "-Algorithm %(Algorithm)s " \
                     "-InputProjections %(InputProjections)s " \
                     "-OutputFile %(OutputFile)s " \
+                    "-FULLIMAGE %(FullImage)s " \
                     "-TILTFILE %(TiltFile)s " \
                     "-THICKNESS %(Thickness)d " \
-                    "-FULLIMAGE %(FullImage)s " \
                     "-SHIFT %(Shift)s " \
                     "-PixelSize %(PixelSize)f " \
-                    "-DefocusStep %(DefocusStep)d"
+                    "-NumberOfInputStacks %(NumberOfStacks)d " \
+                    "-Use3DCTF 1 "
+
+        # Check if rotation angle is greater than 45º.
+        # If so, swap x and y dimensions to adapt output image
+        # sizes to the final sample disposition.
+
+        rotationAngle = ts.getAcquisition().getTiltAxisAngle()
+
+        if 45 < abs(rotationAngle) < 135:
+            params3dctf['FullImage'] = "%d,%d" % (firstItem.getYDim(), firstItem.getXDim())
 
         Plugin.runNovactf(self, 'novaCTF', args3dctf % params3dctf)
 
+        # Trim vol - rotate around X
         paramsTrimvol = {
-            'inputFilePath': outputFilePathFlipped,
-            'outputFilePath': os.path.join(extraPrefix, outputFileName)
+            'inputFilePath': outputFilePath,
+            'outputFilePath': os.path.join(extraPrefix,
+                                           firstItem.parseFileName(extension=".mrc"))
         }
 
-        argsTrimvol = "%(inputFilePath)s " \
-                      "%(outputFilePath)s " \
-                      "-yz "
+        argsTrimvol = "-rx %(inputFilePath)s " \
+                      "%(outputFilePath)s "
 
         imodPlugin.runImod(self, 'trimvol', argsTrimvol % paramsTrimvol)
 
-    def createOutputStep(self, tsObjId):
+        # Remove intermediate files. Necessary for big sets of tilt-series
+        path.cleanPath(self._getTmpPath(tsId))
 
-        ts = self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get()[tsObjId]
+    def createOutputStep(self, tsObjId):
+        with self._lock:
+            ts = self.getInputTs()[tsObjId]
+            firstItem = ts.getFirstItem()
+            acq = ts.getAcquisition()
 
         tsId = ts.getTsId()
-        angleMax = ts[ts.getSize()].getTiltAngle()
-        angleStepAverage = self.getAngleStepFromSeries(ts)
-
         extraPrefix = self._getExtraPath(tsId)
 
-        firstItem = ts.getFirstItem().clone()
+        outputTomos = self.getOutputSetOfTomograms()
+        outputFn = os.path.join(extraPrefix, firstItem.parseFileName(extension=".mrc"))
 
-        """Remove intermediate files. Necessary for big sets of tilt-series"""
-        # path.cleanPath(self._getTmpPath(tsId))
+        if os.path.exists(outputFn):
+            newTomogram = Tomogram()
+            newTomogram.setLocation(outputFn)
+            newTomogram.setTsId(tsId)
+            newTomogram.setSamplingRate(ts.getSamplingRate())
+
+            # Set default tomogram origin
+            newTomogram.setOrigin(newOrigin=None)
+            newTomogram.setAcquisition(acq)
+
+            outputTomos.append(newTomogram)
+            outputTomos.write()
+            self._store()
 
-        """Generate output set"""
-        outputSetOfTomograms = self.getOutputSetOfTomograms()
+    def closeOutputSetsStep(self):
+        self.getOutputSetOfTomograms().setStreamState(Set.STREAM_CLOSED)
+        self._store()
 
-        newTomogram = Tomogram()
-        newTomogram.setLocation(os.path.join(extraPrefix, firstItem.parseFileName(extension=".mrc")))
-
-        if not os.path.exists(newTomogram.getFileName()):
-            raise PyworkflowException("%s does not exist."
-                                      "\ntsObj: %d"
-                                      "\ntsId: %s"
-                                      "\nobject tsId %s"
-                                      % (newTomogram.getFileName(), tsObjId, tsId, firstItem.getTsId()))
-
-        # Set tomogram origin
-        origin = Transform()
-        sr = self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get().getSamplingRate()
-
-        ih = ImageHandler()
-        xDim, yDim, _, _ = ih.getDimensions(firstItem.getFileName()+":mrc")
-
-        origin.setShifts(xDim / -2. * sr,
-                         yDim / -2. * sr,
-                         self.protTomoCtfDefocus.get().tomoThickness.get() / -2 * sr)
-
-        newTomogram.setOrigin(origin)
-
-        # Set tomogram acquisition
-        acquisition = TomoAcquisition()
-        acquisition.setAngleMin(firstItem.getTiltAngle())
-        acquisition.setAngleMax(angleMax)
-        acquisition.setStep(angleStepAverage)
-        newTomogram.setAcquisition(acquisition)
+    # --------------------------- INFO functions ----------------------------
+    def _validate(self):
+        validateMsg = []
 
-        outputSetOfTomograms.append(newTomogram)
-        outputSetOfTomograms.write()
-        self._store()
+        ts = self.getInputTs()
+        if self.applyAlignment and not ts.getFirstItem().getFirstItem().hasTransform():
+            validateMsg.append("Input tilt-series do not have alignment "
+                               "information! You cannot apply alignment.")
 
-    def closeOutputSetsStep(self):
-        self.getOutputSetOfTomograms().setStreamState(Set.STREAM_CLOSED)
+        if self.doEraseGold and not self.inputSetOfLandmarkModels.hasValue():
+            validateMsg.append("You have to provide input set of landmarks to erase gold.")
 
-        self._store()
+        return validateMsg
+
+    def _summary(self):
+        summary = []
+
+        if hasattr(self, 'outputSetOfTomograms'):
+            summary.append(f"Input tilt-series: {self.getInputTs().getSize()}\n"
+                           f"CTF corrected tomos calculated: "
+                           f"{self.outputSetOfTomograms.getSize()}")
+        else:
+            summary.append("Outputs are not ready yet.")
+
+        return summary
+
+    def _methods(self):
+        methods = []
+
+        if hasattr(self, 'outputSetOfTomograms'):
+            methods.append(f"{self.outputSetOfTomograms.getSize()} "
+                           "3D CTF corrected tomograms have been calculated "
+                           "with NovaCTF.")
+
+        return methods
 
     # --------------------------- UTILS functions ----------------------------
+    def getInputTs(self, pointer=False):
+        if pointer:
+            return self.protTomoCtfDefocus.get().inputSetOfTiltSeries
+        else:
+            return self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get()
+
     def getCorrectionType(self):
         if self.protTomoCtfDefocus.get().correctionType.get() == 0:
             correctionType = "phaseflip"
-        elif self.protTomoCtfDefocus.get().correctionType.get() == 1:
+        else:
             correctionType = "multiplication"
 
         return correctionType
 
     def getOutputSetOfTomograms(self):
         if hasattr(self, "outputSetOfTomograms"):
             self.outputSetOfTomograms.enableAppend()
         else:
             outputSetOfTomograms = self._createSetOfTomograms()
-            outputSetOfTomograms.copyInfo(self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get())
+            outputSetOfTomograms.copyInfo(self.getInputTs())
             outputSetOfTomograms.setStreamState(Set.STREAM_OPEN)
             self._defineOutputs(outputSetOfTomograms=outputSetOfTomograms)
-            self._defineSourceRelation(self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get(), outputSetOfTomograms)
+            self._defineSourceRelation(self.getInputTs(pointer=True), outputSetOfTomograms)
 
         return self.outputSetOfTomograms
-
-    @staticmethod
-    def getAngleStepFromSeries(ts):
-        """ This method return the average angles step from a series. """
-
-        angleStepAverage = 0
-        # This was causing "recursive use of cursor not allowed" error.
-        # for i in range(1, ts.getSize()):
-        #     angleStepAverage += abs(ts[i].getTiltAngle() - ts[i + 1].getTiltAngle())
-        angles = []
-        for ti in ts:
-            angles.append(ti.getTiltAngle())
-
-        for i in range(0, len(angles)-1):
-            angleStepAverage += abs(angles[i] - angles[i + 1])
-
-        angleStepAverage /= ts.getSize() - 1
-
-        return angleStepAverage
-
-    # --------------------------- INFO functions ----------------------------
-    def _summary(self):
-        summary = []
-        if hasattr(self, 'outputSetOfTomograms'):
-            summary.append("Input Tilt-Series: %d.\nCTF corrected reconstructions calculated: %d.\n"
-                           % (self.protTomoCtfDefocus.get().inputSetOfTiltSeries.get().getSize(),
-                              self.outputSetOfTomograms.getSize()))
-        else:
-            summary.append("Output classes not ready yet.")
-        return summary
-
-    def _methods(self):
-        methods = []
-        if hasattr(self, 'outputSetOfTomograms'):
-            methods.append("%d CTF corrected tomograms have been calculated using the NovaCtf software.\n"
-                           % (self.outputSetOfTomograms.getSize()))
-        else:
-            methods.append("Output classes not ready yet.")
-        return methods
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `scipion-em-novactf-3.0.5/scipion_em_novactf.egg-info/SOURCES.txt` & `scipion-em-novactf-3.1.1/scipion_em_novactf.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,14 @@
+CHANGES.txt
 LICENSE
 MANIFEST.in
 README.rst
-requirements.txt
 setup.py
 novactf/__init__.py
 novactf/bibtex.py
-novactf/constants.py
 novactf/protocols.conf
 novactf/protocols/__init__.py
 novactf/protocols/protocol_tomoDefocus.py
 novactf/protocols/protocol_tomoReconstruction.py
 novactf/tests/__init__.py
 novactf/tests/test_protocols_novactf.py
 scipion_em_novactf.egg-info/PKG-INFO
```

### Comparing `scipion-em-novactf-3.0.5/setup.py` & `scipion-em-novactf-3.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # *
 # * Authors:     Federico P. de Isidro Gomez (fp.deisidro@cnb.csi.es) [1]
 # *
 # * [1] Centro Nacional de Biotecnologia, CSIC, Spain
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
@@ -21,15 +21,14 @@
 # *
 # *  All comments concerning this program package may be sent to the
 # *  e-mail address 'scipion@cnb.csic.es'
 # *
 # **************************************************************************
 
 """A setuptools based setup module.
-
 See:
 https://packaging.python.org/en/latest/distributing.html
 https://github.com/pypa/sampleproject
 """
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
@@ -41,18 +40,14 @@
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.rst'), encoding='utf-8') as f:
     long_description = f.read()
 
-# Load requirements.txt
-with open('requirements.txt') as f:
-    requirements = f.read().splitlines()
-
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
     # users can install this project, e.g.:
@@ -73,15 +68,15 @@
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
     version=__version__,  # Required
 
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
-    description='novaCTF ready to use in scipion.',  # Required
+    description='Plugin to use NovaCTF in Scipion',  # Required
 
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
     # Often, this is the same as your README, so you can just read it in from
     # that file directly (as we have already done above)
     #
@@ -89,87 +84,121 @@
     # https://packaging.python.org/specifications/core-metadata/#description-optional
     long_description=long_description,  # Optional
 
     # This should be a valid link to your project's main homepage.
     #
     # This field corresponds to the "Home-Page" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#home-page-optional
-    url='https://github.com/scipion-em/scipion-em-novaCtf',  # Optional
+    url='https://github.com/scipion-em/scipion-em-novactf',  # Optional
 
     # This should be your name or the name of the organization which owns the
     # project.
     author='I2PC',  # Optional
 
     # This should be a valid email address corresponding to the author listed
     # above.
     author_email='scipion@cnb.csic.es',  # Optional
 
+    # Classifiers help users find your project by categorizing it.
+    #
+    # For a list of valid classifiers, see
+    # https://pypi.python.org/pypi?%3Aaction=list_classifiers
+    classifiers=[  # Optional
+        # How mature is this project? Common values are
+        #   3 - Alpha
+        #   4 - Beta
+        #   5 - Production/Stable
+        'Development Status :: 4 - Beta',
+
+        # Indicate who your project is intended for
+        #   'Intended Audience :: Users',
+
+        # Pick your license as you wish
+        'License :: OSI Approved :: GNU General Public License v3 (GPLv3)',
+
+        # Specify the Python versions you support here. In particular, ensure
+        # that you indicate whether you support Python 2, Python 3 or both.
+        'Programming Language :: Python :: 3'
+    ],
+
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a string of words separated by whitespace, not a list.
-    keywords='scipion cryoem imageprocessing scipion-3.0',  # Optional
+    keywords='scipion novactf electron-microscopy cryo-em cryo-tomography '
+             'subtomogram-averaging structural-biology image-processing '
+             'scipion-3.0',  # Optional
 
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
     # the `py_modules` argument instead as follows, which will expect a file
     # called `my_module.py` to exist:
     #
     #   py_modules=["my_module"],
     #
-    # packages=find_packages(exclude=['contrib', 'docs', 'tests']),  # Required
+    #packages=find_packages(exclude=['contrib', 'docs', 'tests']),  # Required
     packages=find_packages(),
-
-    # install requires
-    install_requires=[requirements],
-
-    # Although 'package_data' is the preferred approach, in some case you may
-    # need to place data files outside of your packages. See:
-    # http://docs.python.org/3.4/distutils/setupscript.html#installing-additional-files
-    #
-    # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
-    # data_files=[('my_data', ['data/data_file'])],  # Optional
-
-    # To provide executable scripts, use entry points in preference to the
-    # "scripts" keyword. Entry points provide cross-platform support and allow
-    # `pip` to create the appropriate form of executable for the target
-    # platform.
-    #
-    # For example, the following would provide a command called `sample` which
-    # executes the function `main` from this package when invoked:
-    entry_points={
-        'pyworkflow.plugin': 'novactf = novactf'
-    },
-
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/en/latest/requirements.html
-    # install_requires=['peppercorn'],  # Optional
+    install_requires=['scipion-em-tomo', 'scipion-em-imod'],  # Optional
 
     # List additional groups of dependencies here (e.g. development
     # dependencies). Users will be able to install these using the "extras"
     # syntax, for example:
     #
     #   $ pip install sampleproject[dev]
     #
     # Similar to `install_requires` above, these must be valid existing
     # projects.
-    # extras_require={  # Optional
+    #extras_require={  # Optional
     #    'dev': ['check-manifest'],
     #    'tests': ['coverage'],
-    # },
+    #},
 
     # If there are data files included in your packages that need to be
     # installed, specify them here.
     #
     # If using Python 2.6 or earlier, then these have to be included in
     # MANIFEST.in as well.
     # include_package_data=True,
     package_data={  # Optional
-       'novactf': ['novaCtf_logo.png', 'protocols.conf'],
-    }
+       'novactf': ['protocols.conf'],
+    },
+
+    # Although 'package_data' is the preferred approach, in some case you may
+    # need to place data files outside of your packages. See:
+    # http://docs.python.org/3.4/distutils/setupscript.html#installing-additional-files
+    #
+    # In this case, 'data_file' will be installed into '<sys.prefix>/my_data'
+    #data_files=[('my_data', ['data/data_file'])],  # Optional
+
+    # To provide executable scripts, use entry points in preference to the
+    # "scripts" keyword. Entry points provide cross-platform support and allow
+    # `pip` to create the appropriate form of executable for the target
+    # platform.
+    #
+    # For example, the following would provide a command called `sample` which
+    # executes the function `main` from this package when invoked:
+    entry_points={
+        'pyworkflow.plugin': 'novactf = novactf'
+    },
+
+    # List additional URLs that are relevant to your project as a dict.
+    #
+    # This field corresponds to the "Project-URL" metadata fields:
+    # https://packaging.python.org/specifications/core-metadata/#project-url-multiple-use
+    #
+    # Examples listed include a pattern for specifying where the package tracks
+    # issues, where the source is hosted, where to say thanks to the package
+    # maintainers, and where to support the project financially. The key is
+    # what's used to render the link text on PyPI.
+    project_urls={  # Optional
+        'Bug Reports': 'https://github.com/scipion-em/scipion-em-novactf/issues',
+        'Source': 'https://github.com/scipion-em/scipion-em-novactf/',
+    },
 )
```

