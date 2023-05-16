# Comparing `tmp/pyamdgpuinfo-2.1.2.tar.gz` & `tmp/pyamdgpuinfo-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyamdgpuinfo-2.1.2.tar", last modified: Mon Feb  7 21:38:32 2022, max compression
+gzip compressed data, was "pyamdgpuinfo-2.1.3.tar", last modified: Sat Jul 30 16:11:54 2022, max compression
```

## Comparing `pyamdgpuinfo-2.1.2.tar` & `pyamdgpuinfo-2.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 21:38:32.310048 pyamdgpuinfo-2.1.2/
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-02-07 21:38:16.000000 pyamdgpuinfo-2.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      109 2022-02-07 21:38:16.000000 pyamdgpuinfo-2.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-02-07 21:38:32.310048 pyamdgpuinfo-2.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1934 2022-02-07 21:38:16.000000 pyamdgpuinfo-2.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 21:38:32.310048 pyamdgpuinfo-2.1.2/pyamdgpuinfo/
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-02-07 21:38:16.000000 pyamdgpuinfo-2.1.2/pyamdgpuinfo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2905 2022-02-07 21:38:16.000000 pyamdgpuinfo-2.1.2/pyamdgpuinfo/amdgpu_cy.pxd
--rw-r--r--   0 runner    (1001) docker     (121)      404 2022-02-07 21:38:16.000000 pyamdgpuinfo-2.1.2/pyamdgpuinfo/pthread_cy.pxd
--rw-r--r--   0 runner    (1001) docker     (121)    24632 2022-02-07 21:38:16.000000 pyamdgpuinfo-2.1.2/pyamdgpuinfo/pyamdgpuinfo.pyx
--rw-r--r--   0 runner    (1001) docker     (121)      383 2022-02-07 21:38:16.000000 pyamdgpuinfo-2.1.2/pyamdgpuinfo/xf86drm_cy.pxd
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-02-07 21:38:32.310048 pyamdgpuinfo-2.1.2/pyamdgpuinfo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2480 2022-02-07 21:38:32.000000 pyamdgpuinfo-2.1.2/pyamdgpuinfo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      355 2022-02-07 21:38:32.000000 pyamdgpuinfo-2.1.2/pyamdgpuinfo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 21:38:32.000000 pyamdgpuinfo-2.1.2/pyamdgpuinfo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-02-07 21:38:32.000000 pyamdgpuinfo-2.1.2/pyamdgpuinfo.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-02-07 21:38:32.000000 pyamdgpuinfo-2.1.2/pyamdgpuinfo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-02-07 21:38:32.310048 pyamdgpuinfo-2.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1078 2022-02-07 21:38:16.000000 pyamdgpuinfo-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 16:11:54.503825 pyamdgpuinfo-2.1.3/
+-rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-07-30 16:11:36.000000 pyamdgpuinfo-2.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      109 2022-07-30 16:11:36.000000 pyamdgpuinfo-2.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2486 2022-07-30 16:11:54.503825 pyamdgpuinfo-2.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1917 2022-07-30 16:11:36.000000 pyamdgpuinfo-2.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 16:11:54.503825 pyamdgpuinfo-2.1.3/pyamdgpuinfo/
+-rw-r--r--   0 runner    (1001) docker     (121)       57 2022-07-30 16:11:36.000000 pyamdgpuinfo-2.1.3/pyamdgpuinfo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23803 2022-07-30 16:11:36.000000 pyamdgpuinfo-2.1.3/pyamdgpuinfo/_pyamdgpuinfo.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     2713 2022-07-30 16:11:36.000000 pyamdgpuinfo-2.1.3/pyamdgpuinfo/amdgpu_cy.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      404 2022-07-30 16:11:36.000000 pyamdgpuinfo-2.1.3/pyamdgpuinfo/pthread_cy.pxd
+-rw-r--r--   0 runner    (1001) docker     (121)      383 2022-07-30 16:11:36.000000 pyamdgpuinfo-2.1.3/pyamdgpuinfo/xf86drm_cy.pxd
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-30 16:11:54.503825 pyamdgpuinfo-2.1.3/pyamdgpuinfo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2486 2022-07-30 16:11:54.000000 pyamdgpuinfo-2.1.3/pyamdgpuinfo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      356 2022-07-30 16:11:54.000000 pyamdgpuinfo-2.1.3/pyamdgpuinfo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-30 16:11:54.000000 pyamdgpuinfo-2.1.3/pyamdgpuinfo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-30 16:11:54.000000 pyamdgpuinfo-2.1.3/pyamdgpuinfo.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-07-30 16:11:54.000000 pyamdgpuinfo-2.1.3/pyamdgpuinfo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-30 16:11:54.503825 pyamdgpuinfo-2.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-07-30 16:11:36.000000 pyamdgpuinfo-2.1.3/setup.py
```

### Comparing `pyamdgpuinfo-2.1.2/LICENSE` & `pyamdgpuinfo-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyamdgpuinfo-2.1.2/PKG-INFO` & `pyamdgpuinfo-2.1.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: pyamdgpuinfo
-Version: 2.1.2
+Version: 2.1.3
 Summary: AMD GPU stats
 Home-page: https://github.com/mark9064/pyamdgpuinfo
 Author: mark9064
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyamdgpuinfo
 
 AMD GPU information
 
 ## Install
 
-`pip3 install pyamdgpuinfo`
+`pip install pyamdgpuinfo`
 
-Only linux is supported, using the amdgpu driver.
+Only Linux is supported, using the AMDGPU driver.
 
-Precompiled wheels for python 3.6, 3.7, 3.8, 3.9 and 3.10 are the default method of install. This means that you don't need cython or any other dependencies to install it normally.
+The library is written using Cython, meaning that Cython and and a C compiler are needed to build and install from source. Additionally, libdrm development headers are required. 
 
-The library is written using cython, meaning that cython and and a C compiler are needed to build and install from source. Additionally, libdrm development headers are needed. 
+Precompiled wheels for Python 3.7-3.10 are the default method of install. This means that you don't need Cython or any other dependencies to install it normally.
 
 ## Usage
 
 Example:
 ```python
 >>> import pyamdgpuinfo
 >>> n_devices = pyamdgpuinfo.detect_gpus()
@@ -57,15 +58,15 @@
 * query_sclk - Queries shader (core) clock
 * query_mclk - Queries memory clock
 * query_vram_usage - Queries VRAM usage
 * query_gtt_usage - Queries GTT usage
 * query_temperature - Queries temperature
 * query_load - Queries GPU load
 * query_power - Queries power consumption
-* query_northbridge_voltage - Queries northbrige voltage
+* query_northbridge_voltage - Queries northbridge voltage
 * query_graphics_voltage - Queries graphics voltage
 
 
 VRAM and GTT sizes are available as an attribute of GPUInfo.
 
 ## Mentions
```

### Comparing `pyamdgpuinfo-2.1.2/README.md` & `pyamdgpuinfo-2.1.3/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # pyamdgpuinfo
 
 AMD GPU information
 
 ## Install
 
-`pip3 install pyamdgpuinfo`
+`pip install pyamdgpuinfo`
 
-Only linux is supported, using the amdgpu driver.
+Only Linux is supported, using the AMDGPU driver.
 
-Precompiled wheels for python 3.6, 3.7, 3.8, 3.9 and 3.10 are the default method of install. This means that you don't need cython or any other dependencies to install it normally.
+The library is written using Cython, meaning that Cython and and a C compiler are needed to build and install from source. Additionally, libdrm development headers are required. 
 
-The library is written using cython, meaning that cython and and a C compiler are needed to build and install from source. Additionally, libdrm development headers are needed. 
+Precompiled wheels for Python 3.7-3.10 are the default method of install. This means that you don't need Cython or any other dependencies to install it normally.
 
 ## Usage
 
 Example:
 ```python
 >>> import pyamdgpuinfo
 >>> n_devices = pyamdgpuinfo.detect_gpus()
@@ -40,15 +40,15 @@
 * query_sclk - Queries shader (core) clock
 * query_mclk - Queries memory clock
 * query_vram_usage - Queries VRAM usage
 * query_gtt_usage - Queries GTT usage
 * query_temperature - Queries temperature
 * query_load - Queries GPU load
 * query_power - Queries power consumption
-* query_northbridge_voltage - Queries northbrige voltage
+* query_northbridge_voltage - Queries northbridge voltage
 * query_graphics_voltage - Queries graphics voltage
 
 
 VRAM and GTT sizes are available as an attribute of GPUInfo.
 
 ## Mentions
```

### Comparing `pyamdgpuinfo-2.1.2/pyamdgpuinfo/amdgpu_cy.pxd` & `pyamdgpuinfo-2.1.3/pyamdgpuinfo/amdgpu_cy.pxd`

 * *Files 10% similar despite different names*

```diff
@@ -52,13 +52,11 @@
     int AMDGPU_INFO_SENSOR_GFX_SCLK	"AMDGPU_INFO_SENSOR_GFX_SCLK"
     int AMDGPU_INFO_SENSOR_GFX_MCLK	"AMDGPU_INFO_SENSOR_GFX_MCLK"
     int AMDGPU_INFO_SENSOR_GPU_TEMP	"AMDGPU_INFO_SENSOR_GPU_TEMP"
     int AMDGPU_INFO_SENSOR_GPU_LOAD	"AMDGPU_INFO_SENSOR_GPU_LOAD"
     int AMDGPU_INFO_SENSOR_GPU_AVG_POWER "AMDGPU_INFO_SENSOR_GPU_AVG_POWER"
     int AMDGPU_INFO_SENSOR_VDDNB "AMDGPU_INFO_SENSOR_VDDNB"
     int AMDGPU_INFO_SENSOR_VDDGFX "AMDGPU_INFO_SENSOR_VDDGFX"
-    # int AMDGPU_INFO_SENSOR_STABLE_PSTATE_GFX_SCLK "AMDGPU_INFO_SENSOR_STABLE_PSTATE_GFX_SCLK"
-    # int AMDGPU_INFO_SENSOR_STABLE_PSTATE_GFX_MCLK "AMDGPU_INFO_SENSOR_STABLE_PSTATE_GFX_MCLK"
     struct drm_amdgpu_info_vram_gtt:
         uint64_t vram_size
         uint64_t vram_cpu_accessible_size
         uint64_t gtt_size
```

### Comparing `pyamdgpuinfo-2.1.2/pyamdgpuinfo/pyamdgpuinfo.pyx` & `pyamdgpuinfo-2.1.3/pyamdgpuinfo/_pyamdgpuinfo.pyx`

 * *Files 13% similar despite different names*

```diff
@@ -1,48 +1,47 @@
-"""GPU information using amdgpu"""
+"""GPU information using AMDGPU"""
 cimport pyamdgpuinfo.xf86drm_cy as xf86drm_cy
 cimport pyamdgpuinfo.amdgpu_cy as amdgpu_cy
 cimport pyamdgpuinfo.pthread_cy as pthread_cy
 
 from libc.stdint cimport uint32_t
 from libc.stdlib cimport malloc, calloc, free
 from posix.time cimport CLOCK_MONOTONIC, timespec, clock_gettime, nanosleep
 
 import os
-import time
 
 
 # gpu registers location
 cdef int GRBM_OFFSET = 8196
 # search path
 cdef str DEVICE_PATH = "/dev/dri/by-path/"
 cdef str DEVICE_FALLBACK_PATH = "/dev/dri/"
 
-COMPARE_BITS = {
+cdef dict COMPARE_BITS = {
     "texture_addresser": 2 ** 14,
     "shader_export": 2 ** 20,
     "shader_interpolator": 2 ** 22,
     "scan_converter": 2 ** 24,
     "primitive_assembly": 2 ** 25,
     "depth_block": 2 ** 26,
     "colour_block": 2 ** 30,
     "graphics_pipe": 2 ** 31
 }
 
 
 cdef int get_registers(amdgpu_cy.amdgpu_device_handle amdgpu_dev, uint32_t *out) nogil:
-    """Returns whether amdgpu query succeeds, returns query result through out"""
+    """Returns whether AMDGPU query succeeds, returns query result through out"""
     return amdgpu_cy.amdgpu_read_mm_registers(amdgpu_dev, GRBM_OFFSET, 1, 0xffffffff, 0, out)
 
 cdef int query_info(amdgpu_cy.amdgpu_device_handle amdgpu_dev, int info, unsigned long long *out):
-    """Returns whether amdgpu query succeeds, returns query result through out"""
+    """Returns whether AMDGPU query succeeds, returns query result through out"""
     return amdgpu_cy.amdgpu_query_info(amdgpu_dev, info, sizeof(unsigned long long), out)
 
 cdef int query_sensor(amdgpu_cy.amdgpu_device_handle amdgpu_dev, int info, unsigned long long *out):
-    """Returns whether amdgpu query succeeds, returns query result through out"""
+    """Returns whether AMDGPU query succeeds, returns query result through out"""
     return amdgpu_cy.amdgpu_query_sensor_info(amdgpu_dev, info, sizeof(unsigned long long), out)
 
 
 cdef timespec timespec_subtract(timespec left, timespec right) nogil:
     """Performs left - right"""
     cdef:
         timespec temp
@@ -56,15 +55,15 @@
 
 cdef timespec timespec_clamp(timespec time_to_clamp) nogil:
     """Clamps a timespec to 0 if seconds is negative"""
     if time_to_clamp.tv_sec < 0:
         time_to_clamp.tv_sec = 0
         time_to_clamp.tv_nsec = 0
     return time_to_clamp
-    
+
 cdef timespec timespec_sum(timespec left, timespec right) nogil:
     """Performs left + right"""
     cdef:
         timespec temp
     temp.tv_nsec = left.tv_nsec + right.tv_nsec
     temp.tv_sec = left.tv_sec + right.tv_sec
     if temp.tv_nsec >= 1000000000:
@@ -156,32 +155,33 @@
         detected_devices = [x for x in devices if "card" in x]
     detected_devices = [os.path.join(path, x) for x in detected_devices]
     return sorted(detected_devices)
 
 
 cpdef int detect_gpus():
     """Returns the number of GPUs available
-    
+
     Params:
         No params.
     Raises:
-        RuntimeError: if an error occurs when calling amdgpu methods.
+        OSError: if an AMDGPU device couldn't be initialised.
     Returns:
         int; number of GPUs available.
     """
     return get_gpu(-1)
 
 
 cpdef object get_gpu(int gpu_id):
     """Returns GPUInfo object for gpu_id
 
     Params:
         gpu_id: int; the sequential id of the GPU to get
     Raises:
-        RuntimeError: if an error occurs when calling amdgpu methods.
+        OSError: if an AMDGPU device couldn't be initialised.
+        RuntimeError: if the GPU requested could not be found.
     Returns:
         GPUInfo; object providing interface to GPU info calls
     Extra information:
         Find the number of GPUs available by calling detect_gpus() first.
         e.g you could do
             n = pyamdgpuinfo.detect_gpus()
             gpus = [pyamdgpuinfo.get_gpu(x) for x in range(n)]
@@ -209,15 +209,15 @@
         drm_name = ver.name.decode()
         xf86drm_cy.drmFreeVersion(ver)
         if drm_name != "amdgpu":
             os.close(drm_fd)
             continue
         if amdgpu_cy.amdgpu_device_initialize(drm_fd, &major_ver, &minor_ver, &device_handle):
             os.close(drm_fd)
-            raise OSError("Can't initialize amdgpu driver for amdgpu GPU"
+            raise OSError("Can't initialize AMDGPU driver for AMDGPU GPU"
                           " (this is usually a permission error)")
         os.close(drm_fd)
         # ioctl check
         if get_registers(device_handle, &register_data) != 0:
             continue
         amdgpu_cy.amdgpu_device_deinitialize(device_handle)
         if amdgpu_index == gpu_id:
@@ -225,15 +225,15 @@
         amdgpu_index += 1
     if gpu_id == -1:
         return amdgpu_index
     raise RuntimeError("GPU id {0} not found".format(gpu_id))
 
 
 cdef class GPUInfo:
-    """Interface for amdgpu device info queries
+    """Interface for AMDGPU device info queries
 
     Params:
         device_path: str; full path to device in /dev/dri/ or /dev/dri/by-path/.
         gpu_id: int; sequential GPU id (from get_gpu).
     Raises:
         No specific exceptions.
     Attrs:
@@ -253,19 +253,19 @@
         query_vram_usage: queries VRAM usage.
         query_gtt_usage: queries GTT usage.
         query_sclk: queries shader (core) clock.
         query_mclk: queries memory clock.
         query_temperature: queries temperature.
         query_load: queries overall GPU load.
         query_power: queries power consumption.
-        query_northbridge_voltage: queries northbrige voltage.
+        query_northbridge_voltage: queries northbridge voltage.
         query_graphics_voltage: queries graphics voltage.
     Extra information:
         The pci_slot attr can be used to identify cards:
-            - This is tied to a physical PCI slot 
+            - This is tied to a physical PCI slot
             - It will only change if the card is moved to a different slot
               or if the motherboard is changed
         This class can be instantiated directly, but a typical application would be:
             - Find number of GPUs with detect_gpus()
             - Use get_gpu(index) which returns a GPUInfo object
     """
     cdef:
@@ -279,19 +279,24 @@
         amdgpu_cy.amdgpu_device_handle device_handle
         poll_args_t* thread_args
 
     def __cinit__(self):
         self.utilisation_polling = False
 
     def __dealloc__(self):
+        # __del__ not available for extension types until Cython 3.0
+        cdef:
+            timespec sleep_time
+        sleep_time.tv_nsec = 1_000_000
+        sleep_time.tv_sec = 0
         if self.utilisation_polling:
             self.thread_args.desired_state = 0
             # wait for it to exit
             while self.thread_args.current_state != 0:
-                time.sleep(0.001)
+                nanosleep(&sleep_time, NULL)
             free(self.thread_args.results)
             free(self.thread_args)
             self.utilisation_polling = False
         amdgpu_cy.amdgpu_device_deinitialize(self.device_handle)
 
     def __init__(self, device_path, gpu_id):
         cdef:
@@ -305,15 +310,15 @@
         else:
             self.pci_slot = None
         drm_fd = os.open(self.path, os.O_RDWR)
         amdgpu_cy.amdgpu_device_initialize(drm_fd, &major_ver, &minor_ver, &self.device_handle)
         os.close(drm_fd)
         self.memory_info = {}
         if not amdgpu_cy.amdgpu_query_info(self.device_handle, amdgpu_cy.AMDGPU_INFO_VRAM_GTT,
-                                           sizeof(vram_gtt), &vram_gtt): # amdgpu vram gtt query succeeded
+                                           sizeof(vram_gtt), &vram_gtt): # AMDGPU vram gtt query succeeded
             self.memory_info["vram_size"] = vram_gtt.vram_size
             self.memory_info["gtt_size"] = vram_gtt.gtt_size
             self.memory_info["vram_cpu_accessible_size"] = vram_gtt.vram_cpu_accessible_size
         else:
             self.memory_info["vram_size"] = None
             self.memory_info["gtt_size"] = None
             self.memory_info["vram_cpu_accessible_size"] = None
@@ -339,15 +344,15 @@
         Returns:
             Nothing returned.
         Extra information:
             - This function starts a thread which reads GPU performance registers {ticks_per_second} times per second
                 - These registers store the status of GPU components, simply as 1 (in use) or 0 (not in use) for each component
             - The results of these reads is saved to a buffer of {buffer_size_in_ticks}
             - When utilisation is queried, a mean is taken of all the values in the buffer
-                - e.g texture addresser data may be 0000100100, 10 samples with 2 ones, so utilisation is 0.2 
+                - e.g texture addresser data may be 0000100100, 10 samples with 2 ones, so utilisation is 0.2
             - This means that the time period of the mean is buffer_size_in_ticks / ticks_per_second
                 - So at default it is a mean of the past second (100/100 = 1)
             - When the thread has just started, querying utilisation before one time period has elasped will error
                 - The buffer will not have been populated at this point and will be partly zeroes, so a mean would be misleading
             - The polling thread provides data only for query_utilisation
 
             WARNING: Utilisation polling may not work correctly with all devices, in testing it
@@ -358,20 +363,24 @@
             pthread_cy.pthread_attr_t attr
             int index
         if self.utilisation_polling:
             raise RuntimeError("Thread already started")
         pthread_cy.pthread_attr_init(&attr)
         pthread_cy.pthread_attr_setdetachstate(&attr, pthread_cy.PTHREAD_CREATE_DETACHED)
         self.thread_args = <poll_args_t*>malloc(sizeof(poll_args_t))
+        if not self.thread_args:
+            raise MemoryError()
         self.thread_args.desired_state = 1
         self.thread_args.current_state = 0
         self.thread_args.measurement_interval.tv_nsec = int((1 / ticks_per_second * 1e9) % 1e9)
         self.thread_args.measurement_interval.tv_sec = 1 // ticks_per_second
         self.thread_args.buffer_size = buffer_size_in_ticks
         self.thread_args.results = <uint32_t*>calloc(buffer_size_in_ticks, sizeof(uint32_t))
+        if not self.thread_args.results:
+            raise MemoryError()
         self.thread_args.device_handle = &self.device_handle
         self.utilisation_polling = True
         if pthread_cy.pthread_create(&tid, &attr, poll_registers, self.thread_args) != 0:
             # cleans up
             self.stop_utilisation_polling()
             raise OSError("Poll thread failed to start")
 
@@ -383,31 +392,36 @@
         Raises:
             RuntimeError: if the thread was does not exist.
         Returns:
             Nothing returned.
         Extra information:
             This also frees all resources allocated for the thread.
         """
+        cdef:
+            timespec sleep_time
+        sleep_time.tv_nsec = 1_000_000
+        sleep_time.tv_sec = 0
+
         if not self.utilisation_polling:
             raise RuntimeError("Thread non-existent (never started or already stopped)")
         self.thread_args.desired_state = 0
         # wait for it to exit
         while self.thread_args.current_state != 0:
-            time.sleep(0.001)
+            nanosleep(&sleep_time, NULL)
         free(self.thread_args.results)
         free(self.thread_args)
         self.utilisation_polling = False
 
     cpdef object query_utilisation(self):
         """Queries utilisation of different GPU units
-        
+
         Params:
             No params.
         Raises:
-            RuntimeError: details of the error will be in the error message (see extra infomation).
+            RuntimeError: details of the error will be in the error message (see extra information).
         Returns:
             dict containing utilisations from 0 - 1 (float):
                 - "texture_addresser"
                 - "shader_export"
                 - "shader_interpolator"
                 - "scan_converter"
                 - "primitive_assembly"
@@ -443,209 +457,171 @@
             for bit, compare in COMPARE_BITS.items():
                 if gbrm_value & compare:
                     utilisation[bit] += 1
         return {k: v / self.thread_args.buffer_size for k, v in utilisation.items()}
 
     cdef object check_amdgpu_retcode(self, int retcode):
         if retcode != 0:
-            raise RuntimeError("Unknown query failure (an amdgpu call failed). This query may not be supported for this GPU.")
+            raise RuntimeError("Unknown query failure (an AMDGPU call failed). This query may not be supported for this GPU.")
 
     cpdef object query_max_clocks(self):
         """Queries max GPU clocks
-        
+
         Params:
             No params.
         Raises:
-            RuntimeError: if an error occurs when calling amdgpu methods.
+            RuntimeError: if an error occurs when calling AMDGPU methods.
         Returns:
             dict,
                 - "max_sclk": int, hertz
                 - "max_mclk": int, hertz
         """
         cdef:
             int multiplier = 1000
             amdgpu_cy.amdgpu_gpu_info gpu_info_struct
         self.check_amdgpu_retcode(amdgpu_cy.amdgpu_query_gpu_info(self.device_handle, &gpu_info_struct))
         return {k: v * multiplier for k, v in dict(sclk_max=gpu_info_struct.max_engine_clk,
                                                    mclk_max=gpu_info_struct.max_memory_clk).items()}
 
     cpdef object query_vram_usage(self):
         """Queries VRAM usage
-        
+
         Params:
             No params.
         Raises:
-            RuntimeError: if an error occurs when calling amdgpu methods.
+            RuntimeError: if an error occurs when calling AMDGPU methods.
         Returns:
             int, usage in bytes.
         """
         cdef:
             unsigned long long out = 0
             int multiplier = 1
         self.check_amdgpu_retcode(query_info(self.device_handle, amdgpu_cy.AMDGPU_INFO_VRAM_USAGE, &out))
         return out * multiplier
 
     cpdef object query_gtt_usage(self):
         """Queries GTT usage
-        
+
         Params:
             No params.
         Raises:
-            RuntimeError: if an error occurs when calling amdgpu methods.
+            RuntimeError: if an error occurs when calling AMDGPU methods.
         Returns:
             int, usage in bytes.
         """
         cdef:
             unsigned long long out = 0
             int multiplier = 1
         self.check_amdgpu_retcode(query_info(self.device_handle, amdgpu_cy.AMDGPU_INFO_GTT_USAGE, &out))
         return out * multiplier
-    
+
     cpdef object query_sclk(self):
         """Queries shader (core) clock
-        
+
         Params:
             No params.
         Raises:
-            RuntimeError: if an error occurs when calling amdgpu methods.
+            RuntimeError: if an error occurs when calling AMDGPU methods.
         Returns:
             int, shader clock in hertz.
         """
         cdef:
             unsigned long long out = 0
             int multiplier = 1000000
         self.check_amdgpu_retcode(query_sensor(self.device_handle, amdgpu_cy.AMDGPU_INFO_SENSOR_GFX_SCLK, &out))
         return out * multiplier
-    
+
     cpdef object query_mclk(self):
         """Queries memory clock
-        
+
         Params:
             No params.
         Raises:
-            RuntimeError: if an error occurs when calling amdgpu methods.
+            RuntimeError: if an error occurs when calling AMDGPU methods.
         Returns:
             int, memory clock in hertz.
         """
         cdef:
             unsigned long long out = 0
             int multiplier = 1000000
         self.check_amdgpu_retcode(query_sensor(self.device_handle, amdgpu_cy.AMDGPU_INFO_SENSOR_GFX_MCLK, &out))
         return out * multiplier
 
     cpdef object query_temperature(self):
         """Queries temperature
-        
+
         Params:
             No params.
         Raises:
-            RuntimeError: if an error occurs when calling amdgpu methods.
+            RuntimeError: if an error occurs when calling AMDGPU methods.
         Returns:
             float, temperature in °C.
         """
         cdef:
             unsigned long long out = 0
             double multiplier = 0.001
         self.check_amdgpu_retcode(query_sensor(self.device_handle, amdgpu_cy.AMDGPU_INFO_SENSOR_GPU_TEMP, &out))
         return out * multiplier
 
     cpdef object query_load(self):
         """Queries overall GPU load
-        
+
         Params:
             No params.
         Raises:
-            RuntimeError: if an error occurs when calling amdgpu methods.
+            RuntimeError: if an error occurs when calling AMDGPU methods.
         Returns:
             float, value between 0 and 1.
         """
         cdef:
             unsigned long long out = 0
             double multiplier = 0.01
         self.check_amdgpu_retcode(query_sensor(self.device_handle, amdgpu_cy.AMDGPU_INFO_SENSOR_GPU_LOAD, &out))
         return out * multiplier
 
     cpdef object query_power(self):
         """Queries power consumption
-        
+
         Params:
             No params.
         Raises:
-            RuntimeError: if an error occurs when calling amdgpu methods.
+            RuntimeError: if an error occurs when calling AMDGPU methods.
         Returns:
             int, consumption in W.
         """
         cdef:
             unsigned long long out = 0
             int multiplier = 1
         self.check_amdgpu_retcode(query_sensor(self.device_handle, amdgpu_cy.AMDGPU_INFO_SENSOR_GPU_AVG_POWER, &out))
         return out * multiplier
 
     cpdef object query_northbridge_voltage(self):
         """Queries northbridge voltage
-        
+
         Params:
             No params.
         Raises:
-            RuntimeError: if an error occurs when calling amdgpu methods.
+            RuntimeError: if an error occurs when calling AMDGPU methods.
         Returns:
             float, voltage in V.
         """
         cdef:
             unsigned long long out = 0
             double multiplier = 0.001
         self.check_amdgpu_retcode(query_sensor(self.device_handle, amdgpu_cy.AMDGPU_INFO_SENSOR_VDDNB, &out))
         return out * multiplier
-    
+
     cpdef object query_graphics_voltage(self):
         """Queries graphics voltage
-        
+
         Params:
             No params.
         Raises:
-            RuntimeError: if an error occurs when calling amdgpu methods.
+            RuntimeError: if an error occurs when calling AMDGPU methods.
         Returns:
             float, voltage in V.
         """
         cdef:
             unsigned long long out = 0
             double multiplier = 0.001
         self.check_amdgpu_retcode(query_sensor(self.device_handle, amdgpu_cy.AMDGPU_INFO_SENSOR_VDDGFX, &out))
         return out * multiplier
-    
-
-    # THESE ARE UNSUPPORTED AS OF NOW DUE TO THESE REQUIRING RECENT libdrm
-    # THESE ARE ALSO UNTESTED AND PROBABLY DO NOT WORK
-
-
-    # cpdef object query_sclk_pstate(self):
-    #     """Queries shader (core) pstate
-        
-    #     Params:
-    #         No params.
-    #     Raises:
-    #         RuntimeError: if an error occurs when calling amdgpu methods.
-    #     Returns:
-    #         int, pstate.
-    #     """
-    #     cdef:
-    #         unsigned long long out = 0
-    #         int multiplier = 1
-    #     self.check_amdgpu_retcode(query_sensor(self.device_handle, amdgpu_cy.AMDGPU_INFO_SENSOR_STABLE_PSTATE_GFX_SCLK, &out))
-    #     return out * multiplier
-
-    # cpdef object query_mclk_pstate(self):
-    #     """Queries memory pstate
-        
-    #     Params:
-    #         No params.
-    #     Raises:
-    #         RuntimeError: if an error occurs when calling amdgpu methods.
-    #     Returns:
-    #         int, pstate.
-    #     """
-    #     cdef:
-    #         unsigned long long out = 0
-    #         int multiplier = 1
-    #     self.check_amdgpu_retcode(query_sensor(self.device_handle, amdgpu_cy.AMDGPU_INFO_SENSOR_STABLE_PSTATE_GFX_MCLK, &out))
-    #     return out * multiplier
-
```

### Comparing `pyamdgpuinfo-2.1.2/pyamdgpuinfo.egg-info/PKG-INFO` & `pyamdgpuinfo-2.1.3/pyamdgpuinfo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 Metadata-Version: 2.1
 Name: pyamdgpuinfo
-Version: 2.1.2
+Version: 2.1.3
 Summary: AMD GPU stats
 Home-page: https://github.com/mark9064/pyamdgpuinfo
 Author: mark9064
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Cython
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Development Status :: 4 - Beta
 Classifier: Natural Language :: English
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # pyamdgpuinfo
 
 AMD GPU information
 
 ## Install
 
-`pip3 install pyamdgpuinfo`
+`pip install pyamdgpuinfo`
 
-Only linux is supported, using the amdgpu driver.
+Only Linux is supported, using the AMDGPU driver.
 
-Precompiled wheels for python 3.6, 3.7, 3.8, 3.9 and 3.10 are the default method of install. This means that you don't need cython or any other dependencies to install it normally.
+The library is written using Cython, meaning that Cython and and a C compiler are needed to build and install from source. Additionally, libdrm development headers are required. 
 
-The library is written using cython, meaning that cython and and a C compiler are needed to build and install from source. Additionally, libdrm development headers are needed. 
+Precompiled wheels for Python 3.7-3.10 are the default method of install. This means that you don't need Cython or any other dependencies to install it normally.
 
 ## Usage
 
 Example:
 ```python
 >>> import pyamdgpuinfo
 >>> n_devices = pyamdgpuinfo.detect_gpus()
@@ -57,15 +58,15 @@
 * query_sclk - Queries shader (core) clock
 * query_mclk - Queries memory clock
 * query_vram_usage - Queries VRAM usage
 * query_gtt_usage - Queries GTT usage
 * query_temperature - Queries temperature
 * query_load - Queries GPU load
 * query_power - Queries power consumption
-* query_northbridge_voltage - Queries northbrige voltage
+* query_northbridge_voltage - Queries northbridge voltage
 * query_graphics_voltage - Queries graphics voltage
 
 
 VRAM and GTT sizes are available as an attribute of GPUInfo.
 
 ## Mentions
```

### Comparing `pyamdgpuinfo-2.1.2/setup.py` & `pyamdgpuinfo-2.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,26 +2,27 @@
 import setuptools
 from distutils.extension import Extension
 from Cython.Build import cythonize
 
 with open("README.md", "r") as fh:
     LONG_DESCRIPTION = fh.read()
 
-EXTENSIONS = [Extension(name="pyamdgpuinfo.pyamdgpuinfo", sources=["pyamdgpuinfo/pyamdgpuinfo.pyx"],
+EXTENSIONS = [Extension(name="pyamdgpuinfo._pyamdgpuinfo", sources=["pyamdgpuinfo/_pyamdgpuinfo.pyx"],
                         include_dirs=["/usr/include/libdrm"], libraries=["drm_amdgpu"])]
 
 setuptools.setup(
     name="pyamdgpuinfo",
-    version="2.1.2",
+    version="2.1.3",
     author="mark9064",
     description="AMD GPU stats",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/mark9064/pyamdgpuinfo",
     packages=setuptools.find_packages(),
+    python_requires='>=3.7',
     ext_modules=cythonize(EXTENSIONS, language_level=3),
     zip_safe=False,
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Cython",
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Operating System :: POSIX :: Linux",
```

