# Comparing `tmp/ksfctl-0.2.3.tar.gz` & `tmp/ksfctl-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ksfctl-0.2.3.tar", last modified: Sun Apr 23 15:55:57 2023, max compression
+gzip compressed data, was "ksfctl-0.2.4.tar", last modified: Tue May 16 12:00:21 2023, max compression
```

## Comparing `ksfctl-0.2.3.tar` & `ksfctl-0.2.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-04-23 15:55:47.000000 ksfctl-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-23 15:55:57.789500 ksfctl-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-04-23 15:55:47.000000 ksfctl-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/ksfctl/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/ksfctl/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12368 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/cmd/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     7087 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/cmd/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/ksfctl/generate/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/ksfctl/generate/cpp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/cpp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    81038 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/cpp/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    15429 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/cpp/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    27554 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/cpp/template.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/ksfctl/generate/ksf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/ksf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/ksf/generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    11540 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/generate/ksf/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/ksfctl/parser/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22610 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/parser/ksf.py
--rw-r--r--   0 runner    (1001) docker     (123)    34410 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/parser/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/parser/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-23 15:55:47.000000 ksfctl-0.2.3/ksfctl/parser/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 15:55:57.789500 ksfctl-0.2.3/ksfctl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-23 15:55:57.000000 ksfctl-0.2.3/ksfctl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-23 15:55:57.000000 ksfctl-0.2.3/ksfctl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 15:55:57.000000 ksfctl-0.2.3/ksfctl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-23 15:55:57.000000 ksfctl-0.2.3/ksfctl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 15:55:57.000000 ksfctl-0.2.3/ksfctl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-23 15:55:57.000000 ksfctl-0.2.3/ksfctl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-23 15:55:57.789500 ksfctl-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-23 15:55:47.000000 ksfctl-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:00:21.608021 ksfctl-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-05-16 12:00:09.000000 ksfctl-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 12:00:21.608021 ksfctl-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-05-16 12:00:09.000000 ksfctl-0.2.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:00:21.604021 ksfctl-0.2.4/ksfctl/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:00:21.604021 ksfctl-0.2.4/ksfctl/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13915 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/cmd/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8605 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/cmd/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:00:21.608021 ksfctl-0.2.4/ksfctl/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:00:21.608021 ksfctl-0.2.4/ksfctl/generate/cpp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/generate/cpp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89278 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/generate/cpp/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17170 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/generate/cpp/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27681 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/generate/cpp/template.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:00:21.608021 ksfctl-0.2.4/ksfctl/generate/ksf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/generate/ksf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5239 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/generate/ksf/generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11483 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/generate/ksf/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:00:21.608021 ksfctl-0.2.4/ksfctl/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22614 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/parser/ksf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34432 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/parser/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/parser/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-16 12:00:09.000000 ksfctl-0.2.4/ksfctl/parser/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 12:00:21.604021 ksfctl-0.2.4/ksfctl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-05-16 12:00:21.000000 ksfctl-0.2.4/ksfctl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-16 12:00:21.000000 ksfctl-0.2.4/ksfctl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 12:00:21.000000 ksfctl-0.2.4/ksfctl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-16 12:00:21.000000 ksfctl-0.2.4/ksfctl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:00:21.000000 ksfctl-0.2.4/ksfctl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 12:00:21.000000 ksfctl-0.2.4/ksfctl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 12:00:21.608021 ksfctl-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-16 12:00:09.000000 ksfctl-0.2.4/setup.py
```

### Comparing `ksfctl-0.2.3/LICENSE` & `ksfctl-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ksfctl-0.2.3/README.md` & `ksfctl-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ksfctl-0.2.3/ksfctl/cmd/cmd.py` & `ksfctl-0.2.4/ksfctl/cmd/cmd.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import enum
+from pathlib import Path
 
 from ksfctl.cmd.options import *
 from ksfctl.generate.cpp.generator import cpp_gen
 
 
 @click.group(context_settings={'help_option_names': ['-h', '--help']})
 @click.pass_context
@@ -28,30 +29,44 @@
     pass
 
 
 class ModeType(enum.Enum):
     FILE = 'file'
     ALL_IN_ONE = 'all_in_one'
     EXPORT_IMPORT = 'export_import'
+    INVOKE_SEPARATE = 'invoke_separate'
 
 
 class VisibilityType(enum.Enum):
     PUBLIC = 'public'
     PRIVATE = 'private'
 
 
 @ksf_trans.command(name='cxx', context_settings={'help_option_names': ['-h', '--help']})
 @click.pass_context
-@click.argument('files', nargs=-1, required=True, type=str, metavar='...<file>')
+@click.argument('patterns',
+                nargs=-1,
+                required=True,
+                type=str,
+                metavar='...<glob> or ...<regex>'
+                )
+@click.option('--match-mode',
+              'match_mode',
+              default='glob',
+              metavar='<mode>',
+              type=click.Choice(('file', 'glob', 'glob-recursive')),
+              help='匹配模式'
+              )
 @click.option('--mode', 'mode', default=ModeType.FILE.value, type=click.Choice([mode.value for mode in ModeType]),
               help=f'''\
 生成器模式选择.
 
 file=单文件(每一个.ksf对应生成一个文件)
 all_in_one=合并文件(只生成一个聚合文件)
+invoke_separate=调用分离模式
 export_import=导出导入模式(sdk模式), 默认为file)
 '''
               )
 @click.option('--dispatch-mode', 'dispatch_mode', default='array', type=click.Choice(('array', 'set', 'hash')),
               metavar='<dispatch-mode>', help='分发模式, 支持(array, set, hash)'
               )
 @click.option('--visibility', 'visibility', default=VisibilityType.PUBLIC.value,
@@ -66,30 +81,38 @@
 @click.option('-d', '--dir', '--dest', 'destination_path', multiple=False, help='生成的头文件存放的路径',
               metavar='<destination-path>'
               )
 @click.option('-o', '--output-file', 'output_file', multiple=False, default="ksf_out.h",
               help='[聚合模式]生成的聚合头文件名', metavar='<output-file>'
               )
 @click.option('--export-file', 'export_file', multiple=False, default="ksf_export.h",
-              help='[导入导出模式生效]生成的导出符号头文件名(默认为ksf_export.h)', metavar='<export-file>'
+              help='[导入导出模式/调用分离模式生效]生成的导出符号头文件名(默认为ksf_export.h)', metavar='<export-file>'
               )
 @click.option('--invoke-file', 'invoke_file', multiple=False, default="ksf_invoke.h",
-              help='[导入导出模式生效]生成的调用头文件名(默认为ksf_invoke.h)', metavar='<invoke-file>'
+              help='[导入导出模式/调用分离模式生效]生成的调用头文件名(默认为ksf_invoke.h)', metavar='<invoke-file>'
               )
 @click.option('--export', 'export_symbols', multiple=True, help='需要导出的结构体或者函数体')
 @click.option('--hidden', 'hidden_symbols', multiple=True, help='需要隐藏的结构体或者函数体(TODO)')
 @click.option('--replace_ns', '--replace-ns', multiple=False, help='(将被废弃)替换namespace')
 @click.option('--replace-namespace', nargs=2, multiple=True, type=str, help='(推荐)将指定命名空间替换为另一个命名空间')
 @click.option('--replace-include-path', nargs=2, multiple=True, type=str, help='(推荐)替换头文件路径')
 @click.option('--push-function', multiple=True,
               help='携带push模式的函数名, 用于生成push函数，参数形式为module.interface.operator'
               )
 @click.option('--ignore-relative-path', 'ignore_relative_path', is_flag=True, flag_value=True, default=False,
               help='忽略依赖目录'
               )
+@click.option('-w',
+              '--work-directory',
+              'work_directory',
+              multiple=False,
+              default="@pwd",
+              metavar='<work-directory>',
+              help='工作目录'
+              )
 @click.option('--verbose', 'verbose', is_flag=True, flag_value=True, default=False, help='是否打印详细信息')
 # 可选优化选项
 @click.option('--enable-check-default/--disable-check-default',
               'check_default',
               default=True,
               help='是否打包默认值'
               )
@@ -138,31 +161,54 @@
 @click.option('--enable-cxx17/--disable-cxx17',
               'cxx17',
               is_flag=True,
               flag_value=True,
               default=False,
               help='使用C++17'
               )
-def cxx(ctx, files, mode, **kwargs):
+def cxx(ctx, patterns, mode, **kwargs):
     """c++(cpp)语言解析器"""
     ctx.help_option_names += ['-h']
 
     parsed_kwargs = {}
 
     print_verbose = flag_verbose(kwargs)
 
     """解析配置文件"""
     if "config_file" in kwargs:
         """解析配置文件"""
         parse_config_file_to_parsed_args(kwargs, parsed_kwargs)
 
-    """命令的描述"""
+    """文件匹配模式"""
+    print_verbose(var_match_mode(kwargs, parsed_kwargs))
+
+    """文件匹配模式"""
+    print_verbose(var_work_directory(kwargs, parsed_kwargs))
+
+    files = set()
+    work_dir = parsed_kwargs["work_directory"]
+    if parsed_kwargs['match_mode'] == 'glob-recursive':
+        for pattern in patterns:
+            p = Path(pattern)
+            if p.is_absolute():
+                files.update(Path(work_dir).rglob(str(p.relative_to(work_dir))))
+            else:
+                files.update(Path(work_dir).rglob(pattern))
+    elif parsed_kwargs['match_mode'] == 'glob':
+        for pattern in patterns:
+            p = Path(pattern)
+            if p.is_absolute():
+                files.update(Path(work_dir).glob(str(p.relative_to(work_dir))))
+            else:
+                files.update(Path(work_dir).glob(pattern))
+    elif parsed_kwargs['match_mode'] == 'file':
+        files.update(patterns)
+
     if len(files) == 0:
         raise click.BadParameter('未指定任何文件。')
-    print_verbose(f'文件列表: {files}')
 
     """模式"""
     print_verbose(f"""模式: {mode}""")
 
     """将指定命名空间替换为另一个命名空间"""
     print_verbose(list_replace_namespace(kwargs, parsed_kwargs))
 
@@ -210,17 +256,17 @@
 
     """解析所有的flags，携带with_头"""
     parsed_kwargs['flags'] = {}
     for k, v in kwargs.items():
         if isinstance(v, bool):
             parsed_kwargs['flags'].update({f'with_{k}': v})
 
+    print_verbose(var_invoke_file(kwargs, parsed_kwargs))
     if mode == ModeType.EXPORT_IMPORT.value:
         """启动sdk模式，会生成一个export的头文件和一个内部invoke的头文件"""
-        print_verbose(var_invoke_file(kwargs, parsed_kwargs))
         print_verbose(var_export_file(kwargs, parsed_kwargs))
     elif mode == ModeType.FILE.value:
         pass
     else:
         """启动all_one模式，会生成一个聚合的头文件"""
         print_verbose(var_output_file(kwargs, parsed_kwargs))
     cpp_gen(mode, files=files, **parsed_kwargs)
@@ -284,21 +330,21 @@
 #         exit(1)
 #
 #     """解析所有的flags，携带with_头"""
 #     kwargs_with_prefix = {}
 #     for k, v in kwargs.items():
 #         kwargs_with_prefix.update({f'with_{k}': v})
 
-    # case_gen(files=ksf_files,
-    #          include_dirs=include,
-    #          destination_dir=destination_dir,
-    #          out_file=output,
-    #          export_symbols=export_symbols,
-    #          **kwargs_with_prefix
-    #          )
+# case_gen(files=ksf_files,
+#          include_dirs=include,
+#          destination_dir=destination_dir,
+#          out_file=output,
+#          export_symbols=export_symbols,
+#          **kwargs_with_prefix
+#          )
 
 
 if __name__ == '__main__':
     cli()
     exit(0)
 
     runner = CliRunner()
```

### Comparing `ksfctl-0.2.3/ksfctl/cmd/options.py` & `ksfctl-0.2.4/ksfctl/cmd/options.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # 统一解析所有由click传过来的option字段
 import os
+import pathlib
 
 import click
 import yaml
 
 
 # include, destination_dir, replace_ns, replace_namespace, replace_include_path,
 #               push_function, sdk_mode, verbose, sdk_export, sdk_invoke, export_symbols, config_file,
@@ -57,14 +58,52 @@
         print_text = ["未指定替换包含路径."]
 
     del kwargs["replace_include_path"]
 
     return '\n'.join(print_text)
 
 
+def var_match_mode(kwargs, parsed_args: dict):
+    parsed_args["match_mode"] = "glob"
+    default_text = "(默认glob)"
+
+    if "match_mode" in kwargs and kwargs["match_mode"] is not None:
+        parsed_args["match_mode"] = kwargs["match_mode"]
+        default_text = ""
+        del kwargs["match_mode"]
+
+    return f"""匹配模式: {parsed_args["match_mode"]}{default_text}"""
+
+
+def var_work_directory(kwargs, parsed_args: dict):
+    parsed_args["work_directory"] = os.getcwd()
+    default_text = "(默认当前目录[@pwd], 可用其他目录索引格式(用户根目录@home,...))"
+
+    if "work_directory" in kwargs and kwargs["work_directory"] is not None:
+        if kwargs["work_directory"] == "@pwd":
+            parsed_args["work_directory"] = os.getcwd()
+        elif kwargs["work_directory"] == "@home":
+            parsed_args["work_directory"] = os.path.expanduser("~")
+        else:
+            path = pathlib.Path(kwargs["work_directory"])
+
+            if pathlib.Path.is_dir(path):
+                if pathlib.Path.is_absolute(path):
+                    parsed_args["work_directory"] = path
+                else:
+                    parsed_args["work_directory"] = os.path.join(os.getcwd(), path)
+            else:
+                raise click.BadParameter(f"指定的路径 {path} 不存在或不是一个目录。")
+
+        default_text = ""
+        del kwargs["work_directory"]
+
+    return f"""当前执行路径: {parsed_args["work_directory"]}{default_text}"""
+
+
 def var_destination_path(kwargs, parsed_args: dict):
     parsed_args["destination_path"] = os.getcwd()
     default_text = "(默认当前路径@pwd)"
 
     if "destination_path" in kwargs and kwargs["destination_path"] is not None:
         parsed_args["destination_path"] = kwargs["destination_path"]
         default_text = ""
@@ -78,17 +117,17 @@
     print_text = []
 
     if "include_path" in kwargs and kwargs["include_path"] is not None:
         parsed_args["include_path"].update(kwargs["include_path"])
         print_text.append(f"""包含路径: {parsed_args["include_path"]}""")
         del kwargs["include_path"]
 
-    if len(parsed_args["include_path"]) == 0:
-        parsed_args["include_path"].update([os.getcwd()])
-        print_text.append(f"""包含路径: {parsed_args["include_path"]}(当前目录@pwd)""")
+    # if len(parsed_args["include_path"]) == 0:
+    parsed_args["include_path"].update([parsed_args['work_directory']])
+    print_text.append(f"""包含路径: {parsed_args["include_path"]}(当前执行目录@pwd)""")
 
     return '\n'.join(print_text)
 
 
 def list_push_function(kwargs, parsed_args: dict):
     parsed_args["push_function"] = []
     print_text = ""
```

### Comparing `ksfctl-0.2.3/ksfctl/generate/cpp/generator.py` & `ksfctl-0.2.4/ksfctl/generate/cpp/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,71 +4,101 @@
 from ksfctl.generate.cpp.parser import CppParser
 from ksfctl.generate.cpp.template import *
 from ksfctl.parser.ksf import *
 from ksfctl.parser.parser import generate
 
 
 class CppGenerator(CppParser):
-    def __init__(self, ast, repl_ns_dict, repl_inc_dir, destination, push_functions, input_file, output_file,
+    def __init__(self,
+                 ast,
+                 repl_ns_dict,
+                 repl_inc_dir,
+                 destination,
+                 push_functions,
+                 input_file,
+                 output_file,
+                 invoke_file,
                  dispatch_mode,
                  **kwargs
                  ):
-        super().__init__(ast, repl_ns_dict, repl_inc_dir, destination, push_functions, [], dispatch_mode, **kwargs)
+        super().__init__(ast,
+                         repl_ns_dict,
+                         repl_inc_dir,
+                         destination,
+                         push_functions,
+                         [],
+                         dispatch_mode,
+                         **kwargs)
         self.input_file = input_file
         self.output_file = Path(destination) / output_file  # 生成的头文件
+        self.invoke_file = Path(destination) / invoke_file  # 生成的调用文件
 
-    def parse_enum(self, ksf_enum: KsfEnum):
+    def parse_enum(self,
+                   ksf_enum: KsfEnum):
         enum_members = []
         function_etos = []
         function_stoe = []
         for m in ksf_enum.member:
             enum_members.append(self.parse_enum_member(m))
             function_etos.append(self.parse_enum_to_str(m))
             function_stoe.append(self.parse_str_to_enum(m))
 
         return [fstr(template_enum,
                      comment=self.parse_comment_above(ksf_enum.comment),
                      enum_name=ksf_enum.name,
                      enum_members=enum_members,
                      ),
-                fstr(template_etos, enum_name=ksf_enum.name, etos_member=function_etos),
-                fstr(template_stoe, enum_name=ksf_enum.name, stoe_member=function_stoe)]
+                fstr(template_etos,
+                     enum_name=ksf_enum.name,
+                     etos_member=function_etos),
+                fstr(template_stoe,
+                     enum_name=ksf_enum.name,
+                     stoe_member=function_stoe)]
 
-    def parse_resetDefault(self, ksf_struct: KsfStruct):
-        return fstr(template_resetDefault, struct_name=ksf_struct.name)
+    def parse_resetDefault(self,
+                           ksf_struct: KsfStruct):
+        return fstr(template_resetDefault,
+                    struct_name=ksf_struct.name)
 
-    def parse_variable_writeTo(self, ksf_field: KsfField):
+    def parse_variable_writeTo(self,
+                               ksf_field: KsfField):
         value_type = ksf_field.value_type
-        if self.with_check_default:
-            if isinstance(value_type, KsfBuildInType):
-                if isinstance(value_type, KsfBoolType):
+        if self.with_check_default and not ksf_field.is_required:
+            if isinstance(value_type,
+                          KsfBuildInType):
+                if isinstance(value_type,
+                              KsfBoolType):
                     check_default = f"""{'!' if not ksf_field.has_default() or ksf_field.default['value'] else ''}{ksf_field.name}"""
                 else:
                     check_default = self.parse_default_var(f'{ksf_field.name}',
                                                            value_type,
                                                            ksf_field.default,
                                                            is_equal=False
                                                            )
-            elif isinstance(value_type, KsfStructType):
+            elif isinstance(value_type,
+                            KsfStructType):
                 return fstr(template_writeTo_variable,
                             variable_name=ksf_field.name,
                             variable_tag=ksf_field.tag, )
-            elif isinstance(value_type, KsfEnumType):
+            elif isinstance(value_type,
+                            KsfEnumType):
                 module_name = f"{value_type.module}::" if self.curr_module != value_type.module else ""
 
                 # 如果是枚举类型
                 if ksf_field.has_default():
                     # 有枚举默认值的，使用默认值
                     check_default = f"""{ksf_field.name} != {module_name}{value_type.name}::{ksf_field.default['value']}"""
                 else:
                     # 没有默认值的，使用第一个枚举值
                     check_default = f"""{ksf_field.name} != {module_name}{value_type.name}::{ksf_field.value_type.obj_type.member[0].name}"""
-            elif isinstance(value_type, KsfVectorType):
+            elif isinstance(value_type,
+                            KsfVectorType):
                 check_default = f"""!{ksf_field.name}.empty()"""
-            elif isinstance(value_type, KsfMapType):
+            elif isinstance(value_type,
+                            KsfMapType):
                 check_default = f"""!{ksf_field.name}.empty()"""
             else:
                 raise SyntaxError(f"不能被解析的字段类型[{value_type}]")
 
             return fstr(template_writeTo_variable_with_check,
                         check_default=check_default,
                         variable_declare=fstr(template_writeTo_variable,
@@ -76,132 +106,161 @@
                                               variable_tag=ksf_field.tag, ),
                         )
         else:
             return fstr(template_writeTo_variable,
                         variable_name=ksf_field.name,
                         variable_tag=ksf_field.tag, )
 
-    def parse_writeTo(self, ksf_struct: KsfStruct):
+    def parse_writeTo(self,
+                      ksf_struct: KsfStruct):
         var_list = []
         for var in ksf_struct.variable:
             var_list.append(self.parse_variable_writeTo(ksf_struct.variable[var]))
 
-        return fstr(template_writeTo, variables=var_list)
+        return fstr(template_writeTo,
+                    variables=var_list)
 
-    def parse_variable_writeToJson(self, ksf_field: KsfField):
-        return f"""p->value["{ksf_field.name}"] = ksf::JsonOutput::writeJson({ksf_field.name});"""
+    def parse_variable_writeToJson(self,
+                                   ksf_field: KsfField):
+        return f"""p->value["{ksf_field.name}"] = ksf::json::Output::writeJson({ksf_field.name});"""
 
-    def parse_writeToJson(self, ksf_struct: KsfStruct):
+    def parse_writeToJson(self,
+                          ksf_struct: KsfStruct):
         var_list = []
         for var in ksf_struct.variable:
             var_list.append(self.parse_variable_writeToJson(ksf_struct.variable[var]))
 
-        return fstr(template_writeToJson, variables=var_list)
+        return fstr(template_writeToJson,
+                    variables=var_list)
 
-    def parse_variable_readFrom(self, ksf_field: KsfField):
-        return f"""_is.read({ksf_field.name}, {ksf_field.tag}, false);"""
+    def parse_variable_readFrom(self,
+                                ksf_field: KsfField):
+        return f"""_is.read({ksf_field.name}, {ksf_field.tag}, {"true" if ksf_field.is_required else "false"});"""
 
-    def parse_readFrom(self, ksf_struct: KsfStruct):
+    def parse_readFrom(self,
+                       ksf_struct: KsfStruct):
         var_list = []
         for var in ksf_struct.variable:
             var_list.append(self.parse_variable_readFrom(ksf_struct.variable[var]))
 
-        return fstr(template_readFrom, variables=var_list)
+        return fstr(template_readFrom,
+                    variables=var_list,
+                    is_wrap=False)
 
-    def parse_variable_readFromJson(self, ksf_field: KsfField):
-        return f"""ksf::JsonInput::readJson({ksf_field.name}, pObj->value["{ksf_field.name}"], false);"""
+    def parse_variable_readFromJson(self,
+                                    ksf_field: KsfField):
+        return f"""ksf::json::Input::readJson({ksf_field.name}, pObj->value["{ksf_field.name}"], {"true" if ksf_field.is_required else "false"});"""
 
-    def parse_readFromJson(self, ksf_struct: KsfStruct):
+    def parse_readFromJson(self,
+                           ksf_struct: KsfStruct):
         var_list = []
         for var in ksf_struct.variable:
             var_list.append(self.parse_variable_readFromJson(ksf_struct.variable[var]))
 
-        return fstr(template_readFromJson, variables=var_list)
+        return fstr(template_readFromJson,
+                    variables=var_list,
+                    is_wrap=False)
 
-    def parse_display(self, ksf_struct: KsfStruct):
+    def parse_display(self,
+                      ksf_struct: KsfStruct):
         var_list = ""
         for var in ksf_struct.variable:
             field = ksf_struct.variable[var]
-            if isinstance(field.value_type, KsfEnumType):
+            if isinstance(field.value_type,
+                          KsfEnumType):
                 var_list += f'_ds.display(static_cast<int32_t>({ksf_struct.variable[var].name}),"{ksf_struct.variable[var].name}");\n'
             else:
                 var_list += f'_ds.display({ksf_struct.variable[var].name},"{ksf_struct.variable[var].name}");\n'
 
-        return fstr(template_display, variables=var_list)
+        return fstr(template_display,
+                    variables=var_list)
 
-    def parse_displaySimple(self, ksf_struct: KsfStruct):
-        var_list = ""
-        for var in ksf_struct.variable:
-            field = ksf_struct.variable[var]
-            if isinstance(field.value_type, KsfEnumType):
-                var_list += f'_ds.displaySimple(static_cast<int32_t>({ksf_struct.variable[var].name}), true);\n'
+    def parse_displaySimple(self,
+                            ksf_struct: KsfStruct):
+        var_list = []
+        index = 0
+        for field in ksf_struct.variable.values():
+            index += 1
+            if isinstance(field.value_type,
+                          KsfEnumType):
+                var_list.append(
+                    f'_ds.displaySimple(static_cast<int32_t>({field.name}), {"false" if index == len(ksf_struct.variable) else "true"});\n')
             else:
-                var_list += f'_ds.displaySimple({ksf_struct.variable[var].name}, true);\n'
+                var_list.append(
+                    f'_ds.displaySimple({field.name}, {"false" if index == len(ksf_struct.variable) else "true"});')
 
-        return fstr(template_displaySimple, variables=var_list)
+        return fstr(template_displaySimple,
+                    variables=var_list)
 
-    def parse_equal(self, ksf_struct: KsfStruct):
+    def parse_equal(self,
+                    ksf_struct: KsfStruct):
         var_list = []
         for var in ksf_struct.variable:
             field = ksf_struct.variable[var]
-            if isinstance(field.value_type, KsfFloatType):
+            if isinstance(field.value_type,
+                          KsfFloatType):
                 var_list.append(f'ksf::KS_Common::equal(l.{field.name}, r.{field.name})')
             else:
                 var_list.append(f'(l.{field.name} == r.{field.name})')
 
         return fstr(template_operator_equal,
                     struct_name=ksf_struct.name,
                     variables=' && '.join(var_list)
                     )
 
-    def parse_struct_variables(self, ksf_struct: KsfStruct):
+    def parse_struct_variables(self,
+                               ksf_struct: KsfStruct):
         text_lines = []
         # 解析字段
         var_list = []
         for var in ksf_struct.variable:
             var_list.append(self.parse_variable(ksf_struct.variable[var]))
 
         var_widths = self.get_column_widths(var_list)
         for comment, var_type, var_name, var_value in var_list:
             if comment:
-                text_lines.append(self.add_lines(f"{comment:<{var_widths[0]}}", 1))
+                text_lines.append(self.add_lines(f"{comment:<{var_widths[0]}}",
+                                                 1))
             text_lines.append(self.add_lines(f"{var_type:<{var_widths[1]}} {var_name:<{var_widths[2]}}{var_value}",
                                              1
                                              )
                               )
 
         return self.endl().join(text_lines)
 
-    def parse_struct(self, ksf_struct: KsfStruct):
-        self.add_include("<kup/Ksf.h>")
+    def parse_struct(self,
+                     ksf_struct: KsfStruct):
+        self.add_include("ksf/proto/proto.h")
 
         comment = self.parse_comment_above(ksf_struct.comment)
         variables = self.parse_struct_variables(ksf_struct)
         struct_functions = [
             self.parse_resetDefault(ksf_struct),
             self.parse_writeTo(ksf_struct),
             self.parse_readFrom(ksf_struct)
         ]
 
         struct_operators = []
 
         if self.with_json:
-            self.add_include("<kup/KsfJson.h>")
+            self.add_include("ksf/proto/json.h")
             struct_functions.append(self.parse_writeToJson(ksf_struct))
             struct_functions.append(self.parse_readFromJson(ksf_struct))
 
         struct_functions.append(self.parse_display(ksf_struct))
         struct_functions.append(self.parse_displaySimple(ksf_struct))
         struct_operators.append(self.parse_equal(ksf_struct))
 
         if len(ksf_struct.key_fields) != 0:
             key_vars = []
             for key_field in ksf_struct.key_fields:
                 key_vars.append(f"""if(l.{key_field} != r.{key_field})  return (l.{key_field} < r.{key_field});""")
-            struct_operators.append(fstr(template_operator_compare, struct_name=ksf_struct.name, variables=key_vars))
+            struct_operators.append(fstr(template_operator_compare,
+                                         struct_name=ksf_struct.name,
+                                         variables=key_vars))
 
         if self.with_json:
             struct_operators.append(fstr(template_operator_stream_with_json,
                                          wrap_mode=False,
                                          struct_name=ksf_struct.name
                                          )
                                     )
@@ -212,43 +271,53 @@
                     struct_name=ksf_struct.name,
                     md5sum=md5(ksf_struct.id.encode('utf8')).hexdigest(),
                     variables=variables,
                     struct_functions=struct_functions,
                     struct_operators=struct_operators
                     )
 
-    def parse_output_var(self, value_type, name, with_type):
-        if not isinstance(value_type, KsfVoidType):
+    def parse_output_var(self,
+                         value_type,
+                         name,
+                         with_type):
+        if not isinstance(value_type,
+                          KsfVoidType):
             if not self.is_movable_type(value_type):
                 return f"{self.parse_type(value_type)} {name}" if with_type else name
             elif self.with_rvalue_ref:
                 return f"{self.parse_type(value_type)} &&{name}" if with_type else f"std::move({name})"
             else:
                 return f"const {self.parse_type(value_type)} &{name}" if with_type else name
 
-    def parse_output_vars(self, ksf_operator, with_type=True):
+    def parse_output_vars(self,
+                          ksf_operator,
+                          with_type=True):
         vars_list = []
         if ksf_operator.has_return():
-            vars_list.append(self.parse_output_var(ksf_operator.return_type, '_ret', with_type))
+            vars_list.append(self.parse_output_var(ksf_operator.return_type,
+                                                   '_ret',
+                                                   with_type))
 
         for arg in ksf_operator.output.values():
             vars_list.append(self.parse_output_var(arg.value_type,
                                                    arg.name,
                                                    with_type
                                                    )
                              )
 
         return ', '.join(vars_list)
 
-    def parse_InterfacePrxCallBack(self, ksf_interface: KsfInterface):
+    def parse_InterfacePrxCallBack(self,
+                                   ksf_interface: KsfInterface):
         func_case_list = []
         function_handles = []
         dispatch_str = []
 
-        def parse_func_dispatch(index, operator):
+        def parse_func_dispatch(index,
+                                operator):
             """处理函数的分发"""
             output_args = []
 
             if operator.has_return():
                 output_args.append(fstr(template_output_argument_parse,
                                         typename=self.parse_type(operator.return_type),
                                         argument_name='_ret',
@@ -263,50 +332,56 @@
                                         index=var.index
                                         )
                                    )
 
             func_case_list.append(fstr(template_dispatch_case_at_client,
                                        case=index,
                                        function_name=operator.name,
-                                       output_params=self.parse_output_vars(operator, False),
+                                       output_params=self.parse_output_vars(operator,
+                                                                            False),
                                        output_arguments=output_args
                                        )
                                   )
 
             function_handles.append(fstr(template_function_call,
                                          function_name=operator.name,
-                                         arguments=self.parse_output_vars(operator, True)
+                                         arguments=self.parse_output_vars(operator,
+                                                                          True)
                                          )
                                     )
 
         get_response_context = template_getResponseContext
 
         def dispatch(function_names):
             dispatch_str.append(fstr(template_array_style_onDispatch_at_client,
                                      dispatch_case_str=func_case_list,
                                      interface_name=ksf_interface.name,
                                      function_names=function_names
                                      )
                                 )
 
-        self.parse_DispatchOperatorCallBack(ksf_interface, dispatch, parse_func_dispatch)
+        self.parse_DispatchOperatorCallBack(ksf_interface,
+                                            dispatch,
+                                            parse_func_dispatch)
 
         return fstr(template_callback,
                     interface_name=ksf_interface.name,
                     function_handles=function_handles,
                     get_response_context=get_response_context,
                     dispatch_str=dispatch_str
                     )
 
-    def parse_InterfacePrxCallbackPromise(self, ksf_interface: KsfInterface):
+    def parse_InterfacePrxCallbackPromise(self,
+                                          ksf_interface: KsfInterface):
         dispatch_case_str = []
         interface_promises = []
         on_dispatch = []
 
-        def parse_func_dispatch(index, operator):
+        def parse_func_dispatch(index,
+                                operator):
             output_parsed_list = []
             if operator.has_return():
                 output_parsed_list.append(f"{self.parse_type(operator.return_type)} _ret;")
 
             for var in operator.output.values():
                 output_parsed_list.append(f"{self.parse_type(var.value_type)} {var.name};")
 
@@ -336,55 +411,65 @@
             on_dispatch.append(fstr(template_onDispatch_promise,
                                     dispatch_case_str=dispatch_case_str,
                                     interface_name=ksf_interface.name,
                                     function_names=function_names
                                     )
                                )
 
-        self.parse_DispatchOperatorCallBack(ksf_interface, dispatch, parse_func_dispatch)
+        self.parse_DispatchOperatorCallBack(ksf_interface,
+                                            dispatch,
+                                            parse_func_dispatch)
 
         return fstr(template_callback_promise,
                     interface_name=ksf_interface.name,
                     function_names=ksf_interface.operator.keys(),
                     interface_promises=interface_promises,
                     on_dispatch=on_dispatch
                     )
 
-    def parse_InterfaceCoroPrxCallback(self, ksf_interface: KsfInterface):
+    def parse_InterfaceCoroPrxCallback(self,
+                                       ksf_interface: KsfInterface):
         func_case_str = []
         on_dispatch = []
 
-        def parse_case_dispatch(index, operator):
+        def parse_case_dispatch(index,
+                                operator):
             func_case_list = []
             if operator.has_return():
                 func_case_list.append(
                     f"""{self.parse_type(operator.return_type)} _ret;\n_is.read(_ret, 0, true);"""
                 )
 
             for var2 in operator.output.values():
                 func_case_list.append(
                     f"""{self.parse_type(var2.value_type)} {var2.name};\n_is.read({var2.name}, {var2.index}, true);"""
                 )
 
             def parse_output_vars(with_type=True):
-                def parse_output_var(value_type, name, with_type):
+                def parse_output_var(value_type,
+                                     name,
+                                     with_type):
                     if value_type.name != 'void':
                         if not self.is_movable_type(value_type):
                             return f"{self.parse_type(value_type)} {name}" if with_type else name
                         elif self.with_rvalue_ref:
                             return f"{self.parse_type(value_type)} &&{name}" if with_type else f"std::move({name})"
                         else:
                             return f"const {self.parse_type(value_type)} &{name}" if with_type else name
 
                 vars_list = []
                 if operator.has_return():
-                    vars_list.append(parse_output_var(operator.return_type, '_ret', with_type))
+                    vars_list.append(parse_output_var(operator.return_type,
+                                                      '_ret',
+                                                      with_type))
 
                 for argument in operator.output.values():
-                    vars_list.append(parse_output_var(argument.value_type, argument.name, with_type))
+                    vars_list.append(parse_output_var(argument.value_type,
+                                                      argument.name,
+                                                      with_type))
 
                 return vars_list
 
             func_case_str.append(fstr(template_parse_func_dispatch_coroutine,
                                       case=index,
                                       output_arguments=parse_output_vars(with_type=False),
                                       function_name=operator.name,
@@ -396,162 +481,184 @@
             on_dispatch.append(fstr(template_onDispatch_coroutine,
                                     interface_name=ksf_interface.name,
                                     function_names=function_names,
                                     func_case_str=func_case_str
                                     )
                                )
 
-        self.parse_DispatchOperatorCallBack(ksf_interface, dispatch, parse_case_dispatch)
+        self.parse_DispatchOperatorCallBack(ksf_interface,
+                                            dispatch,
+                                            parse_case_dispatch)
         return fstr(template_callback_coroutine_class,
                     interface_name=ksf_interface.name,
                     on_dispatch=on_dispatch
                     )
 
-    def parse_InterfaceProxyOperator(self, ksf_interface: KsfInterface):
+    def parse_InterfaceProxyOperator(self,
+                                     ksf_interface: KsfInterface):
         functions = []
         for operator in ksf_interface.operator.values():
-            input_arguments = []
-            output_arguments = []
+            input_argument_declare = []
+            output_argument_declare = []
             for var in operator.input.values():
-                input_arguments.append(f"""_os.write({var.name}, {var.index});""")
+                input_argument_declare.append(f"""_os.write({var.name}, {var.index});""")
 
             if operator.has_return():
-                output_arguments.append(
+                output_argument_declare.append(
                     f"""{self.parse_type(operator.return_type)} _ret;\n_is.read(_ret, 0, true);"""
                 )
 
             for name in operator.output:
                 var = operator.output[name]
-                output_arguments.append(f"""_is.read({name}, {var.index}, true);""")
+                output_argument_declare.append(f"""_is.read({name}, {var.index}, true);""")
 
             def parse_all_vars(with_output=False):
                 parsed_list = []
                 for var_name, is_output in operator.ordered_var:
                     if is_output:
                         if with_output:
                             parsed_list.append(
                                 f"{self.parse_type(operator.output[var_name].value_type)} &{var_name}"
                             )
                     else:
                         parsed_list.append(
                             f"const {self.parse_type(operator.input[var_name].value_type)} &{var_name}"
                         )
 
-                return ', '.join(parsed_list)
+                return parsed_list
 
             arguments = parse_all_vars(with_output=True)
+            input_arguments = parse_all_vars(with_output=False)
             comment = self.parse_comment_above(operator.comment)
             return_type = self.parse_type(operator.return_type) if operator.has_return() else 'void'
 
-            return_line = self.add_lines(f"\nreturn _ret;", 1) if operator.has_return() else ""
+            return_line = self.add_lines(f"\nreturn _ret;",
+                                         1) if operator.has_return() else ""
 
             functions.append(fstr(template_proxy_function,
                                   interface_name=ksf_interface.name,
                                   function_name=operator.name,
                                   arguments=arguments,
+                                  input_arguments=input_arguments,
                                   argument_async_callback=f'{ksf_interface.name}PrxCallbackPtr callback',
                                   argument_coroutine_callback=f'{ksf_interface.name}CoroPrxCallbackPtr callback',
                                   argument_request_context=f'const _Context_ &_context_ = _Context_()',
                                   argument_response_context=f'_Context_ *_rsp_context_ = nullptr',
-                                  input_arguments=input_arguments,
-                                  output_arguments=output_arguments,
+                                  input_argument_declare=input_argument_declare,
+                                  output_argument_declare=output_argument_declare,
                                   return_type=return_type,
                                   return_line=return_line,
                                   comment=comment
                                   )
                              )
         return functions
 
-    def parse_InterfaceProxy(self, ksf_interface: KsfInterface):
+    def parse_InterfaceProxy(self,
+                             ksf_interface: KsfInterface):
         return fstr(template_proxy_class,
                     interface_name=ksf_interface.name,
                     functions=self.parse_InterfaceProxyOperator(ksf_interface)
                     )
 
-    def parse_OperatorParamsList(self, operator: KsfOperator, mode: str):
+    def parse_OperatorParamsList(self,
+                                 operator: KsfOperator,
+                                 mode: str):
         """mode: json, ksf, kup"""
         parsed_list = []
         for index, (name, is_output) in enumerate(operator.ordered_var):
             if mode == 'json':
                 parsed_list.append(
-                    f"""ksf::JsonInput::readJson({name}, _jsonPtr->value["{name}"], {"false" if is_output else "true"});"""
+                    f"""ksf::json::Input::readJson({name}, _jsonPtr->value["{name}"], {"false" if is_output else "true"});"""
                 )
             elif mode == 'kup':
                 if is_output:
                     parsed_list.append(f"""_ksfAttr_.getByDefault("{name}", {name}, {name});""")
                 else:
                     parsed_list.append(f"""_ksfAttr_.get("{name}", {name});""")
             elif mode == 'ksf':
                 parsed_list.append(f"""_is.read({name}, {index + 1}, {"false" if is_output else "true"});""")
 
         return parsed_list
 
-    def parse_DispatchOperatorCallBack(self, ksf_interface: KsfInterface, interface_callback,
+    def parse_DispatchOperatorCallBack(self,
+                                       ksf_interface: KsfInterface,
+                                       interface_callback,
                                        *operator_callbacks
                                        ):
         if self.dispatch_mode in ['array', 'set']:
             operators = dict(sorted(ksf_interface.operator.items()))
         else:
             operators = ksf_interface.operator
 
         for index, operator in enumerate(operators.values()):
             for cb in operator_callbacks:
-                cb(index, operator)
+                cb(index,
+                   operator)
 
         interface_callback(operators.keys())
 
-    def parse_OperatorInvokeVars(self, index, operator: KsfOperator):
+    def parse_OperatorInvokeVars(self,
+                                 index,
+                                 operator: KsfOperator):
         parsed_list = []
         for name, is_output in operator.ordered_var:
             if not is_output:
                 var = operator.input[name]
                 if self.with_rvalue_ref and self.is_movable_type(var.value_type):
                     parsed_list.append(f"""std::move({var.name}), """)
                 else:
                     parsed_list.append(f"""{var.name}, """)
             else:
                 var = operator.output[name]
                 parsed_list.append(f"""{var.name}, """)
 
         return ''.join(parsed_list)
 
-    def parse_OperatorVarlist(self, index, operator: KsfOperator):
+    def parse_OperatorVarlist(self,
+                              index,
+                              operator: KsfOperator):
         parsed_list = []
         for name, is_output in operator.ordered_var:
             if not is_output:
                 var = operator.input[name]
             else:
                 var = operator.output[name]
             parsed_list.append(f"""{self.parse_type(var.value_type)} {var.name};""")
 
         return parsed_list
 
-    def parse_OperatorOutputVar(self, index, operator: KsfOperator, mode):
+    def parse_OperatorOutputVar(self,
+                                index,
+                                operator: KsfOperator,
+                                mode):
         parsed_list = []
         if operator.return_type['name'] != 'void':
             if mode == 'ksf':
                 parsed_list.append(f"""_os.write(_ret, 0);""")
             elif mode == 'kup':
                 parsed_list.append(f"""_ksfAttr_.put("", _ret);""")
                 parsed_list.append(f"""_ksfAttr_.put("ksf_ret", _ret);""")
             elif mode == 'json':
-                parsed_list.append(f"""_p->value["ksf_ret"] = ksf::JsonOutput::writeJson(_ret);""")
+                parsed_list.append(f"""_p->value["ksf_ret"] = ksf::json::Output::writeJson(_ret);""")
 
         for name in operator.output:
             var = operator.output[name]
             if mode == 'ksf':
                 parsed_list.append(f"""_os.write({name}, {var.index});""")
             elif mode == 'kup':
                 parsed_list.append(f"""_ksfAttr_.put("{name}", {name});""")
             elif mode == 'json':
-                parsed_list.append(f"""_p->value["{name}"] = ksf::JsonOutput::writeJson({name});""")
+                parsed_list.append(f"""_p->value["{name}"] = ksf::json::Output::writeJson({name});""")
 
         return parsed_list
 
-    def parse_OperatorAllVars(self, index, operator: KsfOperator, with_input=False):
+    def parse_OperatorAllVars(self,
+                              index,
+                              operator: KsfOperator,
+                              with_input=False):
         parsed_list = []
         if not with_input and operator.has_return():
             parsed_list.append(f"const {self.parse_type(operator.return_type)} &_ret")
 
         for var_name, is_output in operator.ordered_var:
             if is_output:
                 if with_input:
@@ -575,31 +682,35 @@
                 else:
                     parsed_list.append(
                         f"{self.parse_type(operator.input[var_name].value_type)} {var_name}"
                     )
 
         return parsed_list
 
-    def parse_InterfaceObjModule(self, ksf_interface: KsfInterface):
+    def parse_InterfaceObjModule(self,
+                                 ksf_interface: KsfInterface):
         dispatch_list = []
 
         virtual_func_list = []
         async_func_list = []
         push_func_list = []
         dispatch_case_list = []
 
-        def parse_Operator(index, operator):
+        def parse_Operator(index,
+                           operator):
             async_case = []
             push_func_case = []
             # 当这个方法是异步方法时，需要生成一个同步方法纯虚函数和一个异步方法回调
             if self.enable_async_rsp(f"{self.curr_module}.{ksf_interface.name}.{operator.name}"):
                 # 生成同步方法纯虚函数
                 comment = self.parse_comment_above(operator.comment)
                 return_type = self.parse_type(operator.return_type) if operator.has_return() else 'void'
-                arguments = self.parse_OperatorAllVars(index, operator, True)
+                arguments = self.parse_OperatorAllVars(index,
+                                                       operator,
+                                                       True)
                 virtual_func_list.append(fstr(template_server_pure_function,
                                               comment=comment,
                                               return_type=return_type,
                                               function_name=operator.name,
                                               arguments=arguments,
                                               argument_current='ksf::KsfCurrentPtr _current_'
                                               )
@@ -632,24 +743,25 @@
                                   )
 
                 # 链路追踪
                 if self.with_trace:
                     if not self.with_json:
                         raise SyntaxError("如果需要链路追踪，需要打开生成Json序列化支持(--json)")
 
-                    return_type = '_p_->value[""] = ksf::JsonOutput::writeJson(_ret);' if operator.has_return() else ''
+                    return_type = '_p_->value[""] = ksf::json::Output::writeJson(_ret);' if operator.has_return() else ''
                     async_func_list.append(fstr(template_server_async_response_trace,
                                                 return_type=return_type,
                                                 function_name=operator.name
                                                 )
                                            )
                 # 生成异步方法回调
                 async_func_list.append(fstr(template_server_async_function,
                                             function_name=operator.name,
-                                            arguments=self.parse_OperatorAllVars(index, operator),
+                                            arguments=self.parse_OperatorAllVars(index,
+                                                                                 operator),
                                             argument_current='ksf::KsfCurrentPtr _current_',
                                             async_response_case=async_case,
                                             )
                                        )
 
             # 如果方法为推送方法，需要生成一个推送方法的推送应答
             if self.enable_push(f"{self.curr_module}.{ksf_interface.name}.{operator.name}"):
@@ -696,93 +808,102 @@
                              mode='json'
                          ),
                          response_version_ksf=self.parse_OperatorOutputVar(
                              index,
                              operator,
                              mode='ksf'
                          )
-                         ), 1
+                         ),
+                    1
                 )
                 )
 
             if self.with_push and self.enable_push(f"{self.curr_module}.{ksf_interface.name}.{operator.name}"):
                 push_func_case.append(fstr(template_server_push_function_ksf,
                                            function_name=operator.name,
                                            arguments=self.parse_OperatorOutputVar(index,
                                                                                   operator,
                                                                                   mode='ksf'
                                                                                   ), )
                                       )
 
-                arguments = self.parse_OperatorAllVars(index, operator)
+                arguments = self.parse_OperatorAllVars(index,
+                                                       operator)
                 push_func_list.append(fstr(template_server_push_function,
                                            function_name=operator.name,
                                            arguments=arguments,
                                            argument_request_context=f'const _Context_ &_context_ = _Context_()',
                                            argument_current='ksf::KsfCurrentPtr _current_',
                                            push_func_case=push_func_case, )
                                       )
 
         def dispatch(function_names):
             if self.dispatch_mode == 'array':
                 dispatch_list.append(
                     fstr(template_array_style_onDispatch_at_server,
                          interface_name=ksf_interface.name,
                          function_names=function_names,
-                         dispatch_case_str=self.add_lines(dispatch_case_list, 1)
+                         dispatch_case_str=self.add_lines(dispatch_case_list,
+                                                          1)
                          )
                 )
             elif self.dispatch_mode == 'set':
                 dispatch_list.append(
                     fstr(template_set_style_onDispatch_at_server,
                          interface_name=ksf_interface.name,
                          function_names=function_names,
-                         dispatch_case_str=self.add_lines(dispatch_case_list, 1)
+                         dispatch_case_str=self.add_lines(dispatch_case_list,
+                                                          1)
                          )
                 )
             elif self.dispatch_mode == 'hash':
                 dispatch_list.append(
                     fstr(template_hash_style_onDispatch_at_server,
                          interface_name=ksf_interface.name,
                          function_names=function_names,
-                         dispatch_case_str=self.add_lines(dispatch_case_list, 1)
+                         dispatch_case_str=self.add_lines(dispatch_case_list,
+                                                          1)
                          )
                 )
 
-        self.parse_DispatchOperatorCallBack(ksf_interface, dispatch, parse_Operator)
+        self.parse_DispatchOperatorCallBack(ksf_interface,
+                                            dispatch,
+                                            parse_Operator)
 
         return dispatch_list, virtual_func_list, async_func_list, push_func_list
 
-    def parse_InterfaceObj(self, ksf_interface: KsfInterface):
+    def parse_InterfaceObj(self,
+                           ksf_interface: KsfInterface):
         dispatch, virtual_func, parsed_async_list, parsed_push_list = self.parse_InterfaceObjModule(ksf_interface)
         return fstr(template_server_interface,
                     interface_name=ksf_interface.name,
                     functions=virtual_func,
                     async_functions=parsed_async_list,
                     push_functions=parsed_push_list,
                     dispatch=dispatch,
                     )
 
-    def parse_interface(self, ksf_interface: KsfInterface):
+    def parse_interface(self,
+                        ksf_interface: KsfInterface):
         interface_declare = []
 
         if self.with_invoke_client:
-            self.add_include("<servant/Agent.h>")
+            self.add_include("servant/Agent.h")
             interface_declare.append(self.add_lines(self.parse_InterfacePrxCallBack(ksf_interface)))
             if self.with_promise:
-                self.add_include("<promise/promise.h>")
+                self.add_include("promise/promise.h")
                 interface_declare.append(self.parse_InterfacePrxCallbackPromise(ksf_interface))
 
             if self.with_coroutine:
                 interface_declare.append(self.parse_InterfaceCoroPrxCallback(ksf_interface))
 
             interface_declare.append(self.parse_InterfaceProxy(ksf_interface))
 
         if self.with_invoke_server:
-            self.add_include("<servant/Servant.h>")
+            self.add_include("servant/Servant.h")
             interface_declare.append(self.parse_InterfaceObj(ksf_interface))
 
         return interface_declare
 
     def generate(self):
         self.curr_module = None
         module_declares = []
@@ -805,24 +926,28 @@
                                                 module_begin=self.get_ns_begin(),
                                                 module_end=self.get_ns_end(),
                                                 elements=element_declares
                                                 )
                                            )
                     self.curr_module = ele.module
 
-                if isinstance(ele, KsfConst):
+                if isinstance(ele,
+                              KsfConst):
                     element_declares.append(self.parse_const(ele))
                     pass
-                elif isinstance(ele, KsfEnum):
+                elif isinstance(ele,
+                                KsfEnum):
                     element_declares.append(self.parse_enum(ele))
                     pass
-                elif isinstance(ele, KsfStruct):
+                elif isinstance(ele,
+                                KsfStruct):
                     element_declares.append(self.parse_struct(ele))
                     pass
-                elif isinstance(ele, KsfInterface) and self.with_rpc:
+                elif isinstance(ele,
+                                KsfInterface) and self.with_rpc:
                     element_declares.append(self.parse_interface(ele))
 
             if self.curr_module is not None:
                 module_declares.append(fstr(template_namespace,
                                             module_begin=self.get_ns_begin(self.curr_module),
                                             module_end=self.get_ns_end(self.curr_module),
                                             elements=element_declares
@@ -839,39 +964,23 @@
                               import_headers=self.parse_header(with_ksf=True),
                               namespaces=module_declares
                               )
 
         with self.output_file.open("w") as f:
             f.write(header_content)
 
-    def generate_all(self):
-        self.curr_module = None
-        const_list = []
-        enum_list = []
-        struct_list = []
-        interface_list = []
+    def generate_text(self, modules, with_ksf=False, with_servant=False, includes=[]):
         module_declares = []
-
-        for sym in self.ast.get_all_export_symbol():
-            ele = self.ast.all_element.obj[sym]
-            self.curr_module = ele.module
-
-            if isinstance(ele, KsfConst):
-                const_list.append((ele.module, self.parse_const(ele)))
-            elif isinstance(ele, KsfEnum):
-                enum_list.append((ele.module, self.parse_enum(ele)))
-            elif isinstance(ele, KsfStruct):
-                struct_list.append((ele.module, self.parse_struct(ele)))
-            elif isinstance(ele, KsfInterface) and self.with_rpc:
-                interface_list.append((ele.module, self.parse_interface(ele)))
-
-        # 生成头文件（需要判断是否忽略路径)
         self.curr_module = None
         element_declares = []
-        for module, element_declare in const_list + enum_list + struct_list + interface_list:
+
+        for include in includes:
+            self.add_include(include)
+
+        for module, element_declare in modules:
             if self.curr_module is not None and self.curr_module != module:
                 module_declares.append(fstr(template_namespace,
                                             module_begin=self.get_ns_begin(self.curr_module),
                                             module_end=self.get_ns_end(self.curr_module),
                                             elements=element_declares
                                             )
                                        )
@@ -886,92 +995,170 @@
                                         module_begin=self.get_ns_begin(self.curr_module),
                                         module_end=self.get_ns_end(self.curr_module),
                                         elements=element_declares
                                         )
                                    )
             self.curr_module = None
 
-        header_content = fstr(template_header,
-                              header_description=fstr(template_header_description,
-                                                      file_name=self.output_file.name,
-                                                      date=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
-                                                      version="1.0.0",
-                                                      ),
-                              import_headers=self.parse_header(with_ksf=True),
-                              namespaces=module_declares
-                              )
-        # print(self.file_str)
+        return fstr(template_header,
+                    header_description=fstr(template_header_description,
+                                            file_name=self.output_file.name,
+                                            date=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+                                            version="1.0.0",
+                                            ),
+                    import_headers=self.parse_header(with_ksf=with_ksf, with_servant=with_servant),
+                    namespaces=module_declares
+                    )
 
-        with self.output_file.open("w") as f:
-            f.write(header_content)
+    def generate_all(self,
+                     is_seperate=False):
+        # TODO 调用分离模式，将调用和结构体分离
+        self.curr_module = None
+        const_list = []
+        enum_list = []
+        struct_list = []
+        interface_list = []
+        module_declares = []
+
+        for sym in self.ast.get_all_export_symbol():
+            ele = self.ast.all_element.obj[sym]
+            self.curr_module = ele.module
+
+            if isinstance(ele,
+                          KsfConst):
+                const_list.append((ele.module, self.parse_const(ele)))
+            elif isinstance(ele,
+                            KsfEnum):
+                enum_list.append((ele.module, self.parse_enum(ele)))
+            elif isinstance(ele,
+                            KsfStruct):
+                struct_list.append((ele.module, self.parse_struct(ele)))
+            elif isinstance(ele,
+                            KsfInterface) and self.with_rpc:
+                interface_list.append((ele.module, self.parse_interface(ele)))
+
+        # 生成头文件（需要判断是否忽略路径)
+        if is_seperate:
+            data_list = const_list + enum_list + struct_list
+            if data_list:
+                header_content = self.generate_text(data_list, with_ksf=True, with_servant=False)
+                with self.output_file.open("w") as f:
+                    f.write(header_content)
+
+            if interface_list:
+                header_content = self.generate_text(interface_list,
+                                                    with_ksf=True,
+                                                    with_servant=True,
+                                                    includes=[self.output_file.name])
+                with self.invoke_file.open("w") as f:
+                    f.write(header_content)
+        else:
+            header_content = self.generate_text(const_list + enum_list + struct_list + interface_list,
+                                                with_ksf=True,
+                                                with_servant=True)
+
+            with self.output_file.open("w") as f:
+                f.write(header_content)
 
 
 #############################################################################################################
 
+
 class CppSdkGenerator(CppParser):
-    def __init__(self, ast, repl_ns_dict, repl_inc_dir, destination, push_functions, export_symbols, invoke,
-                 export, **kwargs
+    def __init__(self,
+                 ast,
+                 repl_ns_dict,
+                 repl_inc_dir,
+                 destination,
+                 push_functions,
+                 export_symbols,
+                 invoke,
+                 export,
+                 **kwargs
                  ):
-        super().__init__(ast, repl_ns_dict, repl_inc_dir, destination, push_functions, export_symbols, **kwargs)
+        super().__init__(ast,
+                         repl_ns_dict,
+                         repl_inc_dir,
+                         destination,
+                         push_functions,
+                         export_symbols,
+                         **kwargs)
         self.sdk_invoke = Path(destination) / invoke  # 生成的纯rpc头文件
         self.sdk_export = Path(destination) / export  # 生成的纯结构体头文件
 
-    def parse_enum_pure(self, ksf_enum: KsfEnum):
+    def parse_enum_pure(self,
+                        ksf_enum: KsfEnum):
         enum_members = []
         for m in ksf_enum.member:
             enum_members.append(self.parse_enum_member(m))
 
         return fstr(template_enum,
                     comment=self.parse_comment_above(ksf_enum.comment),
                     enum_name=ksf_enum.name,
                     enum_members=enum_members,
                     )
 
-    def parse_enum_func(self, ksf_enum: KsfEnum):
+    def parse_enum_func(self,
+                        ksf_enum: KsfEnum):
         function_etos = []
         function_stoe = []
         for m in ksf_enum.member:
-            function_etos.append(self.parse_enum_to_str(m, True))
-            function_stoe.append(self.parse_str_to_enum(m, True))
+            function_etos.append(self.parse_enum_to_str(m,
+                                                        True))
+            function_stoe.append(self.parse_str_to_enum(m,
+                                                        True))
 
-        return [fstr(template_etos, enum_name=ksf_enum.name, etos_member=function_etos),
-                fstr(template_stoe, enum_name=ksf_enum.name, stoe_member=function_stoe)]
+        return [fstr(template_etos,
+                     enum_name=ksf_enum.name,
+                     etos_member=function_etos),
+                fstr(template_stoe,
+                     enum_name=ksf_enum.name,
+                     stoe_member=function_stoe)]
 
-    def parse_resetDefault(self, ksf_struct: KsfStruct):
-        return fstr(template_resetDefault, struct_name=ksf_struct.name, )
+    def parse_resetDefault(self,
+                           ksf_struct: KsfStruct):
+        return fstr(template_resetDefault,
+                    struct_name=ksf_struct.name, )
 
-    def parse_variable_writeTo(self, ksf_field: KsfField):
+    def parse_variable_writeTo(self,
+                               ksf_field: KsfField):
         value_type = ksf_field.value_type
-        if self.with_check_default:
-            if isinstance(value_type, KsfBuildInType):
-                if isinstance(value_type, KsfBoolType):
+        if self.with_check_default and not ksf_field.is_required:
+            if isinstance(value_type,
+                          KsfBuildInType):
+                if isinstance(value_type,
+                              KsfBoolType):
                     check_default = f"""{'!' if not ksf_field.has_default() or ksf_field.default['value'] else ''}obj.{ksf_field.name}"""
                 else:
                     check_default = self.parse_default_var(f'obj.{ksf_field.name}',
                                                            value_type,
                                                            ksf_field.default,
                                                            is_equal=False
                                                            )
-            elif isinstance(value_type, KsfStructType):
+            elif isinstance(value_type,
+                            KsfStructType):
                 return fstr(template_writeTo_variable,
                             variable_name=f'obj.{ksf_field.name}',
                             variable_tag=ksf_field.tag, )
-            elif isinstance(value_type, KsfEnumType):
+            elif isinstance(value_type,
+                            KsfEnumType):
                 module_name = f"{value_type.module}::" if self.curr_module != value_type.module else ""
 
                 # 如果是枚举类型
                 if ksf_field.has_default():
                     # 有枚举默认值的，使用默认值
                     check_default = f"""obj.{ksf_field.name} != {module_name}{value_type.name}::{ksf_field.default['value']}"""
                 else:
                     # 没有默认值的，使用第一个枚举值
                     check_default = f"""obj.{ksf_field.name} != {module_name}{value_type.name}::{ksf_field.value_type.obj_type.member[0].name}"""
-            elif isinstance(value_type, KsfVectorType):
+            elif isinstance(value_type,
+                            KsfVectorType):
                 check_default = f"""!obj.{ksf_field.name}.empty()"""
-            elif isinstance(value_type, KsfMapType):
+            elif isinstance(value_type,
+                            KsfMapType):
                 check_default = f"""!obj.{ksf_field.name}.empty()"""
             else:
                 raise SyntaxError(f"不能被解析的字段类型[{value_type}]")
 
             return fstr(template_writeTo_variable_with_check,
                         check_default=check_default,
                         variable_declare=fstr(template_writeTo_variable,
@@ -979,85 +1166,108 @@
                                               variable_tag=ksf_field.tag, ),
                         )
         else:
             return fstr(template_writeTo_variable,
                         variable_name=f'obj.{ksf_field.name}',
                         variable_tag=ksf_field.tag, )
 
-    def parse_writeTo(self, ksf_struct: KsfStruct):
+    def parse_writeTo(self,
+                      ksf_struct: KsfStruct):
         var_list = []
         for var in ksf_struct.variable:
             var_list.append(self.parse_variable_writeTo(ksf_struct.variable[var]))
-        return fstr(template_writeTo, variables=var_list)
+        return fstr(template_writeTo,
+                    variables=var_list)
 
-    def parse_variable_writeToJson(self, ksf_field: KsfField):
-        return f"""p->value["{ksf_field.name}"] = ksf::JsonOutput::writeJson(obj.{ksf_field.name});"""
+    def parse_variable_writeToJson(self,
+                                   ksf_field: KsfField):
+        return f"""p->value["{ksf_field.name}"] = ksf::json::Output::writeJson(obj.{ksf_field.name});"""
 
-    def parse_writeToJson(self, ksf_struct: KsfStruct):
+    def parse_writeToJson(self,
+                          ksf_struct: KsfStruct):
         var_list = []
         for var in ksf_struct.variable.values():
             var_list.append(self.parse_variable_writeToJson(var))
 
-        return fstr(template_writeToJson, variables=var_list)
+        return fstr(template_writeToJson,
+                    variables=var_list)
 
-    def parse_variable_readFrom(self, ksf_field: KsfField):
+    def parse_variable_readFrom(self,
+                                ksf_field: KsfField):
         return f"""_is.read(obj.{ksf_field.name}, {ksf_field.tag}, false);"""
 
-    def parse_readFrom(self, ksf_struct: KsfStruct):
+    def parse_readFrom(self,
+                       ksf_struct: KsfStruct):
         var_list = []
         for var in ksf_struct.variable:
             var_list.append(self.parse_variable_readFrom(ksf_struct.variable[var]))
 
-        return fstr(template_readFrom, variables=var_list)
+        return fstr(template_readFrom,
+                    variables=var_list,
+                    is_wrap=True)
 
-    def parse_variable_readFromJson(self, ksf_field: KsfField):
-        return f"""ksf::JsonInput::readJson(obj.{ksf_field.name}, pObj->value["{ksf_field.name}"], false);"""
+    def parse_variable_readFromJson(self,
+                                    ksf_field: KsfField):
+        return f"""ksf::json::Input::readJson(obj.{ksf_field.name}, pObj->value["{ksf_field.name}"], false);"""
 
-    def parse_readFromJson(self, ksf_struct: KsfStruct):
+    def parse_readFromJson(self,
+                           ksf_struct: KsfStruct):
         var_list = []
         for var in ksf_struct.variable:
             var_list.append(self.parse_variable_readFromJson(ksf_struct.variable[var]))
 
-        return fstr(template_readFromJson, variables=var_list)
+        return fstr(template_readFromJson,
+                    variables=var_list,
+                    is_wrap=True)
 
-    def parse_display(self, ksf_struct: KsfStruct):
+    def parse_display(self,
+                      ksf_struct: KsfStruct):
         var_list = []
         for field in ksf_struct.variable.values():
-            if isinstance(field.value_type, KsfEnumType):
+            if isinstance(field.value_type,
+                          KsfEnumType):
                 var_list.append(f'_ds.display(static_cast<int32_t>(obj.{field.name}), "{field.name}");')
             else:
                 var_list.append(f'_ds.display(obj.{field.name}, "{field.name}");')
 
-        return fstr(template_display, variables=var_list)
+        return fstr(template_display,
+                    variables=var_list)
 
-    def parse_displaySimple(self, ksf_struct: KsfStruct):
+    def parse_displaySimple(self,
+                            ksf_struct: KsfStruct):
         var_list = []
         for field in ksf_struct.variable.values():
-            if isinstance(field.value_type, KsfEnumType):
+            if isinstance(field.value_type,
+                          KsfEnumType):
                 var_list.append(f'_ds.displaySimple(static_cast<int32_t>(obj.{field.name}), true);')
             else:
                 var_list.append(f'_ds.displaySimple(obj.{field.name}, true);')
 
-        return fstr(template_displaySimple, variables=var_list)
+        return fstr(template_displaySimple,
+                    variables=var_list)
 
-    def parse_equal(self, ksf_struct: KsfStruct):
+    def parse_equal(self,
+                    ksf_struct: KsfStruct):
         var_list = []
         for var in ksf_struct.variable:
             field = ksf_struct.variable[var]
-            if isinstance(field.value_type, KsfFloatType):
+            if isinstance(field.value_type,
+                          KsfFloatType):
                 var_list.append(f'ksf::KS_Common::equal(l.{field.name}, r.{field.name})')
             else:
                 var_list.append(f'l.{field.name} == r.{field.name}')
 
         return fstr(template_operator_equal,
                     variables=var_list,
-                    struct_name=self.get_full_name(self.curr_module, ksf_struct.name)
+                    struct_name=self.get_full_name(self.curr_module,
+                                                   ksf_struct.name)
                     )
 
-    def parse_struct_pure(self, ksf_struct: KsfStruct):
+    def parse_struct_pure(self,
+                          ksf_struct: KsfStruct):
         variables = []
         # 解析字段
         var_list = []
         for var in ksf_struct.variable:
             var_list.append(self.parse_variable(ksf_struct.variable[var]))
 
         var_widths = self.get_column_widths(var_list)
@@ -1068,46 +1278,48 @@
         return fstr(template_struct_export,
                     comment=self.parse_comment_above(ksf_struct.comment),
                     struct_name=ksf_struct.name,
                     variables=variables,
                     struct_functions=[self.parse_resetDefault(ksf_struct)]
                     )
 
-    def parse_struct_wrap(self, ksf_struct: KsfStruct):
-        full_struct_name = self.get_full_name(ksf_struct.module, ksf_struct.name)
+    def parse_struct_wrap(self,
+                          ksf_struct: KsfStruct):
+        full_struct_name = self.get_full_name(ksf_struct.module,
+                                              ksf_struct.name)
         struct_functions = [
             self.parse_writeTo(ksf_struct),
             self.parse_readFrom(ksf_struct),
         ]
         struct_operators = [
             self.parse_equal(ksf_struct),
 
         ]
 
         if self.with_json:
-            self.add_include("<kup/KsfJson.h>")
+            self.add_include("ksf/proto/json.h")
             struct_functions.append(self.parse_writeToJson(ksf_struct))  # writeToJson
             struct_functions.append(self.parse_readFromJson(ksf_struct))  # readFromJson
 
-        self.add_include("<ostream>")
+        self.add_include("ostream")
         struct_functions.append(self.parse_display(ksf_struct))  # display
         struct_functions.append(self.parse_displaySimple(ksf_struct))  # displaySimple
 
         if len(ksf_struct.key_fields) != 0:
             key_variables = []
             for key_field in ksf_struct.key_fields:
                 key_variables.append(f'if(l.{key_field} != r.{key_field})  return (l.{key_field} < r.{key_field});')
             struct_operators.append(fstr(template_operator_compare,
                                          struct_name=full_struct_name,
                                          variables=key_variables
                                          )
                                     )
 
         if self.with_json:
-            self.add_include("<kup/KsfJson.h>")
+            self.add_include("ksf/proto/json.h")
             # export
             struct_operators.append(fstr(template_operator_stream_with_json,
                                          wrap_mode=True,
                                          struct_name=full_struct_name
                                          )
                                     )
 
@@ -1116,152 +1328,91 @@
                                          wrap_mode=False,
                                          struct_name=f'{full_struct_name}Wrap'
                                          )
                                     )
 
         return fstr(template_struct_wrap,
                     module_name=self.curr_module,
+                    struct_name_without_namespace=ksf_struct.name,
                     struct_name=full_struct_name,
                     md5sum=md5(ksf_struct.id.encode('utf8')).hexdigest(),
                     struct_functions=struct_functions,
                     struct_operators=struct_operators,
                     namespace_left=self.get_ns_begin(self.curr_module),
                     namespace_right=self.get_ns_end(self.curr_module),
                     )
 
-    def parse_InterfacePrxCallBack(self, ksf_interface: KsfInterface):
-        prx_str = f"""\
-class {ksf_interface.name}WrapPrxCallback : public ksf::AgentCallback
-{{
-public:
-    virtual ~{ksf_interface.name}WrapPrxCallback() = default;
-
-public:
-\n"""
-
-        index = 0
-        func_case_str = ""
-        for item in ksf_interface.operator:
-            operator = ksf_interface.operator[item]
-            if not operator.export:
-                continue
-
-            def parse_output_vars(with_type=True):
-                def parse_output_var(value_type, name, with_type):
-                    if value_type.name != 'void':
-                        if not self.is_movable_type(value_type):
-                            return f"{self.parse_type(value_type, is_wrap=True)} {name}" if with_type else name
-                        elif self.with_rvalue_ref:
-                            return f"{self.parse_type(value_type, is_wrap=True)} &&{name}" if with_type else f"std::move({name})"
-                        else:
-                            return f"const {self.parse_type(value_type, is_wrap=True)} &{name}" if with_type else name
-
-                vars_list = []
-                if operator.return_type['name'] != 'void':
-                    vars_list.append(parse_output_var(operator.return_type, '_ret', with_type))
-
-                for i in operator.output:
-                    vars_list.append(
-                        parse_output_var(operator.output[i].value_type, operator.output[i].name, with_type)
-                    )
-
-                return ', '.join(vars_list)
-
-            prx_str += f"""\
-    virtual void callback_{operator.name}Wrap({parse_output_vars(True)}) \
-{{ throw std::runtime_error("callback_{operator.name}Wrap override incorrect."); }}
-
-    virtual void callback_{operator.name}Wrap_exception(int32_t ret) \
-{{ throw std::runtime_error("callback_{operator.name}Wrap_exception override incorrect."); }}
-
-"""
-
-            def parse_var_dispatch(var, name, index):
-                if var['name'] == 'void':
-                    return ""
-
-                return f"""\
-                {self.parse_type(var, is_wrap=True)} {name};
-                _is.read({name}, {index}, true);\n\n"""
-
-            def parse_func_dispatch():
-                """处理函数的分发"""
-                func_case_str = f"""
-            case {index}: {{
-                if (msg->response->iRet != ksf::KSFSERVERSUCCESS) {{
-                    callback_{operator.name}Wrap_exception(msg->response->iRet);
-                    return msg->response->iRet;
-                }}
-
-                ksf::KsfInputStream<ksf::BufferReader> _is;
-
-                _is.setBuffer(msg->response->sBuffer);\n\n"""
-
-                func_case_str += parse_var_dispatch(operator.return_type, '_ret', 0)
-
-                for i in operator.output:
-                    var = operator.output[i]
-                    func_case_str += parse_var_dispatch(var.value_type, var.name, var.index)
-
-                func_case_str += f"""\
-
-                ksf::CallbackThreadData *pCbtd = ksf::CallbackThreadData::getData();
-                assert(pCbtd != NULL);
-
-                pCbtd->setResponseContext(msg->response->context);
-
-                callback_{operator.name}Wrap({parse_output_vars(False)});
-
-                pCbtd->delResponseContext();
-
-                return ksf::KSFSERVERSUCCESS;
-            }}"""
-                return func_case_str
-
-            func_case_str += parse_func_dispatch()
-            index += 1
-
-        # 函数列表
-        prx_str += f"""\
-public:
-    virtual const std::map<std::string, std::string> &getResponseContext() const {{
-        ksf::CallbackThreadData *pCbtd = ksf::CallbackThreadData::getData();
-        assert(pCbtd != NULL);
+    def parse_InterfacePrxCallBack(self,
+                                   ksf_interface: KsfInterface):
+        func_case_list = []
+        function_handles = []
+        dispatch_str = []
 
-        if (!pCbtd->getContextValid()) {{
-            throw ksf::KS_Exception("cann't get response context");
-        }}
-        return pCbtd->getResponseContext();
-    }}\n\n"""
+        def parse_func_dispatch(index,
+                                operator):
+            """处理函数的分发"""
+            output_args = []
 
-        prx_str += f"""\
-public:
-    int onDispatch(ksf::ReqMessagePtr msg) override {{
-        static std::string __{ksf_interface.name}_all[] = {{"{'", "'.join(ksf_interface.operator.keys())}"}};
+            if operator.has_return():
+                output_args.append(fstr(template_output_argument_parse,
+                                        typename=self.parse_type(operator.return_type,
+                                                                 is_wrap=True),
+                                        argument_name='_ret',
+                                        index=0
+                                        )
+                                   )
 
-        std::pair<std::string *, std::string *> r = equal_range(__{ksf_interface.name}_all, __{ksf_interface.name}_all + {len(ksf_interface.operator.keys())}, std::string(msg->request.sFuncName));
+            for var in operator.output.values():
+                output_args.append(fstr(template_output_argument_parse,
+                                        typename=self.parse_type(var.value_type,
+                                                                 is_wrap=True),
+                                        argument_name=var.name,
+                                        index=var.index
+                                        )
+                                   )
 
-        if (r.first == r.second) {{
-            return ksf::KSFSERVERNOFUNCERR;
-        }}
+            func_case_list.append(fstr(template_dispatch_case_at_client,
+                                       case=index,
+                                       function_name=f'{operator.name}Wrap',
+                                       output_params=self.parse_output_vars(operator,
+                                                                            False),
+                                       output_arguments=output_args
+                                       )
+                                  )
 
-        switch (r.first - __{ksf_interface.name}_all) {{
-{func_case_str}
-        }} //end switch
+            function_handles.append(fstr(template_function_call,
+                                         function_name=f'{operator.name}Wrap',
+                                         arguments=self.parse_output_vars(operator,
+                                                                          True)
+                                         )
+                                    )
 
-        return ksf::KSFSERVERNOFUNCERR;
-    }} //end onDispatch\n"""
+        get_response_context = template_getResponseContext
 
-        prx_str += f"""}}; //end {ksf_interface.name}PrxCallback
+        def dispatch(function_names):
+            dispatch_str.append(fstr(template_array_style_onDispatch_at_client,
+                                     dispatch_case_str=func_case_list,
+                                     interface_name=f'{ksf_interface.name}Wrap',
+                                     function_names=function_names
+                                     )
+                                )
 
-using {ksf_interface.name}WrapPrxCallbackPtr = ksf::KS_AutoPtr<{ksf_interface.name}WrapPrxCallback>;\n\n"""
+        self.parse_DispatchOperatorCallBack(ksf_interface,
+                                            dispatch,
+                                            parse_func_dispatch)
 
-        return prx_str
+        return fstr(template_callback,
+                    interface_name=f'{ksf_interface.name}Wrap',
+                    function_handles=function_handles,
+                    get_response_context=get_response_context,
+                    dispatch_str=dispatch_str
+                    )
 
-    def parse_InterfacePrxCallbackPromise(self, ksf_interface: KsfInterface):
+    def parse_InterfacePrxCallbackPromise(self,
+                                          ksf_interface: KsfInterface):
         parsed_str = f"""\
 class {ksf_interface.name}WrapPrxCallbackPromise: public ksf::AgentCallback
 {{
 public:
     virtual ~{ksf_interface.name}WrapPrxCallbackPromise() = default;
 \n"""
 
@@ -1305,15 +1456,17 @@
         oss << ret;
         _promise_{operator.name}.setException(ksf::copyException(oss.str(), ret));
     }}
 
 protected:
     ksf::Promise<{ksf_interface.name}WrapPrxCallbackPromise::Promise{operator.name}Ptr > _promise_{operator.name};\n\n"""
 
-            def parse_var_dispatch(var, name, index):
+            def parse_var_dispatch(var,
+                                   name,
+                                   index):
                 if var['name'] == 'void':
                     return ""
 
                 return f"""\
                     _is.read(ptr->{name}, {index}, true);\n"""
 
             def parse_func_dispatch():
@@ -1328,21 +1481,25 @@
                 ksf::KsfInputStream<ksf::BufferReader> _is;
                 _is.setBuffer(msg->response->sBuffer);
                 {ksf_interface.name}WrapPrxCallbackPromise::Promise{operator.name}Ptr ptr = new {ksf_interface.name}WrapPrxCallbackPromise::Promise{operator.name}();
 
                 try {{\n"""
 
                 func_case_list = []
-                ret = parse_var_dispatch(operator.return_type, '_ret', 0)
+                ret = parse_var_dispatch(operator.return_type,
+                                         '_ret',
+                                         0)
                 if ret != "":
                     func_case_list.append(ret)
 
                 for item2 in operator.output:
                     var2 = operator.output[item2]
-                    func_case_list.append(parse_var_dispatch(var2.value_type, var2.name, var2.index))
+                    func_case_list.append(parse_var_dispatch(var2.value_type,
+                                                             var2.name,
+                                                             var2.index))
 
                 func_case_str += ''.join(func_case_list)
                 return func_case_str
 
             case_index += 1
             dispatch_case_str += parse_func_dispatch()
             dispatch_case_str += f"""\
@@ -1380,16 +1537,19 @@
     }} //end onDispatch\n"""
 
         parsed_str += f"\n}}; //end {ksf_interface.name}WrapPrxCallbackPromise\n\n" \
                       f"using {ksf_interface.name}WrapPrxCallbackPromisePtr = ksf::KS_AutoPtr<{ksf_interface.name}WrapPrxCallbackPromise>;\n" \
                       f"\n"
         return parsed_str
 
-    def parse_InterfaceCoroPrxCallback(self, ksf_interface: KsfInterface):
-        def parse_var_dispatch(var, name, index):
+    def parse_InterfaceCoroPrxCallback(self,
+                                       ksf_interface: KsfInterface):
+        def parse_var_dispatch(var,
+                               name,
+                               index):
             if var['name'] == 'void':
                 return ""
 
             return f"""\
                     {self.parse_type(var)} {name};
                     _is.read({name}, {index}, true);\n\n"""
 
@@ -1400,30 +1560,36 @@
             for item in ksf_interface.operator:
                 operator = ksf_interface.operator[item]
                 if not operator.export:
                     index += 1
                     continue
 
                 def parse_output_vars(with_type=True):
-                    def parse_output_var(value_type, name, with_type):
+                    def parse_output_var(value_type,
+                                         name,
+                                         with_type):
                         if value_type.name != 'void':
                             if not self.is_movable_type(value_type):
                                 return f"{self.parse_type(value_type)} {name}" if with_type else name
                             elif self.with_rvalue_ref:
                                 return f"{self.parse_type(value_type)} &&{name}" if with_type else f"std::move({name})"
                             else:
                                 return f"const {self.parse_type(value_type)} &{name}" if with_type else name
 
                     vars_list = []
                     if operator.return_type.name != 'void':
-                        vars_list.append(parse_output_var(operator.return_type, '_ret', with_type))
+                        vars_list.append(parse_output_var(operator.return_type,
+                                                          '_ret',
+                                                          with_type))
 
                     for item in operator.output:
                         vars_list.append(
-                            parse_output_var(operator.output[item].value_type, operator.output[item].name, with_type)
+                            parse_output_var(operator.output[item].value_type,
+                                             operator.output[item].name,
+                                             with_type)
                         )
 
                     return ', '.join(vars_list)
 
                 func_case_str += f"""
             case {index}: {{
                 if (msg->response->iRet != ksf::KSFSERVERSUCCESS) {{
@@ -1432,21 +1598,25 @@
                 }}
 
                 ksf::KsfInputStream<ksf::BufferReader> _is;
                 _is.setBuffer(msg->response->sBuffer);
 
                 try {{\n"""
                 func_case_list = []
-                ret = parse_var_dispatch(operator.return_type, '_ret', 0)
+                ret = parse_var_dispatch(operator.return_type,
+                                         '_ret',
+                                         0)
                 if ret != "":
                     func_case_list.append(ret)
 
                 for item2 in operator.output:
                     var2 = operator.output[item2]
-                    func_case_list.append(parse_var_dispatch(var2.value_type, var2.name, var2.index))
+                    func_case_list.append(parse_var_dispatch(var2.value_type,
+                                                             var2.name,
+                                                             var2.index))
 
                 func_case_str += ''.join(func_case_list)
 
                 func_case_str += f"""\
                     callback_{operator.name}Wrap({parse_output_vars(with_type=False)});
                 }} catch (std::exception &ex) {{
                     callback_{operator.name}Wrap_exception(ksf::KSFCLIENTDECODEERR);
@@ -1496,15 +1666,16 @@
 protected:
     std::map<std::string, std::string> _mRspContext;
 }}; //end {ksf_interface.name}WrapCoroPrxCallback
 
 using {ksf_interface.name}WrapCoroPrxCallbackPtr = ksf::KS_AutoPtr<{ksf_interface.name}WrapCoroPrxCallback>;\n\n"""
         return parsed_str
 
-    def parse_InterfaceProxy(self, ksf_interface: KsfInterface):
+    def parse_InterfaceProxy(self,
+                             ksf_interface: KsfInterface):
         def parse_operators():
             parsed_oper_str = ""
             for item in ksf_interface.operator:
                 operator = ksf_interface.operator[item]
                 if not operator.export:
                     continue
 
@@ -1617,22 +1788,23 @@
 {parse_operators()}
 }}; //end {ksf_interface.name}WrapProxy
 
 using {ksf_interface.name}WrapPrx = ksf::KS_AutoPtr<{ksf_interface.name}WrapProxy>;\n\n"""
 
         return parsed_str
 
-    def parse_interface(self, ksf_interface: KsfInterface):
+    def parse_interface(self,
+                        ksf_interface: KsfInterface):
         interface_declare = []
 
-        self.add_include("<servant/Agent.h>")
-        self.add_include("<servant/Servant.h>")
+        self.add_include("servant/Agent.h")
+        self.add_include("servant/Servant.h")
 
         interface_declare.append(self.parse_InterfacePrxCallBack(ksf_interface))
-        self.add_include("<promise/promise.h>")
+        self.add_include("promise/promise.h")
         interface_declare.append(self.parse_InterfacePrxCallbackPromise(ksf_interface))
         interface_declare.append(self.parse_InterfaceCoroPrxCallback(ksf_interface))
         interface_declare.append(self.parse_InterfaceProxy(ksf_interface))
 
         return fstr(template_namespace,
                     module_begin=self.get_ns_begin(self.curr_module),
                     module_end=self.get_ns_end(self.curr_module),
@@ -1652,26 +1824,30 @@
         hidden_str = []
         export_str = ''
 
         for sym in self.ast.get_all_export_symbol():
             ele = self.ast.all_element.obj[sym]
             self.curr_module = ele.module
 
-            if isinstance(ele, KsfConst):
+            if isinstance(ele,
+                          KsfConst):
                 const_list.append((ele.module, self.parse_const(ele)))
                 pass
-            elif isinstance(ele, KsfEnum):
+            elif isinstance(ele,
+                            KsfEnum):
                 enum_list.append((ele.module, self.parse_enum_pure(ele)))
                 invoke_module_declares.append(self.parse_enum_func(ele))
                 pass
-            elif isinstance(ele, KsfStruct):
+            elif isinstance(ele,
+                            KsfStruct):
                 struct_list.append((ele.module, self.parse_struct_pure(ele)))
                 invoke_module_declares.append(self.parse_struct_wrap(ele))
                 pass
-            elif isinstance(ele, KsfInterface) and self.with_rpc:
+            elif isinstance(ele,
+                            KsfInterface) and self.with_rpc:
                 invoke_module_declares.append(self.parse_interface(ele))
 
         self.curr_module = None
         element_declares = []
         for module, element_declare in const_list + enum_list + struct_list:
             if self.curr_module is not None and self.curr_module != module:
                 export_module_declares.append(fstr(template_namespace,
@@ -1681,14 +1857,16 @@
                                                    )
                                               )
                 element_declares = []
             self.curr_module = module
 
             element_declares.append(element_declare)
 
+        self.add_include("ksf/proto/proto.h")
+
         if self.curr_module is not None:
             export_module_declares.append(fstr(template_namespace,
                                                module_begin=self.get_ns_begin(self.curr_module),
                                                module_end=self.get_ns_end(self.curr_module),
                                                elements=element_declares
                                                )
                                           )
@@ -1700,14 +1878,15 @@
                                                            date=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
                                                            version="1.0.0",
                                                            ),
                                    import_headers=self.parse_header(with_ksf=False),
                                    namespaces=export_module_declares
                                    )
 
+        self.add_include(self.sdk_export.name)
         invoke_file_declare = fstr(template_header,
                                    header_description=fstr(template_header_description,
                                                            file_name=self.sdk_invoke.name,
                                                            date=datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
                                                            version="1.0.0",
                                                            ),
                                    import_headers=self.parse_header(with_ksf=True),
@@ -1717,56 +1896,96 @@
         with self.sdk_export.open("w") as f:
             f.write(export_file_declare)
 
         with self.sdk_invoke.open("w") as f:
             f.write(invoke_file_declare)
 
 
-def cpp_gen(mode, files,
+def cpp_gen(mode,
+            files,
             replace_namespace,
             replace_include_path,
             include_path,
             destination_path,
             push_function,
             export_symbol,
             dispatch_mode,
-            flags: dict, **kwargs
+            flags: dict,
+            **kwargs
             ):
     """生成cpp文件"""
     if flags is None:
         flags = defaultdict(bool)
 
     file_path = files
 
     real_inc_dirs = set()
     for inc in include_path:
         real_inc_dirs.add(str(Path(inc).resolve()))
 
     if mode == 'file':
-        ast = generate(file_path, real_inc_dirs, flags['with_current_priority'], [])
+        ast = generate(file_path,
+                       real_inc_dirs,
+                       flags['with_current_priority'],
+                       [])
         for file in ast.files.values():
             if file.is_source:
                 output_file = f"{file.path.name[:-4]}.h"
-                CppGenerator(ast, replace_namespace, replace_include_path, destination_path, push_function,
-                             input_file=[file], output_file=output_file, dispatch_mode=dispatch_mode,
+                CppGenerator(ast,
+                             replace_namespace,
+                             replace_include_path,
+                             destination_path,
+                             push_function,
+                             input_file=[file],
+                             output_file=output_file,
+                             invoke_file=kwargs['invoke_file'],
+                             dispatch_mode=dispatch_mode,
                              **flags
                              ).generate()
-    elif mode in ('export_import', 'all_in_one'):
-        ast = generate(file_path, real_inc_dirs, flags['with_current_priority'], export_symbol)
+    elif mode in ('export_import', 'all_in_one', 'invoke_separate'):
+        ast = generate(file_path,
+                       real_inc_dirs,
+                       flags['with_current_priority'],
+                       export_symbol)
         if mode == 'export_import':
-            CppSdkGenerator(ast, replace_namespace, replace_include_path, destination_path, push_function,
+            CppSdkGenerator(ast,
+                            replace_namespace,
+                            replace_include_path,
+                            destination_path,
+                            push_function,
                             export_symbol,
-                            invoke=kwargs['invoke_file'], export=kwargs['export_file'], dispatch_mode=dispatch_mode,
+                            invoke=kwargs['invoke_file'],
+                            export=kwargs['export_file'],
+                            dispatch_mode=dispatch_mode,
                             **flags
                             ).generate()
-        else:
-            CppGenerator(ast, replace_namespace, replace_include_path, destination_path, push_function,
-                         input_file=ast.files.values(), output_file=kwargs['output_file'], dispatch_mode=dispatch_mode,
+        elif mode == 'all_in_one':
+            CppGenerator(ast,
+                         replace_namespace,
+                         replace_include_path,
+                         destination_path,
+                         push_function,
+                         input_file=ast.files.values(),
+                         output_file=kwargs['output_file'],
+                         invoke_file=kwargs['invoke_file'],
+                         dispatch_mode=dispatch_mode,
                          **flags
                          ).generate_all()
+        else:
+            CppGenerator(ast,
+                         replace_namespace,
+                         replace_include_path,
+                         destination_path,
+                         push_function,
+                         input_file=ast.files.values(),
+                         output_file=kwargs['output_file'],
+                         invoke_file=kwargs['invoke_file'],
+                         dispatch_mode=dispatch_mode,
+                         **flags
+                         ).generate_all(is_seperate=True)
     else:
         raise RuntimeError(f"未知的模式 {mode}")
 
 
 # 测试用例
 if __name__ == '__main__':
     file_path = [
@@ -1775,9 +1994,19 @@
         'example/struct_simple.ksf'
     ]
 
     include_path = ['../../']
 
     destination_path = '../../../gen'
 
-    cpp_gen('file', file_path, {}, {}, include_path, destination_path)
-    cpp_gen('export_import', file_path, {}, {}, include_path, destination_path)
+    cpp_gen('file',
+            file_path,
+            {},
+            {},
+            include_path,
+            destination_path)
+    cpp_gen('export_import',
+            file_path,
+            {},
+            {},
+            include_path,
+            destination_path)
```

### Comparing `ksfctl-0.2.3/ksfctl/generate/cpp/parser.py` & `ksfctl-0.2.4/ksfctl/generate/cpp/parser.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,56 +13,59 @@
                  dispatch_mode,
                  **kwargs
                  ):
         self.__dict__.update(kwargs)
         self.ast = ast
         self.curr_module = None
 
-        Path(destination).mkdir(parents=True, exist_ok=True)
+        Path(destination).mkdir(parents=True,
+                                exist_ok=True)
         self.dest_path = Path(destination)
         self.repl_ns_dict = repl_ns_dict  # 命名空间替换字典
         self.repl_inc_dir = repl_inc_dir  # 头文件替换字典
         self.push_functions = push_functions  # 推送函数列表
         self.export_symbols = export_symbols  # 导出符号列表
         self.dispatch_mode = dispatch_mode  # 分发模式[支持array, set, hash]
 
         self.inc_ordered = [[
-            "<ostream>",
-            "<string>",
-            "<vector>",
-            "<set>",
-            "<unordered_set>",
-            "<map>",
-            "<unordered_map>",
-        ], ["<kup/Ksf.h>",
-            "<kup/KsfJson.h>",
-            "<servant/Agent.h>",
-            "<servant/Servant.h>",
-            "<promise/promise.h>", ]]
+            "ostream",
+            "string",
+            "vector",
+            "set",
+            "unordered_set",
+            "map",
+            "unordered_map",
+        ], [
+            "ksf/proto/proto.h",
+            "ksf/proto/json.h"
+        ], [
+            "servant/Agent.h",
+            "servant/Servant.h",
+            "promise/promise.h", ]]
 
         self.inc_native = {
-            "<ostream>": False,
-            "<string>": True,
-            "<vector>": False,
-            "<set>": False,
-            "<unordered_set>": False,
-            "<map>": False,
-            "<unordered_map>": False,
-            "<kup/Ksf.h>": False,
-            "<kup/KsfJson.h>": False,
-            "<servant/Agent.h>": False,
-            "<servant/Servant.h>": False,
-            "<promise/promise.h>": False,
+            "ostream": False,
+            "string": True,
+            "vector": False,
+            "set": False,
+            "unordered_set": False,
+            "map": False,
+            "unordered_map": False,
+            "ksf/proto/proto.h": False,
+            "ksf/proto/json.h": False,
+            "servant/Agent.h": False,
+            "servant/Servant.h": False,
+            "promise/promise.h": False,
         }
-        self.inc_depends = {
-        }
-        self.curr_tab = ''
+        self.inc_depends = set()
 
-    def __getattr__(self, name):
-        if name.startswith('with_') and not hasattr(self, 'name'):
+    def __getattr__(self,
+                    name):
+        if name.startswith('with_') and not hasattr(self,
+                                                    'name'):
             return False
         return super().__getattr__(name)
 
     @staticmethod
     def endl():
         return '\n'
 
@@ -70,274 +73,334 @@
     def get_column_widths(lst):
         # 创建一个空列表来保存每列的最大宽度
         column_widths = [0] * len(lst[0])
 
         # 遍历列表中的所有元素，找到每列的最大宽度
         for item in lst:
             for i, value in enumerate(item):
-                column_widths[i] = max(column_widths[i], len(value))
+                column_widths[i] = max(column_widths[i],
+                                       len(value))
 
         return column_widths
 
-    def add_include(self, header):
+    def add_include(self,
+                    header):
         """添加头文件"""
         if header in self.inc_native:
             self.inc_native[header] = True
-        elif header in self.inc_depends:
-            self.inc_native[header] = True
+        else:
+            self.inc_depends.add(header)
 
-    def enable_push(self, operator_name):
+    def enable_push(self,
+                    operator_name):
         """启用推送函数"""
         if operator_name in self.push_functions:
             return True
         return False
 
-    def enable_async_rsp(self, operator_name):
+    def enable_async_rsp(self,
+                         operator_name):
         """启用异步响应"""
         if not self.push_functions or operator_name not in self.push_functions:
             return True
         return False
 
-    def has_return(self, operator):
-        return not isinstance(operator.return_type, KsfVoidType)
-
-    def get_repl_headfile(self, header):
-        if header[1:-1] in self.repl_inc_dir:
-            return f'"{self.repl_inc_dir[header[1:-1]]}"'
+    def has_return(self,
+                   operator):
+        return not isinstance(operator.return_type,
+                              KsfVoidType)
+
+    def get_repl_headfile(self,
+                          header):
+        if header in self.repl_inc_dir:
+            return self.repl_inc_dir[header]
         return header
 
-    def get_module(self, module):
+    def get_module(self,
+                   module):
         if module in self.repl_ns_dict:
             return self.repl_ns_dict[module]
         return module
 
-    def get_full_name(self, module, name):
+    def get_full_name(self,
+                      module,
+                      name):
         return f"{self.get_module(module)}::{name}"
 
-    def get_ns_begin(self, module, with_endl=True):
+    def get_ns_begin(self,
+                     module,
+                     with_endl=True):
         if self.with_cxx17:
             return f"""namespace {self.get_module(module)} {{"""
         """获取命名空间开始，将::替换为{"""
         ns = self.get_module(module)
         braces = ""
         for ns_simple in ns.split('::'):
             braces += f'namespace {ns_simple} {{{self.endl() if with_endl else " "}'
         return f"{braces}"
 
-    def get_ns_end(self, module, with_endl=True):
+    def get_ns_end(self,
+                   module,
+                   with_endl=True):
         if self.with_cxx17:
             return f"""}} // namespace {self.get_module(module)}"""
 
         """获取命名空间结束，有多少::就有多少}"""
         ns = self.get_module(module)
         braces = ""
         for ns_simple in ns.split('::'):
             braces = f'}} {f"// namespace {ns_simple}{self.endl()}" if with_endl else ""}{braces}'
         return f"{braces}"
 
-    def parse_header(self, with_ksf):
-        output = ""
+    def parse_header(self,
+                     with_ksf=True,
+                     with_servant=True):
+        output = []
         for header in self.inc_ordered[0]:
             if self.inc_native[header]:
-                output += "#include " + header + "\n"
-
-        output += "\n"
+                output.append(f'''#include <{header}>''')
 
+        output.append('')
         if with_ksf:
             for header in self.inc_ordered[1]:
                 if self.inc_native[header]:
-                    output += "#include " + header + "\n"
+                    output.append(f'''#include <{header}>''')
+
+        if with_servant:
+            for header in self.inc_ordered[2]:
+                if self.inc_native[header]:
+                    output.append(f'''#include <{header}>''')
+
+        output.append('')
+        for header in self.inc_depends:
+            output.append(f'''#include "{self.get_repl_headfile(header)}"''')
         return output
 
-    def is_movable_type(self, value_type):
+    def is_movable_type(self,
+                        value_type):
         """判断是否是可以进行std::move的类型"""
-        if isinstance(value_type, KsfStringType):
+        if isinstance(value_type,
+                      KsfStringType):
             return True
-        elif isinstance(value_type, (KsfStructType, KsfEnumType)):
-            if hasattr(value_type, 'module'):
+        elif isinstance(value_type,
+                        (KsfStructType, KsfEnumType)):
+            if hasattr(value_type,
+                       'module'):
                 class_full_name = value_type['module'] + "." + value_type['name']
             else:
                 class_full_name = self.curr_module + "." + value_type['name']
 
             return class_full_name not in self.ast.enums
-        elif isinstance(value_type, KsfVectorType):
+        elif isinstance(value_type,
+                        KsfVectorType):
             return True
-        elif isinstance(value_type, KsfMapType):
+        elif isinstance(value_type,
+                        KsfMapType):
             return True
         else:
             return False
 
-    def parse_type(self, value_type: KsfType, is_wrap=False):
-        if isinstance(value_type, KsfBuildInType):
-            if isinstance(value_type, KsfIntType):
+    def parse_type(self,
+                   value_type: KsfType,
+                   is_wrap=False):
+        if isinstance(value_type,
+                      KsfBuildInType):
+            if isinstance(value_type,
+                          KsfIntType):
                 if value_type.bit == 8:
                     return f'{"unsigned char" if value_type.is_unsigned else "char"}'
                 return f'{"u" if value_type.is_unsigned else ""}int{value_type.bit}_t'
-            elif isinstance(value_type, KsfFloatType):
+            elif isinstance(value_type,
+                            KsfFloatType):
                 return value_type.name
-            elif isinstance(value_type, KsfStringType):
-                self.add_include(f"<string>")
+            elif isinstance(value_type,
+                            KsfStringType):
+                self.add_include(f"string")
                 return 'std::string'
-            elif isinstance(value_type, KsfBoolType):
+            elif isinstance(value_type,
+                            KsfBoolType):
                 return 'bool'
             else:
                 raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
-        elif isinstance(value_type, (KsfStructType, KsfEnumType)):
+        elif isinstance(value_type,
+                        (KsfStructType, KsfEnumType)):
             if value_type.module is not None and self.curr_module != value_type.module:
                 return self.get_module(value_type['module']) + "::" + value_type.name + ("Wrap" if is_wrap else "")
             else:
                 return value_type.name + ("Wrap" if is_wrap else "")
-        elif isinstance(value_type, KsfVectorType):
+        elif isinstance(value_type,
+                        KsfVectorType):
             if value_type.is_ordered and not value_type.is_hashed and not value_type.is_unique_member:
                 true_type = 'std::vector'
-                self.add_include('<vector>')
+                self.add_include("vector")
             elif value_type.is_ordered and not value_type.is_hashed and value_type.is_unique_member:
                 true_type = 'std::set'
-                self.add_include('<set>')
+                self.add_include("set")
             elif not value_type.is_ordered and value_type.is_hashed and value_type.is_unique_member:
                 true_type = 'std::unordered_set'
-                self.add_include('<unordered_set>')
+                self.add_include("unordered_set")
             else:
                 raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
 
             return f"{true_type}<{self.parse_type(value_type.value_type, is_wrap=is_wrap)}>"
-        elif isinstance(value_type, KsfMapType):
+        elif isinstance(value_type,
+                        KsfMapType):
             if not value_type.is_ordered and value_type.is_hashed and value_type.is_unique_member:
                 true_type = 'std::unordered_map'
-                self.add_include('<unordered_map>')
+                self.add_include("unordered_map")
             elif value_type.is_ordered and not value_type.is_hashed and value_type.is_unique_member:
                 true_type = 'std::map'
-                self.add_include('<map>')
+                self.add_include('map')
             else:
                 raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
             return f"{true_type}<{self.parse_type(value_type.key_type, is_wrap=is_wrap)}, {self.parse_type(value_type.value_type, is_wrap=is_wrap)}>"
 
         raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
 
-    def parse_comment_above(self, comment, tab=None):
+    def parse_comment_above(self,
+                            comment):
         if comment is None or comment == '':
             return ''
 
-        if tab is None:
-            tab = self.curr_tab
-
         comment_lines = comment.split('\n')
         if len(comment_lines) == 1:
-            return f"{tab}//{comment}\n"
+            return f"//{comment}\n"
         else:
-            import re
-            matches = re.findall(r"\s+\*\s+(.*)\n", f"/*{comment}*/")
-            comment_str = f'{tab}/**\n'
-
-            # 将每行注释内容拼接为Python风格的注释
-            for match in matches:
-                comment_str += f"{tab} * {match}\n"
-            comment_str += f'{tab} */\n'
-            return comment_str
+            return self.add_lines(f"/*{comment}*/") + '\n'
 
-    def parse_comment_line(self, comment):
+    def parse_comment_line(self,
+                           comment):
         if comment is None or comment == '':
             return ''
 
         comment_lines = comment.split('\n')
         if len(comment_lines) == 1:
             return f"//{comment}"
         else:
             raise SyntaxError("不支持的注释方式")
 
-    def parse_value(self, value):
+    def parse_value(self,
+                    value):
         return value['value'] if value['is_number'] else f'"{value["value"]}"'
 
-    def parse_const(self, ksf_const: KsfConst):
-        if isinstance(ksf_const.value_type, KsfStringType):
-            return f"{self.parse_comment_above(ksf_const.comment)}{self.curr_tab}constexpr const char *{ksf_const.name} = {self.parse_value(ksf_const.value)};"
-        return f"{self.parse_comment_above(ksf_const.comment)}{self.curr_tab}constexpr {self.parse_type(ksf_const.value_type)} {ksf_const.name} = {self.parse_value(ksf_const.value)};"
-
-    def parse_enum_member(self, ksf_enum_member: KsfEnumMember):
-        return f"{self.curr_tab}{ksf_enum_member.name} = {ksf_enum_member.value},"
-
-    def parse_enum_to_str(self, ksf_enum_member: KsfEnumMember, with_module=False):
+    def parse_const(self,
+                    ksf_const: KsfConst):
+        if isinstance(ksf_const.value_type,
+                      KsfStringType):
+            return f"{self.parse_comment_above(ksf_const.comment)}constexpr const char *{ksf_const.name} = {self.parse_value(ksf_const.value)};"
+        return f"{self.parse_comment_above(ksf_const.comment)}constexpr {self.parse_type(ksf_const.value_type)} {ksf_const.name} = {self.parse_value(ksf_const.value)};"
+
+    def parse_enum_member(self,
+                          ksf_enum_member: KsfEnumMember):
+        return f"{ksf_enum_member.name} = {ksf_enum_member.value},"
+
+    def parse_enum_to_str(self,
+                          ksf_enum_member: KsfEnumMember,
+                          with_module=False):
         if with_module:
             return f"case {self.curr_module}::{ksf_enum_member.name}: return \"{ksf_enum_member.name}\";"
         else:
             return f"case {ksf_enum_member.name}: return \"{ksf_enum_member.name}\";"
 
-    def parse_str_to_enum(self, ksf_enum_member: KsfEnumMember, with_module=False):
+    def parse_str_to_enum(self,
+                          ksf_enum_member: KsfEnumMember,
+                          with_module=False):
         if with_module:
             return f"if (s == \"{ksf_enum_member.name}\") {{ e = {self.curr_module}::{ksf_enum_member.name}; return 0; }}"
         else:
             return f"if (s == \"{ksf_enum_member.name}\") {{ e = {ksf_enum_member.name}; return 0; }}"
 
-    def parse_default_var(self, name, value_type, default, is_equal=True):
+    def parse_default_var(self,
+                          name,
+                          value_type,
+                          default,
+                          is_equal=True):
         if default is None:
-            if isinstance(value_type, KsfIntType):
+            if isinstance(value_type,
+                          KsfIntType):
                 return f'''{name} {"=" if is_equal else "!"}= 0'''
-            elif isinstance(value_type, KsfFloatType):
+            elif isinstance(value_type,
+                            KsfFloatType):
                 if value_type.bit == 32:
                     return f'{"" if is_equal else "!"}ksf::KS_Common::equal(0.0f, {name})'
                 else:
                     return f'{"" if is_equal else "!"}ksf::KS_Common::equal(0.0, {name})'
-            elif isinstance(value_type, KsfBoolType):
+            elif isinstance(value_type,
+                            KsfBoolType):
                 return f'{"" if is_equal else "!"}{name}'
-            elif isinstance(value_type, KsfStringType):
+            elif isinstance(value_type,
+                            KsfStringType):
                 return f'{"" if is_equal else "!"}{name}.empty()'
 
             return ''
 
         # 特殊处理一下bool型
         if default['is_bool']:
             return f'{"" if default["value"] == is_equal else "!"}{name}'
         elif default['is_number']:
-            if isinstance(value_type, KsfFloatType):
+            if isinstance(value_type,
+                          KsfFloatType):
                 if value_type.bit == 32:
                     return f'{"" if default["value"] == is_equal else "!"}ksf::KS_Common::equal({name}, {default["value"]}f)'
                 else:
                     return f'{"" if default["value"] == is_equal else "!"}ksf::KS_Common::equal({name}, {default["value"]})'
             return f'{name} {"=" if default["value"] == is_equal else "!"}= {default["value"]}'
         elif default['is_enum']:
             return f'{name} {"=" if default["value"] == is_equal else "!"}= {default["value"]}'
         else:
             return f'{name} {"=" if default["value"] == is_equal else "!"}= "{default["value"]}"'
 
-    def parse_variable(self, ksf_var: KsfField):
-        def parse_default_var(value_type, default):
+    def parse_variable(self,
+                       ksf_var: KsfField):
+        def parse_default_var(value_type,
+                              default):
             if default is None:
-                if isinstance(value_type, KsfIntType):
+                if isinstance(value_type,
+                              KsfIntType):
                     return '0'
-                elif isinstance(value_type, KsfFloatType):
+                elif isinstance(value_type,
+                                KsfFloatType):
                     if value_type.bit == 32:
                         return '0.0f'
                     else:
                         return '0.0'
-                elif isinstance(value_type, KsfBoolType):
+                elif isinstance(value_type,
+                                KsfBoolType):
                     return 'true'
-                elif isinstance(value_type, KsfStringType):
+                elif isinstance(value_type,
+                                KsfStringType):
                     return '""'
                 else:
                     return None
 
             # 特殊处理一下bool型
             if default['is_bool']:
                 return f'{"true" if default["value"] else "false"}'
             elif default['is_number'] or default['is_enum']:
                 return f'{default["value"]}'
             else:
                 return f'"{default["value"]}"'
 
-        default_var = parse_default_var(ksf_var.value_type, ksf_var.default)
+        default_var = parse_default_var(ksf_var.value_type,
+                                        ksf_var.default)
         comment = self.parse_comment_line(ksf_var.comment)
 
         return comment, self.parse_type(ksf_var.value_type
                                         ), ksf_var.name, f' = {default_var};' if default_var is not None else ';'
 
-    def add_lines(self, lines, tab=0):
-        if isinstance(lines, str):
+    def add_lines(self,
+                  lines,
+                  tab=0):
+        if isinstance(lines,
+                      str):
             lines = lines.split('\n')
-        elif isinstance(lines, (list, tuple, set)):
-            return '\n'.join(self.add_lines(line, tab) for line in lines)
+        elif isinstance(lines,
+                        (list, tuple, set)):
+            return '\n'.join(self.add_lines(line,
+                                            tab) for line in lines)
         else:
             raise TypeError(f"不支持的类型{type(lines)}")
 
         space = ' ' * (4 * tab)
         return f"\n".join(space + line for line in lines)
 
 
@@ -354,16 +417,25 @@
         flags = defaultdict(bool)
 
     file_path = files
 
     real_inc_dirs = set()
     for inc in include_dirs:
         real_inc_dirs.add(str(Path(inc).resolve()))
-    ast = generate(file_path, real_inc_dirs, flags['with_current_priority'], export_symbols)
-    return CppParser(ast, repl_ns_dict, repl_inc_dir, destination_dir, push_functions, export_symbols, **flags)
+    ast = generate(file_path,
+                   real_inc_dirs,
+                   flags['with_current_priority'],
+                   export_symbols)
+    return CppParser(ast,
+                     repl_ns_dict,
+                     repl_inc_dir,
+                     destination_dir,
+                     push_functions,
+                     export_symbols,
+                     **flags)
 
 
 # 测试用例
 if __name__ == '__main__':
     file_path = [
         'example/enum_simple.ksf',
         'example/const_definition.ksf',
@@ -388,8 +460,9 @@
                            include_dirs,
                            destination_dir,
                            push_functions,
                            export_symbols,
                            flags={'with_current_priority': True}
                            )
 
-    parser.parse_variable(parser.ast.modules[0], parser.ast.modules[0].fields[0])
+    parser.parse_variable(parser.ast.modules[0],
+                          parser.ast.modules[0].fields[0])
```

### Comparing `ksfctl-0.2.3/ksfctl/generate/cpp/template.py` & `ksfctl-0.2.4/ksfctl/generate/cpp/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,30 +260,31 @@
 ///序列化为Json字符串
 std::string writeToJsonString() const {{
     return ksf::KS_Json::writeValue(writeToJson());
 }}
 '''
 
 # readFrom
-# 填充variables
+# 填充variables, is_wrap
 template_readFrom = '''\
 ///二进制反序列化为结构体
 template<typename ReaderT>
 void readFrom(ksf::KsfInputStream<ReaderT>& _is) {{
-    resetDefault();
+    {"obj." if is_wrap else ""}resetDefault();
+    
 {add_lines(variables, 1)}
 }}
 '''
 
 # readFromJson
-# 填充 variables
+# 填充 variables, is_wrap
 template_readFromJson = '''\
 ///Json反序列化为结构体
 void readFromJson(const ksf::JsonValuePtr &p, bool isRequire = true) {{
-    resetDefault();
+    {"obj." if is_wrap else ""}resetDefault();
     if(!p || p->getType() != ksf::eJsonTypeObj) {{
         char s[128];
         snprintf(s, sizeof(s), "read 'struct' type mismatch, get type: %d.", (p ? p->getType() : 0));
         throw ksf::KS_Json_Exception(s);
     }}
 
     ksf::JsonValueObjPtr pObj=ksf::JsonValueObjPtr::dynamicCast(p);
@@ -297,26 +298,26 @@
 '''
 
 # display
 # 填充 variables
 template_display = '''\
 ///打印
 std::ostream& display(std::ostream& _os, int _level = 0) const {{
-    ksf::KsfDisplayer _ds(_os, _level);
+    ksf::Displayer _ds(_os, _level);
 {add_lines(variables, 1)}
     return _os;
 }}
 '''
 
 # displaySimple
 # 填充 variables
 template_displaySimple = '''\
 ///简单打印
 std::ostream& displaySimple(std::ostream& _os, int _level = 0) const {{
-    ksf::KsfDisplayer _ds(_os, _level);
+    ksf::Displayer _ds(_os, _level);
 {add_lines(variables, 1)}
     return _os;
 }}
 '''
 
 # operator== & operator!=
 # 填充 struct_name, variables
@@ -618,52 +619,52 @@
 # 填充 input_arguments, output_arguments, return_type, return_line, comment
 # 填充 argument_request_context, argument_response_context
 # 填充 argument_async_callback, argument_coroutine_callback
 template_proxy_function = """\
 {comment}\
 {return_type} {function_name}({add_connect(', ', arguments, argument_request_context, argument_response_context)}) {{
     ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
-{add_lines(input_arguments, 1)}
+{add_lines(input_argument_declare, 1)}
     _Status_ _status_;
     std::shared_ptr<ksf::ResponsePacket> rsp = ksf_invoke(ksf::KSFNORMAL, "{function_name}", _os, _context_, _status_);
     
     if (_rsp_context_) {{
         _rsp_context_->swap(rsp->context);
     }}
 
     ksf::KsfInputStream<ksf::BufferReader> _is;
     _is.setBuffer(rsp->sBuffer);
-{add_lines(output_arguments, 1)}
+{add_lines(output_argument_declare, 1)}
     {return_line}
 }}
 
-void async_{function_name}({add_connect(', ', argument_async_callback, arguments, argument_request_context)}) {{
+void async_{function_name}({add_connect(', ', argument_async_callback, input_arguments, argument_request_context)}) {{
     ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
-{add_lines(input_arguments, 1)}
+{add_lines(input_argument_declare, 1)}
     _Status_ _status_;
     ksf_invoke_async(ksf::KSFNORMAL, "{function_name}", _os, _context_, _status_, callback);
 }}
 
 ksf::Future<{interface_name}PrxCallbackPromise::Promise{function_name}Ptr> \
-promise_async_{function_name}({add_connect(', ', arguments, argument_request_context)}) {{
+promise_async_{function_name}({add_connect(', ', input_arguments, argument_request_context)}) {{
     ksf::Promise<{interface_name}PrxCallbackPromise::Promise{function_name}Ptr> promise;
     {interface_name}PrxCallbackPromisePtr callback = new {interface_name}PrxCallbackPromise(promise);
 
     ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
-{add_lines(input_arguments, 1)}
+{add_lines(input_argument_declare, 1)}
     _Status_ _status_;
     
     ksf_invoke_async(ksf::KSFNORMAL, "{function_name}", _os, _context_, _status_, callback);
 
     return promise.getFuture();
 }}
 
-void coro_{function_name}({add_connect(', ', argument_async_callback, arguments, argument_request_context)}) {{
+void coro_{function_name}({add_connect(', ', argument_async_callback, input_arguments, argument_request_context)}) {{
     ksf::KsfOutputStream<ksf::BufferWriterVector> _os;
-{add_lines(input_arguments, 1)}
+{add_lines(input_argument_declare, 1)}
     _Status_ _status_;
     ksf_invoke_async(ksf::KSFNORMAL, "{function_name}", _os, _context_, _status_, callback, true);
 }}
 """
 
 ############################################################################################################
 # 服务端接口类同步方法纯虚函数
@@ -804,25 +805,27 @@
 """
 
 # 头文件内容
 template_header = """\
 {header_description}
 #pragma once
     
-{import_headers}
+{add_lines(import_headers)}
+
+
 {add_lines(namespaces)}
     
 """
 
 ############################################################################################################
 # 结构体模版
 # 填充 struct_name, comment, members
 template_struct = """\
 {comment}\
-struct {struct_name} : public ksf::KsfStructBase
+struct {struct_name} : public ksf::Struct
 {{
 {variables}
 
 public:
     ///获取类名
     static std::string className() {{
         return "{module_name}::{struct_name}";
@@ -852,24 +855,24 @@
 public:
 {add_lines(struct_functions, 1)}
 }}; // end {struct_name}
 """
 
 template_struct_wrap = """\
 template<> 
-struct ksf::Wrap<{struct_name}> : public ksf::KsfStructBase
+struct ksf::Wrap<{struct_name}> : public ksf::Struct
 {{
 public:
     {struct_name} sobj; //结构体对象
     {struct_name} &obj; //结构体对象引用
 
 public:
     ///获取类名
     static std::string className() {{
-        return "{module_name}::{struct_name}";
+        return "{struct_name}";
     }}
     
     ///获取类的md5
     static std::string MD5() {{
         return "{md5sum}";
     }}
 
@@ -881,12 +884,11 @@
     Wrap(const {struct_name}& object): obj(*(const_cast<{struct_name}*>(&object))) {{}}
     virtual ~Wrap() = default;
 
 public:
 {add_lines(struct_functions, 1)}
 }}; // end {struct_name}
 
-{namespace_left}
+{namespace_left} using {struct_name_without_namespace}Wrap = ksf::Wrap<{struct_name}>; {namespace_right}
+
 {add_lines(struct_operators)}
-using {struct_name}Wrap = ksf::Wrap<{struct_name}>;
-{namespace_right}
 """
```

### Comparing `ksfctl-0.2.3/ksfctl/generate/ksf/generator.py` & `ksfctl-0.2.4/ksfctl/generate/ksf/generator.py`

 * *Files identical despite different names*

### Comparing `ksfctl-0.2.3/ksfctl/generate/ksf/parser.py` & `ksfctl-0.2.4/ksfctl/generate/ksf/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,17 +157,14 @@
 
         raise SyntaxError(f"不支持解析的字段类型[{value_type}]")
 
     def parse_comment_above(self, comment, tab=None):
         if comment is None or comment == '':
             return ''
 
-        if tab is None:
-            tab = self.curr_tab
-
         comment_lines = comment.split('\n')
         if len(comment_lines) == 1:
             return f"{tab}//{comment}\n"
         else:
             import re
             matches = re.findall(r"\s+\*\s+(.*)\n", f"/*{comment}*/")
             comment_str = f'{tab}/**\n'
```

### Comparing `ksfctl-0.2.3/ksfctl/parser/ksf.py` & `ksfctl-0.2.4/ksfctl/parser/ksf.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,16 +120,16 @@
         self.tag = tag
         self.is_required = is_required
         self.value_type = value_type
         self.default = default
 
         self.id = '.'.join([self.module, self.struct, self.name])
 
-        if self.is_required and self.default is not None:
-            raise SyntaxError(f"require的字段[{self.id}]不允许有默认值")
+        # if self.is_required and self.default is not None:
+        #     raise SyntaxError(f"require的字段[{self.id}]不允许有默认值")
 
     def update_export_symbol(self):
         """
         更新导出符号, 需要更新所有依赖的结构体
         :return:
         """
         for obj_type in self.value_type.get_no_native_obj():
```

### Comparing `ksfctl-0.2.3/ksfctl/parser/parser.py` & `ksfctl-0.2.4/ksfctl/parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import warnings
 
 import ply.yacc as yacc
 
-from ksfctl.parser.token import KsfLexer
 from ksfctl.parser.ksf import *
+from ksfctl.parser.token import KsfLexer
 from ksfctl.parser.tools import *
 
 
 class KsfParser:
     def __init__(self):
         # 解析语法的准备
         self.lexer = KsfLexer()
@@ -897,16 +897,16 @@
     file = Path(file_path)
     if with_curr_dir_first and file.exists():
         return file
 
     if file.is_absolute() and not file.exists():
         return None
 
-    for dir in search_dirs:
-        search_file = Path(dir) / file_path
+    for search_dir in search_dirs:
+        search_file = Path(search_dir) / file_path
         if search_file.exists():
             return search_file
 
     return None
 
 
 def generate(files, search_dirs: set, with_curr_dir_first: bool, export_symbols):
@@ -930,15 +930,15 @@
                     for include in curr_file_grammar['include']:
                         # 在search路径中添加当前文件所在路径
                         curr_search_dirs = search_dirs
                         curr_search_dirs.add(str(file.parent.resolve()))
 
                         inc_path = find_file(include, curr_search_dirs, with_curr_dir_first)
                         if inc_path is None:
-                            raise FileNotFoundError(f"依赖的头文件[{include}]未找到")
+                            raise FileNotFoundError(f"{f.name}依赖的头文件[{include}]未找到")
 
                         Ksf.add_include(file, inc_path, include)
 
                         if str(Path(inc_path).name) not in parser_grammar:
                             parse_depends(inc_path)
 
     for file in files:
```

### Comparing `ksfctl-0.2.3/ksfctl/parser/token.py` & `ksfctl-0.2.4/ksfctl/parser/token.py`

 * *Files identical despite different names*

### Comparing `ksfctl-0.2.3/ksfctl/parser/tools.py` & `ksfctl-0.2.4/ksfctl/parser/tools.py`

 * *Files identical despite different names*

### Comparing `ksfctl-0.2.3/ksfctl.egg-info/SOURCES.txt` & `ksfctl-0.2.4/ksfctl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ksfctl-0.2.3/setup.py` & `ksfctl-0.2.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ksfctl',
-    version='0.2.3',
+    version='0.2.4',
     keywords='ksf, client, generator, tool',
     description='a auto generator tools for ksf protocol files, and some useful tools',
     packages=find_packages(),
     include_package_data=True,
     package_data={
         'ksfctl': ['parser/parser.out'],
     },
@@ -14,11 +14,11 @@
         'Click>=8.0.0',
         'ply>=3.0.0',
         'pyyaml>=5.4.1',
     ],
     entry_points='''
         [console_scripts]
         ksfctl=ksfctl.cmd.cmd:cli
-        ksf2cpp=ksfctl.cmd.cmd:parse_cxx
-        ksf2cxx=ksfctl.cmd.cmd:parse_cxx
+        ksf2cpp=ksfctl.cmd.cmd:cxx
+        ksf2cxx=ksfctl.cmd.cmd:cxx
     ''',
 )
```

