# Comparing `tmp/tritondse-0.1.2.tar.gz` & `tmp/tritondse-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tritondse-0.1.2.tar", last modified: Tue Apr 25 05:15:22 2023, max compression
+gzip compressed data, was "tritondse-0.1.3.tar", last modified: Tue May 16 08:02:40 2023, max compression
```

## Comparing `tritondse-0.1.2.tar` & `tritondse-0.1.3.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:15:22.614865 tritondse-0.1.2/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11357 2023-04-25 05:15:20.000000 tritondse-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-25 05:15:22.614865 tritondse-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-04-25 05:15:20.000000 tritondse-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 05:15:22.614865 tritondse-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-25 05:15:20.000000 tritondse-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:15:22.614865 tritondse-0.1.2/tritondse/
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/arch.py
--rw-r--r--   0 runner    (1001) docker     (123)    36095 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    29656 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/heap_allocator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:15:22.614865 tritondse-0.1.2/tritondse/loaders/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7346 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/loaders/cle_loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/loaders/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/loaders/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/loaders/quokkaprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)    22801 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/memory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:15:22.614865 tritondse-0.1.2/tritondse/probes/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/probes/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/probes/basic_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    50567 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/process_state.py
--rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/qbdi_trace.py
--rw-r--r--   0 runner    (1001) docker     (123)    73739 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/routines.py
--rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/sanitizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/seeds_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    35783 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/symbolic_executor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/symbolic_explorator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/thread_context.py
--rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/worklist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-04-25 05:15:20.000000 tritondse-0.1.2/tritondse/workspace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 05:15:22.614865 tritondse-0.1.2/tritondse.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-04-25 05:15:22.000000 tritondse-0.1.2/tritondse.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-04-25 05:15:22.000000 tritondse-0.1.2/tritondse.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 05:15:22.000000 tritondse-0.1.2/tritondse.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 05:15:22.000000 tritondse-0.1.2/tritondse.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-25 05:15:22.000000 tritondse-0.1.2/tritondse.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:02:40.786338 tritondse-0.1.3/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11357 2023-05-16 08:02:33.000000 tritondse-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-16 08:02:40.786338 tritondse-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2613 2023-05-16 08:02:33.000000 tritondse-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 08:02:40.786338 tritondse-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-16 08:02:33.000000 tritondse-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:02:40.786338 tritondse-0.1.3/tritondse/
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4986 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/arch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36097 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8020 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29656 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4605 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/heap_allocator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:02:40.786338 tritondse-0.1.3/tritondse/loaders/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/loaders/cle_loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6381 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/loaders/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9260 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/loaders/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4297 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/loaders/quokkaprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22801 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/memory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:02:40.786338 tritondse-0.1.3/tritondse/probes/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/probes/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/probes/basic_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50962 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/process_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/qbdi_trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)    75538 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/routines.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12351 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/sanitizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9055 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18501 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/seeds_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35948 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/symbolic_executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/symbolic_explorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/thread_context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6881 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6149 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11555 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/worklist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-05-16 08:02:33.000000 tritondse-0.1.3/tritondse/workspace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 08:02:40.786338 tritondse-0.1.3/tritondse.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3202 2023-05-16 08:02:40.000000 tritondse-0.1.3/tritondse.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-16 08:02:40.000000 tritondse-0.1.3/tritondse.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 08:02:40.000000 tritondse-0.1.3/tritondse.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 08:02:40.000000 tritondse-0.1.3/tritondse.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-16 08:02:40.000000 tritondse-0.1.3/tritondse.egg-info/top_level.txt
```

### Comparing `tritondse-0.1.2/LICENSE` & `tritondse-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/PKG-INFO` & `tritondse-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritondse
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library of Dynamic Symbolic Exploration based the Triton library
 Home-page: https://github.com/quarkslab/tritondse
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/tritondse/
 Project-URL: Bug Tracker, https://github.com/quarkslab/tritondse/issues
 Project-URL: Source, https://github.com/quarkslab/tritondse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tritondse Version: 0.1.2 Summary: A library of
+Metadata-Version: 2.1 Name: tritondse Version: 0.1.3 Summary: A library of
 Dynamic Symbolic Exploration based the Triton library Home-page: https://
 github.com/quarkslab/tritondse Author: Quarkslab License: AGPL-3.0 Project-URL:
 Documentation, https://quarkslab.github.io/tritondse/ Project-URL: Bug Tracker,
 https://github.com/quarkslab/tritondse/issues Project-URL: Source, https://
 github.com/quarkslab/tritondse Classifier: Topic :: Security Classifier:
 Environment :: Console Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # TritonDSE
```

### Comparing `tritondse-0.1.2/README.md` & `tritondse-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/setup.py` & `tritondse-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 with open("README.md") as f:
     README = f.read()
 
 
 setup(
     name="tritondse",
-    version="0.1.2",
+    version="0.1.3",
     description="A library of Dynamic Symbolic Exploration based the Triton library",
     packages=find_packages(),
     long_description=README,
     long_description_content_type='text/markdown',
     url="https://github.com/quarkslab/tritondse",
     project_urls={
         "Documentation": "https://quarkslab.github.io/tritondse/",
```

### Comparing `tritondse-0.1.2/tritondse/__init__.py` & `tritondse-0.1.3/tritondse/__init__.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/arch.py` & `tritondse-0.1.3/tritondse/arch.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,21 +4,33 @@
 
 # third-party module
 from triton import OPCODE, TritonContext
 
 # local imports
 from tritondse.types import Architecture, Addr
 
-Arch = namedtuple("Arch", "ret_reg pc_reg bp_reg sp_reg sys_reg reg_args halt_inst")
+Arch = namedtuple("Arch", "ret_reg pc_reg bp_reg sp_reg sys_reg reg_args halt_inst syscall_inst")
 
 ARCHS = {
-    Architecture.X86:     Arch('eax', 'eip', 'ebp', 'esp', 'eax', [], OPCODE.X86.HLT),
-    Architecture.X86_64:  Arch('rax', 'rip', 'rbp', 'rsp', 'rax', ['rdi', 'rsi', 'rdx', 'rcx', 'r8', 'r9'], OPCODE.X86.HLT),
-    Architecture.AARCH64: Arch('x0', 'pc', 'sp', 'sp', 'x8', ['x0', 'x1', 'x2', 'x3', 'x4', 'x5', 'x6', 'x7'], OPCODE.AARCH64.HLT),
-    Architecture.ARM32:   Arch('r0', 'pc', 'r11', 'sp', 'r7', ['r0', 'r1', 'r2', 'r3'], OPCODE.AARCH64.HLT)
+    Architecture.X86:     Arch('eax', 'eip', 'ebp', 'esp', 'eax',
+                               [],
+                               OPCODE.X86.HLT,
+                               [OPCODE.X86.SYSCALL, OPCODE.X86.SYSENTER]),  # ignore int 80
+    Architecture.X86_64:  Arch('rax', 'rip', 'rbp', 'rsp', 'rax',
+                               ['rdi', 'rsi', 'rdx', 'rcx', 'r8', 'r9'],
+                               OPCODE.X86.HLT,
+                               [OPCODE.X86.SYSCALL, OPCODE.X86.SYSENTER]),  # ignore int 80
+    Architecture.AARCH64: Arch('x0', 'pc', 'sp', 'sp', 'x8',
+                               ['x0', 'x1', 'x2', 'x3', 'x4', 'x5', 'x6', 'x7'],
+                               OPCODE.AARCH64.HLT,
+                               [OPCODE.AARCH64.SVC]),
+    Architecture.ARM32:   Arch('r0', 'pc', 'r11', 'sp', 'r7',
+                               ['r0', 'r1', 'r2', 'r3'],
+                               OPCODE.ARM32.HLT,
+                               [OPCODE.ARM32.SVC])
 }
 
 
 class CpuState(dict):
     """
     Thin wrapper on a TritonContext, to allow accessing
     and modifying registers in a Pythonic way. It also
```

### Comparing `tritondse-0.1.2/tritondse/callbacks.py` & `tritondse-0.1.3/tritondse/callbacks.py`

 * *Files 0% similar despite different names*

```diff
@@ -241,15 +241,15 @@
                 for fname in list(self._func_to_register):
                     cbs = self._func_to_register.pop(fname)
                     addr = se.loader.find_function_addr(fname)
                     if addr:
                         for cb in cbs:
                             self.register_pre_addr_callback(addr, cb)
                     else:
-                        logging.warning(f"can't find function {fname} in {se.loader}")
+                        logging.warning(f"can't find function '{fname}' in {se.loader}")
             else:
                 logging.warning(f"function callback to resolve but no program provided")
 
 
     def register_addr_callback(self, pos: CbPos, addr: Addr, callback: AddrCallback) -> None:
         """
         Register a callback function on a given address before or after the execution
```

### Comparing `tritondse-0.1.2/tritondse/config.py` & `tritondse-0.1.3/tritondse/config.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/coverage.py` & `tritondse-0.1.3/tritondse/coverage.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/exception.py` & `tritondse-0.1.3/tritondse/exception.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/heap_allocator.py` & `tritondse-0.1.3/tritondse/heap_allocator.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/loaders/cle_loader.py` & `tritondse-0.1.3/tritondse/loaders/cle_loader.py`

 * *Files 10% similar despite different names*

```diff
@@ -157,22 +157,35 @@
         for obj in self.ld.all_objects:
             for (resolver_func, got_rva) in obj.irelatives:
                 got_slot = got_rva + obj.mapped_base
                 sym = self.ld.find_symbol(resolver_func)
                 if sym is None:
                     continue
                 fun = sym.name
-                yield fun, got_slot
+                if fun in SUPPORTED_ROUTINES:
+                    yield fun, got_slot
 
     def imported_variable_symbols_relocations(self) -> Generator[Tuple[str, Addr], None, None]:
         """
         Iterate over all imported variable symbols. Yield for each of them the name and
         the relocation address in the binary.
 
         :return: Generator of tuples with symbol name, relocation address
         """
         # TODO I think there's a problem here. We only deal with imports from the main binary
         for s in self.ld.main_object.symbols:
             if s.resolved and s._type == cle.SymbolType.TYPE_OBJECT:
                 logging.debug(f"CleLoader: hooking symbol {s.name} @ {s.relative_addr:#x} {s.resolved} {s.resolvedby} {s._type}")
                 s_addr = s.relative_addr + self.ld.main_object.mapped_base
                 yield s.name, s_addr
+
+    def find_function_addr(self, name: str) -> Optional[Addr]:
+        """
+        Search for the function name in fonctions of the binary.
+
+        :param name: Function name
+        :type name: str
+        :return: Address of function if found
+        :rtype: Addr
+        """
+        res = [x for x in self.ld.find_all_symbols(name) if x.is_function]
+        return res[0].rebased_addr if res else None  # if multiple elements return the first
```

### Comparing `tritondse-0.1.2/tritondse/loaders/loader.py` & `tritondse-0.1.3/tritondse/loaders/loader.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/loaders/program.py` & `tritondse-0.1.3/tritondse/loaders/program.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/loaders/quokkaprogram.py` & `tritondse-0.1.3/tritondse/loaders/quokkaprogram.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/memory.py` & `tritondse-0.1.3/tritondse/memory.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/probes/basic_trace.py` & `tritondse-0.1.3/tritondse/probes/basic_trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/process_state.py` & `tritondse-0.1.3/tritondse/process_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -460,22 +460,29 @@
         :type ptr: :py:obj:`tritondse.types.Addr`
         :return: True if pointer points to the heap area *(allocated or not)*.
         """
         if self.BASE_HEAP <= ptr < self.END_HEAP:
             return True
         return False
 
-    def fetch_instruction(self, address: Addr = None) -> Instruction:
+    def is_syscall(self) -> bool:
+        """
+        Check whether the current instrution fetched is a syscall or not.
+        """
+        return bool(self.current_instruction.getType() in self._archinfo.syscall_inst)
+
+    def fetch_instruction(self, address: Addr = None, set_as_current: bool = True) -> Instruction:
         """
         Fetch the instruction at the given address. If no address
         is specified the current program counter one is used.
 
         :raise MemoryAccessViolation: If the instruction cannot be fetched in the memory.
 
         :param address: address where to get the instruction from
+        :param set_as_current: set as the current instruction in the process state
         :return: instruction disassembled
         """
         if address is None:
             address = self.cpu.program_counter
         with self.memory.without_segmentation(disable_callbacks=True):
             data = self.memory.read(address, 16)
         i = Instruction(address, data)
@@ -483,14 +490,16 @@
         self.tt_ctx.disassembly(i)  # This needs to be done before using i.getSize()
                                     # otherwise, i.getSize() will always be 16
         map = self.memory.get_map(address, i.getSize())
         if map is None:
             raise MemoryAccessViolation(address, Perm.X, memory_not_mapped=True)
         if Perm.X not in map.perm:  # Note: in this model we can execute code in non-readable pages
             raise MemoryAccessViolation(address, Perm.X, map_perm=map.perm, perm_error=True)
+        if set_as_current:
+            self.__current_inst = i
         return i
 
     def process_instruction(self, instruction: Instruction) -> bool:
         """
         Process the given triton instruction on this process state.
 
         :param instruction: Triton Instruction object
```

### Comparing `tritondse-0.1.2/tritondse/qbdi_trace.py` & `tritondse-0.1.3/tritondse/qbdi_trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/routines.py` & `tritondse-0.1.3/tritondse/routines.py`

 * *Files 2% similar despite different names*

```diff
@@ -181,16 +181,18 @@
     logging.debug(f"argc = {argc}")
 
     # Define argv
     addrs = list()
 
     if se.config.is_format_composite() and se.seed.content.argv: # Use the seed provided (and ignore config.program_argv !!)
         argvs = se.seed.content.argv
+        src = 'seed'
     else:  # use the config argv
         argvs = [x.encode("latin-1") for x in se.config.program_argv]  # Convert it from str to bytes
+        src = 'config'
 
     # Compute the allocation size: size of strings, + all \x00 + all pointers
     size = sum(len(x) for x in argvs)+len(argvs)+len(argvs)*pstate.ptr_size
     if size == 0:  # Falback on a single pointer that will hold not even be initialized
         size = pstate.ptr_size
 
     # We put the ARGV stuff on the heap even though its normally on stack
@@ -201,15 +203,15 @@
         pstate.memory.write(base, arg + b'\x00')
 
         if se.config.is_format_composite() and se.seed.content.argv: # Use the seed provided (and ignore config.program_argv !!)
             # Symbolize the argv string
             se.inject_symbolic_argv_memory(base, i, arg)
             # FIXME: Shall add a constraint on every char to be != \x00
 
-        logging.debug(f"argv[{i}] = {repr(pstate.memory.read(base, len(arg)))}")
+        logging.debug(f"({src}) argv[{i}] = {repr(pstate.memory.read(base, len(arg)))}")
         base += len(arg) + 1
 
 
     # NOTE: the array of pointers will be after the string themselves
     b_argv = base
     for addr in addrs:
         pstate.memory.write_ptr(base, addr)
@@ -573,14 +575,15 @@
     # Concretize the whole path name
     pstate.concretize_memory_bytes(arg0, len(arg0s)+1)  # Concretize the whole string + \0
 
     # We use mode as concrete value
     pstate.concretize_argument(1)
 
     if se.seed.is_file_defined(arg0s):
+        logging.info(f"opening an input file: {arg0s}")
         # Program is opening an input
         data = se.seed.get_file_input(arg0s)
         filedesc = pstate.create_file_descriptor(arg0s, io.BytesIO(data))
         return filedesc.id
     else:
         # Try to open it as a regular file
         try:
@@ -889,14 +892,62 @@
     size = pstate.get_argument_value(0)
     ptr = pstate.heap_allocator.alloc(size)
 
     # Return value
     return ptr
 
 
+def rtn_open(se: 'SymbolicExecutor', pstate: 'ProcessState'):
+    """
+    The open behavior.
+    """
+    logging.debug('open hooked')
+
+    # Get arguments
+    arg0 = pstate.get_argument_value(0)  # const char *pathname
+    flags = pstate.get_argument_value(1)  # int flags
+    mode = pstate.get_argument_value(2)  # we ignore it
+    arg0s = pstate.memory.read_string(arg0)
+
+    # Concretize the whole path name
+    pstate.concretize_memory_bytes(arg0, len(arg0s)+1)  # Concretize the whole string + \0
+
+    # We use flags as concrete value
+    pstate.concretize_argument(1)
+
+    # Use the flags to open the file in the write mode.
+    mode = ""
+    if (flags & 0xFF) == 0x00:   # O_RDONLY
+        mode = "r"
+    elif (flags & 0xFF) == 0x01: # O_WRONLY
+        mode = "w"
+    elif (flags & 0xFF) == 0x02: # O_RDWR
+        mode = "r+"
+
+    if flags & 0x0100: # O_CREAT
+        mode += "x"
+    if flags & 0x0200: # O_APPEND
+        mode = "a"  # replace completely value
+
+    if se.seed.is_file_defined(arg0s) and "r" in mode:  # input file and opened in reading
+        logging.info(f"opening an input file: {arg0s}")
+        # Program is opening an input
+        data = se.seed.get_file_input(arg0s)
+        filedesc = pstate.create_file_descriptor(arg0s, io.BytesIO(data))
+        return filedesc.id
+    else:
+        # Try to open it as a regular file
+        try:
+            fd = open(arg0s, mode)  # use the mode here
+            filedesc = pstate.create_file_descriptor(arg0s, fd)
+            return filedesc.id
+        except Exception as e:
+            logging.debug(f"Failed to open {arg0s} {e}")
+            return pstate.minus_one
+
 def rtn_realloc(se: 'SymbolicExecutor', pstate: 'ProcessState'):
     """
     The realloc behavior.
     """
     logging.debug('realloc hooked')
 
     # Get arguments
@@ -1285,15 +1336,15 @@
             if se.seed.is_raw() and se.seed.is_bootstrap_seed() and not data:
                 data = b'\x00' * size
 
             if len(data) == size:  # if `size` limited the fgets its an indirect constraint
                 pstate.push_constraint(size_ast.getAst() == size)
 
             se.inject_symbolic_file_memory(buff, filedesc.name, data, offset)
-            logging.debug(f"read in {filedesc.name} = {repr(data)}")
+            logging.debug(f"read in (input) {filedesc.name} = {repr(data)}")
         else:
             pstate.concretize_argument(2)
             pstate.memory.write(buff, data)
 
         return len(data)
     else:
         logging.warning(f'File descriptor ({fd}) not found')
@@ -2164,14 +2215,15 @@
     'gettimeofday':            rtn_gettimeofday,
     'malloc':                  rtn_malloc,
     'memcmp':                  rtn_memcmp,
     'memcpy':                  rtn_memcpy,
     'memmem':                  rtn_memmem,
     'memmove':                 rtn_memmove,
     'memset':                  rtn_memset,
+    'open':                    rtn_open,
     'printf':                  rtn_printf,
     'pthread_create':          rtn_pthread_create,
     'pthread_exit':            rtn_pthread_exit,
     'pthread_join':            rtn_pthread_join,
     'pthread_mutex_destroy':   rtn_pthread_mutex_destroy,
     'pthread_mutex_init':      rtn_pthread_mutex_init,
     'pthread_mutex_lock':      rtn_pthread_mutex_lock,
```

### Comparing `tritondse-0.1.2/tritondse/sanitizers.py` & `tritondse-0.1.3/tritondse/sanitizers.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/seed.py` & `tritondse-0.1.3/tritondse/seed.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/seeds_manager.py` & `tritondse-0.1.3/tritondse/seeds_manager.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/symbolic_executor.py` & `tritondse-0.1.3/tritondse/symbolic_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,14 +300,17 @@
                 # Trigger pre-instruction callback
                 pre_insts, post_insts = self.cbm.get_instruction_callbacks()
                 for cb in pre_insts:
                     cb(self, self.pstate, instruction)
             except SkipInstructionException as _:
                 continue
 
+            if self.pstate.is_syscall():
+                logging.warning(f"execute syscall instruction {self.pstate.read_register(self.pstate._syscall_register)}")
+
             # Process
             prev_pc = self.current_pc
             self._in_processing = True
             if not self.pstate.process_instruction(instruction):
                 if self.pstate.is_halt_instruction():
                     logging.info(f"hit {str(instruction)} instruction stop.")
                 else:
```

### Comparing `tritondse-0.1.2/tritondse/symbolic_explorator.py` & `tritondse-0.1.3/tritondse/symbolic_explorator.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/thread_context.py` & `tritondse-0.1.3/tritondse/thread_context.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/trace.py` & `tritondse-0.1.3/tritondse/trace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/types.py` & `tritondse-0.1.3/tritondse/types.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/worklist.py` & `tritondse-0.1.3/tritondse/worklist.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse/workspace.py` & `tritondse-0.1.3/tritondse/workspace.py`

 * *Files identical despite different names*

### Comparing `tritondse-0.1.2/tritondse.egg-info/PKG-INFO` & `tritondse-0.1.3/tritondse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tritondse
-Version: 0.1.2
+Version: 0.1.3
 Summary: A library of Dynamic Symbolic Exploration based the Triton library
 Home-page: https://github.com/quarkslab/tritondse
 Author: Quarkslab
 License: AGPL-3.0
 Project-URL: Documentation, https://quarkslab.github.io/tritondse/
 Project-URL: Bug Tracker, https://github.com/quarkslab/tritondse/issues
 Project-URL: Source, https://github.com/quarkslab/tritondse
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tritondse Version: 0.1.2 Summary: A library of
+Metadata-Version: 2.1 Name: tritondse Version: 0.1.3 Summary: A library of
 Dynamic Symbolic Exploration based the Triton library Home-page: https://
 github.com/quarkslab/tritondse Author: Quarkslab License: AGPL-3.0 Project-URL:
 Documentation, https://quarkslab.github.io/tritondse/ Project-URL: Bug Tracker,
 https://github.com/quarkslab/tritondse/issues Project-URL: Source, https://
 github.com/quarkslab/tritondse Classifier: Topic :: Security Classifier:
 Environment :: Console Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown License-File: LICENSE # TritonDSE
```

### Comparing `tritondse-0.1.2/tritondse.egg-info/SOURCES.txt` & `tritondse-0.1.3/tritondse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

