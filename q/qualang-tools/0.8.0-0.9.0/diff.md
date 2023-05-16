# Comparing `tmp/qualang-tools-0.8.0.tar.gz` & `tmp/qualang-tools-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qualang-tools-0.8.0.tar", max compression
+gzip compressed data, was "qualang-tools-0.9.0.tar", max compression
```

## Comparing `qualang-tools-0.8.0.tar` & `qualang-tools-0.9.0.tar`

### file list

```diff
@@ -1,46 +1,50 @@
--rw-r--r--   0        0        0     1520 2022-04-04 13:06:13.613439 qualang-tools-0.8.0/LICENSE
--rw-r--r--   0        0        0     3674 2022-04-04 13:06:13.613439 qualang-tools-0.8.0/README.md
--rw-r--r--   0        0        0     1625 2022-04-04 13:06:20.609524 qualang-tools-0.8.0/pyproject.toml
--rw-r--r--   0        0        0       92 2022-04-04 13:06:13.613439 qualang-tools-0.8.0/qualang_tools/__init__.py
--rw-r--r--   0        0        0    89954 2022-04-04 13:06:13.617439 qualang-tools-0.8.0/qualang_tools/addons/InteractivePlotLib.py
--rw-r--r--   0        0        0   868183 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/addons/InteractivePlotLib_demonstration.png
--rw-r--r--   0        0        0     3908 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/addons/README.md
--rw-r--r--   0        0        0        0 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/addons/__init__.py
--rw-r--r--   0        0        0    21854 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/bakery/README.md
--rw-r--r--   0        0        0      122 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/bakery/__init__.py
--rw-r--r--   0        0        0    53345 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/bakery/bakery.py
--rw-r--r--   0        0        0     7161 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/bakery/randomized_benchmark.py
--rw-r--r--   0        0        0     3044 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/bakery/randomized_benchmark_c1.py
--rw-r--r--   0        0        0     3667 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/bakery/xeb.py
--rw-r--r--   0        0        0      663 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/README.md
--rw-r--r--   0        0        0     1585 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/README_config_GUI.md
--rw-r--r--   0        0        0     6364 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/README_config_builder.md
--rw-r--r--   0        0        0      673 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/README_integration_weights_tools.md
--rw-r--r--   0        0        0     1080 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/README_waveform_tools.md
--rw-r--r--   0        0        0     1332 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/__init__.py
--rw-r--r--   0        0        0     8868 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/builder.py
--rw-r--r--   0        0        0    34943 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/components.py
--rw-r--r--   0        0        0     8412 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/configuration.py
--rw-r--r--   0        0        0      148 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/exceptions.py
--rw-r--r--   0        0        0     3732 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/gui.py
--rw-r--r--   0        0        0     4619 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/integration_weights_tools.py
--rw-r--r--   0        0        0     1763 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/parameters.py
--rw-r--r--   0        0        0     4978 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/primitive_components.py
--rw-r--r--   0        0        0      351 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/server/app.py
--rw-r--r--   0        0        0    31848 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/server/component_editor.py
--rw-r--r--   0        0        0    15490 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/server/config_editor.py
--rw-r--r--   0        0        0     1625 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/server/download.py
--rw-r--r--   0        0        0     8871 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/server/editors.py
--rw-r--r--   0        0        0    19715 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/server/qua1_openapi.json
--rw-r--r--   0        0        0     1611 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/server/readme.md
--rw-r--r--   0        0        0     4828 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/server/upload.py
--rw-r--r--   0        0        0     3738 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/config/waveform_tools.py
--rw-r--r--   0        0        0      783 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/control_panel/README.md
--rw-r--r--   0        0        0     6587 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/control_panel/README_manual_output_control.md
--rw-r--r--   0        0        0     6678 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/control_panel/README_vna.md
--rw-r--r--   0        0        0      172 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/control_panel/__init__.py
--rw-r--r--   0        0        0    30529 2022-04-04 13:06:13.621440 qualang-tools-0.8.0/qualang_tools/control_panel/manual_output_control.py
--rw-r--r--   0        0        0    29044 2022-04-04 13:06:13.625440 qualang-tools-0.8.0/qualang_tools/control_panel/vna.py
--rw-r--r--   0        0        0     1976 2022-04-04 13:06:13.625440 qualang-tools-0.8.0/qualang_tools/simulator_tools.py
--rw-r--r--   0        0        0     5115 2022-04-04 13:06:21.686342 qualang-tools-0.8.0/setup.py
--rw-r--r--   0        0        0     5016 2022-04-04 13:06:21.687210 qualang-tools-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1520 2022-05-24 13:51:16.064985 qualang-tools-0.9.0/LICENSE
+-rw-r--r--   0        0        0     3685 2022-05-24 13:51:16.064985 qualang-tools-0.9.0/README.md
+-rw-r--r--   0        0        0     1625 2022-05-24 13:51:22.144976 qualang-tools-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0       92 2022-05-24 13:51:16.064985 qualang-tools-0.9.0/qualang_tools/__init__.py
+-rw-r--r--   0        0        0    89954 2022-05-24 13:51:16.064985 qualang-tools-0.9.0/qualang_tools/addons/InteractivePlotLib.py
+-rw-r--r--   0        0        0   868183 2022-05-24 13:51:16.068986 qualang-tools-0.9.0/qualang_tools/addons/InteractivePlotLib_demonstration.png
+-rw-r--r--   0        0        0     3908 2022-05-24 13:51:16.068986 qualang-tools-0.9.0/qualang_tools/addons/README.md
+-rw-r--r--   0        0        0        0 2022-05-24 13:51:16.068986 qualang-tools-0.9.0/qualang_tools/addons/__init__.py
+-rw-r--r--   0        0        0   130526 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/analysis/IQ.png
+-rw-r--r--   0        0        0      779 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/analysis/README.md
+-rw-r--r--   0        0        0      119 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/analysis/__init__.py
+-rw-r--r--   0        0        0     5557 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/analysis/discriminator.py
+-rw-r--r--   0        0        0    21920 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/bakery/README.md
+-rw-r--r--   0        0        0      122 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/bakery/__init__.py
+-rw-r--r--   0        0        0    53345 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/bakery/bakery.py
+-rw-r--r--   0        0        0     7161 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/bakery/randomized_benchmark.py
+-rw-r--r--   0        0        0     3044 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/bakery/randomized_benchmark_c1.py
+-rw-r--r--   0        0        0     3667 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/bakery/xeb.py
+-rw-r--r--   0        0        0      663 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/README.md
+-rw-r--r--   0        0        0     1585 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/README_config_GUI.md
+-rw-r--r--   0        0        0     6441 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/README_config_builder.md
+-rw-r--r--   0        0        0      673 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/README_integration_weights_tools.md
+-rw-r--r--   0        0        0     1080 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/README_waveform_tools.md
+-rw-r--r--   0        0        0     1350 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/__init__.py
+-rw-r--r--   0        0        0     9436 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/builder.py
+-rw-r--r--   0        0        0    41865 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/components.py
+-rw-r--r--   0        0        0    10538 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/configuration.py
+-rw-r--r--   0        0        0      148 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/exceptions.py
+-rw-r--r--   0        0        0     3732 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/gui.py
+-rw-r--r--   0        0        0     4619 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/integration_weights_tools.py
+-rw-r--r--   0        0        0    10180 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/parameters.py
+-rw-r--r--   0        0        0     7426 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/primitive_components.py
+-rw-r--r--   0        0        0      351 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/server/app.py
+-rw-r--r--   0        0        0    31848 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/server/component_editor.py
+-rw-r--r--   0        0        0    15490 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/server/config_editor.py
+-rw-r--r--   0        0        0     1625 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/server/download.py
+-rw-r--r--   0        0        0     8871 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/server/editors.py
+-rw-r--r--   0        0        0    19715 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/server/qua1_openapi.json
+-rw-r--r--   0        0        0     1611 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/server/readme.md
+-rw-r--r--   0        0        0     4828 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/server/upload.py
+-rw-r--r--   0        0        0     3738 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/config/waveform_tools.py
+-rw-r--r--   0        0        0      783 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/control_panel/README.md
+-rw-r--r--   0        0        0     6587 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/control_panel/README_manual_output_control.md
+-rw-r--r--   0        0        0     6678 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/control_panel/README_vna.md
+-rw-r--r--   0        0        0      172 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/control_panel/__init__.py
+-rw-r--r--   0        0        0    30529 2022-05-24 13:51:16.072986 qualang-tools-0.9.0/qualang_tools/control_panel/manual_output_control.py
+-rw-r--r--   0        0        0    29044 2022-05-24 13:51:16.076986 qualang-tools-0.9.0/qualang_tools/control_panel/vna.py
+-rw-r--r--   0        0        0     1976 2022-05-24 13:51:16.076986 qualang-tools-0.9.0/qualang_tools/simulator_tools.py
+-rw-r--r--   0        0        0     5153 2022-05-24 13:51:23.170210 qualang-tools-0.9.0/setup.py
+-rw-r--r--   0        0        0     5027 2022-05-24 13:51:23.170716 qualang-tools-0.9.0/PKG-INFO
```

### Comparing `qualang-tools-0.8.0/LICENSE` & `qualang-tools-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/README.md` & `qualang-tools-0.9.0/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
   * [ManualOutputControl](README_manual_output_control.md) - This module allows controlling the outputs from the OPX in CW mode. Once created, it has an API for defining which channels are on. Analog channels also have an API for defining their amplitude and frequency.
   * [VNA](README_vna.md) - This module allows to configure the OPX as a VNA for a given element (readout resonator for instance) and operation (readout pulse for instance) already defined in the configuration. Once created, it has an API for defining which measurements are to be run depending on the down-conversion solution used (ED: envelope detector, IR: image rejection mixer, IQ: IQ mixer).
 
 ## Installation
 
 Install the current version using `pip`, the `--upgrade` flag ensures that you will get the latest version.
 
-```
+```commandline
 pip install --upgrade qualang-tools
 ```
 
 ## Support and Contribution
 Have an idea for another tool? A way to improve an existing one? Found a bug in our code?
 
 We'll be happy if you could let us know by opening an [issue](https://github.com/qua-platform/py-qua-tools/issues) on the [GitHub repository](https://github.com/qua-platform/py-qua-tools).
```

### Comparing `qualang-tools-0.8.0/pyproject.toml` & `qualang-tools-0.9.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qualang-tools"
-version = "v0.8.0"
+version = "v0.9.0"
 description = "The qualang_tools package includes various tools related to QUA programs in Python"
 license = "BSD-3-Clause"
 authors = [
       "QM <qua-libs@quantum-machines.co>",
 ]
 packages = [
     { include = "qualang_tools" }
```

### Comparing `qualang-tools-0.8.0/qualang_tools/addons/InteractivePlotLib.py` & `qualang-tools-0.9.0/qualang_tools/addons/InteractivePlotLib.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/addons/InteractivePlotLib_demonstration.png` & `qualang-tools-0.9.0/qualang_tools/addons/InteractivePlotLib_demonstration.png`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/addons/README.md` & `qualang-tools-0.9.0/qualang_tools/addons/README.md`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/bakery/README.md` & `qualang-tools-0.9.0/qualang_tools/bakery/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     - “symmetric_r' pads 0s symmetrically before and after the baked samples , putting one more 0 after it in case the baked waveform's length is odd
     - "none" puts a hard constraint by raising an error if any padding is required to upload the waveform to the configuration. It is useful when one wants to run another statement in QUA after the baked waveform without any gaps (which could be up to 3 ns).
 - override: boolean indicating if the baked waveform shall bear the flag "is_overridable" in the config (see example below with add_compiled, default value set to False)
 - baking_index: integer specifying the reference number of a previously defined baking object in order to impose a length constraint on the baked waveform (useful for ensuring compatibility with override feature of the add_compiled feature)
 
 The simplest declaration is done before the QUA program as follows: 
 
-```
+```python
 with baking(config, padding_method = "symmetric_r") as b:
   b.align("qe1", "qe2", "qe3")
   b.frame_rotation(0.78, "qe2")
   b.ramp(amp=0.3, duration=9, qe="qe1")
 ```
 
 When executed, the content manager edits the input configuration file and adds:
@@ -52,15 +52,15 @@
 3. Use a baking ``play()`` statement, specifying the operation name (which should correspond to the name introduced in the ```add_op``` method), and the quantum element to play the operation on. Note that it is also possible to play pre-existing pulses in the configuration.
 
 All those commands concatenated altogether eventually build one single “big” waveform per quantum element involved in the baking that contains all the instructions specified in the baking environment. The exiting procedure of the baking ensures that the appropriate padding is done to ensure that the OPX will be able to play this arbitrary waveform.
 
 Here is a basic code example that simply plays two pulses of short lengths: 
 
 
-```
+```python
 with baking(config, padding_method = "symmetric_r") as b:
 
 # Create arbitrary waveforms 
 
   singleInput_sample = [0.4, 0.3, 0.2, 0.3, 0.3]
   mixInput_sample_I = [0.2, 0.3, 0.4]
   mixInput_sample_Q = [0.1, 0.2, 0.4]
@@ -98,40 +98,40 @@
 
        
 # **How to play in QUA my baked waveforms?**
 
 The baking object has a method called run, which takes no inputs and simply does appropriate alignment between quantum elements involved in the baking and play simultaneously (using this time a QUA play statement) the previously baked waveforms.
 Therefore, all that is left is to **call the run method associated to the baking object within the actual QUA program**.
 
-```
+```python
 with baking(config, "left"):
   #Create your baked waveform, see snippet above
   
 #Open QUA program: 
 with program() as QUA_prog:
   b.run()
 ```
 
 As in QUA, you can still modulate in real time (using QUA variables) properties of the pulse like its amplitude, or to truncate it.
 You can indeed pass into a set of two lists, parameters for truncating pulses and for amplitude modulation. The syntax goes as follows:
-```
+```python
 with program() as QUA_prog:
     truncate = declare(int, value = 18)
     amp = declare(fixed, value = 0.4)
     b.run(amp_array = [(qe1, amp), (qe2, 0.5)], truncate_array = [(qe1, truncate), (qe3, 74)]) 
 ```
 Note that you do not have to provide tuples for every quantum element. The parameters you can pass can either Python or QUA variables. Beware though, you should make sure that the elements
 indicated in the parameter arrays are actually used within the baking context manager.
 # **Additional features of the baking environment**
 
 The baking aims to be as versatile as possible in the way of editing samples. The idea is therefore to generate desired samples up to the precision of the nanosecond, without having to worry about its format and its insertion in the configuration file. It is even possible to generate a waveform based on two previous samples (like a pulse superposition) by using two commands introduced in the baking: ``play_at()`` and ``negative_wait()``.
 
 Let’s take a look at the code below to understand what these two features do: 
 
-```
+```python
 with baking(config=config, padding_method="symmetric_r") as b:
     const_Op = [0.3, 0.3, 0.3, 0.3, 0.3]
     const_Op2 = [0.2, 0.2, 0.2, 0.3, 0.3]
     b.add_Op("Op1", "qe1", [const_Op, const_Op2]) # qe1 is a mixInputs element
     Op3 = [0.1, 0.1, 0.1]
     Op4 = [0.1, 0.1, 0.1]
     b.add_Op("Op2", "qe1", [Op3, Op4])
@@ -148,15 +148,15 @@
 At the baking exit, the config will have an updated samples 
 adapted for QUA compilation, according to the padding_method chosen, in this case:
 I: [0, 0, 0, 0, 0, 0.3, 0.3, 0.4, 0.4, 0.4, 0, 0, 0, 0, 0, 0], 
 Q: [0, 0, 0, 0, 0, 0.2, 0.2, 0.3, 0.4, 0.4, 0, 0, 0, 0, 0, 0]
 ```
 If the time index t is positive, the samples will be added precisely at the index indicated in the existing samples.
 Contrariwise, if the provided index t is negative, we call here automatically the function ``negative_wait()``, which adds the samples at the provided index starting to count from the end of the existing samples: 
-```
+```python
 with baking(config=config, padding_method="symmetric_r") as b:
     const_Op = [0.3, 0.3, 0.3, 0.3, 0.3]
     const_Op2 = [0.2, 0.2, 0.2, 0.3, 0.3]
     b.add_op("Op1", "qe2", [const_Op, const_Op2])  # qe1 is a mixInputs element
     Op3 = [0.1, 0.1, 0.1, 0.1]
     Op4 = [0.1, 0.1, 0.1, 0.1]
     b.add_op("Op2", "qe2", [Op3, Op4])
@@ -170,15 +170,15 @@
 At the baking exit, the config will have updated samples 
 adapted for QUA compilation, according to the padding_method chosen, in this case: """
 I: [0, 0, 0, 0, 0, 0.3, 0.3, 0.3, 0.4, 0.4, 0.1, 0.1, 0, 0, 0, 0], 
 Q:  [0, 0, 0, 0, 0, 0.2, 0.2, 0.2, 0.4, 0.4, 0.1, 0.1, 0, 0, 0, 0]
 ```
 The ``play_at()`` command can also be used as a single play statement involving a wait time and a play statement. In fact, if the time index indicated in the function is actually out of the range of the existing samples, a wait command is automatically added until reaching this time index (recall that the index corresponds to the time in ns) and starts inserting the operation indicated at this time. See the example below: 
 
-```
+```python
 with baking(config=config, padding_method="symmetric_r") as b:
     const_Op = [0.3, 0.3, 0.3, 0.3, 0.3]
     const_Op2 = [0.2, 0.2, 0.2, 0.3, 0.4]
     b.add_op("Op1", "qe1", [const_Op, const_Op2]) #qe1 is a mixInputs element
     Op3 = [0.1, 0.1, 0.1]
     Op4 = [0.2, 0.2, 0.2]
     b.add_Op("Op2", "qe1", [Op3, Op4])
@@ -212,27 +212,27 @@
 # The negative wait
 
 Negative wait is at the moment, just an equivalent way of writing the ``play_at()`` statement.
 
 The idea is to move backwards the time index at which the following play statement should start. For example, wait[-3] means that the following waveform will be added on top of the existing sequence on the 3 last samples and will append the rest like a usual play statement.
 
 We have the equivalence between:
-```
+```python
 b.wait(-3)
 b.play('my_pulse',qe)
 ```
 and 
-```
+```python
 b.play_at('my_pulse', qe, t=-3)
 ```
 
 # Editing the sampling rate with the baking
 
 The baking tool can also be used to tune up the sampling rate of your baked waveform by declaring the baking with the following argument:
-```
+```python
 my_sampling_rate = 3e9  # Expressed in number of samples per second
 with baking(config, ..., sampling_rate = my_sampling_rate) as b:
     ...
 ```
 Note that when adding new operations using the add_op() function, the waveforms have to be specified in the given sampling rate.
 We distinguish two cases:
 1. The provided sampling rate is lower than 1 Gs/sec (=1e9 samples/sec): in this scenario, the config is updated with
@@ -252,15 +252,15 @@
 
 The baking tool can also be used as a simple waveform generator, without having to necessarily update the configuration 
 file with associated new operations and pulses. A good use case is the precompile feature, and to override waveforms
 in order to save waveform memory (see example below).
 To do so, one can use the baking tool to generate the waveform, store the waveform in a Python variable using the method
 ```b.get_waveform_dict() ```, followed by a deletion of the operation in the input configuration using ```b.delete_op(qe)```:
 
-```
+```python
 with baking(config, padding_method = "right") as b :
     # Generate the desired set of baked waveforms
      # (one per involved quantum element)
     
 waveforms_dict = b.get_waveforms_dict()
 b.delete_op() # Deletes all operations created by the baking object in the config
 ```
```

### Comparing `qualang-tools-0.8.0/qualang_tools/bakery/bakery.py` & `qualang-tools-0.9.0/qualang_tools/bakery/bakery.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/bakery/randomized_benchmark.py` & `qualang-tools-0.9.0/qualang_tools/bakery/randomized_benchmark.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/bakery/randomized_benchmark_c1.py` & `qualang-tools-0.9.0/qualang_tools/bakery/randomized_benchmark_c1.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/bakery/xeb.py` & `qualang-tools-0.9.0/qualang_tools/bakery/xeb.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/config/README.md` & `qualang-tools-0.9.0/qualang_tools/config/README.md`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/config/README_config_GUI.md` & `qualang-tools-0.9.0/qualang_tools/config/README_config_GUI.md`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/config/README_config_builder.md` & `qualang-tools-0.9.0/qualang_tools/config/README_config_builder.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,86 +9,86 @@
 
 We provide classes (essentially wrappers to the underlying dictionary) for all fields that appear in the configuration and methods that help you to manipulate them.
 
  <ins> **Controller** </ins>
 
  A Quantum Orchestration Platform controller class. It can be initialized simply by providing the controller name and type (the default is `opx1`).
 
- ```
+ ```python
  cont = Controller("con1")
  ```
  
  All digital & analog ports that you use in any quantum element can be opened through the methods: `analog_output`, `analog_input`, `digital_input`, `digital_output`.
 
  For example, to open (if it is not already open) and get an instance of analog output with port id 5 and offset 0.2, you can do,
 
-```
+```python
 port = cont.analog_output(5, 0.2)
 ```
 
 The additional attributes of ports can be directly accessed or set from the instance of the port. For the AnalogOutputPort that we just opened we can configure the additional attributes as shown below:
-```
+```python
  port.delay = 32
  port.filter = AnalogOutputFilter([1.0, 1.5], [1.4, 2.5])
 ```
 
 <ins> **Waveforms** </ins>
 
 There are three types of waveforms `ConstantWaveform`, `ArbitraryWaveform` and `DigitalWaveform`. These objects can be created by specifying the names and the sample(s) as follows:
 
-```
+```python
 cont_wf = ConstantWaveform("wf1", 0.2)
 arb_wf = ArbitraryWaveform("wf2", [0.2, 0.1, 0.0])
 digital_wf = DigitalWaveform("wf3", [(1, 16)])
 ```
 
 Each waveform object once created can be shared among several different pulses.
  
 <ins> **Pulses** </ins>
 
 There are two types of pulses `ControlPulse` and `MeasurePulse`. These can be initialized by specifying the name, list of waveforms and their durations.
 
-```
+```python
 pulse1 = ControlPulse("p1", [ConstantWaveform("wf1",0.5), ConstantWaveform("wf1",0.5)], 16)
 pulse2 = MeasurePulse("p2", [ConstantWaveform("wf1",0.5), ConstantWaveform("wf1",0.5)], 16)
 ```
 
 In addition for `MeasurePulse`s we can add digital markers and weights (see below) with the `add` method.
 
-```
+```python
 pulse2.add(digital_wf)
 ```
 
 <ins> **IntegrationWeights**  </ins>
 
 There are two types of integration weights `ConstantIntegrationWeights` and `ArbitraryIntegrationWeights`. `ConstantIntegrationWeights` are initialized by specifying the name, the cosine and sine values and the duration.
 
-```
+```python
 const_iw = ConstantIntegrationWeights("iw1", 1.0, 0.0, 16)
 ```
 Similarly, `ArbitraryIntegrationWeights` are initialized as follows by providing the list of cosine and sine values.
-```
+```python
 arb_iw = ConstantIntegrationWeights("iw2", [1.0, 0.2], [0.0, -0.2], 2)
 ```
 
 In order to add integration weights to a `MeasurePulse` you need to give a name that can be then used in a QUA measure statement. We introduced `Weights` (nothing but a named `IntegrationWeights`) to facilitate this. Consider the following two ways of adding `Weights`:
 
-```
+```python
 pulse2.add(Weight(const_iw))
 ```
 or 
-```
+```python
 pulse2.add(Weight(const_iw, "my_iw"))
 ```
 in the first case, you will use `iw1` in the `measure` statement, whereas in the second case, you will use `my_iw` to refer to the integration weights.
 
 <ins> **Mixers** </ins>
 
 A microwave mixer is initialized with the name, lo_frequency, intermediate_frequency and a correction matrix,
-```
+```python
 mixer = Mixers("mx1", 5e9, 4e6, Matrix2x2([[1, 0],[0, 1]]))
 ```
 Mixers can be added to an `Element` or `MeasureElement` (see below) with the `add` method.
 
 <ins> **Elements and collection of elements...** </ins>
 
 An element describes a control entity which is connected to some ports of the controller. It can be initialized by specifying the name, list of Analog/Digital Input/Output ports and optionally `intermediate_frequency` or `lo_frequency` (if inputs are mixed by the element).
@@ -106,19 +106,19 @@
 For more details, check the examples in `qua-libs/examples/config-builder/`.
 
 ## Parameters
 --------------
 
 There are several usecases where it is useful to write a QUA configuration without assigning a specific value to component attributes for e.g. fields based on some calibration data that can change everyday. `ConfigVar` class maintains a dictionary of parameters, it helps you to write a generic configuration with parametric values. For example, in the following code
 
-```
+```python
 p = ConfigVar()
 wf = ConstantWaveform("wf1", p.parameter("sample"))
 ```
 
 the value of the constant waveform is initialised with a parameter called `sample`, the waveform object can be further used in other components added to config builder. Here the `parameter` method returns a lambda function, you may access the value of the parameter (if it is already set, otherwise you get an `AssertionError`) by calling this lambda function.
 
-```
+```python
 p.set(sample=2.0)
-print(p.parameter("sample)())
+print(p.parameter("sample"))
 ```
 Finally, to generate an instance of the configuration it is enough to set all parameters used in the config builder before calling the `build` method.
```

### Comparing `qualang-tools-0.8.0/qualang_tools/config/README_integration_weights_tools.md` & `qualang-tools-0.9.0/qualang_tools/config/README_integration_weights_tools.md`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/config/README_waveform_tools.md` & `qualang-tools-0.9.0/qualang_tools/config/README_waveform_tools.md`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/config/__init__.py` & `qualang-tools-0.9.0/qualang_tools/config/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,10 +42,11 @@
     "Waveform",
     "Pulse",
     "Operation",
     "IntegrationWeights",
     "Weights",
     "DigitalSample",
     "Matrix2x2",
+    "MixerData",
     "AnalogOutputFilter",
     "ConfigBuilder",
 ]
```

### Comparing `qualang-tools-0.8.0/qualang_tools/config/builder.py` & `qualang-tools-0.9.0/qualang_tools/config/builder.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,59 @@
-from typing import Union, Dict
+import copy
+from typing import Union, List
 
-from qualang_tools.config.configuration import *
+from qualang_tools.config.components import (
+    Controller,
+    ElementCollection,
+    Element,
+    Mixer,
+    Oscillator,
+    MeasureElement,
+    MeasurePulse,
+)
+from qualang_tools.config.configuration import QMConfiguration
 from qualang_tools.config.exceptions import ConfigurationError
-from qualang_tools.config.components import *
-from qualang_tools.config.parameters import isparametric
+from qualang_tools.config.parameters import _is_parametric
+from qualang_tools.config.primitive_components import (
+    AnalogOutputPort,
+    AnalogInputPort,
+    DigitalOutputPort,
+    Waveform,
+    Pulse,
+    IntegrationWeights,
+    DigitalInputPort,
+    Port,
+)
 
 
 class ConfigBuilder:
     def __init__(self) -> None:
         """A class used to build the configuration of an experiment with QUA"""
         self.objects = []
         self.configuration = QMConfiguration([])
         self.controllers = []
-        self.components = []
+        self.components: List[ElementCollection] = []
 
     def add(self, obj):
         """Adds an entity to the configuraiton.
 
         :param obj: Any entity type supported by the configuration system, e.g. Element, ArbitraryWaveform or Transmon
         :type obj:
         """
         if isinstance(obj, list):
             for _obj in obj:
-                self.objects.append(_obj)
+                if isinstance(_obj, ElementCollection):
+                    self.components.append(_obj)
+                else:
+                    self.objects.append(_obj)
         else:
-            self.objects.append(obj)
+            if isinstance(obj, ElementCollection):
+                self.components.append(obj)
+            else:
+                self.objects.append(obj)
         return self
 
     @property
     def ports(self):
         ports = []
         for cont in self.controllers:
             ports += cont.ports
@@ -45,69 +70,72 @@
                         "feedback": port.filter.feedback,
                         "feedforward": port.filter.feedforward,
                     }
                 if port.channel_weights is not None:
                     cont.dict["analog_outputs"][port.info[1]][
                         "channel_weights"
                     ] = port.channel_weights
+                cont.dict["analog_outputs"][port.info[1]]["offset"] = port.offset
             elif isinstance(port, AnalogInputPort):
                 if port.gain_db is not None:
                     cont.dict["analog_inputs"][port.info[1]]["gain_db"] = port.gain_db
+                cont.dict["analog_inputs"][port.info[1]]["offset"] = port.offset
             elif isinstance(port, DigitalOutputPort):
-                pass
+                cont.dict["digital_outputs"][port.info[1]]["offset"] = port.offset
             elif isinstance(port, DigitalInputPort):
                 if port.polarity is not None:
                     cont.dict["digital_inputs"][port.info[1]][
                         "polarity"
                     ] = port.polarity
                 if port.threshold is not None:
                     cont.dict["digital_inputs"][port.info[1]][
                         "threshold"
                     ] = port.threshold
                 if port.window is not None:
                     cont.dict["digital_inputs"][port.info[1]]["window"] = port.window
 
         self.configuration.config["controllers"][cont.name] = cont.dict
 
-    def _add_component(self, comp: ElementCollection):
-        self.components.append(comp)
-        for elm in comp.elements:
-            self.configuration.add_element(elm)
-
-    def build(self, config: Dict = {}):
+    def build(self, config=None):
         """Generates the QUA configuration represented by the current state of the builder object
 
         :param config: An initial QUA config, defaults to {}
         :type config: Dict, optional
         :return: QUA configuration
         :rtype: Dict
         """
+        if config is None:
+            config = {}
         if config == {}:
             self.configuration.reset()
             self.controllers = []
-            self.components = []
         else:
             self.configuration.config = copy.deepcopy(config)
-        for obj in self.objects:
-            if isparametric(obj):
+        objects = self.objects
+        for c in self.components:
+            objects = objects + c.get_elements()
+
+        for obj in objects:
+            if _is_parametric(obj):
                 raise ConfigurationError("set the parameters of {0}".format(obj.name))
             if isinstance(obj, Controller):
                 self._add_controller(obj)
+            # elif isinstance(obj, ElementCollection):
+            #    for _obj in obj.get_elements():
+            #        self._objects.append(_obj)
             elif isinstance(obj, Waveform):
                 self.configuration.add_waveform(obj)
             elif isinstance(obj, Pulse):
                 self.configuration.add_pulse(obj)
-            elif isinstance(obj, ElementCollection):
-                self._add_component(obj)
             elif isinstance(obj, Element):
                 self.configuration.add_element(obj)
             elif isinstance(obj, IntegrationWeights):
                 self.configuration.add_integration_weights(obj)
             elif isinstance(obj, Mixer):
-                self.configuraiton.add_mixer(obj)
+                self.configuration.add_mixer(obj)
             elif isinstance(obj, Oscillator):
                 self.configuration.add_oscillator(obj)
             else:
                 raise NotImplementedError(
                     "Can not add objects of type {0}".format(type(obj))
                 )
         return self.configuration.config
@@ -162,60 +190,42 @@
             raise NotImplementedError(
                 "can not find objects of type {}".format(type(elm))
             )
 
     def _find_users_of_port(self, port: Port):
         objects = []
         for obj in self.objects:
-            if (
-                isinstance(obj, Element)
-                or isinstance(obj, ElementCollection)
-                or isinstance(obj, MeasureElement)
-            ):
+            if isinstance(obj, Element) or isinstance(obj, MeasureElement):
                 if port in obj.ports:
                     objects.append(obj)
         return set(objects)
 
     def _find_users_of_controller(self, cont: Controller):
         objects = []
         for obj in self.objects:
             if isinstance(obj, Element) or isinstance(obj, MeasureElement):
                 for port in obj.ports:
                     if port in cont.ports:
                         objects.append(obj)
                         break
-            elif isinstance(obj, ElementCollection):
-                for _obj in obj.elements:
-                    for port in _obj.ports:
-                        if port in cont.ports:
-                            objects.append(obj)
-                        break
         return set(objects)
 
     def _find_users_of_waveform(self, wf: Waveform):
         objects = []
         for obj in self.objects:
-            if (
-                isinstance(obj, Element)
-                or isinstance(obj, MeasureElement)
-                or isinstance(obj, ElementCollection)
-            ):
+            if isinstance(obj, Element) or isinstance(obj, MeasureElement):
                 for name in obj.waveform_names:
                     if name == wf.name:
                         objects.append(obj)
         return set(objects)
 
     def _find_users_of_pulse(self, elm: Pulse):
         objects = []
         for obj in self.objects:
-            if (
-                isinstance(obj, Element)
-                or isinstance(obj, MeasureElement)
-                or isinstance(obj, ElementCollection)
-            ):
+            if isinstance(obj, Element) or isinstance(obj, MeasureElement):
                 for name in obj.pulse_names:
                     if name == elm.name:
                         objects.append(obj)
         return set(objects)
 
     def _find_users_of_integration_weights(self, elm: IntegrationWeights):
         objects = []
@@ -232,7 +242,16 @@
             if isinstance(obj, Oscillator):
                 if obj.mixer == elm.name:
                     objects.append(obj)
             elif isinstance(obj, Element):
                 if obj.mixer.name == elm.name:
                     objects.append(obj)
         return set(objects)
+
+    def component(self, name: str):
+        """Returns a config builder object with the given name
+        :param name: name of the object
+        :type name: str
+        """
+        for c in self.objects + self.components:
+            if c.name == name:
+                return c
```

### Comparing `qualang-tools-0.8.0/qualang_tools/config/components.py` & `qualang-tools-0.9.0/qualang_tools/config/components.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,65 +1,52 @@
-from typing import Union, List, Tuple
+import abc
+from typing import Union, List, Tuple, Optional, Dict
 
-from qualang_tools.config.primitive_components import *
 from qualang_tools.config.exceptions import ConfigurationError
+from qualang_tools.config.primitive_components import (
+    ConfigBuilderElement,
+    AnalogInputPort,
+    DigitalOutputPort,
+    Waveform,
+    DigitalSample,
+    Pulse,
+    Weights,
+    AnalogOutputPort,
+    DigitalInputPort,
+    Operation,
+    IntegrationWeights,
+    MixerData,
+)
 
 
-class Controller:
+class Controller(ConfigBuilderElement):
     def __init__(
         self,
         name: str,
-        n_analog_outputs: int = 0,
-        n_analog_inputs: int = 0,
-        n_digital_outputs: int = 0,
-        n_digital_inputs: int = 0,
         controller_type: str = "opx1",
     ):
         """A QOP controller
 
         :param name: Name for this controller
         :type name: str
-        :param n_analog_outputs: Number of analog outputs defined at initialization, defaults to 0
-        :type n_analog_outputs: int, optional
-        :param n_analog_inputs: Number of analog inputs defined at initialization, defaults to 0
-        :type n_analog_inputs: int, optional
-        :param n_digital_outputs: Number of digital outputs defined at initialization, defaults to 0
-        :type n_digital_outputs: int, optional
-        :param n_digital_inputs: Number of digital inputs defined at initialization, defaults to 0
-        :type n_digital_inputs: int, optional
         :param controller_type: defaults to "opx1"
         :type controller_type: str, optional
         """
-        self.name = name
+        super(Controller, self).__init__(name)
         self.dict = dict()
         self.dict["type"] = controller_type
-        self.dict["analog_outputs"] = {
-            i: {"offset": 0} for i in range(1, n_analog_outputs + 1)
-        }
-        self.dict["analog_inputs"] = {
-            i: {"offset": 0} for i in range(1, n_analog_inputs + 1)
-        }
-        self.dict["digital_outputs"] = {
-            i: {"offset": 0} for i in range(1, n_digital_outputs + 1)
-        }
-        self.dict["digital_inputs"] = {
-            i: {"offset": 0} for i in range(1, n_digital_inputs + 1)
-        }
-        self.analog_input_ports = [
-            AnalogInputPort(name, i) for i in range(1, n_analog_inputs + 1)
-        ]
-        self.analog_output_ports = [
-            AnalogOutputPort(name, i) for i in range(1, n_analog_outputs + 1)
-        ]
-        self.digital_output_ports = [
-            DigitalOutputPort(name, i) for i in range(1, n_digital_outputs + 1)
-        ]
-        self.digital_input_ports = [
-            DigitalInputPort(name, i) for i in range(1, n_digital_inputs + 1)
-        ]
+        self.controller_type = controller_type
+        self.dict["analog_outputs"] = {}
+        self.analog_output_ports = []
+        self.dict["analog_inputs"] = {}
+        self.analog_input_ports = []
+        self.dict["digital_outputs"] = {}
+        self.digital_output_ports = []
+        self.dict["digital_inputs"] = {}
+        self.digital_input_ports = []
 
     def analog_output(self, port: int, offset: float = 0):
         """Returns an instance of AnalogOutputPort associated  with a specific port number and offset if already in the configuration.
         otherwise, opens a new instance with the given port number.
 
         :param port: physical output port numebr
         :type port: int
@@ -68,15 +55,15 @@
         :return: An instance of the analog port
         :rtype: AnalogOutputPort
         """
         for (i, p) in enumerate(self.analog_output_ports):
             if port == p.info[1]:
                 p.offset = offset
                 return p
-        self.use_analog_output_port(port, offset)
+        self._use_analog_output_port(port, offset)
         return self.analog_output_ports[-1]
 
     def analog_input(self, port: int, offset: float = 0):
         """Returns an instance of AnalogInputPort with a specific port number and offset if already in the configuration.
         otherwise, opens a new instance with the given port number and offset.
 
         :param port: physical input port numebr
@@ -86,15 +73,15 @@
         :return: An instance of the input port
         :rtype: AnalogInputPort
         """
         for (i, p) in enumerate(self.analog_input_ports):
             if port == p.info[1]:
                 p.offset = offset
                 return p
-        self.use_analog_input_port(port, offset)
+        self._use_analog_input_port(port, offset)
         return self.analog_input_ports[-1]
 
     def digital_output(self, port: int, offset: float = 0):
         """Returns an instance of DigitalOutputPort with a specific port number and offset if already in the configuration.
         otherwise, opens a new instance with the given port number and offset.
 
         :param port: port number in the range 1-10
@@ -104,87 +91,90 @@
         :return:
         :rtype: DigitalOutputPort
         """
         for (i, p) in enumerate(self.digital_output_ports):
             if port == p.info[1]:
                 p.offset = offset
                 return p
-        self.use_digital_output_port(port, offset)
+        self._use_digital_output_port(port, offset)
         return self.digital_output_ports[-1]
 
-    def digital_input(self, port: int, offset: float = 0):
+    def digital_input(self, port: int):
+        """Returns an instance of DigitalInputPort with a specific port number if already in the configuration.
+        otherwise, opens a new instance with the given port number.
+
+        :param port: port number in the range 1-10
+        :type port: int
+        :return:
+        :rtype: DigitalOutputPort
+        """
 
-        for (i, p) in enumerate(self.digital_ports):
+        for (i, p) in enumerate(self.digital_input_ports):
             if port == p.info[1]:
-                p.offset = offset
                 return p
-        self.use_digital_input_port(port, offset)
+        self._use_digital_input_port(port)
         return self.digital_input_ports[-1]
 
     def __contains__(self, port) -> bool:
-        for p in self.input_ports + self.output_ports + self.digital_ports:
+        for p in self.ports:
             if port == p:
                 return True
         return False
 
-    def use_analog_input_port(self, port_num: int, offset: float = 0.0):
+    def _use_analog_input_port(self, port_num: int, offset: float = 0.0):
         """Adds an instance of  AnalogInputPort to configuration if it is not used
 
         :param port_num: port number
         :type port_num: int
         :param offset: voltage offset for this port, defaults to 0.0
         :type offset: float, optional
         """
         if port_num not in self.dict["analog_inputs"]:
             self.dict["analog_inputs"][port_num] = {"offset": offset}
             self.analog_input_ports += [
                 AnalogInputPort(self.name, port_num, offset=offset)
             ]
 
-    def use_analog_output_port(self, port_num: int, offset: float = 0.0):
+    def _use_analog_output_port(self, port_num: int, offset: float = 0.0):
         """Adds an instance of  AnalogOutputPort to configuration if it is not used
 
         :param port_num: port number
         :type port_num: int
         :param offset: voltage offset for this port, defaults to 0.0
         :type offset: float, optional
         """
         if port_num not in self.dict["analog_outputs"]:
             self.dict["analog_outputs"][port_num] = {"offset": offset}
             self.analog_output_ports += [
                 AnalogOutputPort(self.name, port_num, offset=offset)
             ]
 
-    def use_digital_output_port(self, port_num: int, offset: float = 0.0):
+    def _use_digital_output_port(self, port_num: int, offset: float = 0.0):
         """Adds an instance of  DigitalOutputPort to configuration if it is not used
 
         :param port_num: port number
         :type port_num: int
         :param offset: defaults to 0.0
         :type offset: float, optional
         """
         if port_num not in self.dict["digital_outputs"]:
             self.dict["digital_outputs"][port_num] = {"offset": offset}
             self.digital_output_ports += [
                 DigitalOutputPort(self.name, port_num, offset=offset)
             ]
 
-    def use_digital_input_port(self, port_num: int, offset: float = 0.0):
+    def _use_digital_input_port(self, port_num: int):
         """Adds an instance of  DigitalInputPort to configuration if it is not used
 
         :param port_num: port number
         :type port_num: int
-        :param offset: defaults to 0.0
-        :type offset: float, optional
         """
         if port_num not in self.dict["digital_inputs"]:
-            self.dict["digital_inputs"][port_num] = {"offset": offset}
-            self.digital_input_ports += [
-                DigitalInputPort(self.name, port_num, offset=offset)
-            ]
+            self.dict["digital_inputs"][port_num] = {}
+            self.digital_input_ports += [DigitalInputPort(self.name, port_num)]
 
     @property
     def ports(self):
         """Returns the set of all used ports in this configuration
 
         :return:
         :rtype: Set
@@ -204,45 +194,62 @@
         :param name: name of the played WF
         :type name: str
         :param samples: list of samples to be played (in the range -.5 to .5), specified at 1 sample per nanosecond
         :type samples: List[float]
         """
         super().__init__(name, {"type": "arbitrary", "samples": samples})
 
+    @property
+    def samples(self):
+        return self.dict["samples"]
+
+    @samples.setter
+    def samples(self, samples: List[float]):
+        self.dict["samples"] = samples
+
 
 class ConstantWaveform(Waveform):
     def __init__(self, name: str, sample: float):
         """A constant amplitude WF
 
         :param name: name of the WF
         :type name: str
         :param sample: Amplitude of the WF in the range -.5 to .5
         :type sample: float
         """
         super().__init__(name, {"type": "constant", "sample": sample})
 
+    @property
+    def sample(self):
+        return self.dict["sample"]
+
+    @sample.setter
+    def sample(self, samples: List[float]):
+        self.dict["sample"] = samples
+
 
-class DigitalWaveform:
+class DigitalWaveform(Waveform):
     def __init__(self, name: str, samples: List[DigitalSample]):
-        """A ditial waveform played from a digital output
+        """A digital waveform played from a digital output
 
         :param name: The name of the digital waveform, defaults to "ON"
         :type name: str
         :param samples: The digital waveforms, specified in the format [(1/0, dur),...] where dur is in nanoseconds.  defaults to [(1, 0)]
         :type samples: List[DigitalSample]
         """
-        self.name = name
-        self.dict = dict()
+
         if isinstance(samples[0], DigitalSample):
             self._samples = samples
         else:
             self._samples = [
                 DigitalSample(state, duration) for (state, duration) in samples
             ]
-        self.dict["samples"] = [(ds.state, ds.duration) for ds in self._samples]
+        dic = dict()
+        dic["samples"] = [(ds.state, ds.duration) for ds in self._samples]
+        super(DigitalWaveform, self).__init__(name, dic)
 
     @property
     def samples(self):
         return self._samples
 
     @samples.setter
     def samples(self, samples: Union[List[Tuple[int, int]], List[DigitalSample]]):
@@ -252,124 +259,113 @@
             self._samples = [
                 DigitalSample(state, duration) for (state, duration) in samples
             ]
         self.dict["samples"] = [(ds.state, ds.duration) for ds in self._samples]
 
 
 class MeasurePulse(Pulse):
-    def __init__(self, name: str, wfs: List[Waveform], length: int):
+    def __init__(self, name: str, wfs: List[Waveform], length: int, **kwargs):
         """A pulse which can be used by a QUA measure() command
 
         :param name: name for this pulse
         :type name: str
         :param wfs: waveforms to be played during measurement
         :type wfs: List[Waveform]
         :param length: duration of the measurment pulse
         :type length: int, optional
         """
-        super().__init__(name, wfs, "measure", length)
-        self.integration_weights = []
+
+        integration_weights: List[Weights] = kwargs.get("integration_weights", None)
+        digital_marker: Optional[DigitalWaveform] = kwargs.get("digital_marker", None)
+        super().__init__(name, wfs, "measure", length, digital_marker)
+        if integration_weights is None:
+            integration_weights = []
+        self.integration_weights = integration_weights
 
     def add(
         self,
         objs: Union[Weights, DigitalWaveform, List[Union[Weights, DigitalWaveform]]],
     ):
         if isinstance(objs, list):
             for obj in objs:
                 self._add(obj)
         else:
             self._add(objs)
         return self
 
-    def _add(self, w: Union[Weights, DigitalWaveform]):
+    def _add(self, w: Union[Weights, IntegrationWeights, DigitalWaveform]):
+        if isinstance(w, IntegrationWeights):
+            w = Weights(w)
+
         if isinstance(w, Weights):
-            if isinstance(w.weights, ConstantIntegrationWeights):
-                assert w.weights.dict["cosine"][0][1] == self.dict["length"]
-            else:
-                assert len(w.weights.dict["sine"]) == self.dict["length"] // 4
+            if callable(self.dict):
+                if isinstance(w.weights, ConstantIntegrationWeights):
+                    if w.weights.dict["cosine"][0][1] == self.dict["length"]:
+                        assert w.weights.dict["cosine"][0][1]() == self.dict["length"]()
+
+                else:
+                    assert len(w.weights.dict["sine"]) == self.dict["length"] // 4
             self.integration_weights.append(w)
         elif isinstance(w, DigitalWaveform):
             self.digital_marker = w
 
 
 class ControlPulse(Pulse):
-    def __init__(self, name: str, wfs: List[Waveform], length: int):
+    def __init__(self, name: str, wfs: List[Waveform], length: int, **kwargs):
         """A pulse which can be used by a QUA play() command
         :return:
         :rtype: ControlPulse
         """
-        super().__init__(name, wfs, "control", length)
+        digital_marker: Optional[DigitalWaveform] = kwargs.get("digital_marker", None)
+        super().__init__(name, wfs, "control", length, digital_marker)
 
     def add(self, w: DigitalWaveform):
         self.digital_marker = w
         return self
 
 
-class Mixer:
-    def __init__(
-        self,
-        name: str,
-        intermediate_frequency: int,
-        lo_frequency: int,
-        correction: Matrix2x2,
-    ):
+class Mixer(ConfigBuilderElement):
+    def __init__(self, name: str, data: Optional[List[MixerData]] = None):
         """A microwave mixer
 
         :param name: name for this mixer
         :type name: str
-        :param intermediate_frequency: intermediate_frequency in MHz
-        :type intermediate_frequency: int
-        :param lo_frequency:  local oscillator frequency in MHz
-        :type lo_frequency: int
-        :param correction: correction matrix for this mixer
-        :type correction: Matrix2x2
-        """
-        self.name = name
-        self._correction = correction
-        self.dict = dict()
-        self.dict["intermediate_frequency"] = intermediate_frequency
-        self.dict["lo_frequency"] = lo_frequency
-        self.dict["correction"] = list(correction.data[0] + correction.data[1])
+        :param data: a list of mixer data with correction matrices for every pair of IF and LO
+        :type data: List[MixerData]
 
-    @property
-    def intermediate_frequency(self):
-        return self.dict["intermediate_frequency"]
-
-    @intermediate_frequency.setter
-    def intermediate_frequency(self, if_freq: int):
-        self.dict["intermediate_frequency"] = if_freq
-
-    @property
-    def lo_frequency(self):
-        return self.dict["lo_frequency"]
-
-    @lo_frequency.setter
-    def lo_frequency(self, lo_freq: int):
-        self.dict["lo_frequency"] = lo_freq
-
-    @property
-    def correction(self):
-        return self._correction
-
-    @correction.setter
-    def correction(self, correction: Matrix2x2):
-        self._correction = correction
-        self.dict["correction"] = list(correction.data[0] + correction.data[1])
+        """
+        super(Mixer, self).__init__(name)
+        if data is None:
+            data = []
+        self.dict = []
+        for e in data:
+            self.add(e)
+
+    def add(self, data: MixerData):
+        self.dict.append(
+            {
+                "intermediate_frequency": data.intermediate_frequency,
+                "lo_frequency": data.lo_frequency,
+                "correction": list(data.correction.data[0] + data.correction.data[1]),
+            }
+        )
+        return self
 
 
-class Element:
+class Element(ConfigBuilderElement):
     def __init__(
         self,
         name: str,
-        analog_input_ports: List[AnalogOutputPort] = [],
-        analog_output_ports: List[AnalogInputPort] = [],
-        digital_input_ports: List[DigitalOutputPort] = [],
-        digital_output_ports: List[DigitalInputPort] = [],
-        intermediate_frequency: int = None,
-        lo_frequency: int = None,
+        analog_input_ports: Optional[List[AnalogOutputPort]] = None,
+        analog_output_ports: Optional[List[AnalogInputPort]] = None,
+        digital_input_ports: Optional[List[DigitalOutputPort]] = None,
+        digital_output_ports: Optional[List[DigitalInputPort]] = None,
+        intermediate_frequency: Optional[int] = None,
+        lo_frequency: Optional[int] = None,
+        **kwargs
     ):
         """A quantum element in a configuration
 
         :param name: element name
         :type name: int
         :param analog_input_ports: AnalogOutputPort(s) associated with this element, defaults to []
         :type analog_input_ports: List[AnalogOutputPort], optional
@@ -378,70 +374,92 @@
         :param digital_input_ports: DigitalOutputPort(s) associated with this element, defaults to []
         :type digital_input_ports: List[DigitalOutputPort], optional
         :param intermediate_frequency: intermediate frequency associated wit this element, defaults to None
         :type intermediate_frequency: int, optional
         :param lo_frequency: LO frequency associated wit this element, defaults to None
         :type lo_frequency: int, optional
         """
-        self.name = name
+        super(Element, self).__init__(name)
+
+        mixer: Optional[Mixer] = kwargs.get("mixer", None)
+        pulses: Optional[List[Pulse]] = kwargs.get("pulses", None)
+        operations: Optional[Dict[str, str]] = kwargs.get("digital_marker", None)
+
         self.dict = dict()
         assert len(analog_input_ports) <= 2
         self.type = "singleInput" if len(analog_input_ports) == 1 else "mixInputs"
         self.pulses = []
-        self.analog_input_ports = analog_input_ports
-        self.analog_output_ports = analog_output_ports
-        self.digital_output_ports = digital_output_ports
-        self.digital_input_ports = digital_input_ports
-        self.mixer = None
-        if len(analog_input_ports) > 0:
+        if pulses is not None:
+            self.pulses = pulses
+        self.analog_input_ports = (
+            [] if analog_input_ports is None else analog_input_ports
+        )
+        self.analog_output_ports = (
+            [] if analog_output_ports is None else analog_output_ports
+        )
+        self.digital_output_ports = (
+            [] if digital_output_ports is None else digital_output_ports
+        )
+        self.digital_input_ports = (
+            [] if digital_input_ports is None else digital_input_ports
+        )
+        self.mixer: Mixer = mixer
+
+        if len(self.analog_input_ports) > 0:
             if self.type == "singleInput":
-                port = analog_input_ports[0]
+                port = self.analog_input_ports[0]
                 self.dict["singleInput"] = dict()
                 self.dict["singleInput"]["port"] = port.info
             elif self.type == "mixInputs":
-                I = analog_input_ports[0]
-                Q = analog_input_ports[1]
+                I = self.analog_input_ports[0]
+                Q = self.analog_input_ports[1]
                 self.dict["mixInputs"] = dict()
                 self.dict["mixInputs"]["I"] = I.info
                 self.dict["mixInputs"]["Q"] = Q.info
                 self.dict["mixInputs"]["lo_frequency"] = lo_frequency
-        if len(analog_output_ports) > 0:
+        if len(self.analog_output_ports) > 0:
             self.dict["outputs"] = dict()
-            for i, port in enumerate(analog_output_ports):
+            for i, port in enumerate(self.analog_output_ports):
                 self.dict["outputs"]["out" + str(i + 1)] = port.info
         self.dict["operations"] = dict()
+        if operations is not None:
+            self.dict["operations"] = operations
         self.dict["intermediate_frequency"] = intermediate_frequency
         # self.dict["outputPulseParameters"] = dict()
-        if len(digital_input_ports) > 0:
+        if len(self.digital_input_ports) > 0:
             self.dict["digitalInputs"] = dict()
-            for i, port in enumerate(digital_input_ports):
+            for i, port in enumerate(self.digital_input_ports):
                 self.dict["digitalInputs"]["in" + str(i + 1)] = {
                     "port": port.info,
                     "delay": 0,
                     "buffer": 0,
                 }
 
-    def set_delay(self, port_id: int, val: int):
+    def set_digital_input_delay(self, port_id: int, val: int):
         if "in" + str(port_id) in self.dict["digitalInputs"].keys():
             self.dict["digitalInputs"]["in" + str(port_id)]["delay"] = val
         else:
             raise ConfigurationError("digital input port must be set first")
 
-    def set_buffer(self, port_id: int, val: int):
+    def set_digital_input_buffer(self, port_id: int, val: int):
         if "in" + str(port_id) in self.dict["digitalInputs"].keys():
             self.dict["digitalInputs"]["in" + str(port_id)]["buffer"] = val
         else:
             raise ConfigurationError("digital input port must be set first")
 
-    def _add_mixer(self, mix: Mixer):
+    def _set_mixer(self, mix: Mixer):
         assert "mixInputs" in self.dict.keys()
         self.dict["mixInputs"]["mixer"] = mix.name
         self.mixer = mix
 
     @property
+    def has_lo_frequency(self):
+        return "mixInputs" in self.dict.keys()
+
+    @property
     def lo_frequency(self):
         assert "mixInputs" in self.dict.keys()
         return self.dict["mixInputs"]["lo_frequency"]
 
     @lo_frequency.setter
     def lo_frequency(self, lo_frequency: int):
         assert "mixInputs" in self.dict.keys()
@@ -457,29 +475,36 @@
 
         :param omega_IF:
         :type omega_IF: int
         """
         assert self.type == "mixInputs"
         self.dict["intermediate_frequency"] = omega_IF
 
+    @property
+    def operations(self):
+        return self.dict["operations"]
+
     def _add_operation(self, op: Operation):
         self.dict["operations"][op.name] = op.pulse.name
         self.pulses.append(op.pulse)
 
-    def _add(self, obj: Union[Operation, Mixer]):
+    def _add(self, obj: Union[Operation, Mixer, ControlPulse, MeasurePulse]):
         """A method to add components to an element
 
         :param obj: The component to be added
         :type obj: [type]
         :raises ConfigurationError: [description]
         """
         if isinstance(obj, Operation):
             self._add_operation(obj)
         elif isinstance(obj, Mixer):
-            self._add_mixer(obj)
+            self._set_mixer(obj)
+        elif isinstance(obj, ControlPulse) or isinstance(obj, MeasurePulse):
+            self.dict["operations"][obj.name] = obj.name
+            self.pulses.append(obj)
         else:
             raise ConfigurationError("Adding unsupported object")
 
     def add(self, objs: Union[Operation, Mixer, List[Union[Operation, Mixer]]]):
         if isinstance(objs, list):
             for obj in objs:
                 self._add(obj)
@@ -508,53 +533,81 @@
             self.analog_input_ports
             + self.analog_output_ports
             + self.digital_output_ports
             + self.digital_input_ports
         )
 
     @property
+    def has_signal_threshold(self):
+        return (
+            "outputPulseParameters" in self.dict
+            and "signalThreshold" in self.dict["outputPulseParameters"].keys()
+        )
+
+    @property
     def signal_threshold(self):
         if "signalThreshold" in self.dict["outputPulseParameters"].keys():
             return self.dict["outputPulseParameters"]["signalThreshold"]
         else:
             raise ConfigurationError("set the signal threshold")
 
     @signal_threshold.setter
     def signal_threshold(self, val: int):
         if "outputPulseParameters" not in self.dict.keys():
             self.dict["outputPulseParameters"] = dict()
         self.dict["outputPulseParameters"]["signalThreshold"] = val
 
     @property
+    def has_signal_polarity(self):
+        return (
+            "outputPulseParameters" in self.dict
+            and "signalPolarity" in self.dict["outputPulseParameters"].keys()
+        )
+
+    @property
     def signal_polarity(self):
         if "signalPolarity" in self.dict["outputPulseParameters"].keys():
             return self.dict["outputPulseParameters"]["signalPolarity"]
         else:
             raise ConfigurationError("set the signal polarity")
 
     @signal_polarity.setter
     def signal_polarity(self, val: str):
         if "outputPulseParameters" not in self.dict.keys():
             self.dict["outputPulseParameters"] = dict()
         self.dict["outputPulseParameters"]["signalPolarity"] = val
 
     @property
+    def has_derivative_threshold(self):
+        return (
+            "outputPulseParameters" in self.dict
+            and "derivativeThreshold" in self.dict["outputPulseParameters"].keys()
+        )
+
+    @property
     def derivative_threshold(self):
         if "derivativeThreshold" in self.dict["outputPulseParameters"].keys():
             return self.dict["outputPulseParameters"]["derivativeThreshold"]
         else:
             raise ConfigurationError("set the derivative threshold")
 
     @derivative_threshold.setter
     def derivative_threshold(self, val: int):
         if "outputPulseParameters" not in self.dict.keys():
             self.dict["outputPulseParameters"] = dict()
         self.dict["outputPulseParameters"]["derivativeThreshold"] = val
 
     @property
+    def has_derivative_polarity(self):
+        return (
+            "outputPulseParameters" in self.dict
+            and "derivativePolarity" in self.dict["outputPulseParameters"].keys()
+        )
+
+    @property
     def derivative_polarity(self):
         if "derivativePolarity" in self.dict["outputPulseParameters"].keys():
             return self.dict["outputPulseParameters"]["derivativePolarity"]
         else:
             raise ConfigurationError("set the derivative polarity")
 
     @derivative_polarity.setter
@@ -566,17 +619,18 @@
 
 class MeasureElement(Element):
     def __init__(
         self,
         name: str,
         analog_input_ports: List[AnalogOutputPort],
         analog_output_ports: List[AnalogInputPort],
-        digital_input_ports: List[DigitalOutputPort] = [],
-        intermediate_frequency: int = None,
-        lo_frequency: int = None,
+        digital_input_ports: Optional[List[DigitalOutputPort]] = None,
+        intermediate_frequency: Optional[int] = None,
+        lo_frequency: Optional[int] = None,
+        **kwargs
     ):
         """A quantum element set for performing measurment
 
         :param name: [description]
         :type name: int
         :param analog_input_ports: [description]
         :type analog_input_ports: List[AnalogOutputPort]
@@ -585,20 +639,37 @@
         :param digital_input_ports: [description], defaults to []
         :type digital_input_ports: List[DigitalOutputPort], optional
         :param intermediate_frequency: intermediate frequency associated wit this element, defaults to None
         :type intermediate_frequency: int, optional
         :param lo_frequency: [description], defaults to None
         :type lo_frequency: int, optional
         """
+
+        time_of_flight: Optional[int] = kwargs.get("time_of_flight", 0)
+        smearing: Optional[int] = kwargs.get("smearing", 0)
+        digital_output_ports: Optional[List[DigitalInputPort]] = kwargs.get(
+            "digital_output_ports", None
+        )
+        mixer: Optional[Mixer] = kwargs.get("mixer", None)
+        pulses: Optional[List[Pulse]] = kwargs.get("pulses", None)
+        operations: Optional[Dict[str, str]] = kwargs.get("operations", None)
         super().__init__(
-            name, analog_output_ports, analog_input_ports, digital_input_ports
+            name,
+            analog_input_ports,
+            analog_output_ports,
+            digital_input_ports,
+            digital_output_ports,
+            intermediate_frequency,
+            lo_frequency,
+            mixer=mixer,
+            pulses=pulses,
+            operations=operations,
         )
-        self.dict["time_of_flight"] = 0
-        self.dict["smearing"] = 0
-        self.dict["intermediate_frequency"] = intermediate_frequency
+        self.dict["time_of_flight"] = time_of_flight
+        self.dict["smearing"] = smearing
 
     @property
     def time_of_flight(self):
         return self.dict["time_of_flight"]
 
     @time_of_flight.setter
     def time_of_flight(self, tof: int):
@@ -622,15 +693,19 @@
         :type cosine: float
         :param sine: value of the cosine vector
         :type sine: float
         :param duration: duration of the read out pulse
         :type duration: int
         """
         self._duration = duration
-        super().__init__(name, [(cosine, duration)], [(sine, duration)])
+        self._cosine = cosine
+        self._sine = sine
+        super(ConstantIntegrationWeights, self).__init__(
+            name, [(cosine, duration)], [(sine, duration)]
+        )
 
     @property
     def cosine(self):
         return self.dict["cosine"]
 
     @cosine.setter
     def cosine(self, v: float):
@@ -651,16 +726,16 @@
         :param name: name for the weights vector
         :type name: str
         :param cosine: a list of weights to be used with the cosine demodulation element, specified at 1 sample per 4 nanoseconds
         :type cosine: List
         :param sine: a list of weights to be used with the sine demodulation element, specified at 1 sample per 4 nanoseconds
         :type sine: List
         """
-        assert len(sine) == len(cosine)
         super().__init__(name, cosine, sine)
+        assert len(sine) == len(cosine)
 
     @property
     def cosine(self):
         return self.dict["cosine"]
 
     @cosine.setter
     def cosine(self, w: List[float]):
@@ -671,336 +746,477 @@
         return self.dict["sine"]
 
     @sine.setter
     def sine(self, w: List[float]):
         self.dict["sine"] = w
 
 
-class ElementCollection:
-    def __init__(self, name: str, elements: List[Element] = []):
+class ElementCollection(ConfigBuilderElement):
+    def __init__(self, name: str):
         """A named collection of Elements
 
         It also a useful base class for building components.
         """
-        self.name = name
-        self.elements = elements
+        super(ElementCollection, self).__init__(name)
+
+    @abc.abstractmethod
+    def get_elements(self) -> List[ConfigBuilderElement]:
+        pass
 
     @property
     def ports(self):
         ports = []
-        for elm in self.elements:
+        for elm in self.get_elements():
             ports += elm.ports
         return ports
 
     @property
     def waveform_names(self):
         names = []
-        for elm in self.elements:
+        for elm in self.get_elements():
             names += elm.waveform_names
         return names
 
     @property
     def operation_names(self):
         names = []
-        for elm in self.elements:
+        for elm in self.get_elements():
             names += elm.operation_names
         return names
 
     @property
     def pulse_names(self):
         names = []
-        for elm in self.elements:
+        for elm in self.get_elements():
             names += elm.pulse_names
         return names
 
 
 class ReadoutResonator(ElementCollection):
     def __init__(
         self,
         name: str,
         outputs: List[AnalogOutputPort],
         inputs: List[AnalogInputPort],
         intermediate_frequency: int,
+        **kwargs
     ):
         """
         A Microwave readout resonator
 
         :param name: A name for this resonator
         :type name: str
         :param outputs: A pair of output ports
         :type outputs: List[AnalogOutputPort]
         :param inputs: A pair of input ports
         :type inputs: List[AnalogInputPort]
         :param intermediate_frequency: The intermediate frequency
         :type intermediate_frequency: int
         """
+
+        operations: Optional[List[Operation]] = kwargs.get("operations", None)
+        time_of_flight: Optional[int] = kwargs.get("time_of_flight", 0)
+        smearing: Optional[int] = kwargs.get("smearing", 0)
+        mixer: Optional[Mixer] = kwargs.get("mixer", None)
+        lo_frequency: Optional[int] = kwargs.get("lo_frequency", None)
+
+        super(ReadoutResonator, self).__init__(name=name)
         if len(outputs) != 2:
             raise ConfigurationError("Number of output ports is not equal to 2")
         if len(inputs) != 2:
             raise ConfigurationError("Number of input ports is not equal to 2")
+        self.drive_name = name
+        self.drive_outputs = outputs
+        self.drive_inputs = inputs
+        self.drive_operations = []
+        if operations is not None:
+            self.drive_operations = operations
+        self.drive_intermediate_frequency = intermediate_frequency
+        self.drive_time_of_flight = time_of_flight
+
+        self.drive_mixer = mixer
+        self.drive_lo_frequency = lo_frequency
+        self.drive_smearing = smearing
+
+    def get_elements(self) -> List[ConfigBuilderElement]:
         drive = MeasureElement(
-            name, outputs, inputs, intermediate_frequency=intermediate_frequency
+            self.drive_name,
+            self.drive_outputs,
+            self.drive_inputs,
+            intermediate_frequency=self.drive_intermediate_frequency,
+            time_of_flight=self.drive_time_of_flight,
+            mixer=self.drive_mixer,
+            lo_frequency=self.drive_lo_frequency,
+            smearing=self.drive_smearing,
         )
-        super().__init__(name=name, elements=[drive])
+        for op in self.drive_operations:
+            drive.add(op)
+
+        if self.drive_inputs:
+            for (i, port) in enumerate(self.drive_inputs):
+                drive.dict["outputs"]["out" + str(i + 1)] = port.info
+
+        drive.dict["mixInputs"]["I"] = self.drive_outputs[0].info
+        drive.dict["mixInputs"]["Q"] = self.drive_outputs[1].info
+
+        if self.drive_mixer:
+            drive.dict["mixInputs"]["mixer"] = self.drive_mixer.name
+
+        return [drive]
 
     @property
     def intermediate_frequency(self):
-        return self.elements[0].intermediate_frequency
+        return self.drive_intermediate_frequency
 
     @intermediate_frequency.setter
     def intermediate_frequency(self, if_freq: int):
         """Set an IF for the resonator
 
         :param if_freq: A frequency in MHz
         :type if_freq: int
         """
-        self.elements[0].intermediate_frequency = if_freq
+        self.drive_intermediate_frequency = if_freq
 
     def add(self, obj: Union[Operation, List[Operation]]):
         """Add list of operations associated with the Transmon
 
         :param obj: The list of operations
         :type obj: list or an instance of Operation
         """
         if isinstance(obj, list):
             for o in obj:
                 self._add(o)
         else:
             self._add(obj)
         return self
 
-    def _add(self, op: Operation):
+    def _add(self, op: Union[Operation, MeasurePulse]):
         """Add operation associated with the Readout resonator
 
         :param obj: The operation
         :type obj: Operation
 
         """
-        if len(op.pulse.wfs) == 2:
-            self.elements[0].add(op)
+        if isinstance(op, Operation):
+            if len(op.pulse.wfs) == 2:
+                self.drive_operations.append(op)
+            else:
+                raise ConfigurationError("adding unsupported object")
+        elif isinstance(op, MeasurePulse):
+            if len(op.wfs) == 2:
+                self.drive_operations.append(op)
+            else:
+                raise ConfigurationError("adding unsupported object")
         else:
             raise ConfigurationError("adding unsupported object")
 
     @property
     def time_of_flight(self):
-        return self.elements[0].time_of_flight
+        return self.drive_time_of_flight
 
     @time_of_flight.setter
     def time_of_flight(self, tof: int):
-        self.elements[0].time_of_flight = tof
+        self.drive_time_of_flight = tof
 
     @property
     def smearing(self):
-        return self.elements[0].smearing
+        return self.drive_smearing
 
     @smearing.setter
     def smearing(self, t: int):
-        self.elements[0].smearing = t
+        self.drive_smearing = t
 
     @property
     def lo_frequency(self):
-        return self.elements[0].lo_frequency
+        return self.drive_lo_frequency
 
     @lo_frequency.setter
     def lo_frequency(self, lo_frequency: int):
-        self.elements[0].lo_frequency = lo_frequency
+        self.drive_lo_frequency = lo_frequency
 
     @property
     def input_ports(self):
-        return self.elements[0].analog_input_ports
+        return self.drive_inputs
 
     @input_ports.setter
     def input_ports(self, ports: List[AnalogInputPort]):
         assert len(ports) == 2
-        self.elements[0].analog_input_ports = ports
-        for i, port in enumerate(ports):
-            self.elements[0].dict["outputs"]["out" + str(i)] = port.info
+        self.drive_inputs = ports
 
     @property
     def output_ports(self):
-        return self.elements[0].analog_output_ports
+        return self.drive_outputs
 
     @output_ports.setter
     def output_ports(self, ports: List[AnalogOutputPort]):
         assert len(ports) == 2
-        self.elements[0].analog_output_ports = ports
-        self.elements[0].dict["mixInputs"]["I"] = ports[0].info
-        self.elements[0].dict["mixInputs"]["Q"] = ports[1].info
+        self.drive_outputs = ports
 
     @property
     def mixer(self):
-        return self.elements[0].mixer
+        return self.drive_mixer
 
     @mixer.setter
     def mixer(self, mixer: Mixer):
-        self.elements[0].mixer = mixer
-        self.elements[0].dict["mixInputs"]["mixer"] = mixer.name
+        self.drive_mixer = mixer
 
 
 class Transmon(ElementCollection):
     def __init__(
         self,
         name: str,
         I: AnalogOutputPort,
         Q: AnalogOutputPort,
         intermediate_frequency: int,
+        **kwargs
     ):
         """A superconducting transmon qubit
 
         :param name: A name for this transmon
         :type name: str
         :param I: I output port
         :type I: AnalogOutputPort
         :param Q: Q output port
         :type Q: AnalogOutputPort
         :param intermediate_frequency: intermediate frequency of the upconversion IQ mixer in MHz
         :type intermediate_frequency: int
         """
-        drive = Element(name, [I, Q], intermediate_frequency=intermediate_frequency)
-        super().__init__(name=name, elements=[drive])
+
+        mixer: Optional[Mixer] = kwargs.get("mixer", None)
+        lo_frequency: Optional[int] = kwargs.get("lo_frequency", None)
+        operations: Optional[List[Operation]] = kwargs.get("operations", None)
+
+        super(Transmon, self).__init__(name=name)
+        self.drive_I = I
+        self.drive_Q = Q
+        self.drive_intermediate_frequency = intermediate_frequency
+
+        self.drive_operations = []
+        if operations is not None:
+            self.drive_operations = operations
+        self.drive_intermediate_frequency = intermediate_frequency
+        self.drive_mixer = mixer
+        self.drive_lo_frequency = lo_frequency
+
+    def get_elements(self) -> List[ConfigBuilderElement]:
+        drive = Element(
+            self.name,
+            [self.drive_I, self.drive_Q],
+            intermediate_frequency=self.drive_intermediate_frequency,
+            mixer=self.drive_mixer,
+            lo_frequency=self.drive_lo_frequency,
+        )
+        drive.dict["mixInputs"]["I"] = self.drive_I.info
+        drive.dict["mixInputs"]["Q"] = self.drive_Q.info
+
+        for op in self.drive_operations:
+            drive.add(op)
+
+        if self.drive_mixer:
+            drive.dict["mixInputs"]["mixer"] = self.drive_mixer.name
+
+        return [drive]
 
     @property
     def I(self):
-        return self.elements[0].output_ports[0]
+        return self.drive_I
 
     @I.setter
     def I(self, p: AnalogOutputPort):
-        self.elements[0].output_ports[0] = p
-        self.elements[0].dict["mixInputs"]["I"] = p.info
+        self.drive_I = p
 
     @property
     def Q(self):
-        return self.elements[0].output_ports[1]
+        return self.drive_Q
 
     @Q.setter
     def Q(self, p: AnalogOutputPort):
-        self.elements[0].output_ports[1] = p
-        self.elements[0].dict["mixInputs"]["Q"] = p.info
+        self.drive_Q = p
 
     @property
     def lo_frequency(self):
-        return self.elements[0].lo_frequency
+        return self.drive_lo_frequency
 
     @lo_frequency.setter
     def lo_frequency(self, lo_frequency: int):
-        self.elements[0].lo_frequency = lo_frequency
+        self.drive_lo_frequency = lo_frequency
 
     @property
     def intermediate_frequency(self):
-        return self.elements[0].intermediate_frequency
+        return self.drive_intermediate_frequency
 
     @intermediate_frequency.setter
     def intermediate_frequency(self, if_freq: int):
-        """Set an IF for the transmon
-
+        """
+            Set an IF for the transmon
         :param if_freq: A frequency in MHz
         :type if_freq: int
         """
-        self.elements[0].intermediate_frequency = if_freq
+        self.drive_intermediate_frequency = if_freq
 
     def add(self, op: Union[Operation, List[Operation]]):
-        """Add list of operations associated with the Transmon
-
-        :param obj: The operations
-        :type obj: list or an instance of Operation
+        """
+            Add list of operations associated with the Transmon
+        :param op: The operations
+        :type op: list or an instance of Operation
         """
         if isinstance(op, list):
             for o in op:
                 self._add(o)
         else:
             self._add(op)
         return self
 
-    def _add(self, op: Operation):
-        if len(op.pulse.wfs) == 2:
-            self.elements[0].add(op)
+    def _add(self, op: Union[Operation, ControlPulse]):
+        if isinstance(op, Operation):
+            if len(op.pulse.wfs) == 2:
+                self.drive_operations.append(op)
+            else:
+                raise ConfigurationError("adding unsupported object")
+        elif isinstance(op, ControlPulse):
+            if len(op.wfs) == 2:
+                self.drive_operations.append(op)
+            else:
+                raise ConfigurationError("adding unsupported object")
         else:
             raise ConfigurationError("adding unsupported object")
 
     @property
     def mixer(self):
-        return self.elements[0].mixer
+        return self.drive_mixer
 
     @mixer.setter
     def mixer(self, mixer: Mixer):
-        self.elements[0].mixer = mixer
-        self.elements[0].dict["mixInputs"]["mixer"] = mixer.name
+        self.drive_mixer = mixer
 
 
 class FluxTunableTransmon(Transmon):
     def __init__(
         self,
         name: str,
         I: AnalogOutputPort,
         Q: AnalogOutputPort,
-        fl_port: AnalogOutputPort,
+        flux_port: AnalogOutputPort,
         intermediate_frequency: int,
+        **kwargs
     ):
         """A flux tuneable superconducting transmon qubit
 
         :param name: A name for this transmon
         :type name: str
         :param I: I output port
         :type I: AnalogOutputPort
         :param Q: Q output port
         :type Q: AnalogOutputPort
-        :param fl_port:  Flux line output Port
-        :type fl_port: AnalogOutputPort
+        :param flux_port:  Flux line output Port
+        :type flux_port: AnalogOutputPort
         :param intermediate_frequency: intermediate frequency of the upconversion IQ mixer in MHz
         :type intermediate_frequency: int
         """
-        super().__init__(name, I, Q, intermediate_frequency)
-        self.elements.append(Element(name + "_flux_line", [fl_port]))
 
-    def _add(self, op: Operation):
-        if len(op.pulse.wfs) == 2:
-            self.elements[0].add(op)
-        elif len(op.pulse.wfs) == 1:
-            self.elements[1].add(op)
+        mixer: Optional[Mixer] = kwargs.get("mixer", None)
+        lo_frequency: Optional[int] = kwargs.get("lo_frequency", None)
+        operations: Optional[List[Operation]] = kwargs.get("operations", None)
+        flux_operations: Optional[List[Operation]] = kwargs.get("flux_operations", None)
+
+        super(FluxTunableTransmon, self).__init__(
+            name,
+            I,
+            Q,
+            intermediate_frequency,
+            mixer=mixer,
+            lo_frequency=lo_frequency,
+            operations=operations,
+        )
+        self.flux_port = flux_port
+        self.flux_operations = []
+        if flux_operations is not None:
+            self.flux_operations = flux_operations
+
+    def get_elements(self) -> List[ConfigBuilderElement]:
+        els = super().get_elements()
+
+        el = Element(self.name + "_flux_line", [self.flux_port])
+        for op in self.flux_operations:
+            el.add(op)
+
+        els.append(el)
+        return els
+
+    def _add(self, op: Union[Operation, ControlPulse]):
+        if isinstance(op, Operation):
+            if len(op.pulse.wfs) == 2:
+                super(FluxTunableTransmon, self)._add(op)
+            elif len(op.pulse.wfs) == 1:
+                self.flux_operations.append(op)
+            else:
+                raise ConfigurationError(
+                    "Can not add a pulse with {0} waveforms".format(len(op.pulse.wfs))
+                )
+        elif isinstance(op, ControlPulse):
+            if len(op.wfs) == 2:
+                super(FluxTunableTransmon, self)._add(op)
+            elif len(op.wfs) == 1:
+                self.flux_operations.append(op)
+            else:
+                raise ConfigurationError(
+                    "Can not add a pulse with {0} waveforms".format(len(op.wfs))
+                )
+
         else:
             raise ConfigurationError(
-                "Can not add a pulse with {0} waveforms".format(len(op.pulse.wfs))
+                "adding unsupported object of type {}".format(type(op))
             )
 
 
 class Coupler(ElementCollection):
-    def __init__(self, name: str, p: AnalogOutputPort):
-        coupler = Element(name, analog_output_ports=[p])
-        super().__init__(name=name, elements=[coupler])
+    def __init__(self, name: str, port: AnalogOutputPort, **kwargs):
+        operations: Optional[List[Operation]] = kwargs.get("operations", None)
+        super(Coupler, self).__init__(name=name)
+        self._port = port
+        self.operations = []
+        if operations is not None:
+            self.operations = operations
+
+    def get_elements(self) -> List[ConfigBuilderElement]:
+        coupler = Element(self.name, analog_input_ports=[self._port])
+        for op in self.operations:
+            coupler.add(op)
+        return [coupler]
 
     def _add(self, op: Operation):
         if len(op.pulse.wfs) == 1:
-            self.elements[0].add(op)
+            self.operations.append(op)
         else:
             raise ConfigurationError(
                 "Can not add a pulse with {0} waveforms".format(len(op.pulse.wfs))
             )
 
     def add(self, op: Union[List[Operation], Operation]):
         if isinstance(op, list):
             for o in op:
                 self._add(o)
         else:
             self._add(op)
         return self
 
     @property
-    def p(self):
-        return self.elements[0].analog_output_ports[0]
+    def port(self):
+        return self._port
 
-    @p.setter
-    def p(self, p: AnalogOutputPort):
-        self.elements[0].analog_output_ports[0] = p
+    @port.setter
+    def port(self, p: AnalogOutputPort):
+        self._port = p
 
 
-class Oscillator:
+class Oscillator(ConfigBuilderElement):
     def __init__(
         self, name: str, intermediate_frequency: int, lo_frequency: int, mixer: str
     ):
-        self.name = name
+        super(Oscillator, self).__init__(name)
         self.dict = dict()
         self.dict["intermediate_frequency"] = intermediate_frequency
         self.dict["lo_frequency"] = lo_frequency
         self.dict["mixer"] = mixer
 
     @property
     def lo_frequency(self):
```

### Comparing `qualang-tools-0.8.0/qualang_tools/config/configuration.py` & `qualang-tools-0.9.0/qualang_tools/config/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,25 @@
 import copy
 from typing import List, Dict
 
-from qualang_tools.config.primitive_components import *
-from qualang_tools.config.components import *
-from qualang_tools.config.parameters import *
+from qualang_tools.config.components import (
+    Controller,
+    MeasurePulse,
+    Element,
+    ConstantWaveform,
+    ArbitraryWaveform,
+    Mixer,
+    Oscillator,
+)
+from qualang_tools.config.parameters import _is_callable, _is_parametric
+from qualang_tools.config.primitive_components import (
+    Waveform,
+    Pulse,
+    IntegrationWeights,
+)
 
 
 class QMConfiguration:
     def __init__(self, controllers: List[Controller] = None, version: int = 1):
         """A class to generate the QM configuration
 
         :param controllers: A controller or list of controllers used in this configuration, defaults to None
@@ -15,15 +27,17 @@
         :param version: Controller version, defaults to 1
         :type version: int, optional
         """
         self.config = dict()
         self.config["version"] = 1
         self.config["controllers"] = dict()
         for cont in controllers:
-            self.config["controllers"][cont.name] = cont.dict
+            self.config["controllers"][cont.name] = self._call_dict_parameters(
+                cont.dict
+            )
         self.config["elements"] = dict()
         self.config["pulses"] = dict()
         self.config["waveforms"] = dict()
         self.config["digital_waveforms"] = dict()
         self.config["integration_weights"] = dict()
         self.config["mixers"] = dict()
         # self.config["oscillators"] = dict()
@@ -33,20 +47,54 @@
 
         :param wf: a Wavefrom object
         :type wf: Waveform
         """
         self.config["waveforms"][wf.name] = self._call_dict_parameters(wf.dict)
 
     def _call_dict_parameters(self, dic: Dict):
-        if iscallable(dic):
-            if not isparametric(dic):
+        if _is_callable(dic):
+            if not _is_parametric(dic):
                 _dic = copy.deepcopy(dic)
                 for (k, v) in _dic.items():
-                    if iscallable(v):
-                        _dic[k] = v()
+                    if _is_callable(v):
+                        if isinstance(v, dict):
+                            _dic[k] = self._call_dict_parameters(v)
+                        else:
+                            _dic[k] = v()
+                return _dic
+        return dic
+
+    def _call_weights_dict(self, dic: Dict):
+        if _is_callable(dic):
+            if not _is_parametric(dic):
+                _dic = copy.deepcopy(dic)
+                for (k, v) in _dic.items():
+                    if isinstance(_dic["cosine"][0], tuple):
+                        val = _dic["cosine"][0][0]
+                        if _is_callable(_dic["cosine"][0][0]):
+                            val = _dic["cosine"][0][0]()
+                        dur = _dic["cosine"][0][1]
+                        if _is_callable(_dic["cosine"][0][1]):
+                            dur = _dic["cosine"][0][1]()
+                        _dic["cosine"][0] = (val, dur)
+
+                    if isinstance(_dic["sine"][0], tuple):
+                        val = _dic["sine"][0][0]
+                        if _is_callable(_dic["sine"][0][0]):
+                            val = _dic["sine"][0][0]()
+                        dur = _dic["sine"][0][1]
+                        if _is_callable(_dic["sine"][0][1]):
+                            dur = _dic["sine"][0][1]()
+                        _dic["sine"][0] = (val, dur)
+
+                    elif _is_callable(_dic["cosine"]):
+                        _dic["cosine"] = _dic["cosine"]()
+
+                        if _is_callable(_dic["sine"]):
+                            _dic["sine"] = _dic["sine"]()
                 return _dic
         return dic
 
     def add_waveforms(self, wfs: List[Waveform]):
         """Add a list of waveforms to this configuration
 
         :param wfs: a list of Waveform objects
@@ -63,22 +111,23 @@
         """
         _dict = copy.deepcopy(pulse.dict)
         self.add_waveforms(pulse.wfs)
         if pulse.digital_marker is not None:
             _dict["digital_marker"] = pulse.digital_marker.name
             self.config["digital_waveforms"][
                 pulse.digital_marker.name
-            ] = pulse.digital_marker.dict
+            ] = self._call_dict_parameters(pulse.digital_marker.dict)
         if isinstance(pulse, MeasurePulse):
-            _dict["digital_marker"] = {}
             _dict["integration_weights"] = dict()
             for w in pulse.integration_weights:
                 _dict["integration_weights"][w.name] = w.weights.name
-                self.config["integration_weights"][w.weights.name] = w.weights.dict
-        self.config["pulses"][pulse.name] = _dict
+                self.config["integration_weights"][
+                    w.weights.name
+                ] = self._call_weights_dict(w.weights.dict)
+        self.config["pulses"][pulse.name] = self._call_dict_parameters(_dict)
 
     def add_pulses(self, pulses: List[Pulse]):
         """Add a list of Pulses to this configuration
 
         :param pulses: a list of Pulse objects
         :type pulses: List[Pulse]
         """
@@ -88,18 +137,18 @@
     def add_element(self, elm: Element):
         """Add a quantum element to this configuration
 
         :param elm: an object of type Element
         :type elm: Element
         """
         # check if input/output ports belong to the controller
-        self.config["elements"][elm.name] = elm.dict
+        self.config["elements"][elm.name] = self._call_dict_parameters(elm.dict)
         if elm.type == "mixInputs":
             if elm.mixer is not None:
-                self.config["mixers"][elm.mixer.name] = [elm.mixer.dict]
+                self.add_mixer(elm.mixer)
         self.add_pulses(elm.pulses)
 
     def update_pulse(self, elm_name: str, pulse: Pulse):
         """Change the pulse associated with an element to the pulse given
 
         :param elm_name: name of a quantum element in the configuration
         :type elm_name: str
@@ -118,15 +167,17 @@
         :param iw: IntegrationWeights object
         :type iw: IntegrationWeights
         """
         assert pulse_name in self.config["pulses"].keys()
         assert self.config["pulses"][pulse_name]["operation"] == "measure"
         assert len(self.config["pulses"][pulse_name]["waveforms"].keys()) == 2
         weight_name = pulse_name + "_weight"
-        self.config["integration_weights"][weight_name] = iw.dict
+        self.config["integration_weights"][weight_name] = self._call_dict_parameters(
+            iw.dict
+        )
 
     def update_constant_waveform(self, wf_name: str, amp: float):
         """Update the amplitude of an existing constant waveform
 
         :param wf_name: name of the existing waveform
         :type wf_name: str
         :param amp: amplitude to set in the range (-0.5 to 0.5)
@@ -144,15 +195,17 @@
         :param samples: a vector of samples
         :type samples: List[float]
         """
         assert wf_name in self.config["waveforms"].keys()
         assert self.config["waveforms"][wf_name]["type"] == "arbitrary"
         self.config["waveforms"][wf_name]["samples"] = samples
 
-    def reset(self, controllers: List[Controller] = []):
+    def reset(self, controllers=None):
+        if controllers is None:
+            controllers = []
         self.__init__(controllers)
 
     def update_intermediate_frequency(
         self, elm_name: str, freq: float, update_mixer: bool = True
     ):
         self.config["elements"][elm_name]["intermediate_frequency"] = freq
         if update_mixer:
@@ -200,24 +253,30 @@
 
     def add_integration_weights(self, weight: IntegrationWeights):
         """Add integration weights to this configuration
 
         :param weight: an IntegrationWeights object
         :type weight: IntegrationWeights
         """
-        self.config["integration_weights"][weight.name] = weight.dict
+        self.config["integration_weights"][weight.name] = self._call_dict_parameters(
+            weight.dict
+        )
 
     def add_mixer(self, mixer: Mixer):
         """Add a mixer to this configuration
 
         :param mixer: A Mixer object
         :type mixer: Mixer
         """
-        self.config["mixers"][mixer.name] = [mixer.dict]
+        self.config["mixers"][mixer.name] = [
+            self._call_dict_parameters(data) for data in mixer.dict
+        ]
 
     def add_oscillator(self, oscillator: Oscillator):
         """Add an oscillator to this configuration
 
         :param oscillator: an Oscillator object
         :type oscillator: Oscillator
         """
-        self.config["oscillators"][oscillator.name] = oscillator.dict
+        self.config["oscillators"][oscillator.name] = self._call_dict_parameters(
+            oscillator.dict
+        )
```

### Comparing `qualang-tools-0.8.0/qualang_tools/config/gui.py` & `qualang-tools-0.9.0/qualang_tools/config/gui.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/config/integration_weights_tools.py` & `qualang-tools-0.9.0/qualang_tools/config/integration_weights_tools.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/config/server/component_editor.py` & `qualang-tools-0.9.0/qualang_tools/config/server/component_editor.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/config/server/config_editor.py` & `qualang-tools-0.9.0/qualang_tools/config/server/config_editor.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/config/server/download.py` & `qualang-tools-0.9.0/qualang_tools/config/server/download.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/config/server/editors.py` & `qualang-tools-0.9.0/qualang_tools/config/server/editors.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/config/server/qua1_openapi.json` & `qualang-tools-0.9.0/qualang_tools/config/server/qua1_openapi.json`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/config/server/readme.md` & `qualang-tools-0.9.0/qualang_tools/config/server/readme.md`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/config/server/upload.py` & `qualang-tools-0.9.0/qualang_tools/config/server/upload.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/config/waveform_tools.py` & `qualang-tools-0.9.0/qualang_tools/config/waveform_tools.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/control_panel/README.md` & `qualang-tools-0.9.0/qualang_tools/control_panel/README.md`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/control_panel/README_manual_output_control.md` & `qualang-tools-0.9.0/qualang_tools/control_panel/README_manual_output_control.md`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/control_panel/README_vna.md` & `qualang-tools-0.9.0/qualang_tools/control_panel/README_vna.md`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/control_panel/manual_output_control.py` & `qualang-tools-0.9.0/qualang_tools/control_panel/manual_output_control.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/control_panel/vna.py` & `qualang-tools-0.9.0/qualang_tools/control_panel/vna.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/qualang_tools/simulator_tools.py` & `qualang-tools-0.9.0/qualang_tools/simulator_tools.py`

 * *Files identical despite different names*

### Comparing `qualang-tools-0.8.0/setup.py` & `qualang-tools-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['qualang_tools',
  'qualang_tools.addons',
+ 'qualang_tools.analysis',
  'qualang_tools.bakery',
  'qualang_tools.config',
  'qualang_tools.config.server',
  'qualang_tools.control_panel']
 
 package_data = \
 {'': ['*']}
@@ -31,17 +32,17 @@
 extras_require = \
 {'interplot': ['dill>=0.3.4,<0.4.0',
                'pypiwin32>=223,<224',
                'ipython>=7.31.1,<8.0.0']}
 
 setup_kwargs = {
     'name': 'qualang-tools',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'The qualang_tools package includes various tools related to QUA programs in Python',
-    'long_description': "![PyPI](https://img.shields.io/pypi/v/qualang-tools)\n[![discord](https://img.shields.io/discord/806244683403100171?label=QUA&logo=Discord&style=plastic)](https://discord.gg/7FfhhpswbP)\n\n[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\n# QUA Language Tools\n\nThe QUA language tools package includes various tools useful while writing QUA programs and performing experiments.\n\nIt includes:\n\n* [Bakery](qualang_tools/bakery/README.md) - This library introduces a new framework for creating arbitrary waveforms and\nstoring them in the usual configuration file. It allows defining waveforms in a QUA-like manner while working with 1ns resolution (or higher).\n\n* [Interactive Plot Library](qualang_tools/addons/README.md) - This package drastically extends the capabilities of matplotlib,\nenables easily editing various parts of the figure, copy-pasting data between figures and into spreadsheets, \nfitting the data and saving the figures.\n\n* [Config Tools](qualang_tools/config/README.md) - This package includes tools related to the QOP configuration file, including:\n  * [Integration Weights Tools](README_integration_weights_tools.md) - This package includes tools for the creation and manipulation of integration weights. \n  * [Waveform Tools](README_waveform_tools.md) - This package includes tools for creating waveforms useful for experiments with the QOP.\n  * [Config GUI](README_config_GUI.md) - This package contains a GUI for creating and visualizing the configuration file.\n  * [Config Builder](README_config_builder.md) - This package contains an API for creating and manipulation configuration files.\n\n* [Control Panel](qualang_tools/control_panel/README.md)- This package includes tools for directly controlling the OPX.\n  * [ManualOutputControl](README_manual_output_control.md) - This module allows controlling the outputs from the OPX in CW mode. Once created, it has an API for defining which channels are on. Analog channels also have an API for defining their amplitude and frequency.\n  * [VNA](README_vna.md) - This module allows to configure the OPX as a VNA for a given element (readout resonator for instance) and operation (readout pulse for instance) already defined in the configuration. Once created, it has an API for defining which measurements are to be run depending on the down-conversion solution used (ED: envelope detector, IR: image rejection mixer, IQ: IQ mixer).\n\n## Installation\n\nInstall the current version using `pip`, the `--upgrade` flag ensures that you will get the latest version.\n\n```\npip install --upgrade qualang-tools\n```\n\n## Support and Contribution\nHave an idea for another tool? A way to improve an existing one? Found a bug in our code?\n\nWe'll be happy if you could let us know by opening an [issue](https://github.com/qua-platform/py-qua-tools/issues) on the [GitHub repository](https://github.com/qua-platform/py-qua-tools).\n\nFeel like contributing code to this library? We're thrilled! Please follow [this guide](https://github.com/qua-platform/py-qua-tools/blob/main/CONTRIBUTING.md) and feel free to contact us if you need any help, you can do it by opening an [issue](https://github.com/qua-platform/py-qua-tools/issues) :)\n\n## Usage\n\nExamples for using various tools can be found on the [QUA Libraries Repository](https://github.com/qua-platform/qua-libs).\n\nExamples for using the Baking toolbox, including 1-qubit randomized benchmarking, cross-entropy benchmark (XEB), high sampling rate baking and more can be found [here](https://github.com/qua-platform/qua-libs/tree/main/examples/bakery).\n",
+    'long_description': "![PyPI](https://img.shields.io/pypi/v/qualang-tools)\n[![discord](https://img.shields.io/discord/806244683403100171?label=QUA&logo=Discord&style=plastic)](https://discord.gg/7FfhhpswbP)\n\n[![License](https://img.shields.io/badge/License-BSD%203--Clause-blue.svg)](https://opensource.org/licenses/BSD-3-Clause)\n\n# QUA Language Tools\n\nThe QUA language tools package includes various tools useful while writing QUA programs and performing experiments.\n\nIt includes:\n\n* [Bakery](qualang_tools/bakery/README.md) - This library introduces a new framework for creating arbitrary waveforms and\nstoring them in the usual configuration file. It allows defining waveforms in a QUA-like manner while working with 1ns resolution (or higher).\n\n* [Interactive Plot Library](qualang_tools/addons/README.md) - This package drastically extends the capabilities of matplotlib,\nenables easily editing various parts of the figure, copy-pasting data between figures and into spreadsheets, \nfitting the data and saving the figures.\n\n* [Config Tools](qualang_tools/config/README.md) - This package includes tools related to the QOP configuration file, including:\n  * [Integration Weights Tools](README_integration_weights_tools.md) - This package includes tools for the creation and manipulation of integration weights. \n  * [Waveform Tools](README_waveform_tools.md) - This package includes tools for creating waveforms useful for experiments with the QOP.\n  * [Config GUI](README_config_GUI.md) - This package contains a GUI for creating and visualizing the configuration file.\n  * [Config Builder](README_config_builder.md) - This package contains an API for creating and manipulation configuration files.\n\n* [Control Panel](qualang_tools/control_panel/README.md)- This package includes tools for directly controlling the OPX.\n  * [ManualOutputControl](README_manual_output_control.md) - This module allows controlling the outputs from the OPX in CW mode. Once created, it has an API for defining which channels are on. Analog channels also have an API for defining their amplitude and frequency.\n  * [VNA](README_vna.md) - This module allows to configure the OPX as a VNA for a given element (readout resonator for instance) and operation (readout pulse for instance) already defined in the configuration. Once created, it has an API for defining which measurements are to be run depending on the down-conversion solution used (ED: envelope detector, IR: image rejection mixer, IQ: IQ mixer).\n\n## Installation\n\nInstall the current version using `pip`, the `--upgrade` flag ensures that you will get the latest version.\n\n```commandline\npip install --upgrade qualang-tools\n```\n\n## Support and Contribution\nHave an idea for another tool? A way to improve an existing one? Found a bug in our code?\n\nWe'll be happy if you could let us know by opening an [issue](https://github.com/qua-platform/py-qua-tools/issues) on the [GitHub repository](https://github.com/qua-platform/py-qua-tools).\n\nFeel like contributing code to this library? We're thrilled! Please follow [this guide](https://github.com/qua-platform/py-qua-tools/blob/main/CONTRIBUTING.md) and feel free to contact us if you need any help, you can do it by opening an [issue](https://github.com/qua-platform/py-qua-tools/issues) :)\n\n## Usage\n\nExamples for using various tools can be found on the [QUA Libraries Repository](https://github.com/qua-platform/qua-libs).\n\nExamples for using the Baking toolbox, including 1-qubit randomized benchmarking, cross-entropy benchmark (XEB), high sampling rate baking and more can be found [here](https://github.com/qua-platform/qua-libs/tree/main/examples/bakery).\n",
     'author': 'QM',
     'author_email': 'qua-libs@quantum-machines.co',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/qua-platform/py-qua-tools',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `qualang-tools-0.8.0/PKG-INFO` & `qualang-tools-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qualang-tools
-Version: 0.8.0
+Version: 0.9.0
 Summary: The qualang_tools package includes various tools related to QUA programs in Python
 Home-page: https://github.com/qua-platform/py-qua-tools
 License: BSD-3-Clause
 Author: QM
 Author-email: qua-libs@quantum-machines.co
 Requires-Python: >=3.7.1,<3.10
 Classifier: License :: OSI Approved :: BSD License
@@ -59,15 +59,15 @@
   * [ManualOutputControl](README_manual_output_control.md) - This module allows controlling the outputs from the OPX in CW mode. Once created, it has an API for defining which channels are on. Analog channels also have an API for defining their amplitude and frequency.
   * [VNA](README_vna.md) - This module allows to configure the OPX as a VNA for a given element (readout resonator for instance) and operation (readout pulse for instance) already defined in the configuration. Once created, it has an API for defining which measurements are to be run depending on the down-conversion solution used (ED: envelope detector, IR: image rejection mixer, IQ: IQ mixer).
 
 ## Installation
 
 Install the current version using `pip`, the `--upgrade` flag ensures that you will get the latest version.
 
-```
+```commandline
 pip install --upgrade qualang-tools
 ```
 
 ## Support and Contribution
 Have an idea for another tool? A way to improve an existing one? Found a bug in our code?
 
 We'll be happy if you could let us know by opening an [issue](https://github.com/qua-platform/py-qua-tools/issues) on the [GitHub repository](https://github.com/qua-platform/py-qua-tools).
```

