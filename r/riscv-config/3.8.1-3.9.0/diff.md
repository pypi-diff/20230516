# Comparing `tmp/riscv_config-3.8.1.tar.gz` & `tmp/riscv_config-3.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/riscv_config-3.8.1.tar", last modified: Tue Apr 25 10:52:37 2023, max compression
+gzip compressed data, was "dist/riscv_config-3.9.0.tar", last modified: Tue May 16 12:59:35 2023, max compression
```

## Comparing `riscv_config-3.8.1.tar` & `riscv_config-3.9.0.tar`

### file list

```diff
@@ -1,27 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:52:37.000000 riscv_config-3.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-04-25 10:52:09.000000 riscv_config-3.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-25 10:52:37.000000 riscv_config-3.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-25 10:52:09.000000 riscv_config-3.8.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:52:37.000000 riscv_config-3.8.1/riscv_config/
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    93762 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/isa_validator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    16744 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/schemaValidator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:52:37.000000 riscv_config-3.8.1/riscv_config/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    60390 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/schemas/schema_debug.yaml
--rw-r--r--   0 runner    (1001) docker     (123)   551237 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/schemas/schema_isa.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/schemas/schema_platform.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    31975 2023-04-25 10:52:09.000000 riscv_config-3.8.1/riscv_config/warl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 10:52:37.000000 riscv_config-3.8.1/riscv_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-04-25 10:52:36.000000 riscv_config-3.8.1/riscv_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-04-25 10:52:36.000000 riscv_config-3.8.1/riscv_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 10:52:36.000000 riscv_config-3.8.1/riscv_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-25 10:52:36.000000 riscv_config-3.8.1/riscv_config.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 10:52:36.000000 riscv_config-3.8.1/riscv_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-25 10:52:36.000000 riscv_config-3.8.1/riscv_config.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-04-25 10:52:37.000000 riscv_config-3.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-04-25 10:52:09.000000 riscv_config-3.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:59:35.000000 riscv_config-3.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-16 12:59:06.000000 riscv_config-3.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-16 12:59:35.000000 riscv_config-3.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-16 12:59:06.000000 riscv_config-3.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config/
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    96921 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7090 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/isa_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16423 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/schemaValidator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     5165 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/schemas/schema_custom.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    60390 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/schemas/schema_debug.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)   551237 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/schemas/schema_isa.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/schemas/schema_platform.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36995 2023-05-16 12:59:06.000000 riscv_config-3.9.0/riscv_config/warl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-16 12:59:35.000000 riscv_config-3.9.0/riscv_config.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-16 12:59:35.000000 riscv_config-3.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-05-16 12:59:06.000000 riscv_config-3.9.0/setup.py
```

### Comparing `riscv_config-3.8.1/riscv_config/checker.py` & `riscv_config-3.9.0/riscv_config/checker.py`

 * *Files 4% similar despite different names*

```diff
@@ -1167,14 +1167,16 @@
     return spec
         
 def check_fields(spec):
     errors = {} 
     for csr, node, in spec.items() :
          fault_node = node
          error=[]
+         if csr.startswith('uarch_'):
+             continue
          if node['rv32']['accessible']:
                 node['rv32']['fields'] = get_fields(node['rv32'], 32)
          if node['rv64']['accessible']:
                 node['rv64']['fields'] = get_fields(node['rv64'], 64)
          fields = list(set(['rv32', 'rv64', 'description', 'address', 'priv_mode', 'reset-val']) - set(node.keys()) )
          if fields:
             error.append("The fields " + "".join(fields) + " are missing")
@@ -1349,14 +1351,20 @@
     virtualization_possible = False
     if 'ro_constant' in satp_mode_type:
         if satp_mode_type['ro_constant'] == 0:
             virtualization_possible = False
         else:
             virtualization_possible = True
     elif 'warl' in satp_mode_type:
+        warl_inst = warl_class(satp_mode_type['warl'], 'satp::mode',63, 60)
+        for x in [1,2,3,4,5,6,7,11,12,13]:
+            err = warl_inst.islegal(x)
+            if not err:
+                errors.append(f'warl function for satp::mode accepts \
+"{x}" as a legal value - which is incorrect')
         warl_inst = warl_class(satp_mode_type['warl'], 'satp::mode', msb, lsb, spec)
         for x in virt_modes:
             err = warl_inst.islegal(x)
             if not err:
                 virtualization_possible = True
                 break
 
@@ -1469,14 +1477,17 @@
     return errors
 
 def check_warl_legality(spec, logging = False):
     errors = {}
     warlnodes = {}
     xlen = 64 if 64 in spec['supported_xlen'] else 32
     for csrname, csrnode in spec.items():
+        # don't perform any warl legality checks for uarch signal definitions.
+        if csrname == 'uarch_signals':
+            continue
         if isinstance(csrnode, dict) and 'priv_mode' in csrnode:
             if csrnode[f'rv{xlen}']['accessible']:
                 if 'indexing_reg' in csrnode:
                     for n in csrnode[f'rv{xlen}']['index_list']:
                         _csrname = f'{csrname}[{n["index_val"]}]'
                         if 'warl' in n['type'] and n['shadow'] is None:
                             warlnodes[_csrname] = {}
@@ -1743,56 +1754,26 @@
 
         normalized['ISA'] = isa_string
 
         if logging:
             logger.info(f' Updating fields node for each CSR')
         normalized = update_fields(normalized, logging)
 
-        if logging:
-            logger.info("Initiating WARL legality checks.")
-        errors = check_warl_legality(normalized, logging)
-        if errors:
-            raise ValidationError("Error in " + foo + ".", errors)
-
-        if logging:
-            logger.info("Initiating post processing and reset value checks.")
-        errors = check_reset(normalized, logging)
-        if errors:
-            raise ValidationError("Error in " + foo + ".", errors)
-        
-        if logging:
-            logger.info(f'Initiating validation checks for indexed csrs')
-        errors = check_indexing(normalized, logging)
-        if errors:
-            raise ValidationError("Error in " + foo + ".", errors)
-        
-        if logging:
-            logger.info(f'Initiating validation checks for trigger csrs')
-        errors = check_triggers(normalized, logging)
-        if errors:
-            raise ValidationError("Error in " + foo + ".", errors)
-
-        if logging:
-            logger.info(f'Initiating validation checks for shadow fields')
-        errors = check_shadows(normalized, logging)
-        if errors:
-            raise ValidationError("Error in " + foo + ".", errors)
-
         outyaml['hart'+str(x)] = trim(normalized)
     file_name = os.path.split(foo)
     file_name_split = file_name[1].split('.')
     output_filename = os.path.join(
         work_dir, file_name_split[0] + '_checked.' + file_name_split[1])
-    ifile = output_filename
+    dfile = output_filename
     outfile = open(output_filename, 'w')
     if logging:
         logger.info('Dumping out Normalized Checked YAML: ' + output_filename)
     utils.dump_yaml(outyaml, outfile, no_anchors )
-    return ifile
-    
+    return dfile
+
 def check_isa_specs(isa_spec,
                 work_dir,
                 logging=False,
                 no_anchors=False):
     '''
         Function to perform ensure that the isa and platform specifications confirm
         to their schemas. The :py:mod:`Cerberus` module is used to validate that the
@@ -1860,66 +1841,26 @@
         else:
             error_list = validator.errors
             raise ValidationError("Error in " + foo + ".", error_list)
         if logging:
             logger.info(f' Updating fields node for each CSR')
         normalized = update_fields(normalized, logging)
 
-        if logging:
-            logger.info("Initiating WARL legality checks.")
-        errors = check_warl_legality(normalized, logging)
-        if errors:
-            raise ValidationError("Error in " + foo + ".", errors)
-
-        if logging:
-            logger.info("Initiating post processing and reset value checks.")
-        errors = check_reset(normalized, logging)
-        if errors:
-            raise ValidationError("Error in " + foo + ".", errors)
-
-        if normalized['mhartid']['reset-val'] != x:
-            raise ValidationError('Error in ' + foo + ".", 
-                    {'mhartid': ['wrong reset-val of for hart'+str(x)]})
-
-        if logging:
-            logger.info(f'Initiating validation checks for indexed csrs')
-        errors = check_indexing(normalized, logging)
-        if errors:
-            raise ValidationError("Error in " + foo + ".", errors)
-
-        if logging:
-            logger.info(f'Initiating validation checks for shadow fields')
-        errors = check_shadows(normalized, logging)
-        if errors:
-            raise ValidationError("Error in " + foo + ".", errors)
-
-        errors = check_mhpm(normalized, logging)
-        if errors:
-            raise ValidationError("Error in " + foo + ".", errors)
-
-        errors = check_pmp(normalized, logging)
-        if errors:
-            raise ValidationError("Error in " + foo + ".", errors) 
-
-        errors = check_supervisor(normalized, logging)
-        if errors:
-            raise ValidationError("Error in " + foo + ".", errors) 
-              
         outyaml['hart'+str(x)] = trim(normalized)
     file_name = os.path.split(foo)
     file_name_split = file_name[1].split('.')
     output_filename = os.path.join(
         work_dir, file_name_split[0] + '_checked.' + file_name_split[1])
     ifile = output_filename
     outfile = open(output_filename, 'w')
     if logging:
         logger.info('Dumping out Normalized Checked YAML: ' + output_filename)
     utils.dump_yaml(outyaml, outfile, no_anchors )
     return ifile
-    
+
 def check_custom_specs(custom_spec,
                 work_dir,
                 logging=False,
                 no_anchors=False):
     '''
         Function to perform ensure that the isa and platform specifications confirm
         to their schemas. The :py:mod:`Cerberus` module is used to validate that the
@@ -1944,20 +1885,32 @@
 
     foo = custom_spec
     
     # Load input YAML file
     if logging:
         logger.info('Loading input file: ' + str(foo))
     master_custom_yaml = utils.load_yaml(foo, no_anchors)
+    schema_yaml = utils.load_yaml(constants.custom_schema, no_anchors)
+    validator = schemaValidator(schema_yaml, xlen=[])
+    validator.allow_unknown = True
 
     outyaml = copy.deepcopy(master_custom_yaml)
+    normalized = {}
     for x in master_custom_yaml['hart_ids']:
         if logging:
             logger.info('Processing Hart: hart'+str(x))
         inp_yaml = master_custom_yaml['hart'+str(x)]
+        valid = validator.validate(inp_yaml)
+        if valid:
+            if logging:
+                logger.info('No errors for Hart: '+str(x) + ' :)')
+        else:
+            error_list = validator.errors
+            raise ValidationError("Error in " + foo + ".", error_list)
+        normalized[f'hart{x}'] = validator.normalized(inp_yaml, schema_yaml)
     errors = check_fields(inp_yaml)
     if errors:
             raise ValidationError("Error in " + foo + ".", errors)
     outyaml['hart'+str(x)] = trim(inp_yaml)
     file_name = os.path.split(foo)
     file_name_split = file_name[1].split('.')
     output_filename = os.path.join(
@@ -2017,7 +1970,132 @@
     pfile = output_filename
     outfile = open(output_filename, 'w')
     if logging:
         logger.info('Dumping out Normalized Checked YAML: ' + output_filename)
     utils.dump_yaml(trim(normalized), outfile, no_anchors)
 
     return pfile
+
+def check_csr_specs(ispec=None, customspec=None, dspec=None, pspec=None, work_dir=None, logging=False, no_anchors=True) -> list:
+    '''
+        Merge the isa, custom and debug CSR specs into a single CSR spec file.
+        Perform all warl checks on this merged CSR spec file.
+        This function needs to be called hart-wise.
+
+        :param ispec: The isa spec yaml. Defaults to None.
+        :param customspec: The custom spec yaml. Defaults to None.
+        :param dspec: The debug spec yaml. Defaults to None.
+        :param pspec: The platform spec yaml. Defaults to None.
+        :param work_dir: The working directory. Defaults to None.
+        :param logging: A boolean to indicate whether log is to be printed. Defaults to False.
+        :param no_anchors: A boolean to indicate whether anchors are not to be used. Defaults to True.
+
+        :type ispec: dict
+        :type customspec: dict
+        :type dspec: dict
+        :type pspec: dict
+        :type work_dir: str
+        :type logging: bool
+        :type no_anchors: bool
+
+        :return: List of validated CSR specs. Position holds 'None' if a certain spec was not passed.
+    '''
+
+    if ispec is not None:
+        isa_file = check_isa_specs(os.path.abspath(ispec), work_dir, logging, no_anchors)
+    else:
+        logger.error("ISA spec not passed. This is mandatory.")
+        isa_file = None
+        raise SystemExit
+
+    if customspec is not None:
+        custom_file = check_custom_specs(os.path.abspath(customspec), work_dir, logging, no_anchors)
+    else:
+        custom_file = None
+
+    if dspec is not None:
+        debug_file = check_debug_specs(os.path.abspath(dspec), ispec, work_dir, logging, no_anchors)
+    else:
+        debug_file = None
+
+    if pspec is not None:
+        platform_file = check_platform_specs(os.path.abspath(pspec), work_dir, logging, no_anchors)
+    else:
+        platform_file = None
+
+    specs_list = [isa_file, custom_file, debug_file, platform_file]
+
+    if logging:
+        logger.info("Initiating checks on all CSR specs.")
+
+    # merge the dicts ispec, customspec and dspec after loading the YAMLs into dicts
+    ispec_dict = utils.load_yaml(isa_file, no_anchors)
+    customspec_dict = utils.load_yaml(custom_file, no_anchors) if custom_file is not None else {}
+    dspec_dict = utils.load_yaml(debug_file, no_anchors) if debug_file is not None else {}
+
+    merged = {}
+    hart_ids = []
+    for entry in ispec_dict['hart_ids']:
+        hart_ids.append(entry)
+        merged[entry] = {}
+        merged[entry].update(ispec_dict['hart'+str(entry)])
+        merged[entry].update(customspec_dict['hart'+str(entry)])
+        merged[entry].update(dspec_dict['hart'+str(entry)])
+
+        try:
+            uarch_signals = merged[entry]['uarch_signals']
+        except KeyError as e:
+            logger.info("No uarch signals found for hart"+str(entry))
+            uarch_signals = {}
+
+    for entry in hart_ids:
+        csr_db = merged[entry]
+        if logging:
+            logger.info("Initiating WARL legality checks.")
+        errors = check_warl_legality(csr_db, logging)
+        if errors:
+            raise ValidationError("Error in csr definitions", errors)
+
+        errors = check_supervisor(csr_db, logging)
+        if errors:
+            raise ValidationError("Error in csr definitions", errors)
+
+        if logging:
+            logger.info("Initiating post processing and reset value checks.")
+        errors = check_reset(csr_db, logging)
+        if errors:
+            raise ValidationError("Error in csr definitions", errors)
+
+        if csr_db['mhartid']['reset-val'] != entry:
+            raise ValidationError('Error in csr definitions.',
+                    {'mhartid': ['wrong reset-val of for hart'+str(entry)]})
+
+        if logging:
+            logger.info(f'Initiating validation checks for indexed csrs')
+        errors = check_indexing(csr_db, logging)
+        if errors:
+            raise ValidationError("Error in csr definitions", errors)
+
+        if logging:
+            logger.info(f'Initiating validation checks for shadow fields')
+        errors = check_shadows(csr_db, logging)
+        if errors:
+            raise ValidationError("Error in csr definitions", errors)
+
+        errors = check_mhpm(csr_db, logging)
+        if errors:
+            raise ValidationError("Error in csr definitions", errors)
+
+        errors = check_pmp(csr_db, logging)
+        if errors:
+            raise ValidationError("Error in csr definitions", errors)
+
+        if logging:
+            logger.info(f'Initiating validation checks for trigger csrs')
+        errors = check_triggers(csr_db, logging)
+        if errors:
+            raise ValidationError("Error in csr definitions", errors)
+
+        if logging and not errors:
+            logger.info(f'All checks completed for hart{entry}. No errors found.')
+
+    return specs_list
```

### Comparing `riscv_config-3.8.1/riscv_config/constants.py` & `riscv_config-3.9.0/riscv_config/constants.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import re
 
 root = os.path.abspath(os.path.dirname(__file__))
 
 isa_schema = os.path.join(root, 'schemas/schema_isa.yaml')
 debug_schema = os.path.join(root, 'schemas/schema_debug.yaml')
 platform_schema = os.path.join(root, 'schemas/schema_platform.yaml')
+custom_schema = os.path.join(root, 'schemas/schema_custom.yaml')
 Zvl_extensions = [
         "Zvl32b", "Zvl64b", "Zvl128b", "Zvl256b", "Zve512b", "Zvl1024b"
 ]
 Zvef_extensions = [
         "Zve32f", "Zve64f"
 ]
 Zved_extensions = [
```

### Comparing `riscv_config-3.8.1/riscv_config/errors.py` & `riscv_config-3.9.0/riscv_config/errors.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.1/riscv_config/isa_validator.py` & `riscv_config-3.9.0/riscv_config/isa_validator.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.1/riscv_config/schemaValidator.py` & `riscv_config-3.9.0/riscv_config/schemaValidator.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,22 +38,15 @@
       if value and 'Smrnmi' not in extension_list:
         self._error(field,
                   "Register cannot be implemented without Smrnmi extension in ISA."
               )
 
     
     def _check_with_satp_modes64(self, field, value):
-
-        if 'warl' in value:
-            warl = warl_class(value['warl'], 'satp::mode',63, 60)
-            for x in [1,2,3,4,5,6,7,11,12,13]:
-                err = warl.islegal(x)
-                if not err:
-                    self._error(field, f'warl function for satp::mode accepts \
-"{x}" as a legal value - which is incorrect')
+        pass
 
     def _check_with_isa_xlen(self, field, value):
         global supported_xlen
         global isa_string
         if str(max(supported_xlen)) not in isa_string:
             self._error(field, 'XLEN in ISA and supported_xlen fields do not match')
```

### Comparing `riscv_config-3.8.1/riscv_config/schemas/schema_debug.yaml` & `riscv_config-3.9.0/riscv_config/schemas/schema_debug.yaml`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.1/riscv_config/schemas/schema_isa.yaml` & `riscv_config-3.9.0/riscv_config/schemas/schema_isa.yaml`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.1/riscv_config/schemas/schema_platform.yaml` & `riscv_config-3.9.0/riscv_config/schemas/schema_platform.yaml`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.1/riscv_config/utils.py` & `riscv_config-3.9.0/riscv_config/utils.py`

 * *Files identical despite different names*

### Comparing `riscv_config-3.8.1/riscv_config/warl.py` & `riscv_config-3.9.0/riscv_config/warl.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 import os
 import logging
 import riscv_config.utils as utils
 import textwrap
 import random
+import pprint as pp
 
 logger = logging.getLogger(__name__)
 
 class warl_class():
     """This is a class for handling various operations and checks for the WARL
     type of registers and/or subfields as defined by the riscv-config spec<TODO:
     link here>. While riscv-config remains to be the major user of this package,
@@ -51,17 +52,27 @@
         self.f_lsb = f_lsb
         self.bitlen = f_msb - f_lsb + 1
         self.maxval = (2**(self.bitlen))-1
         self.spec = spec
         self.regex_legal = re.compile('\[(.*?)\]\s*(bitmask|in|not in)\s*\[(.*?)\]')
         self.regex_dep_legal = re.compile('(?P<csrname>.*?)\s*\[(?P<indices>.*?)\]\s*(?P<op>in|not in.*?)\s*\[(?P<values>.*?)\]\s*')
         self.dependencies = node['dependency_fields']
+        self.uarch_depends = {'uarch_signals': []}
+        try:
+            if spec is not None:
+                self.uarch_signals = spec['uarch_signals']
+            else:
+                self.uarch_signals = {}
+        except KeyError:
+            logger.info(f'No uarch_signals found in spec.')
+            self.uarch_signals = {}
         self.csrname = csrname
         if spec is not None:
             self.isa = 'rv32' if '32' in spec['ISA'] else 'rv64'
+        self.create_uarch_depends(self.uarch_signals)
 
     def check_subval_legal(self, legalstr, value):
         """This function checks if a given value satifies the conditions present
         in a given legal string.
 
         :param legalstr: This is a string following the warl-legal syntax.
         :type legalstr: str
@@ -391,15 +402,15 @@
                             renamed_csr = self.csrname.split('::')[0]
                             subfield = self.csrname.split('::')[1]
                         else:
                             renamed_csr = self.csrname
                             subfield = ''
                     else:
                         _csrname = re.sub('{\d*}','',csrname)
-                        renamed_csr = list(filter(re.compile(f'[a-zA-Z0-9]*[:]*{_csrname}\s*$').match, self.dependencies))[0]
+                        renamed_csr = list(filter(re.compile(f'[a-zA-Z0-9_]*[:]*{_csrname}\s*$').match, self.dependencies))[0]
                         if '::' in renamed_csr:
                             subfield = renamed_csr.split('::')[1]
                         else:
                             subfield = ''
                         renamed_csr = renamed_csr.split('::')[0]
                     # if the dependency_vals dict is not empty, then pick the
                     # values of the csrs/subfields from there. Here we expect
@@ -422,18 +433,25 @@
                             logger.debug(f'dependent csr is indexed with val {index_val}')
                             for i in self.spec[renamed_csr][self.isa]['index_list']:
                                 logger.debug(f'parsing {i["index_val"]}')
                                 if index_val == i['index_val']:
                                     dep_csr_val = i['reset-val']
                                     break
                         else:
-                            dep_csr_val = self.spec[renamed_csr]['reset-val']
+                            if 'uarch_' in renamed_csr:
+                                dep_csr_val = self.uarch_signals[renamed_csr]['reset-val']
+                            else:
+                                dep_csr_val = self.spec[renamed_csr]['reset-val']
                         if subfield != '':
-                            msb = self.spec[renamed_csr][self.isa][subfield]['msb']
-                            lsb = self.spec[renamed_csr][self.isa][subfield]['lsb']
+                            if 'uarch_' in renamed_csr:
+                                msb = self.uarch_signals[renamed_csr]['subfields'][subfield]['msb']
+                                lsb = self.uarch_signals[renamed_csr]['subfields'][subfield]['lsb']
+                            else:
+                                msb = self.spec[renamed_csr][self.isa][subfield]['msb']
+                                lsb = self.spec[renamed_csr][self.isa][subfield]['lsb']
                             bitlen = msb - lsb + 1
                             dep_csr_val = (dep_csr_val >> lsb) & \
                                 ((1 << bitlen)-1)
                     else:
                         err.append(f'No dependency_vals or spec exists to \
 check the values of the csrs in the dependency_fields of csr {self.csrname}')
                         return err
@@ -453,14 +471,79 @@
                 if assign_legal and dep_pass:
                     logger.debug(f' warl legal string "{legalstr}" treats the \
 input value {value} as legal')
                     err = []
                     break
         return err
 
+    def create_uarch_depends(self, uarch_signals):
+        '''
+        This function populates the uarch_depends dict with the csr/subfield
+        '''
+
+        csrname = self.csrname
+        reg_lsb = 0
+        if self.f_lsb != 0:
+            reg_msb = self.f_msb - self.f_lsb
+        else:
+            reg_msb = self.f_msb
+        reg_bitlen = reg_msb - reg_lsb + 1
+        for legalstr in self.node['legal']:
+            depstr = legalstr.split('->')[0]
+            raw_depstr = re.sub('\(|\)|and|or|\&\&|\|\|','',depstr)
+            dep_str_matches = self.regex_dep_legal.findall(raw_depstr)
+
+            if '->' in legalstr:
+                dependencies = self.node['dependency_fields']
+                if dependencies != [] and self.spec is not None:
+                    for d in dependencies:
+                        subfield = ''
+                        if '::' in d:
+                            depcsrname = d.split('::')[0]
+                            subfield = d.split('::')[1]
+                        else:
+                            depcsrname = d
+                            subfield = None
+
+                        # if the depcsrname has the 'uarch_' prefix, then drop that dependency for all checks entirely
+                        if depcsrname.startswith('uarch_'):
+                            subfield_str = '' if subfield is None else f'{subfield} field from '
+                            logger.warning(f'WARL for csr {csrname} depends on \
+{subfield_str}uarch csr {depcsrname}. Treating this as a uarch dependency.')
+                            if subfield is None:
+                                subfield = depcsrname
+                                depcsrname = 'uarch_signals'
+                            if depcsrname not in self.uarch_depends:
+                                self.uarch_depends[depcsrname] = []
+                            if subfield is not None and subfield not in self.uarch_depends[depcsrname]:
+                                self.uarch_depends[depcsrname].append(subfield)
+                            logger.debug(f'uArch dependencies are: {self.uarch_depends}')
+
+        for entry, signode in self.uarch_depends.items():
+            if signode == []:
+                continue
+            else:
+                # grouped uarch signals
+                if entry in uarch_signals:
+                    for subfield in signode:
+                        if subfield in uarch_signals[entry]['subfields']:
+                            logger.debug(f'found csr {csrname} to depend on uArch signal {entry} \
+for the following subfields: {signode}.')
+                        else:
+                            logger.error(f'csr {csrname} depends on uArch signal {entry} \
+for the following subfields: {signode} but the uArch signal is not defined.')
+                # ungrouped uarch signals
+                else:
+                    for entry in signode:
+                        if entry in uarch_signals:
+                            logger.debug(f'found csr {csrname} to depend on uArch signal {entry}.')
+                        else:
+                            logger.error(f'csr {csrname} depends on uArch signal {entry} \
+but the uArch signal is not defined.')
+
     def iserr(self):
         logger.debug(f'---- Checking for Errors in {self.csrname}')
         csrname = self.csrname
         reg_lsb = 0
         if self.f_lsb != 0:
             reg_msb = self.f_msb - self.f_lsb
         else:
@@ -498,17 +581,24 @@
                     for d in dependencies:
                         subfield = ''
                         if '::' in d:
                             depcsrname = d.split('::')[0]
                             subfield = d.split('::')[1]
                         else:
                             depcsrname = d
+                            subfield = None
+
+                        # if the csr is a uarch dependency and also exists in the spec, throw an error
+                        if depcsrname in self.uarch_depends and depcsrname in self.spec:
+                            err.append(f' csr {csrname} depends on uarch csr \
+{depcsrname} which is also present in the spec. This is not allowed.')
+
                         # if the dependency is on writeval or currval of the
-                        # same csr, then no more checks required.
-                        if depcsrname not in ['writeval', 'currval']:
+                        # same csr, or is a uArch dependency, then no more checks required.
+                        if depcsrname not in ['writeval', 'currval'] and depcsrname not in self.uarch_depends and depcsrname not in self.uarch_depends['uarch_signals']:
                             # if the csr doesn't exist then its probably a typo
                             if depcsrname not in self.spec:
                                 err.append(f' warl for csr {csrname} depends on csr \
 {depcsrname} is not a valid csrname as per spec')
                             # if csr exists, but is not accessible, then its a
                             # pointless dependency
                             elif not self.spec[depcsrname][self.isa]['accessible']:
@@ -527,15 +617,21 @@
 
                     # ensure that all dependency csrs/subfields found in the
                     # strings, are indeed present in the dependency_fields list
                     # of the warl node.
                     for matches in dep_str_matches:
                         (csr, ind, op, val) = matches
                         csr = re.sub('{\d*}','', csr)
-                        csr_in_dependencies = list(filter(re.compile(f'[a-zA-Z0-9]*[:]*{csr}\s*$').match, dependencies))
+                        csr_in_dependencies = list(filter(re.compile(f'[a-zA-Z0-9_]*[:]*{csr}\s*$').match, dependencies))
+                        if csr_in_dependencies == []:
+                            for entry, subfields in self.uarch_signals.items():
+                                if csr == entry:
+                                    csr_in_dependencies.append(csr)
+                                elif csr in subfields['subfields']:
+                                    csr_in_dependencies.append(f'{csr}::{subfield}')
                         if csr_in_dependencies == []:
                             err.append(f' dependency_vals string "{depstr}" for csr \
 {csrname} is dependent on field {csr} which is not present in the \
 dependency_fields list of the node')
 
                 for matches in dep_str_matches:
                     (csr, indices, op, val) = matches
```

### Comparing `riscv_config-3.8.1/riscv_config.egg-info/PKG-INFO` & `riscv_config-3.9.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
-Name: riscv-config
-Version: 3.8.1
+Name: riscv_config
+Version: 3.9.0
 Summary: RISC-V Configuration Validator
 Home-page: https://github.com/riscv/riscv-config
 Author: InCore Semiconductors Pvt. Ltd.
 Author-email: neelgala@incoresemi.com
 License: BSD-3-Clause
 Description: RISCV-Config
         ==============
```

### Comparing `riscv_config-3.8.1/riscv_config.egg-info/SOURCES.txt` & `riscv_config-3.9.0/riscv_config.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,10 +13,11 @@
 riscv_config/warl.py
 riscv_config.egg-info/PKG-INFO
 riscv_config.egg-info/SOURCES.txt
 riscv_config.egg-info/dependency_links.txt
 riscv_config.egg-info/entry_points.txt
 riscv_config.egg-info/requires.txt
 riscv_config.egg-info/top_level.txt
+riscv_config/schemas/schema_custom.yaml
 riscv_config/schemas/schema_debug.yaml
 riscv_config/schemas/schema_isa.yaml
 riscv_config/schemas/schema_platform.yaml
```

### Comparing `riscv_config-3.8.1/setup.py` & `riscv_config-3.9.0/setup.py`

 * *Files identical despite different names*

